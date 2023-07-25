# Comparing `tmp/hdc_bin_collection-0.5.0.tar.gz` & `tmp/hdc_bin_collection-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdc_bin_collection-0.5.0.tar", max compression
+gzip compressed data, was "hdc_bin_collection-0.6.0.tar", max compression
```

## Comparing `hdc_bin_collection-0.5.0.tar` & `hdc_bin_collection-0.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-04-25 20:19:19.838018 hdc_bin_collection-0.5.0/LICENSE
--rw-r--r--   0        0        0      235 2023-04-25 20:19:19.838018 hdc_bin_collection-0.5.0/README.md
--rw-r--r--   0        0        0       33 2023-07-25 13:07:42.194737 hdc_bin_collection-0.5.0/hdc_bin_collection/__init__.py
--rw-r--r--   0        0        0     8497 2023-07-25 17:21:39.222688 hdc_bin_collection-0.5.0/hdc_bin_collection/hdc_bin_collection.py
--rw-r--r--   0        0        0      953 2023-07-25 17:21:02.594341 hdc_bin_collection-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 hdc_bin_collection-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-25 20:19:19.838018 hdc_bin_collection-0.6.0/LICENSE
+-rw-r--r--   0        0        0      235 2023-04-25 20:19:19.838018 hdc_bin_collection-0.6.0/README.md
+-rw-r--r--   0        0        0       33 2023-07-25 13:07:42.194737 hdc_bin_collection-0.6.0/hdc_bin_collection/__init__.py
+-rw-r--r--   0        0        0     8498 2023-07-25 18:00:32.232847 hdc_bin_collection-0.6.0/hdc_bin_collection/hdc_bin_collection.py
+-rw-r--r--   0        0        0      953 2023-07-25 18:00:53.033008 hdc_bin_collection-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 hdc_bin_collection-0.6.0/PKG-INFO
```

### Comparing `hdc_bin_collection-0.5.0/LICENSE` & `hdc_bin_collection-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdc_bin_collection-0.5.0/hdc_bin_collection/hdc_bin_collection.py` & `hdc_bin_collection-0.6.0/hdc_bin_collection/hdc_bin_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     bin_div = soup.select_one(".block-your-next-scheduled-bin-collection-days")
     bin_types = [
         bin_type.strip()
         for bin_type in bin_div.find_all(string=True)
         if bin_type.parent.name == "li" and "green" not in bin_type
     ]
     bin_dates = [
-        datetime.strptime(bin_date.strip() + " @ 07:00", "%d %B %Y @ %H:%M").isoformat()
+        datetime.strptime(bin_date.strip() + " @ 07:00", "%d %B %Y @ %H:%M")
         for bin_date in bin_div.find_all(string=True)
         if bin_date.parent.name == "span" and "subscribed" not in bin_date
     ]
     for x in range(len(bin_types)):
         bin_types[x] = bin_types[x][
             bin_types[x].find("(") + 1 : bin_types[x].find(")")
         ][:-4].split("-")[0]
@@ -161,15 +161,15 @@
         if await verify_uprn(session, args.uprn):
             bin_data = await collect_data(session, args.uprn)
             if bin_data == "invalid_uprn":
                 print("The UPRN is not valid for Harborough District Council.")
             elif str(bin_data).startswith("connection_error"):
                 print(f"Connection error: {bin_data.split(': ')[1]}")
             else:
-                print(json.dumps(bin_data, indent=4, sort_keys=True))
+                print(json.dumps(bin_data, indent=4, sort_keys=True, default=str))
 
         else:
             print("The UPRN is not valid for Harborough District Council.")
 
 
 if __name__ == "__main__":
     import json
```

### Comparing `hdc_bin_collection-0.5.0/pyproject.toml` & `hdc_bin_collection-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hdc_bin_collection"
-version = "0.5.0"
+version = "0.6.0"
 description = "An async module that finds the next bin collection dates for a specific address in Market Harborough, UK. Uses the UPRN to find the address."
 authors = ["Aaron Carson <aaron@aaroncarson.co.uk>"]
 keywords = ["hdc", "bin", "collection", "Market Harborough", "Harborough", "LE16", "garbage", "trash", "rubbish", "recycling"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/caraar12345/hdc-bin-collection"
 include = ["LICENSE"]
```

### Comparing `hdc_bin_collection-0.5.0/PKG-INFO` & `hdc_bin_collection-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdc-bin-collection
-Version: 0.5.0
+Version: 0.6.0
 Summary: An async module that finds the next bin collection dates for a specific address in Market Harborough, UK. Uses the UPRN to find the address.
 Home-page: https://github.com/caraar12345/hdc-bin-collection
 License: MIT
 Keywords: hdc,bin,collection,Market Harborough,Harborough,LE16,garbage,trash,rubbish,recycling
 Author: Aaron Carson
 Author-email: aaron@aaroncarson.co.uk
 Requires-Python: >=3.9,<4.0
```

