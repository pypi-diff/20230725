# Comparing `tmp/lsrestclient-0.1.0.tar.gz` & `tmp/lsrestclient-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsrestclient-0.1.0.tar", max compression
+gzip compressed data, was "lsrestclient-0.2.0.tar", max compression
```

## Comparing `lsrestclient-0.1.0.tar` & `lsrestclient-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     6181 2023-07-25 09:41:02.649481 lsrestclient-0.1.0/README.md
--rw-r--r--   0        0        0     1068 2023-07-25 09:37:43.277069 lsrestclient-0.1.0/lsrestclient/__init__.py
--rw-r--r--   0        0        0      360 2023-07-25 11:53:13.281435 lsrestclient-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6577 1970-01-01 00:00:00.000000 lsrestclient-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6181 2023-07-25 09:41:02.649481 lsrestclient-0.2.0/README.md
+-rw-r--r--   0        0        0     3117 2023-07-25 14:47:43.639742 lsrestclient-0.2.0/lsrestclient/__init__.py
+-rw-r--r--   0        0        0      707 2023-07-25 14:51:03.406972 lsrestclient-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6623 1970-01-01 00:00:00.000000 lsrestclient-0.2.0/PKG-INFO
```

### Comparing `lsrestclient-0.1.0/README.md` & `lsrestclient-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lsrestclient-0.1.0/PKG-INFO` & `lsrestclient-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: lsrestclient
-Version: 0.1.0
+Version: 0.2.0
 Summary: REST Api Client
 Author: mba
 Author-email: bartel@electronic-shop.lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: lsjsonclasses (>=1.1.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # lsrestclient
```

