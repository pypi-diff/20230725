# Comparing `tmp/aeronet-0.1.0a8.tar.gz` & `tmp/aeronet-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet-0.1.0a8.tar", last modified: Tue Jul 25 06:48:25 2023, max compression
+gzip compressed data, was "aeronet-0.1.0a9.tar", last modified: Tue Jul 25 07:15:10 2023, max compression
```

## Comparing `aeronet-0.1.0a8.tar` & `aeronet-0.1.0a9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:25.407722 aeronet-0.1.0a8/
--rw-r--r--   0 trekin     (501) staff       (20)     1077 2023-04-01 13:22:48.000000 aeronet-0.1.0a8/LICENSE
--rw-r--r--   0 trekin     (501) staff       (20)       18 2023-07-24 09:31:48.000000 aeronet-0.1.0a8/MANIFEST.in
--rw-r--r--   0 trekin     (501) staff       (20)      728 2023-07-25 06:48:25.407396 aeronet-0.1.0a8/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)     4586 2023-07-24 09:42:18.000000 aeronet-0.1.0a8/README.rst
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:25.403120 aeronet-0.1.0a8/aeronet/
--rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet-0.1.0a8/aeronet/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-25 06:44:46.000000 aeronet-0.1.0a8/aeronet/__version__.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:25.405400 aeronet-0.1.0a8/aeronet/converters/
--rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet-0.1.0a8/aeronet/converters/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)      225 2023-07-21 05:30:39.000000 aeronet-0.1.0a8/aeronet/converters/split.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:25.406942 aeronet-0.1.0a8/aeronet/dataset/
--rw-r--r--   0 trekin     (501) staff       (20)      807 2023-07-25 06:45:44.000000 aeronet-0.1.0a8/aeronet/dataset/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)      263 2023-07-24 13:46:37.000000 aeronet-0.1.0a8/aeronet/dataset/coords.py
--rw-r--r--   0 trekin     (501) staff       (20)      415 2023-07-25 06:46:23.000000 aeronet-0.1.0a8/aeronet/dataset/io.py
--rw-r--r--   0 trekin     (501) staff       (20)      230 2023-07-21 14:31:48.000000 aeronet-0.1.0a8/aeronet/dataset/utils.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:25.404721 aeronet-0.1.0a8/aeronet.egg-info/
--rw-r--r--   0 trekin     (501) staff       (20)      728 2023-07-25 06:48:25.000000 aeronet-0.1.0a8/aeronet.egg-info/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)      396 2023-07-25 06:48:25.000000 aeronet-0.1.0a8/aeronet.egg-info/SOURCES.txt
--rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-25 06:48:25.000000 aeronet-0.1.0a8/aeronet.egg-info/dependency_links.txt
--rw-r--r--   0 trekin     (501) staff       (20)      190 2023-07-25 06:48:25.000000 aeronet-0.1.0a8/aeronet.egg-info/requires.txt
--rw-r--r--   0 trekin     (501) staff       (20)       43 2023-07-25 06:48:25.000000 aeronet-0.1.0a8/aeronet.egg-info/top_level.txt
--rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-25 06:48:25.407813 aeronet-0.1.0a8/setup.cfg
--rw-r--r--   0 trekin     (501) staff       (20)     4135 2023-07-24 08:53:55.000000 aeronet-0.1.0a8/setup.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:10.932572 aeronet-0.1.0a9/
+-rw-r--r--   0 trekin     (501) staff       (20)     1077 2023-04-01 13:22:48.000000 aeronet-0.1.0a9/LICENSE
+-rw-r--r--   0 trekin     (501) staff       (20)       18 2023-07-24 09:31:48.000000 aeronet-0.1.0a9/MANIFEST.in
+-rw-r--r--   0 trekin     (501) staff       (20)      728 2023-07-25 07:15:10.932296 aeronet-0.1.0a9/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)     4586 2023-07-24 09:42:18.000000 aeronet-0.1.0a9/README.rst
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:10.928565 aeronet-0.1.0a9/aeronet/
+-rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet-0.1.0a9/aeronet/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-25 07:14:31.000000 aeronet-0.1.0a9/aeronet/__version__.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:10.930734 aeronet-0.1.0a9/aeronet/converters/
+-rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet-0.1.0a9/aeronet/converters/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)      225 2023-07-21 05:30:39.000000 aeronet-0.1.0a9/aeronet/converters/split.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:10.931922 aeronet-0.1.0a9/aeronet/dataset/
+-rw-r--r--   0 trekin     (501) staff       (20)      807 2023-07-25 06:45:44.000000 aeronet-0.1.0a9/aeronet/dataset/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)      263 2023-07-24 13:46:37.000000 aeronet-0.1.0a9/aeronet/dataset/coords.py
+-rw-r--r--   0 trekin     (501) staff       (20)      415 2023-07-25 06:46:23.000000 aeronet-0.1.0a9/aeronet/dataset/io.py
+-rw-r--r--   0 trekin     (501) staff       (20)      230 2023-07-21 14:31:48.000000 aeronet-0.1.0a9/aeronet/dataset/utils.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:10.930190 aeronet-0.1.0a9/aeronet.egg-info/
+-rw-r--r--   0 trekin     (501) staff       (20)      728 2023-07-25 07:15:10.000000 aeronet-0.1.0a9/aeronet.egg-info/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)      396 2023-07-25 07:15:10.000000 aeronet-0.1.0a9/aeronet.egg-info/SOURCES.txt
+-rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-25 07:15:10.000000 aeronet-0.1.0a9/aeronet.egg-info/dependency_links.txt
+-rw-r--r--   0 trekin     (501) staff       (20)      190 2023-07-25 07:15:10.000000 aeronet-0.1.0a9/aeronet.egg-info/requires.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       43 2023-07-25 07:15:10.000000 aeronet-0.1.0a9/aeronet.egg-info/top_level.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-25 07:15:10.932656 aeronet-0.1.0a9/setup.cfg
+-rw-r--r--   0 trekin     (501) staff       (20)     4135 2023-07-24 08:53:55.000000 aeronet-0.1.0a9/setup.py
```

### Comparing `aeronet-0.1.0a8/LICENSE` & `aeronet-0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `aeronet-0.1.0a8/PKG-INFO` & `aeronet-0.1.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: Deep learning with remote sensing data.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet-0.1.0a8/README.rst` & `aeronet-0.1.0a9/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet-0.1.0a8/aeronet/dataset/__init__.py` & `aeronet-0.1.0a9/aeronet/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `aeronet-0.1.0a8/aeronet.egg-info/PKG-INFO` & `aeronet-0.1.0a9/aeronet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: Deep learning with remote sensing data.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet-0.1.0a8/setup.py` & `aeronet-0.1.0a9/setup.py`

 * *Files identical despite different names*

