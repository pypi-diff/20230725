# Comparing `tmp/aeronet_raster-0.1.0a4.tar.gz` & `tmp/aeronet_raster-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet_raster-0.1.0a4.tar", last modified: Mon Jul 24 13:30:39 2023, max compression
+gzip compressed data, was "aeronet_raster-0.1.0a5.tar", last modified: Tue Jul 25 05:37:14 2023, max compression
```

## Comparing `aeronet_raster-0.1.0a4.tar` & `aeronet_raster-0.1.0a5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:30:39.545996 aeronet_raster-0.1.0a4/
--rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-24 13:30:39.544285 aeronet_raster-0.1.0a4/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)     4784 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a4/README.rst
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:30:39.531464 aeronet_raster-0.1.0a4/aeronet_raster/
--rw-r--r--   0 trekin     (501) staff       (20)      392 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-24 13:30:18.000000 aeronet_raster-0.1.0a4/aeronet_raster/__version__.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:30:39.537522 aeronet_raster-0.1.0a4/aeronet_raster/band/
--rw-r--r--   0 trekin     (501) staff       (20)       58 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster/band/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)    17952 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster/band/band.py
--rw-r--r--   0 trekin     (501) staff       (20)    12101 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster/band/bandsample.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:30:39.539547 aeronet_raster-0.1.0a4/aeronet_raster/bandcollection/
--rw-r--r--   0 trekin     (501) staff       (20)       98 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster/bandcollection/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     7413 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster/bandcollection/bandcollection.py
--rw-r--r--   0 trekin     (501) staff       (20)     5936 2023-07-21 14:48:40.000000 aeronet_raster-0.1.0a4/aeronet_raster/bandcollection/bandcollectionsample.py
--rw-r--r--   0 trekin     (501) staff       (20)    10679 2023-07-24 13:11:22.000000 aeronet_raster-0.1.0a4/aeronet_raster/collectionprocessor.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:30:39.540766 aeronet_raster-0.1.0a4/aeronet_raster/geoobject/
--rw-r--r--   0 trekin     (501) staff       (20)       32 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster/geoobject/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     2642 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster/geoobject/geoobject.py
--rw-r--r--   0 trekin     (501) staff       (20)     1997 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster/merge.py
--rw-r--r--   0 trekin     (501) staff       (20)     5729 2023-07-24 13:07:04.000000 aeronet_raster-0.1.0a4/aeronet_raster/split.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:30:39.542466 aeronet_raster-0.1.0a4/aeronet_raster/utils/
--rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster/utils/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)     1267 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster/utils/coords.py
--rw-r--r--   0 trekin     (501) staff       (20)     1796 2023-07-24 13:27:46.000000 aeronet_raster-0.1.0a4/aeronet_raster/utils/utils.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 13:30:39.535404 aeronet_raster-0.1.0a4/aeronet_raster.egg-info/
--rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-24 13:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster.egg-info/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)      758 2023-07-24 13:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster.egg-info/SOURCES.txt
--rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-24 13:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster.egg-info/dependency_links.txt
--rw-r--r--   0 trekin     (501) staff       (20)       49 2023-07-24 13:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster.egg-info/requires.txt
--rw-r--r--   0 trekin     (501) staff       (20)       15 2023-07-24 13:30:39.000000 aeronet_raster-0.1.0a4/aeronet_raster.egg-info/top_level.txt
--rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-24 13:30:39.546212 aeronet_raster-0.1.0a4/setup.cfg
--rw-r--r--   0 trekin     (501) staff       (20)     3757 2023-07-24 06:59:44.000000 aeronet_raster-0.1.0a4/setup.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:14.125111 aeronet_raster-0.1.0a5/
+-rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-25 05:37:14.124817 aeronet_raster-0.1.0a5/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)     4784 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/README.rst
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:14.119211 aeronet_raster-0.1.0a5/aeronet_raster/
+-rw-r--r--   0 trekin     (501) staff       (20)      392 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-24 14:22:22.000000 aeronet_raster-0.1.0a5/aeronet_raster/__version__.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:14.121887 aeronet_raster-0.1.0a5/aeronet_raster/band/
+-rw-r--r--   0 trekin     (501) staff       (20)       58 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/band/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)    17952 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/band/band.py
+-rw-r--r--   0 trekin     (501) staff       (20)    12101 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/band/bandsample.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:14.122884 aeronet_raster-0.1.0a5/aeronet_raster/bandcollection/
+-rw-r--r--   0 trekin     (501) staff       (20)       98 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/bandcollection/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     7448 2023-07-24 14:21:08.000000 aeronet_raster-0.1.0a5/aeronet_raster/bandcollection/bandcollection.py
+-rw-r--r--   0 trekin     (501) staff       (20)     5936 2023-07-21 14:48:40.000000 aeronet_raster-0.1.0a5/aeronet_raster/bandcollection/bandcollectionsample.py
+-rw-r--r--   0 trekin     (501) staff       (20)    10643 2023-07-24 14:19:26.000000 aeronet_raster-0.1.0a5/aeronet_raster/collectionprocessor.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:14.123543 aeronet_raster-0.1.0a5/aeronet_raster/geoobject/
+-rw-r--r--   0 trekin     (501) staff       (20)       32 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/geoobject/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     2642 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/geoobject/geoobject.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1997 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/merge.py
+-rw-r--r--   0 trekin     (501) staff       (20)     5729 2023-07-24 13:07:04.000000 aeronet_raster-0.1.0a5/aeronet_raster/split.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:14.124431 aeronet_raster-0.1.0a5/aeronet_raster/utils/
+-rw-r--r--   0 trekin     (501) staff       (20)        0 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/utils/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1267 2023-07-21 05:30:39.000000 aeronet_raster-0.1.0a5/aeronet_raster/utils/coords.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1796 2023-07-24 13:27:46.000000 aeronet_raster-0.1.0a5/aeronet_raster/utils/utils.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-25 05:37:14.120863 aeronet_raster-0.1.0a5/aeronet_raster.egg-info/
+-rw-r--r--   0 trekin     (501) staff       (20)      704 2023-07-25 05:37:14.000000 aeronet_raster-0.1.0a5/aeronet_raster.egg-info/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)      758 2023-07-25 05:37:14.000000 aeronet_raster-0.1.0a5/aeronet_raster.egg-info/SOURCES.txt
+-rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-25 05:37:14.000000 aeronet_raster-0.1.0a5/aeronet_raster.egg-info/dependency_links.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       49 2023-07-25 05:37:14.000000 aeronet_raster-0.1.0a5/aeronet_raster.egg-info/requires.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       15 2023-07-25 05:37:14.000000 aeronet_raster-0.1.0a5/aeronet_raster.egg-info/top_level.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-25 05:37:14.125196 aeronet_raster-0.1.0a5/setup.cfg
+-rw-r--r--   0 trekin     (501) staff       (20)     3757 2023-07-24 06:59:44.000000 aeronet_raster-0.1.0a5/setup.py
```

### Comparing `aeronet_raster-0.1.0a4/PKG-INFO` & `aeronet_raster-0.1.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet_raster
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Raster operations for deep learning with remote sensing data. Based on Rasterio.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_raster-0.1.0a4/README.rst` & `aeronet_raster-0.1.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a4/aeronet_raster/band/band.py` & `aeronet_raster-0.1.0a5/aeronet_raster/band/band.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a4/aeronet_raster/band/bandsample.py` & `aeronet_raster-0.1.0a5/aeronet_raster/band/bandsample.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a4/aeronet_raster/bandcollection/bandcollection.py` & `aeronet_raster-0.1.0a5/aeronet_raster/bandcollection/bandcollection.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     @property
     def bounds(self):
         return self._bands[0].bounds
 
     @property
     def shape(self) -> tuple:
-        return self._bands[0].shape
+        return self.count, self._bands[0].height, self._bands[0].width
 
     @property
     def res(self) -> tuple:
         return self._bands[0].res
 
     @property
     def bands(self) -> list:
```

### Comparing `aeronet_raster-0.1.0a4/aeronet_raster/bandcollection/bandcollectionsample.py` & `aeronet_raster-0.1.0a5/aeronet_raster/bandcollection/bandcollectionsample.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a4/aeronet_raster/collectionprocessor.py` & `aeronet_raster-0.1.0a5/aeronet_raster/collectionprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,22 +246,21 @@
 
     def _processing(self, sample: np.ndarray, block: dict, dst: SampleCollectionWindowWriter):
         raster = self.processing_fn(sample)
         with self.lock:
             dst.write(raster, **block)
 
     def process(self, bc: BandCollection, output_directory: str) -> BandCollection:
-        shape = bc.shape[1], bc.shape[0]
         src = SequentialSampler(bc, self.input_channels, self.sample_size, self.bound)
         dst = SampleCollectionWindowWriter(output_directory, self.output_labels,
-                                           shape, **bc.profile, **self.kwargs)
+                                           bc.shape[1:], **bc.profile, **self.kwargs)
 
-        args = ((sample.numpy(), block, dst) for sample, block in src)
-        blocks_num = ((shape[0] + self.bound) // self.sample_size[0] + 1) * \
-                     ((shape[1] + self.bound) // self.sample_size[1] + 1)
+        args = ((sample, block, dst) for sample, block in src)
+        blocks_num = ((bc.shape[1] + self.bound) // self.sample_size[0] + 1) * \
+                     ((bc.shape[2] + self.bound) // self.sample_size[1] + 1)
 
         if self.n_workers > 1:
             with ThreadPool(self.n_workers) as p:
                 with tqdm(total=blocks_num, disable=(not self.verbose)) as pbar:
                     for _ in p.imap(self._threaded_processing, args):
                         pbar.update()
         else:
```

### Comparing `aeronet_raster-0.1.0a4/aeronet_raster/geoobject/geoobject.py` & `aeronet_raster-0.1.0a5/aeronet_raster/geoobject/geoobject.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a4/aeronet_raster/merge.py` & `aeronet_raster-0.1.0a5/aeronet_raster/merge.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a4/aeronet_raster/split.py` & `aeronet_raster-0.1.0a5/aeronet_raster/split.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a4/aeronet_raster/utils/coords.py` & `aeronet_raster-0.1.0a5/aeronet_raster/utils/coords.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a4/aeronet_raster/utils/utils.py` & `aeronet_raster-0.1.0a5/aeronet_raster/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a4/aeronet_raster.egg-info/PKG-INFO` & `aeronet_raster-0.1.0a5/aeronet_raster.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet-raster
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Raster operations for deep learning with remote sensing data. Based on Rasterio.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_raster-0.1.0a4/aeronet_raster.egg-info/SOURCES.txt` & `aeronet_raster-0.1.0a5/aeronet_raster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.1.0a4/setup.py` & `aeronet_raster-0.1.0a5/setup.py`

 * *Files identical despite different names*

