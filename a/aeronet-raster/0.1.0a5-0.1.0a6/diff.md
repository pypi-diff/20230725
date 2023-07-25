# Comparing `tmp/aeronet_raster-0.1.0a5.tar.gz` & `tmp/aeronet_raster-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet_raster-0.1.0a5.tar", last modified: Tue Jul 25 05:37:14 2023, max compression
+gzip compressed data, was "aeronet_raster-0.1.0a6.tar", last modified: Tue Jul 25 06:48:24 2023, max compression
```

## Comparing `aeronet_raster-0.1.0a5.tar` & `aeronet_raster-0.1.0a6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:14.125111 aeronet_raster-0.1.0a5/
--rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-25 05:37:14.124817 aeronet_raster-0.1.0a5/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)     4784 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/README.rst
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:14.119211 aeronet_raster-0.1.0a5/aeronet_raster/
--rw-r--r--   0 trekin     (501) staff       (20)      392 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-24 14:22:22.000000 aeronet_raster-0.1.0a5/aeronet_raster/__version__.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:14.121887 aeronet_raster-0.1.0a5/aeronet_raster/band/
--rw-r--r--   0 trekin     (501) staff       (20)       58 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/band/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)    17952 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/band/band.py
--rw-r--r--   0 trekin     (501) staff       (20)    12101 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/band/bandsample.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:14.122884 aeronet_raster-0.1.0a5/aeronet_raster/bandcollection/
--rw-r--r--   0 trekin     (501) staff       (20)       98 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/bandcollection/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     7448 2023-07-24 14:21:08.000000 aeronet_raster-0.1.0a5/aeronet_raster/bandcollection/bandcollection.py
--rw-r--r--   0 trekin     (501) staff       (20)     5936 2023-07-21 14:48:40.000000 aeronet_raster-0.1.0a5/aeronet_raster/bandcollection/bandcollectionsample.py
--rw-r--r--   0 trekin     (501) staff       (20)    10643 2023-07-24 14:19:26.000000 aeronet_raster-0.1.0a5/aeronet_raster/collectionprocessor.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:14.123543 aeronet_raster-0.1.0a5/aeronet_raster/geoobject/
--rw-r--r--   0 trekin     (501) staff       (20)       32 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/geoobject/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     2642 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/geoobject/geoobject.py
--rw-r--r--   0 trekin     (501) staff       (20)     1997 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/merge.py
--rw-r--r--   0 trekin     (501) staff       (20)     5729 2023-07-24 13:07:04.000000 aeronet_raster-0.1.0a5/aeronet_raster/split.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:14.124431 aeronet_raster-0.1.0a5/aeronet_raster/utils/
--rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/utils/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     1267 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/utils/coords.py
--rw-r--r--   0 trekin     (501) staff       (20)     1796 2023-07-24 13:27:46.000000 aeronet_raster-0.1.0a5/aeronet_raster/utils/utils.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:14.120863 aeronet_raster-0.1.0a5/aeronet_raster.egg-info/
--rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-25 05:37:14.000000 aeronet_raster-0.1.0a5/aeronet_raster.egg-info/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)      758 2023-07-25 05:37:14.000000 aeronet_raster-0.1.0a5/aeronet_raster.egg-info/SOURCES.txt
--rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-25 05:37:14.000000 aeronet_raster-0.1.0a5/aeronet_raster.egg-info/dependency_links.txt
--rw-r--r--   0 trekin     (501) staff       (20)       49 2023-07-25 05:37:14.000000 aeronet_raster-0.1.0a5/aeronet_raster.egg-info/requires.txt
--rw-r--r--   0 trekin     (501) staff       (20)       15 2023-07-25 05:37:14.000000 aeronet_raster-0.1.0a5/aeronet_raster.egg-info/top_level.txt
--rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-25 05:37:14.125196 aeronet_raster-0.1.0a5/setup.cfg
--rw-r--r--   0 trekin     (501) staff       (20)     3757 2023-07-24 06:59:44.000000 aeronet_raster-0.1.0a5/setup.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:24.321954 aeronet_raster-0.1.0a6/
+-rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-25 06:48:24.321687 aeronet_raster-0.1.0a6/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)     4784 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/README.rst
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:24.316233 aeronet_raster-0.1.0a6/aeronet_raster/
+-rw-r--r--   0 trekin     (501) staff       (20)      392 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-25 06:46:50.000000 aeronet_raster-0.1.0a6/aeronet_raster/__version__.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:24.318843 aeronet_raster-0.1.0a6/aeronet_raster/band/
+-rw-r--r--   0 trekin     (501) staff       (20)       58 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/band/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)    17952 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/band/band.py
+-rw-r--r--   0 trekin     (501) staff       (20)    12101 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/band/bandsample.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:24.319790 aeronet_raster-0.1.0a6/aeronet_raster/bandcollection/
+-rw-r--r--   0 trekin     (501) staff       (20)       98 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/bandcollection/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     7447 2023-07-25 06:42:12.000000 aeronet_raster-0.1.0a6/aeronet_raster/bandcollection/bandcollection.py
+-rw-r--r--   0 trekin     (501) staff       (20)     5935 2023-07-25 06:42:47.000000 aeronet_raster-0.1.0a6/aeronet_raster/bandcollection/bandcollectionsample.py
+-rw-r--r--   0 trekin     (501) staff       (20)    10643 2023-07-24 14:19:26.000000 aeronet_raster-0.1.0a6/aeronet_raster/collectionprocessor.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:24.320424 aeronet_raster-0.1.0a6/aeronet_raster/geoobject/
+-rw-r--r--   0 trekin     (501) staff       (20)       32 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/geoobject/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     2642 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/geoobject/geoobject.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1997 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/merge.py
+-rw-r--r--   0 trekin     (501) staff       (20)     5729 2023-07-24 13:07:04.000000 aeronet_raster-0.1.0a6/aeronet_raster/split.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:24.321306 aeronet_raster-0.1.0a6/aeronet_raster/utils/
+-rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/utils/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1267 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/utils/coords.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1796 2023-07-24 13:27:46.000000 aeronet_raster-0.1.0a6/aeronet_raster/utils/utils.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:24.317886 aeronet_raster-0.1.0a6/aeronet_raster.egg-info/
+-rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-25 06:48:24.000000 aeronet_raster-0.1.0a6/aeronet_raster.egg-info/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)      758 2023-07-25 06:48:24.000000 aeronet_raster-0.1.0a6/aeronet_raster.egg-info/SOURCES.txt
+-rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-25 06:48:24.000000 aeronet_raster-0.1.0a6/aeronet_raster.egg-info/dependency_links.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       49 2023-07-25 06:48:24.000000 aeronet_raster-0.1.0a6/aeronet_raster.egg-info/requires.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       15 2023-07-25 06:48:24.000000 aeronet_raster-0.1.0a6/aeronet_raster.egg-info/top_level.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-25 06:48:24.322032 aeronet_raster-0.1.0a6/setup.cfg
+-rw-r--r--   0 trekin     (501) staff       (20)     3757 2023-07-24 06:59:44.000000 aeronet_raster-0.1.0a6/setup.py
```

### Comparing `aeronet_raster-0.1.0a5/PKG-INFO` & `aeronet_raster-0.1.0a6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet_raster
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: Raster operations for deep learning with remote sensing data. Based on Rasterio.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_raster-0.1.0a5/README.rst` & `aeronet_raster-0.1.0a6/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a5/aeronet_raster/band/band.py` & `aeronet_raster-0.1.0a6/aeronet_raster/band/band.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a5/aeronet_raster/band/bandsample.py` & `aeronet_raster-0.1.0a6/aeronet_raster/band/bandsample.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a5/aeronet_raster/bandcollection/bandcollection.py` & `aeronet_raster-0.1.0a6/aeronet_raster/bandcollection/bandcollection.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,9 +196,9 @@
             BandCollectionSample: sequential samples of the specified dimensions
         """
 
         for x in range(0, self.width, width):
             for y in range(0, self.height, height):
                 yield self.sample(y, x, height, width)
 
-    def numpy(self, frame: Optional[Union[tuple, np.ndarray]] = None, ch_axis: int = -1) -> np.ndarray:
+    def numpy(self, frame: Optional[Union[tuple, np.ndarray]] = None, ch_axis: int = 0) -> np.ndarray:
         return np.stack([band.numpy(frame) for band in self._bands], axis=ch_axis)
```

### Comparing `aeronet_raster-0.1.0a5/aeronet_raster/bandcollection/bandcollectionsample.py` & `aeronet_raster-0.1.0a6/aeronet_raster/bandcollection/bandcollectionsample.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         """
         Reprojects every BandSample of the collection, see :meth:`BandSample.reproject`
         and returns a new reprojected BandCollectionSample
         """
         resamples = [s.resample(dst_res, dst_shape, interpolation) for s in self._samples]
         return BandCollectionSample(resamples)
 
-    def numpy(self, axis: int = -1) -> np.ndarray:
+    def numpy(self, axis: int = 0) -> np.ndarray:
         return np.stack([x.numpy() for x in self._samples], axis=axis)
 
     def ordered(self, *names: str) -> GeoObject:
         """
         Creates a new object, containing the specified bands in the specific order.
 
         Args:
```

### Comparing `aeronet_raster-0.1.0a5/aeronet_raster/collectionprocessor.py` & `aeronet_raster-0.1.0a6/aeronet_raster/collectionprocessor.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a5/aeronet_raster/geoobject/geoobject.py` & `aeronet_raster-0.1.0a6/aeronet_raster/geoobject/geoobject.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a5/aeronet_raster/merge.py` & `aeronet_raster-0.1.0a6/aeronet_raster/merge.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a5/aeronet_raster/split.py` & `aeronet_raster-0.1.0a6/aeronet_raster/split.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a5/aeronet_raster/utils/coords.py` & `aeronet_raster-0.1.0a6/aeronet_raster/utils/coords.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a5/aeronet_raster/utils/utils.py` & `aeronet_raster-0.1.0a6/aeronet_raster/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a5/aeronet_raster.egg-info/PKG-INFO` & `aeronet_raster-0.1.0a6/aeronet_raster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet-raster
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: Raster operations for deep learning with remote sensing data. Based on Rasterio.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_raster-0.1.0a5/aeronet_raster.egg-info/SOURCES.txt` & `aeronet_raster-0.1.0a6/aeronet_raster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a5/setup.py` & `aeronet_raster-0.1.0a6/setup.py`

 * *Files identical despite different names*

