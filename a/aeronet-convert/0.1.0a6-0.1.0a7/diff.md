# Comparing `tmp/aeronet_convert-0.1.0a6.tar.gz` & `tmp/aeronet_convert-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet_convert-0.1.0a6.tar", last modified: Tue Jul 25 06:48:25 2023, max compression
+gzip compressed data, was "aeronet_convert-0.1.0a7.tar", last modified: Tue Jul 25 07:15:10 2023, max compression
```

## Comparing `aeronet_convert-0.1.0a6.tar` & `aeronet_convert-0.1.0a7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:25.048300 aeronet_convert-0.1.0a6/
--rw-r--r--   0 trekin     (501) staff       (20)      753 2023-07-25 06:48:25.048033 aeronet_convert-0.1.0a6/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)     2053 2023-07-21 05:30:39.000000 aeronet_convert-0.1.0a6/README.rst
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:25.045882 aeronet_convert-0.1.0a6/aeronet_convert/
--rw-r--r--   0 trekin     (501) staff       (20)       67 2023-07-21 05:30:39.000000 aeronet_convert-0.1.0a6/aeronet_convert/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-25 06:47:01.000000 aeronet_convert-0.1.0a6/aeronet_convert/__version__.py
--rw-r--r--   0 trekin     (501) staff       (20)     1250 2023-07-21 06:21:28.000000 aeronet_convert-0.1.0a6/aeronet_convert/rasterize.py
--rw-r--r--   0 trekin     (501) staff       (20)     5428 2023-07-21 06:21:18.000000 aeronet_convert-0.1.0a6/aeronet_convert/vectorize.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:25.047642 aeronet_convert-0.1.0a6/aeronet_convert.egg-info/
--rw-r--r--   0 trekin     (501) staff       (20)      753 2023-07-25 06:48:25.000000 aeronet_convert-0.1.0a6/aeronet_convert.egg-info/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)      330 2023-07-25 06:48:25.000000 aeronet_convert-0.1.0a6/aeronet_convert.egg-info/SOURCES.txt
--rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-25 06:48:25.000000 aeronet_convert-0.1.0a6/aeronet_convert.egg-info/dependency_links.txt
--rw-r--r--   0 trekin     (501) staff       (20)       71 2023-07-25 06:48:25.000000 aeronet_convert-0.1.0a6/aeronet_convert.egg-info/requires.txt
--rw-r--r--   0 trekin     (501) staff       (20)       16 2023-07-25 06:48:25.000000 aeronet_convert-0.1.0a6/aeronet_convert.egg-info/top_level.txt
--rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-25 06:48:25.048381 aeronet_convert-0.1.0a6/setup.cfg
--rw-r--r--   0 trekin     (501) staff       (20)     4373 2023-07-24 09:02:15.000000 aeronet_convert-0.1.0a6/setup.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:10.590779 aeronet_convert-0.1.0a7/
+-rw-r--r--   0 trekin     (501) staff       (20)      753 2023-07-25 07:15:10.590522 aeronet_convert-0.1.0a7/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)     2053 2023-07-21 05:30:39.000000 aeronet_convert-0.1.0a7/README.rst
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:10.588596 aeronet_convert-0.1.0a7/aeronet_convert/
+-rw-r--r--   0 trekin     (501) staff       (20)       67 2023-07-21 05:30:39.000000 aeronet_convert-0.1.0a7/aeronet_convert/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-25 07:14:31.000000 aeronet_convert-0.1.0a7/aeronet_convert/__version__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1250 2023-07-21 06:21:28.000000 aeronet_convert-0.1.0a7/aeronet_convert/rasterize.py
+-rw-r--r--   0 trekin     (501) staff       (20)     5428 2023-07-21 06:21:18.000000 aeronet_convert-0.1.0a7/aeronet_convert/vectorize.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:10.590145 aeronet_convert-0.1.0a7/aeronet_convert.egg-info/
+-rw-r--r--   0 trekin     (501) staff       (20)      753 2023-07-25 07:15:10.000000 aeronet_convert-0.1.0a7/aeronet_convert.egg-info/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)      330 2023-07-25 07:15:10.000000 aeronet_convert-0.1.0a7/aeronet_convert.egg-info/SOURCES.txt
+-rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-25 07:15:10.000000 aeronet_convert-0.1.0a7/aeronet_convert.egg-info/dependency_links.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       71 2023-07-25 07:15:10.000000 aeronet_convert-0.1.0a7/aeronet_convert.egg-info/requires.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       16 2023-07-25 07:15:10.000000 aeronet_convert-0.1.0a7/aeronet_convert.egg-info/top_level.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-25 07:15:10.590855 aeronet_convert-0.1.0a7/setup.cfg
+-rw-r--r--   0 trekin     (501) staff       (20)     4373 2023-07-24 09:02:15.000000 aeronet_convert-0.1.0a7/setup.py
```

### Comparing `aeronet_convert-0.1.0a6/PKG-INFO` & `aeronet_convert-0.1.0a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet_convert
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Raster-vector conversion for deep learning with remote sensing data. Based on opencv, rasterio, shapely.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_convert-0.1.0a6/README.rst` & `aeronet_convert-0.1.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet_convert-0.1.0a6/aeronet_convert/rasterize.py` & `aeronet_convert-0.1.0a7/aeronet_convert/rasterize.py`

 * *Files identical despite different names*

### Comparing `aeronet_convert-0.1.0a6/aeronet_convert/vectorize.py` & `aeronet_convert-0.1.0a7/aeronet_convert/vectorize.py`

 * *Files identical despite different names*

### Comparing `aeronet_convert-0.1.0a6/aeronet_convert.egg-info/PKG-INFO` & `aeronet_convert-0.1.0a7/aeronet_convert.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet-convert
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Raster-vector conversion for deep learning with remote sensing data. Based on opencv, rasterio, shapely.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_convert-0.1.0a6/setup.py` & `aeronet_convert-0.1.0a7/setup.py`

 * *Files identical despite different names*

