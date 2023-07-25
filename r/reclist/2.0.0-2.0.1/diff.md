# Comparing `tmp/reclist-2.0.0.tar.gz` & `tmp/reclist-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reclist-2.0.0.tar", last modified: Tue Jul 25 01:03:04 2023, max compression
+gzip compressed data, was "reclist-2.0.1.tar", last modified: Tue Jul 25 03:36:06 2023, max compression
```

## Comparing `reclist-2.0.0.tar` & `reclist-2.0.1.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 01:03:04.736948 reclist-2.0.0/
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      165 2023-02-28 04:47:32.000000 reclist-2.0.0/AUTHORS.rst
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     3499 2023-02-28 04:47:32.000000 reclist-2.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 vinid     (1000) vinid     (1000)       89 2023-02-28 04:47:32.000000 reclist-2.0.0/HISTORY.rst
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     1074 2023-07-14 01:35:32.000000 reclist-2.0.0/LICENSE
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      262 2023-02-28 04:47:32.000000 reclist-2.0.0/MANIFEST.in
--rw-rw-r--   0 vinid     (1000) vinid     (1000)    14391 2023-07-25 01:03:04.736948 reclist-2.0.0/PKG-INFO
--rw-rw-r--   0 vinid     (1000) vinid     (1000)    13598 2023-07-25 01:02:28.000000 reclist-2.0.0/README.rst
-drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 01:03:04.732948 reclist-2.0.0/reclist/
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      103 2023-07-24 17:04:06.000000 reclist-2.0.0/reclist/__init__.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      107 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/charts.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     2884 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/logs.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     1612 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/metadata.py
-drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 01:03:04.736948 reclist-2.0.0/reclist/metrics/
--rw-rw-r--   0 vinid     (1000) vinid     (1000)        0 2023-02-28 04:47:32.000000 reclist-2.0.0/reclist/metrics/__init__.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     7003 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/metrics/distance_metrics.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     4855 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/metrics/hits.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     1032 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/metrics/perturbation.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     1567 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/metrics/price_homogeneity.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)    11840 2023-07-24 17:02:51.000000 reclist-2.0.0/reclist/metrics/standard_metrics.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     9036 2023-07-24 17:02:51.000000 reclist-2.0.0/reclist/reclist.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     5106 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/similarity_models.py
-drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 01:03:04.736948 reclist-2.0.0/reclist.egg-info/
--rw-rw-r--   0 vinid     (1000) vinid     (1000)    14391 2023-07-25 01:03:04.000000 reclist-2.0.0/reclist.egg-info/PKG-INFO
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      629 2023-07-25 01:03:04.000000 reclist-2.0.0/reclist.egg-info/SOURCES.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)        1 2023-07-25 01:03:04.000000 reclist-2.0.0/reclist.egg-info/dependency_links.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)        1 2023-03-11 01:25:56.000000 reclist-2.0.0/reclist.egg-info/not-zip-safe
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      258 2023-07-25 01:03:04.000000 reclist-2.0.0/reclist.egg-info/requires.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)        8 2023-07-25 01:03:04.000000 reclist-2.0.0/reclist.egg-info/top_level.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      424 2023-07-25 01:03:04.736948 reclist-2.0.0/setup.cfg
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     1540 2023-07-24 17:04:06.000000 reclist-2.0.0/setup.py
-drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 01:03:04.736948 reclist-2.0.0/tests/
--rw-rw-r--   0 vinid     (1000) vinid     (1000)       37 2023-02-28 04:47:32.000000 reclist-2.0.0/tests/__init__.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     2619 2023-07-17 19:47:56.000000 reclist-2.0.0/tests/test_reclist.py
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 03:36:06.209228 reclist-2.0.1/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      165 2023-02-28 04:47:32.000000 reclist-2.0.1/AUTHORS.rst
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     3499 2023-02-28 04:47:32.000000 reclist-2.0.1/CONTRIBUTING.rst
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)       89 2023-02-28 04:47:32.000000 reclist-2.0.1/HISTORY.rst
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1074 2023-07-14 01:35:32.000000 reclist-2.0.1/LICENSE
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      317 2023-07-25 03:35:16.000000 reclist-2.0.1/MANIFEST.in
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    14391 2023-07-25 03:36:06.209228 reclist-2.0.1/PKG-INFO
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    13598 2023-07-25 01:02:28.000000 reclist-2.0.1/README.rst
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 03:36:06.209228 reclist-2.0.1/reclist/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      103 2023-07-25 03:36:04.000000 reclist-2.0.1/reclist/__init__.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      107 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/charts.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     2884 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/logs.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1612 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/metadata.py
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 03:36:06.209228 reclist-2.0.1/reclist/metrics/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        0 2023-02-28 04:47:32.000000 reclist-2.0.1/reclist/metrics/__init__.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     7003 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/metrics/distance_metrics.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     4855 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/metrics/hits.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1032 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/metrics/perturbation.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1567 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/metrics/price_homogeneity.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    11840 2023-07-24 17:02:51.000000 reclist-2.0.1/reclist/metrics/standard_metrics.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     9036 2023-07-24 17:02:51.000000 reclist-2.0.1/reclist/reclist.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     5106 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/similarity_models.py
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 03:36:06.209228 reclist-2.0.1/reclist.egg-info/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    14391 2023-07-25 03:36:06.000000 reclist-2.0.1/reclist.egg-info/PKG-INFO
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      667 2023-07-25 03:36:06.000000 reclist-2.0.1/reclist.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        1 2023-07-25 03:36:06.000000 reclist-2.0.1/reclist.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        1 2023-03-11 01:25:56.000000 reclist-2.0.1/reclist.egg-info/not-zip-safe
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      258 2023-07-25 03:36:06.000000 reclist-2.0.1/reclist.egg-info/requires.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        8 2023-07-25 03:36:06.000000 reclist-2.0.1/reclist.egg-info/top_level.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      204 2023-07-24 17:02:51.000000 reclist-2.0.1/requirements.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      159 2023-07-17 19:47:56.000000 reclist-2.0.1/requirements_dev.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      424 2023-07-25 03:36:06.209228 reclist-2.0.1/setup.cfg
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1540 2023-07-25 03:36:04.000000 reclist-2.0.1/setup.py
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 03:36:06.209228 reclist-2.0.1/tests/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)       37 2023-02-28 04:47:32.000000 reclist-2.0.1/tests/__init__.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     2619 2023-07-17 19:47:56.000000 reclist-2.0.1/tests/test_reclist.py
```

### Comparing `reclist-2.0.0/CONTRIBUTING.rst` & `reclist-2.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `reclist-2.0.0/LICENSE` & `reclist-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reclist-2.0.0/PKG-INFO` & `reclist-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reclist
-Version: 2.0.0
+Version: 2.0.1
 Summary: RecList
 Home-page: https://github.com/jacopotagliabue/reclist
 Author: RecList
 Author-email: 
 License: MIT license
 Keywords: reclist
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `reclist-2.0.0/README.rst` & `reclist-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `reclist-2.0.0/reclist/logs.py` & `reclist-2.0.1/reclist/logs.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.0/reclist/metadata.py` & `reclist-2.0.1/reclist/metadata.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.0/reclist/metrics/distance_metrics.py` & `reclist-2.0.1/reclist/metrics/distance_metrics.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.0/reclist/metrics/hits.py` & `reclist-2.0.1/reclist/metrics/hits.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.0/reclist/metrics/perturbation.py` & `reclist-2.0.1/reclist/metrics/perturbation.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.0/reclist/metrics/price_homogeneity.py` & `reclist-2.0.1/reclist/metrics/price_homogeneity.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.0/reclist/metrics/standard_metrics.py` & `reclist-2.0.1/reclist/metrics/standard_metrics.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.0/reclist/reclist.py` & `reclist-2.0.1/reclist/reclist.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.0/reclist/similarity_models.py` & `reclist-2.0.1/reclist/similarity_models.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.0/reclist.egg-info/PKG-INFO` & `reclist-2.0.1/reclist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reclist
-Version: 2.0.0
+Version: 2.0.1
 Summary: RecList
 Home-page: https://github.com/jacopotagliabue/reclist
 Author: RecList
 Author-email: 
 License: MIT license
 Keywords: reclist
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `reclist-2.0.0/reclist.egg-info/SOURCES.txt` & `reclist-2.0.1/reclist.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
+requirements.txt
+requirements_dev.txt
 setup.cfg
 setup.py
 reclist/__init__.py
 reclist/charts.py
 reclist/logs.py
 reclist/metadata.py
 reclist/reclist.py
```

### Comparing `reclist-2.0.0/setup.py` & `reclist-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,13 +51,13 @@
     keywords="reclist",
     name="reclist",
     packages=find_packages(include=["reclist", "reclist.*"]),
     test_suite="tests",
     tests_require=test_requirements,
 
     url='https://github.com/jacopotagliabue/reclist',
-    version='2.0.0',
+    version='2.0.1',
     zip_safe=False,
     extras_require={
         "dev": style_packages + ["pre-commit==2.20.0"],
     },
 )
```

### Comparing `reclist-2.0.0/tests/test_reclist.py` & `reclist-2.0.1/tests/test_reclist.py`

 * *Files identical despite different names*

