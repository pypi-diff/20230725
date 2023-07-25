# Comparing `tmp/easyquery_query_builder-2.0.0.tar.gz` & `tmp/easyquery_query_builder-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyquery_query_builder-2.0.0.tar", max compression
+gzip compressed data, was "easyquery_query_builder-2.0.1.tar", max compression
```

## Comparing `easyquery_query_builder-2.0.0.tar` & `easyquery_query_builder-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-04-04 22:01:26.361168 easyquery_query_builder-2.0.0/easyquery_query_builder/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 22:06:50.899067 easyquery_query_builder-2.0.0/easyquery_query_builder/queries/__init__.py
--rw-r--r--   0        0        0      122 2023-04-17 22:16:32.162595 easyquery_query_builder-2.0.0/easyquery_query_builder/queries/query.py
--rw-r--r--   0        0        0     2192 2023-04-17 22:16:32.139892 easyquery_query_builder-2.0.0/easyquery_query_builder/queries/read_query.py
--rw-r--r--   0        0        0     3014 2023-04-17 22:16:32.122425 easyquery_query_builder-2.0.0/easyquery_query_builder/queries/read_query_builder.py
--rw-r--r--   0        0        0     2527 2023-04-17 22:16:32.114251 easyquery_query_builder-2.0.0/easyquery_query_builder/queries/read_query_with_joins.py
--rw-r--r--   0        0        0     1396 2023-04-17 22:16:32.155202 easyquery_query_builder-2.0.0/easyquery_query_builder/queries/read_query_with_joins_builder.py
--rw-r--r--   0        0        0      505 2023-04-17 22:25:15.831231 easyquery_query_builder-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    13170 2023-04-17 22:25:15.821965 easyquery_query_builder-2.0.0/README.md
--rw-r--r--   0        0        0    13528 1970-01-01 00:00:00.000000 easyquery_query_builder-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-04 22:01:26.361168 easyquery_query_builder-2.0.1/easyquery_query_builder/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:06:50.899067 easyquery_query_builder-2.0.1/easyquery_query_builder/queries/__init__.py
+-rw-r--r--   0        0        0      122 2023-04-17 22:16:32.162595 easyquery_query_builder-2.0.1/easyquery_query_builder/queries/query.py
+-rw-r--r--   0        0        0     2192 2023-04-17 22:16:32.139892 easyquery_query_builder-2.0.1/easyquery_query_builder/queries/read_query.py
+-rw-r--r--   0        0        0     3014 2023-04-17 22:16:32.122425 easyquery_query_builder-2.0.1/easyquery_query_builder/queries/read_query_builder.py
+-rw-r--r--   0        0        0     2527 2023-04-17 22:16:32.114251 easyquery_query_builder-2.0.1/easyquery_query_builder/queries/read_query_with_joins.py
+-rw-r--r--   0        0        0     1396 2023-04-17 22:16:32.155202 easyquery_query_builder-2.0.1/easyquery_query_builder/queries/read_query_with_joins_builder.py
+-rw-r--r--   0        0        0      503 2023-07-25 20:34:35.599346 easyquery_query_builder-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    13170 2023-04-17 22:25:15.821965 easyquery_query_builder-2.0.1/README.md
+-rw-r--r--   0        0        0    13528 1970-01-01 00:00:00.000000 easyquery_query_builder-2.0.1/PKG-INFO
```

### Comparing `easyquery_query_builder-2.0.0/easyquery_query_builder/queries/read_query.py` & `easyquery_query_builder-2.0.1/easyquery_query_builder/queries/read_query.py`

 * *Files identical despite different names*

### Comparing `easyquery_query_builder-2.0.0/easyquery_query_builder/queries/read_query_builder.py` & `easyquery_query_builder-2.0.1/easyquery_query_builder/queries/read_query_builder.py`

 * *Files identical despite different names*

### Comparing `easyquery_query_builder-2.0.0/easyquery_query_builder/queries/read_query_with_joins.py` & `easyquery_query_builder-2.0.1/easyquery_query_builder/queries/read_query_with_joins.py`

 * *Files identical despite different names*

### Comparing `easyquery_query_builder-2.0.0/easyquery_query_builder/queries/read_query_with_joins_builder.py` & `easyquery_query_builder-2.0.1/easyquery_query_builder/queries/read_query_with_joins_builder.py`

 * *Files identical despite different names*

### Comparing `easyquery_query_builder-2.0.0/README.md` & `easyquery_query_builder-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `easyquery_query_builder-2.0.0/PKG-INFO` & `easyquery_query_builder-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: easyquery-query-builder
-Version: 2.0.0
+Version: 2.0.1
 Summary: 
 Author: Smolke
 Author-email: d.smolczynski1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: easyvalid-data-validator (>=0.1.1,<0.2.0)
+Requires-Dist: easyvalid-data-validator (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 
 # easyquery-query-builder
 
 Main purpose of package is to provide user with ability to create sql queries using QueryBuilders which are implemented in Builder Project Pattern.
```

