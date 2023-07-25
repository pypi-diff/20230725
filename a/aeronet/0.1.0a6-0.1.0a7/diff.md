# Comparing `tmp/aeronet-0.1.0a6.tar.gz` & `tmp/aeronet-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet-0.1.0a6.tar", last modified: Mon Jul 24 13:49:37 2023, max compression
+gzip compressed data, was "aeronet-0.1.0a7.tar", last modified: Tue Jul 25 05:37:15 2023, max compression
```

## Comparing `aeronet-0.1.0a6.tar` & `aeronet-0.1.0a7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:49:37.850647 aeronet-0.1.0a6/
--rw-r--r--   0 trekin     (501) staff       (20)     1077 2023-04-01 13:22:48.000000 aeronet-0.1.0a6/LICENSE
--rw-r--r--   0 trekin     (501) staff       (20)       18 2023-07-24 09:31:48.000000 aeronet-0.1.0a6/MANIFEST.in
--rw-r--r--   0 trekin     (501) staff       (20)      728 2023-07-24 13:49:37.850226 aeronet-0.1.0a6/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)     4586 2023-07-24 09:42:18.000000 aeronet-0.1.0a6/README.rst
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:49:37.845290 aeronet-0.1.0a6/aeronet/
--rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet-0.1.0a6/aeronet/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-24 13:49:22.000000 aeronet-0.1.0a6/aeronet/__version__.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:49:37.848118 aeronet-0.1.0a6/aeronet/converters/
--rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet-0.1.0a6/aeronet/converters/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)      225 2023-07-21 05:30:39.000000 aeronet-0.1.0a6/aeronet/converters/split.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:49:37.849444 aeronet-0.1.0a6/aeronet/dataset/
--rw-r--r--   0 trekin     (501) staff       (20)      972 2023-07-21 14:58:33.000000 aeronet-0.1.0a6/aeronet/dataset/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)      263 2023-07-24 13:46:37.000000 aeronet-0.1.0a6/aeronet/dataset/coords.py
--rw-r--r--   0 trekin     (501) staff       (20)      230 2023-07-21 14:31:48.000000 aeronet-0.1.0a6/aeronet/dataset/utils.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:49:37.847446 aeronet-0.1.0a6/aeronet.egg-info/
--rw-r--r--   0 trekin     (501) staff       (20)      728 2023-07-24 13:49:37.000000 aeronet-0.1.0a6/aeronet.egg-info/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)      374 2023-07-24 13:49:37.000000 aeronet-0.1.0a6/aeronet.egg-info/SOURCES.txt
--rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-24 13:49:37.000000 aeronet-0.1.0a6/aeronet.egg-info/dependency_links.txt
--rw-r--r--   0 trekin     (501) staff       (20)      190 2023-07-24 13:49:37.000000 aeronet-0.1.0a6/aeronet.egg-info/requires.txt
--rw-r--r--   0 trekin     (501) staff       (20)       43 2023-07-24 13:49:37.000000 aeronet-0.1.0a6/aeronet.egg-info/top_level.txt
--rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-24 13:49:37.850760 aeronet-0.1.0a6/setup.cfg
--rw-r--r--   0 trekin     (501) staff       (20)     4135 2023-07-24 08:53:55.000000 aeronet-0.1.0a6/setup.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:15.084599 aeronet-0.1.0a7/
+-rw-r--r--   0 trekin     (501) staff       (20)     1077 2023-04-01 13:22:48.000000 aeronet-0.1.0a7/LICENSE
+-rw-r--r--   0 trekin     (501) staff       (20)       18 2023-07-24 09:31:48.000000 aeronet-0.1.0a7/MANIFEST.in
+-rw-r--r--   0 trekin     (501) staff       (20)      728 2023-07-25 05:37:15.084322 aeronet-0.1.0a7/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)     4586 2023-07-24 09:42:18.000000 aeronet-0.1.0a7/README.rst
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:15.080765 aeronet-0.1.0a7/aeronet/
+-rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet-0.1.0a7/aeronet/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-24 14:22:22.000000 aeronet-0.1.0a7/aeronet/__version__.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:15.083040 aeronet-0.1.0a7/aeronet/converters/
+-rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet-0.1.0a7/aeronet/converters/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)      225 2023-07-21 05:30:39.000000 aeronet-0.1.0a7/aeronet/converters/split.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:15.083957 aeronet-0.1.0a7/aeronet/dataset/
+-rw-r--r--   0 trekin     (501) staff       (20)      972 2023-07-21 14:58:33.000000 aeronet-0.1.0a7/aeronet/dataset/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)      263 2023-07-24 13:46:37.000000 aeronet-0.1.0a7/aeronet/dataset/coords.py
+-rw-r--r--   0 trekin     (501) staff       (20)      230 2023-07-21 14:31:48.000000 aeronet-0.1.0a7/aeronet/dataset/utils.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:15.082483 aeronet-0.1.0a7/aeronet.egg-info/
+-rw-r--r--   0 trekin     (501) staff       (20)      728 2023-07-25 05:37:15.000000 aeronet-0.1.0a7/aeronet.egg-info/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)      374 2023-07-25 05:37:15.000000 aeronet-0.1.0a7/aeronet.egg-info/SOURCES.txt
+-rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-25 05:37:15.000000 aeronet-0.1.0a7/aeronet.egg-info/dependency_links.txt
+-rw-r--r--   0 trekin     (501) staff       (20)      190 2023-07-25 05:37:15.000000 aeronet-0.1.0a7/aeronet.egg-info/requires.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       43 2023-07-25 05:37:15.000000 aeronet-0.1.0a7/aeronet.egg-info/top_level.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-25 05:37:15.084685 aeronet-0.1.0a7/setup.cfg
+-rw-r--r--   0 trekin     (501) staff       (20)     4135 2023-07-24 08:53:55.000000 aeronet-0.1.0a7/setup.py
```

### Comparing `aeronet-0.1.0a6/LICENSE` & `aeronet-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `aeronet-0.1.0a6/PKG-INFO` & `aeronet-0.1.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Deep learning with remote sensing data.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet-0.1.0a6/README.rst` & `aeronet-0.1.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet-0.1.0a6/aeronet/dataset/__init__.py` & `aeronet-0.1.0a7/aeronet/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `aeronet-0.1.0a6/aeronet.egg-info/PKG-INFO` & `aeronet-0.1.0a7/aeronet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Deep learning with remote sensing data.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet-0.1.0a6/setup.py` & `aeronet-0.1.0a7/setup.py`

 * *Files identical despite different names*

