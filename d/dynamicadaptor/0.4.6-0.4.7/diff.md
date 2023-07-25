# Comparing `tmp/dynamicadaptor-0.4.6.tar.gz` & `tmp/dynamicadaptor-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicadaptor-0.4.6.tar", max compression
+gzip compressed data, was "dynamicadaptor-0.4.7.tar", max compression
```

## Comparing `dynamicadaptor-0.4.6.tar` & `dynamicadaptor-0.4.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    18431 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/LICENSE
--rw-r--r--   0        0        0    10010 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/README.md
--rw-r--r--   0        0        0     2136 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/AddonCard.py
--rw-r--r--   0        0        0      926 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/Content.py
--rw-r--r--   0        0        0    20383 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/DynamicConversion.py
--rw-r--r--   0        0        0      575 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/Header.py
--rw-r--r--   0        0        0     3882 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/Majors.py
--rw-r--r--   0        0        0      410 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/Message.py
--rw-r--r--   0        0        0      323 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/Repost.py
--rw-r--r--   0        0        0       10 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/dynamicadaptor/__init__.py
--rw-r--r--   0        0        0      500 2023-07-25 12:38:05.875671 dynamicadaptor-0.4.6/pyproject.toml
--rw-r--r--   0        0        0    10528 1970-01-01 00:00:00.000000 dynamicadaptor-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0    18431 2023-07-25 13:15:44.106340 dynamicadaptor-0.4.7/LICENSE
+-rw-r--r--   0        0        0    10010 2023-07-25 13:15:44.106340 dynamicadaptor-0.4.7/README.md
+-rw-r--r--   0        0        0     2136 2023-07-25 13:15:44.106340 dynamicadaptor-0.4.7/dynamicadaptor/AddonCard.py
+-rw-r--r--   0        0        0      926 2023-07-25 13:15:44.106340 dynamicadaptor-0.4.7/dynamicadaptor/Content.py
+-rw-r--r--   0        0        0    20383 2023-07-25 13:15:44.106340 dynamicadaptor-0.4.7/dynamicadaptor/DynamicConversion.py
+-rw-r--r--   0        0        0      575 2023-07-25 13:15:44.110340 dynamicadaptor-0.4.7/dynamicadaptor/Header.py
+-rw-r--r--   0        0        0     3882 2023-07-25 13:15:44.110340 dynamicadaptor-0.4.7/dynamicadaptor/Majors.py
+-rw-r--r--   0        0        0      410 2023-07-25 13:15:44.110340 dynamicadaptor-0.4.7/dynamicadaptor/Message.py
+-rw-r--r--   0        0        0      323 2023-07-25 13:15:44.110340 dynamicadaptor-0.4.7/dynamicadaptor/Repost.py
+-rw-r--r--   0        0        0       10 2023-07-25 13:15:44.110340 dynamicadaptor-0.4.7/dynamicadaptor/__init__.py
+-rw-r--r--   0        0        0      500 2023-07-25 13:15:44.110340 dynamicadaptor-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0    10528 1970-01-01 00:00:00.000000 dynamicadaptor-0.4.7/PKG-INFO
```

### Comparing `dynamicadaptor-0.4.6/LICENSE` & `dynamicadaptor-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.6/README.md` & `dynamicadaptor-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.6/dynamicadaptor/AddonCard.py` & `dynamicadaptor-0.4.7/dynamicadaptor/AddonCard.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.6/dynamicadaptor/Content.py` & `dynamicadaptor-0.4.7/dynamicadaptor/Content.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.6/dynamicadaptor/DynamicConversion.py` & `dynamicadaptor-0.4.7/dynamicadaptor/DynamicConversion.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.6/dynamicadaptor/Header.py` & `dynamicadaptor-0.4.7/dynamicadaptor/Header.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.6/dynamicadaptor/Majors.py` & `dynamicadaptor-0.4.7/dynamicadaptor/Majors.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.6/PKG-INFO` & `dynamicadaptor-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicadaptor
-Version: 0.4.6
+Version: 0.4.7
 Summary: 
 Author: DMC
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

