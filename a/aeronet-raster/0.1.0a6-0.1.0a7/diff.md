# Comparing `tmp/aeronet_raster-0.1.0a6.tar.gz` & `tmp/aeronet_raster-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet_raster-0.1.0a6.tar", last modified: Tue Jul 25 06:48:24 2023, max compression
+gzip compressed data, was "aeronet_raster-0.1.0a7.tar", last modified: Tue Jul 25 07:15:09 2023, max compression
```

## Comparing `aeronet_raster-0.1.0a6.tar` & `aeronet_raster-0.1.0a7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:24.321954 aeronet_raster-0.1.0a6/
--rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-25 06:48:24.321687 aeronet_raster-0.1.0a6/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)     4784 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/README.rst
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:24.316233 aeronet_raster-0.1.0a6/aeronet_raster/
--rw-r--r--   0 trekin     (501) staff       (20)      392 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-25 06:46:50.000000 aeronet_raster-0.1.0a6/aeronet_raster/__version__.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:24.318843 aeronet_raster-0.1.0a6/aeronet_raster/band/
--rw-r--r--   0 trekin     (501) staff       (20)       58 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/band/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)    17952 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/band/band.py
--rw-r--r--   0 trekin     (501) staff       (20)    12101 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/band/bandsample.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:24.319790 aeronet_raster-0.1.0a6/aeronet_raster/bandcollection/
--rw-r--r--   0 trekin     (501) staff       (20)       98 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/bandcollection/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     7447 2023-07-25 06:42:12.000000 aeronet_raster-0.1.0a6/aeronet_raster/bandcollection/bandcollection.py
--rw-r--r--   0 trekin     (501) staff       (20)     5935 2023-07-25 06:42:47.000000 aeronet_raster-0.1.0a6/aeronet_raster/bandcollection/bandcollectionsample.py
--rw-r--r--   0 trekin     (501) staff       (20)    10643 2023-07-24 14:19:26.000000 aeronet_raster-0.1.0a6/aeronet_raster/collectionprocessor.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:24.320424 aeronet_raster-0.1.0a6/aeronet_raster/geoobject/
--rw-r--r--   0 trekin     (501) staff       (20)       32 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/geoobject/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     2642 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/geoobject/geoobject.py
--rw-r--r--   0 trekin     (501) staff       (20)     1997 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/merge.py
--rw-r--r--   0 trekin     (501) staff       (20)     5729 2023-07-24 13:07:04.000000 aeronet_raster-0.1.0a6/aeronet_raster/split.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:24.321306 aeronet_raster-0.1.0a6/aeronet_raster/utils/
--rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/utils/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     1267 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a6/aeronet_raster/utils/coords.py
--rw-r--r--   0 trekin     (501) staff       (20)     1796 2023-07-24 13:27:46.000000 aeronet_raster-0.1.0a6/aeronet_raster/utils/utils.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 06:48:24.317886 aeronet_raster-0.1.0a6/aeronet_raster.egg-info/
--rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-25 06:48:24.000000 aeronet_raster-0.1.0a6/aeronet_raster.egg-info/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)      758 2023-07-25 06:48:24.000000 aeronet_raster-0.1.0a6/aeronet_raster.egg-info/SOURCES.txt
--rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-25 06:48:24.000000 aeronet_raster-0.1.0a6/aeronet_raster.egg-info/dependency_links.txt
--rw-r--r--   0 trekin     (501) staff       (20)       49 2023-07-25 06:48:24.000000 aeronet_raster-0.1.0a6/aeronet_raster.egg-info/requires.txt
--rw-r--r--   0 trekin     (501) staff       (20)       15 2023-07-25 06:48:24.000000 aeronet_raster-0.1.0a6/aeronet_raster.egg-info/top_level.txt
--rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-25 06:48:24.322032 aeronet_raster-0.1.0a6/setup.cfg
--rw-r--r--   0 trekin     (501) staff       (20)     3757 2023-07-24 06:59:44.000000 aeronet_raster-0.1.0a6/setup.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:09.820060 aeronet_raster-0.1.0a7/
+-rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-25 07:15:09.819542 aeronet_raster-0.1.0a7/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)     4784 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a7/README.rst
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:09.808475 aeronet_raster-0.1.0a7/aeronet_raster/
+-rw-r--r--   0 trekin     (501) staff       (20)      392 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a7/aeronet_raster/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-25 07:14:31.000000 aeronet_raster-0.1.0a7/aeronet_raster/__version__.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:09.813405 aeronet_raster-0.1.0a7/aeronet_raster/band/
+-rw-r--r--   0 trekin     (501) staff       (20)       58 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a7/aeronet_raster/band/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)    16937 2023-07-25 07:12:58.000000 aeronet_raster-0.1.0a7/aeronet_raster/band/band.py
+-rw-r--r--   0 trekin     (501) staff       (20)    12101 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a7/aeronet_raster/band/bandsample.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:09.815356 aeronet_raster-0.1.0a7/aeronet_raster/bandcollection/
+-rw-r--r--   0 trekin     (501) staff       (20)       98 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a7/aeronet_raster/bandcollection/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     7392 2023-07-25 07:13:43.000000 aeronet_raster-0.1.0a7/aeronet_raster/bandcollection/bandcollection.py
+-rw-r--r--   0 trekin     (501) staff       (20)     5935 2023-07-25 06:42:47.000000 aeronet_raster-0.1.0a7/aeronet_raster/bandcollection/bandcollectionsample.py
+-rw-r--r--   0 trekin     (501) staff       (20)    10643 2023-07-24 14:19:26.000000 aeronet_raster-0.1.0a7/aeronet_raster/collectionprocessor.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:09.816517 aeronet_raster-0.1.0a7/aeronet_raster/geoobject/
+-rw-r--r--   0 trekin     (501) staff       (20)       32 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a7/aeronet_raster/geoobject/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     2642 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a7/aeronet_raster/geoobject/geoobject.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1997 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a7/aeronet_raster/merge.py
+-rw-r--r--   0 trekin     (501) staff       (20)     5729 2023-07-24 13:07:04.000000 aeronet_raster-0.1.0a7/aeronet_raster/split.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:09.818779 aeronet_raster-0.1.0a7/aeronet_raster/utils/
+-rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a7/aeronet_raster/utils/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1267 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a7/aeronet_raster/utils/coords.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1796 2023-07-24 13:27:46.000000 aeronet_raster-0.1.0a7/aeronet_raster/utils/utils.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 07:15:09.811570 aeronet_raster-0.1.0a7/aeronet_raster.egg-info/
+-rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-25 07:15:09.000000 aeronet_raster-0.1.0a7/aeronet_raster.egg-info/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)      758 2023-07-25 07:15:09.000000 aeronet_raster-0.1.0a7/aeronet_raster.egg-info/SOURCES.txt
+-rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-25 07:15:09.000000 aeronet_raster-0.1.0a7/aeronet_raster.egg-info/dependency_links.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       49 2023-07-25 07:15:09.000000 aeronet_raster-0.1.0a7/aeronet_raster.egg-info/requires.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       15 2023-07-25 07:15:09.000000 aeronet_raster-0.1.0a7/aeronet_raster.egg-info/top_level.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-25 07:15:09.820229 aeronet_raster-0.1.0a7/setup.cfg
+-rw-r--r--   0 trekin     (501) staff       (20)     3757 2023-07-24 06:59:44.000000 aeronet_raster-0.1.0a7/setup.py
```

### Comparing `aeronet_raster-0.1.0a6/PKG-INFO` & `aeronet_raster-0.1.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet_raster
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Raster operations for deep learning with remote sensing data. Based on Rasterio.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_raster-0.1.0a6/README.rst` & `aeronet_raster-0.1.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a6/aeronet_raster/band/band.py` & `aeronet_raster-0.1.0a7/aeronet_raster/band/band.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,39 +139,19 @@
     def is_valid(self) -> bool:
         if self._band.count == 1:
             return True
         return False
 
     # ======================== METHODS BLOCK ========================
 
-    def numpy(self, frame: Optional[Union[tuple, np.ndarray]] = None) -> np.ndarray:
+    def numpy(self) -> np.ndarray:
         """
-        Read crop from the raster data into memory as a numpy array
-
-        Args:
-            frame: if None - read all data;
-                  if int - read [[0:frame],[0:frame]] square;
-                  if tuple (xmax, ymax) - read [[0:xmax],[0:ymax]] square;
-                  if tuple ((xmin, ymin), (xmax, ymax)) - read [[xmin:xmax],[ymin:ymax]] square;
-
-        Returns:
-            numpy array containing the whole Band raster data
+        Return numpy representation of the sample
         """
-        if frame is None:
-            frame = ((0, 0), (self.width, self.height))
-        if isinstance(frame, int):
-            frame = ((0, 0), (frame, frame))
-        if isinstance(frame, (tuple, list, np.ndarray)):
-            if len(frame) == 2:
-                if isinstance(frame[0], int) and isinstance(frame[1], int):
-                    frame = ((0, 0), (frame[0], frame[1]))
-
-        dst_nodata = self.nodata if self.nodata is not None else 0
-        return self._band.read(window=((frame[0, 1], frame[1, 1]), (frame[0, 0], frame[1, 0])),
-                               boundless=True, fill_value=dst_nodata)[0].astype(np.uint8)
+        return self.sample(0, 0, self.height, self.width).numpy()
 
     def same(self, other: GeoObject) -> bool:
         """Compare if samples have same resolution, crs and shape.
 
         This means that the samples represent the same territory (like different spectral channels of the same image)
         and can be processed together as collection.
```

### Comparing `aeronet_raster-0.1.0a6/aeronet_raster/band/bandsample.py` & `aeronet_raster-0.1.0a7/aeronet_raster/band/bandsample.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a6/aeronet_raster/bandcollection/bandcollection.py` & `aeronet_raster-0.1.0a7/aeronet_raster/bandcollection/bandcollection.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,9 +196,9 @@
             BandCollectionSample: sequential samples of the specified dimensions
         """
 
         for x in range(0, self.width, width):
             for y in range(0, self.height, height):
                 yield self.sample(y, x, height, width)
 
-    def numpy(self, frame: Optional[Union[tuple, np.ndarray]] = None, ch_axis: int = 0) -> np.ndarray:
-        return np.stack([band.numpy(frame) for band in self._bands], axis=ch_axis)
+    def numpy(self, ch_axis: int = 0) -> np.ndarray:
+        return np.stack([band.numpy() for band in self._bands], axis=ch_axis)
```

### Comparing `aeronet_raster-0.1.0a6/aeronet_raster/bandcollection/bandcollectionsample.py` & `aeronet_raster-0.1.0a7/aeronet_raster/bandcollection/bandcollectionsample.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a6/aeronet_raster/collectionprocessor.py` & `aeronet_raster-0.1.0a7/aeronet_raster/collectionprocessor.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a6/aeronet_raster/geoobject/geoobject.py` & `aeronet_raster-0.1.0a7/aeronet_raster/geoobject/geoobject.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a6/aeronet_raster/merge.py` & `aeronet_raster-0.1.0a7/aeronet_raster/merge.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a6/aeronet_raster/split.py` & `aeronet_raster-0.1.0a7/aeronet_raster/split.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a6/aeronet_raster/utils/coords.py` & `aeronet_raster-0.1.0a7/aeronet_raster/utils/coords.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a6/aeronet_raster/utils/utils.py` & `aeronet_raster-0.1.0a7/aeronet_raster/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a6/aeronet_raster.egg-info/PKG-INFO` & `aeronet_raster-0.1.0a7/aeronet_raster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet-raster
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Raster operations for deep learning with remote sensing data. Based on Rasterio.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_raster-0.1.0a6/aeronet_raster.egg-info/SOURCES.txt` & `aeronet_raster-0.1.0a7/aeronet_raster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a6/setup.py` & `aeronet_raster-0.1.0a7/setup.py`

 * *Files identical despite different names*

