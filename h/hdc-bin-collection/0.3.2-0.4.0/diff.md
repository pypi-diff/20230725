# Comparing `tmp/hdc_bin_collection-0.3.2.tar.gz` & `tmp/hdc_bin_collection-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdc_bin_collection-0.3.2.tar", max compression
+gzip compressed data, was "hdc_bin_collection-0.4.0.tar", max compression
```

## Comparing `hdc_bin_collection-0.3.2.tar` & `hdc_bin_collection-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-04-25 20:19:19.838018 hdc_bin_collection-0.3.2/LICENSE
--rw-r--r--   0        0        0      235 2023-04-25 20:19:19.838018 hdc_bin_collection-0.3.2/README.md
--rw-r--r--   0        0        0       33 2023-07-25 13:07:42.194737 hdc_bin_collection-0.3.2/hdc_bin_collection/__init__.py
--rw-r--r--   0        0        0     8338 2023-07-25 13:02:04.055281 hdc_bin_collection-0.3.2/hdc_bin_collection/hdc_bin_collection.py
--rw-r--r--   0        0        0      953 2023-07-25 13:08:08.911006 hdc_bin_collection-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 hdc_bin_collection-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-25 20:19:19.838018 hdc_bin_collection-0.4.0/LICENSE
+-rw-r--r--   0        0        0      235 2023-04-25 20:19:19.838018 hdc_bin_collection-0.4.0/README.md
+-rw-r--r--   0        0        0       33 2023-07-25 13:07:42.194737 hdc_bin_collection-0.4.0/hdc_bin_collection/__init__.py
+-rw-r--r--   0        0        0     8342 2023-07-25 17:11:39.000641 hdc_bin_collection-0.4.0/hdc_bin_collection/hdc_bin_collection.py
+-rw-r--r--   0        0        0      953 2023-07-25 17:11:53.960805 hdc_bin_collection-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 hdc_bin_collection-0.4.0/PKG-INFO
```

### Comparing `hdc_bin_collection-0.3.2/LICENSE` & `hdc_bin_collection-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdc_bin_collection-0.3.2/hdc_bin_collection/hdc_bin_collection.py` & `hdc_bin_collection-0.4.0/hdc_bin_collection/hdc_bin_collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,35 +77,34 @@
 VXyNWQKV3WKdwrnuWih0hKWbt5DHDAff9Yk2dDLWKMGwsAvgnEzDHNb842m1R0aB
 L6KCq9NjRHDEjf8tM7qtj3u1cIiuPhnPQCjY/MiQu12ZIvVS5ljFH4gxQ+6IHdfG
 jjxDah2nGN59PRbxYvnKkKj9
 -----END CERTIFICATE-----"""
 
 SSL_CONTEXT = ssl.create_default_context(cadata=CA_PEM)
 
-async def collect_data(uprn):
+async def collect_data(session: aiohttp.ClientSession, uprn):
     """
     Returns the next collection dates from the bin collection page.
 
     :param uprn: The UPRN of the address to find the next collection dates for.
     :return: A dictionary containing the bin types that HDC collect as keys, and the next collection dates as values.
     """
-    async with aiohttp.ClientSession() as session:
-        try:
-            async with session.post(
-                BIN_DATA_URL, data={"Uprn": uprn}, allow_redirects=False, ssl=SSL_CONTEXT
-            ) as resp:
-                if resp.status == 200:
-                    bin_data_site = await resp.text()
-                elif resp.status == 302:
-                    return "invalid_uprn"
-                else:
-                    print()
-                    return f"connection_error: {str(resp.status)}"
-        except aiohttp.ClientConnectorError as e:
-            return f"connection_error: {e}"
+    try:
+        async with session.post(
+            BIN_DATA_URL, data={"Uprn": uprn}, allow_redirects=False, ssl=SSL_CONTEXT
+        ) as resp:
+            if resp.status == 200:
+                bin_data_site = await resp.text()
+            elif resp.status == 302:
+                return "invalid_uprn"
+            else:
+                print()
+                return f"connection_error: {str(resp.status)}"
+    except aiohttp.ClientConnectorError as e:
+        return f"connection_error: {e}"
 
     soup = BeautifulSoup(bin_data_site, "html.parser")
     bin_div = soup.select_one(".block-your-next-scheduled-bin-collection-days")
     bin_types = [
         bin_type.strip()
         for bin_type in bin_div.find_all(string=True)
         if bin_type.parent.name == "li" and "green" not in bin_type
@@ -118,38 +117,54 @@
     for x in range(len(bin_types)):
         bin_types[x] = bin_types[x][
             bin_types[x].find("(") + 1 : bin_types[x].find(")")
         ][:-4].split("-")[0]
     return dict(zip(bin_types, bin_dates))
 
 
-async def verify_uprn(uprn):
+async def verify_uprn(session: aiohttp.ClientSession, uprn):
     """
     Verifies that the UPRN is valid and that Harborough District Council is the authority for the address.
 
     :param uprn: The UPRN of the address to verify.
     :return: (True,  "") if the UPRN is valid and Harborough District Council is the authority for the address.\n
              (False, "invalid_uprn") if not.\n
              (False, "connection_error: [message]") if there was an unexpected error.
     """
 
+    try:
+        async with session.post(
+            BIN_DATA_URL, data={"Uprn": uprn}, allow_redirects=False, ssl=SSL_CONTEXT
+        ) as resp:
+            if resp.status == 200:
+                return True, ""
+            elif resp.status == 302:
+                return False, "invalid_uprn"
+            else:
+                print()
+                return False, f"connection_error: {str(resp.status)}"
+    except aiohttp.ClientConnectorError as e:
+        return False, f"connection_error: {e}"
+
+
+async def main(args):
     async with aiohttp.ClientSession() as session:
-        try:
-            async with session.post(
-                BIN_DATA_URL, data={"Uprn": uprn}, allow_redirects=False, ssl=SSL_CONTEXT
-            ) as resp:
-                if resp.status == 200:
-                    return True, ""
-                elif resp.status == 302:
-                    return False, "invalid_uprn"
-                else:
-                    print()
-                    return False, f"connection_error: {str(resp.status)}"
-        except aiohttp.ClientConnectorError as e:
-            return False, f"connection_error: {e}"
+        if await verify_uprn(session, args.uprn):
+            bin_data = await collect_data(session, args.uprn)
+            if bin_data == "invalid_uprn":
+                print("The UPRN is not valid for Harborough District Council.")
+            elif str(bin_data).startswith("connection_error"):
+                print(f"Connection error: {bin_data.split(': ')[1]}")
+            else:
+                print(
+                    json.dumps(bin_data, indent=4, sort_keys=True)
+                )
+
+        else:
+            print("The UPRN is not valid for Harborough District Council.")
 
 
 if __name__ == "__main__":
     import json
     import argparse
 
     parser = argparse.ArgumentParser(
@@ -157,20 +172,8 @@
     )
     parser.add_argument(
         "uprn",
         type=int,
         help="The UPRN of the address to find the next collection dates for.",
     )
     args = parser.parse_args()
-    if asyncio.run(verify_uprn(args.uprn)):
-        bin_data = asyncio.run(collect_data(args.uprn))
-        if bin_data == "invalid_uprn":
-            print("The UPRN is not valid for Harborough District Council.")
-        elif str(bin_data).startswith("connection_error"):
-            print(f"Connection error: {bin_data.split(': ')[1]}")
-        else:
-            print(
-                json.dumps(bin_data, indent=4, sort_keys=True)
-            )
-        
-    else:
-        print("The UPRN is not valid for Harborough District Council.")
+    asyncio.run(main(args))
```

### Comparing `hdc_bin_collection-0.3.2/pyproject.toml` & `hdc_bin_collection-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hdc_bin_collection"
-version = "0.3.2"
+version = "0.4.0"
 description = "An async module that finds the next bin collection dates for a specific address in Market Harborough, UK. Uses the UPRN to find the address."
 authors = ["Aaron Carson <aaron@aaroncarson.co.uk>"]
 keywords = ["hdc", "bin", "collection", "Market Harborough", "Harborough", "LE16", "garbage", "trash", "rubbish", "recycling"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/caraar12345/hdc-bin-collection"
 include = ["LICENSE"]
```

### Comparing `hdc_bin_collection-0.3.2/PKG-INFO` & `hdc_bin_collection-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdc-bin-collection
-Version: 0.3.2
+Version: 0.4.0
 Summary: An async module that finds the next bin collection dates for a specific address in Market Harborough, UK. Uses the UPRN to find the address.
 Home-page: https://github.com/caraar12345/hdc-bin-collection
 License: MIT
 Keywords: hdc,bin,collection,Market Harborough,Harborough,LE16,garbage,trash,rubbish,recycling
 Author: Aaron Carson
 Author-email: aaron@aaroncarson.co.uk
 Requires-Python: >=3.9,<4.0
```

