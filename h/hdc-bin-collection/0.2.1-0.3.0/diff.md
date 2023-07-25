# Comparing `tmp/hdc_bin_collection-0.2.1.tar.gz` & `tmp/hdc_bin_collection-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdc_bin_collection-0.2.1.tar", max compression
+gzip compressed data, was "hdc_bin_collection-0.3.0.tar", max compression
```

## Comparing `hdc_bin_collection-0.2.1.tar` & `hdc_bin_collection-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-04-25 20:19:19.838018 hdc_bin_collection-0.2.1/LICENSE
--rw-r--r--   0        0        0      235 2023-04-25 20:19:19.838018 hdc_bin_collection-0.2.1/README.md
--rw-r--r--   0        0        0       45 2023-07-24 18:28:19.170044 hdc_bin_collection-0.2.1/hdc_bin_collection/__init__.py
--rw-r--r--   0        0        0     7665 2023-07-24 19:07:07.873134 hdc_bin_collection-0.2.1/hdc_bin_collection/hdc_bin_collection.py
--rw-r--r--   0        0        0      927 2023-07-24 19:07:20.205252 hdc_bin_collection-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1143 1970-01-01 00:00:00.000000 hdc_bin_collection-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-25 20:19:19.838018 hdc_bin_collection-0.3.0/LICENSE
+-rw-r--r--   0        0        0      235 2023-04-25 20:19:19.838018 hdc_bin_collection-0.3.0/README.md
+-rw-r--r--   0        0        0       45 2023-07-24 18:28:19.170044 hdc_bin_collection-0.3.0/hdc_bin_collection/__init__.py
+-rw-r--r--   0        0        0     7979 2023-07-25 12:25:50.419888 hdc_bin_collection-0.3.0/hdc_bin_collection/hdc_bin_collection.py
+-rw-r--r--   0        0        0      953 2023-07-25 12:25:54.739930 hdc_bin_collection-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 hdc_bin_collection-0.3.0/PKG-INFO
```

### Comparing `hdc_bin_collection-0.2.1/LICENSE` & `hdc_bin_collection-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdc_bin_collection-0.2.1/hdc_bin_collection/hdc_bin_collection.py` & `hdc_bin_collection-0.3.0/hdc_bin_collection/hdc_bin_collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,27 +121,33 @@
 
 
 async def verify_uprn(uprn):
     """
     Verifies that the UPRN is valid and that Harborough District Council is the authority for the address.
 
     :param uprn: The UPRN of the address to verify.
-    :return: True if the UPRN is valid and Harborough District Council is the authority for the address, False otherwise.
+    :return: (True,  "") if the UPRN is valid and Harborough District Council is the authority for the address.\n
+             (False, "invalid_uprn") if not.\n
+             (False, "connection_error: [message]") if there was an unexpected error.
     """
 
     async with aiohttp.ClientSession() as session:
-        async with session.post(
-            BIN_DATA_URL, data={"Uprn": uprn}, allow_redirects=False, ssl=SSL_CONTEXT
-        ) as resp:
-            if resp.status == 200:
-                return True
-            elif resp.status == 302:
-                return False
-            else:
-                raise Exception("Unexpected status code: " + str(resp.status))
+        try:
+            async with session.post(
+                BIN_DATA_URL, data={"Uprn": uprn}, allow_redirects=False, ssl=SSL_CONTEXT
+            ) as resp:
+                if resp.status == 200:
+                    return True, ""
+                elif resp.status == 302:
+                    return False, "invalid_uprn"
+                else:
+                    print()
+                    return False, f"connection_error: {str(resp.status)}"
+        except aiohttp.ClientConnectorError as e:
+            return False, f"connection_error: {e}"
 
 
 if __name__ == "__main__":
     import json
     import argparse
 
     parser = argparse.ArgumentParser(
```

### Comparing `hdc_bin_collection-0.2.1/pyproject.toml` & `hdc_bin_collection-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "hdc_bin_collection"
-version = "0.2.1"
-description = "A module that finds the next bin collection dates for a specific address in Market Harborough, UK. Uses the UPRN to find the address."
+version = "0.3.0"
+description = "An async module that finds the next bin collection dates for a specific address in Market Harborough, UK. Uses the UPRN to find the address."
 authors = ["Aaron Carson <aaron@aaroncarson.co.uk>"]
-keywords = ["hdc", "bin", "collection", "Market", "Harborough", "garbage", "trash", "rubbish", "recycling"]
+keywords = ["hdc", "bin", "collection", "Market Harborough", "Harborough", "LE16", "garbage", "trash", "rubbish", "recycling"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/caraar12345/hdc-bin-collection"
 include = ["LICENSE"]
 packages = [
   { include = "hdc_bin_collection/*.py" }
 ]
```

### Comparing `hdc_bin_collection-0.2.1/PKG-INFO` & `hdc_bin_collection-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: hdc-bin-collection
-Version: 0.2.1
-Summary: A module that finds the next bin collection dates for a specific address in Market Harborough, UK. Uses the UPRN to find the address.
+Version: 0.3.0
+Summary: An async module that finds the next bin collection dates for a specific address in Market Harborough, UK. Uses the UPRN to find the address.
 Home-page: https://github.com/caraar12345/hdc-bin-collection
 License: MIT
-Keywords: hdc,bin,collection,Market,Harborough,garbage,trash,rubbish,recycling
+Keywords: hdc,bin,collection,Market Harborough,Harborough,LE16,garbage,trash,rubbish,recycling
 Author: Aaron Carson
 Author-email: aaron@aaroncarson.co.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

