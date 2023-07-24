# Comparing `tmp/retakesearch-0.0.8.tar.gz` & `tmp/retakesearch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-0.0.8.tar", max compression
+gzip compressed data, was "retakesearch-0.0.9.tar", max compression
```

## Comparing `retakesearch-0.0.8.tar` & `retakesearch-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-24 21:24:24.380447 retakesearch-0.0.8/README.md
--rw-r--r--   0        0        0      412 2023-07-24 21:24:44.168526 retakesearch-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-24 21:24:24.380447 retakesearch-0.0.8/retakesearch/__init__.py
--rw-r--r--   0        0        0     2471 2023-07-24 21:24:24.380447 retakesearch-0.0.8/retakesearch/client.py
--rw-r--r--   0        0        0       67 2023-07-24 21:24:24.380447 retakesearch-0.0.8/retakesearch/search.py
--rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 retakesearch-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 22:36:24.045322 retakesearch-0.0.9/README.md
+-rw-r--r--   0        0        0      412 2023-07-24 22:36:42.666471 retakesearch-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-24 22:36:24.045322 retakesearch-0.0.9/retakesearch/__init__.py
+-rw-r--r--   0        0        0     2471 2023-07-24 22:36:24.045322 retakesearch-0.0.9/retakesearch/client.py
+-rw-r--r--   0        0        0       67 2023-07-24 22:36:24.045322 retakesearch-0.0.9/retakesearch/search.py
+-rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 retakesearch-0.0.9/PKG-INFO
```

### Comparing `retakesearch-0.0.8/retakesearch/client.py` & `retakesearch-0.0.9/retakesearch/client.py`

 * *Files identical despite different names*

### Comparing `retakesearch-0.0.8/PKG-INFO` & `retakesearch-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retakesearch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Open Source Search Infrastructure for Developers
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

