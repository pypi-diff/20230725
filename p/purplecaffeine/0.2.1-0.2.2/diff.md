# Comparing `tmp/purplecaffeine-0.2.1.tar.gz` & `tmp/purplecaffeine-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purplecaffeine-0.2.1.tar", last modified: Sun Jul 23 20:41:21 2023, max compression
+gzip compressed data, was "purplecaffeine-0.2.2.tar", last modified: Tue Jul 25 00:12:57 2023, max compression
```

## Comparing `purplecaffeine-0.2.1.tar` & `purplecaffeine-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:41:21.399161 purplecaffeine-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-23 20:41:21.399161 purplecaffeine-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:41:21.399161 purplecaffeine-0.2.1/purplecaffeine/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/purplecaffeine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21449 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/purplecaffeine/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/purplecaffeine/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:41:21.399161 purplecaffeine-0.2.1/purplecaffeine/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/purplecaffeine/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/purplecaffeine/helpers/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:41:21.399161 purplecaffeine-0.2.1/purplecaffeine/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/purplecaffeine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/purplecaffeine/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/purplecaffeine/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:41:21.399161 purplecaffeine-0.2.1/purplecaffeine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-23 20:41:21.000000 purplecaffeine-0.2.1/purplecaffeine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-23 20:41:21.000000 purplecaffeine-0.2.1/purplecaffeine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 20:41:21.000000 purplecaffeine-0.2.1/purplecaffeine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-23 20:41:21.000000 purplecaffeine-0.2.1/purplecaffeine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-23 20:41:21.000000 purplecaffeine-0.2.1/purplecaffeine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 20:41:21.399161 purplecaffeine-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:41:21.399161 purplecaffeine-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:41:21.399161 purplecaffeine-0.2.1/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/tests/helpers/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/tests/test_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/tests/test_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 20:41:21.399161 purplecaffeine-0.2.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-23 20:41:14.000000 purplecaffeine-0.2.1/tests/utils/test_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:57.790776 purplecaffeine-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-25 00:12:57.790776 purplecaffeine-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:57.786776 purplecaffeine-0.2.2/purplecaffeine/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/purplecaffeine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21449 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/purplecaffeine/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/purplecaffeine/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:57.786776 purplecaffeine-0.2.2/purplecaffeine/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/purplecaffeine/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/purplecaffeine/helpers/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:57.786776 purplecaffeine-0.2.2/purplecaffeine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/purplecaffeine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/purplecaffeine/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/purplecaffeine/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:57.786776 purplecaffeine-0.2.2/purplecaffeine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-25 00:12:57.000000 purplecaffeine-0.2.2/purplecaffeine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-25 00:12:57.000000 purplecaffeine-0.2.2/purplecaffeine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 00:12:57.000000 purplecaffeine-0.2.2/purplecaffeine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 00:12:57.000000 purplecaffeine-0.2.2/purplecaffeine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 00:12:57.000000 purplecaffeine-0.2.2/purplecaffeine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 00:12:57.790776 purplecaffeine-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:57.790776 purplecaffeine-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:57.790776 purplecaffeine-0.2.2/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/tests/helpers/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/tests/test_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/tests/test_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:57.790776 purplecaffeine-0.2.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-25 00:12:43.000000 purplecaffeine-0.2.2/tests/utils/test_json.py
```

### Comparing `purplecaffeine-0.2.1/PKG-INFO` & `purplecaffeine-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purplecaffeine
-Version: 0.2.1
+Version: 0.2.2
 Summary: PurpleCaffeine: tracking of quantum programs and experiments
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum tracking experiments
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `purplecaffeine-0.2.1/README.md` & `purplecaffeine-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.2.1/purplecaffeine/core.py` & `purplecaffeine-0.2.2/purplecaffeine/core.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.2.1/purplecaffeine/helpers/conf.py` & `purplecaffeine-0.2.2/purplecaffeine/helpers/conf.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.2.1/purplecaffeine/utils/json.py` & `purplecaffeine-0.2.2/purplecaffeine/utils/json.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.2.1/purplecaffeine/widget.py` & `purplecaffeine-0.2.2/purplecaffeine/widget.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.2.1/purplecaffeine.egg-info/PKG-INFO` & `purplecaffeine-0.2.2/purplecaffeine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purplecaffeine
-Version: 0.2.1
+Version: 0.2.2
 Summary: PurpleCaffeine: tracking of quantum programs and experiments
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum tracking experiments
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `purplecaffeine-0.2.1/purplecaffeine.egg-info/SOURCES.txt` & `purplecaffeine-0.2.2/purplecaffeine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.2.1/setup.py` & `purplecaffeine-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.2.1/tests/helpers/test_conf.py` & `purplecaffeine-0.2.2/tests/helpers/test_conf.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.2.1/tests/test_storage.py` & `purplecaffeine-0.2.2/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.2.1/tests/test_trial.py` & `purplecaffeine-0.2.2/tests/test_trial.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.2.1/tests/test_widget.py` & `purplecaffeine-0.2.2/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `purplecaffeine-0.2.1/tests/utils/test_json.py` & `purplecaffeine-0.2.2/tests/utils/test_json.py`

 * *Files identical despite different names*

