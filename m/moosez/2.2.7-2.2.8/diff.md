# Comparing `tmp/moosez-2.2.7.tar.gz` & `tmp/moosez-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.2.7.tar", last modified: Tue Jul 25 12:18:15 2023, max compression
+gzip compressed data, was "moosez-2.2.8.tar", last modified: Tue Jul 25 12:39:12 2023, max compression
```

## Comparing `moosez-2.2.7.tar` & `moosez-2.2.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:18:15.891989 moosez-2.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 12:17:58.000000 moosez-2.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 12:18:15.891989 moosez-2.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-07-25 12:17:58.000000 moosez-2.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:18:15.891989 moosez-2.2.7/moosez/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/moosez.py
--rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:18:15.891989 moosez-2.2.7/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 12:18:15.000000 moosez-2.2.7/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-25 12:18:15.000000 moosez-2.2.7/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:18:15.000000 moosez-2.2.7/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 12:18:15.000000 moosez-2.2.7/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-25 12:18:15.000000 moosez-2.2.7/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 12:18:15.000000 moosez-2.2.7/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 12:18:15.891989 moosez-2.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-25 12:17:58.000000 moosez-2.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:39:12.026388 moosez-2.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 12:38:54.000000 moosez-2.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 12:39:12.026388 moosez-2.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-07-25 12:38:54.000000 moosez-2.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:39:12.022388 moosez-2.2.8/moosez/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/moosez.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-07-25 12:38:54.000000 moosez-2.2.8/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:39:12.022388 moosez-2.2.8/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 12:39:12.000000 moosez-2.2.8/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-25 12:39:12.000000 moosez-2.2.8/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:39:12.000000 moosez-2.2.8/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 12:39:12.000000 moosez-2.2.8/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-25 12:39:12.000000 moosez-2.2.8/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 12:39:12.000000 moosez-2.2.8/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 12:39:12.026388 moosez-2.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-25 12:38:54.000000 moosez-2.2.8/setup.py
```

### Comparing `moosez-2.2.7/LICENSE` & `moosez-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.2.7/PKG-INFO` & `moosez-2.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.2.7
+Version: 2.2.8
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.2.7/README.md` & `moosez-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.2.7/moosez/constants.py` & `moosez-2.2.8/moosez/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,16 @@
         5: 'Heart',
         6: 'Kidneys',
         7: 'Liver',
         8: 'Pancreas',
         9: 'Spleen',
         10: 'Thyroid',
         11: 'Inferior-vena-cava',
-        12: 'Lung'
+        12: 'Skeleton',
+        13: 'Lung'
     },
     "clin_ct_bones_v1": {
         1: 'Carpal',
         2: 'Clavicle',
         3: 'Femur',
         4: 'Fibula',
         5: 'Humerus',
```

### Comparing `moosez-2.2.7/moosez/display.py` & `moosez-2.2.8/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.7/moosez/download.py` & `moosez-2.2.8/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.7/moosez/file_utilities.py` & `moosez-2.2.8/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.7/moosez/image_conversion.py` & `moosez-2.2.8/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.7/moosez/image_processing.py` & `moosez-2.2.8/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.7/moosez/input_validation.py` & `moosez-2.2.8/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.7/moosez/moosez.py` & `moosez-2.2.8/moosez/moosez.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.7/moosez/predict.py` & `moosez-2.2.8/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.7/moosez/resources.py` & `moosez-2.2.8/moosez/resources.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.7/moosez.egg-info/PKG-INFO` & `moosez-2.2.8/moosez.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.2.7
+Version: 2.2.8
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.2.7/setup.py` & `moosez-2.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='moosez',
-    version='2.2.7',
+    version='2.2.8',
     author='Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
```

