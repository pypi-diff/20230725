# Comparing `tmp/hdc_bin_collection-0.3.1.tar.gz` & `tmp/hdc_bin_collection-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdc_bin_collection-0.3.1.tar", max compression
+gzip compressed data, was "hdc_bin_collection-0.3.2.tar", max compression
```

## Comparing `hdc_bin_collection-0.3.1.tar` & `hdc_bin_collection-0.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-04-25 20:19:19.838018 hdc_bin_collection-0.3.1/LICENSE
--rw-r--r--   0        0        0      235 2023-04-25 20:19:19.838018 hdc_bin_collection-0.3.1/README.md
--rw-r--r--   0        0        0       45 2023-07-25 12:55:31.655065 hdc_bin_collection-0.3.1/hdc_bin_collection/__init__.py
--rw-r--r--   0        0        0     8338 2023-07-25 13:02:04.055281 hdc_bin_collection-0.3.1/hdc_bin_collection/hdc_bin_collection.py
--rw-r--r--   0        0        0      953 2023-07-25 13:02:09.039332 hdc_bin_collection-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 hdc_bin_collection-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-25 20:19:19.838018 hdc_bin_collection-0.3.2/LICENSE
+-rw-r--r--   0        0        0      235 2023-04-25 20:19:19.838018 hdc_bin_collection-0.3.2/README.md
+-rw-r--r--   0        0        0       33 2023-07-25 13:07:42.194737 hdc_bin_collection-0.3.2/hdc_bin_collection/__init__.py
+-rw-r--r--   0        0        0     8338 2023-07-25 13:02:04.055281 hdc_bin_collection-0.3.2/hdc_bin_collection/hdc_bin_collection.py
+-rw-r--r--   0        0        0      953 2023-07-25 13:08:08.911006 hdc_bin_collection-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 hdc_bin_collection-0.3.2/PKG-INFO
```

### Comparing `hdc_bin_collection-0.3.1/LICENSE` & `hdc_bin_collection-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hdc_bin_collection-0.3.1/hdc_bin_collection/hdc_bin_collection.py` & `hdc_bin_collection-0.3.2/hdc_bin_collection/hdc_bin_collection.py`

 * *Files identical despite different names*

### Comparing `hdc_bin_collection-0.3.1/pyproject.toml` & `hdc_bin_collection-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hdc_bin_collection"
-version = "0.3.1"
+version = "0.3.2"
 description = "An async module that finds the next bin collection dates for a specific address in Market Harborough, UK. Uses the UPRN to find the address."
 authors = ["Aaron Carson <aaron@aaroncarson.co.uk>"]
 keywords = ["hdc", "bin", "collection", "Market Harborough", "Harborough", "LE16", "garbage", "trash", "rubbish", "recycling"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/caraar12345/hdc-bin-collection"
 include = ["LICENSE"]
```

### Comparing `hdc_bin_collection-0.3.1/PKG-INFO` & `hdc_bin_collection-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdc-bin-collection
-Version: 0.3.1
+Version: 0.3.2
 Summary: An async module that finds the next bin collection dates for a specific address in Market Harborough, UK. Uses the UPRN to find the address.
 Home-page: https://github.com/caraar12345/hdc-bin-collection
 License: MIT
 Keywords: hdc,bin,collection,Market Harborough,Harborough,LE16,garbage,trash,rubbish,recycling
 Author: Aaron Carson
 Author-email: aaron@aaroncarson.co.uk
 Requires-Python: >=3.9,<4.0
```

