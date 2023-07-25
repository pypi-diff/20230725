# Comparing `tmp/moosez-2.2.6.tar.gz` & `tmp/moosez-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.2.6.tar", last modified: Tue Jul 25 12:14:34 2023, max compression
+gzip compressed data, was "moosez-2.2.7.tar", last modified: Tue Jul 25 12:18:15 2023, max compression
```

## Comparing `moosez-2.2.6.tar` & `moosez-2.2.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:14:34.767500 moosez-2.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 12:14:21.000000 moosez-2.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 12:14:34.767500 moosez-2.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-07-25 12:14:21.000000 moosez-2.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:14:34.767500 moosez-2.2.6/moosez/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-25 12:14:21.000000 moosez-2.2.6/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-25 12:14:21.000000 moosez-2.2.6/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-25 12:14:21.000000 moosez-2.2.6/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-25 12:14:21.000000 moosez-2.2.6/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-25 12:14:21.000000 moosez-2.2.6/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-25 12:14:21.000000 moosez-2.2.6/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-07-25 12:14:21.000000 moosez-2.2.6/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-25 12:14:21.000000 moosez-2.2.6/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-25 12:14:21.000000 moosez-2.2.6/moosez/moosez.py
--rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-07-25 12:14:21.000000 moosez-2.2.6/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-07-25 12:14:21.000000 moosez-2.2.6/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:14:34.767500 moosez-2.2.6/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 12:14:34.000000 moosez-2.2.6/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-25 12:14:34.000000 moosez-2.2.6/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:14:34.000000 moosez-2.2.6/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 12:14:34.000000 moosez-2.2.6/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-25 12:14:34.000000 moosez-2.2.6/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 12:14:34.000000 moosez-2.2.6/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 12:14:34.767500 moosez-2.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-25 12:14:21.000000 moosez-2.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:18:15.891989 moosez-2.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 12:17:58.000000 moosez-2.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 12:18:15.891989 moosez-2.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-07-25 12:17:58.000000 moosez-2.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:18:15.891989 moosez-2.2.7/moosez/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/moosez.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-07-25 12:17:58.000000 moosez-2.2.7/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:18:15.891989 moosez-2.2.7/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 12:18:15.000000 moosez-2.2.7/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-25 12:18:15.000000 moosez-2.2.7/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:18:15.000000 moosez-2.2.7/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 12:18:15.000000 moosez-2.2.7/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-25 12:18:15.000000 moosez-2.2.7/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 12:18:15.000000 moosez-2.2.7/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 12:18:15.891989 moosez-2.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-25 12:17:58.000000 moosez-2.2.7/setup.py
```

### Comparing `moosez-2.2.6/LICENSE` & `moosez-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.2.6/PKG-INFO` & `moosez-2.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.2.6
+Version: 2.2.7
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.2.6/README.md` & `moosez-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.2.6/moosez/constants.py` & `moosez-2.2.7/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.6/moosez/display.py` & `moosez-2.2.7/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.6/moosez/download.py` & `moosez-2.2.7/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.6/moosez/file_utilities.py` & `moosez-2.2.7/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.6/moosez/image_conversion.py` & `moosez-2.2.7/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.6/moosez/image_processing.py` & `moosez-2.2.7/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.6/moosez/input_validation.py` & `moosez-2.2.7/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.6/moosez/moosez.py` & `moosez-2.2.7/moosez/moosez.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.6/moosez/predict.py` & `moosez-2.2.7/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.2.6/moosez/resources.py` & `moosez-2.2.7/moosez/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,59 +46,59 @@
 #    - voxel_spacing: The voxel spacing used in the model in the form [x, y, z], this is basically the median voxel
 #    spacing generated by nnunetv2, and you can find this in the plans.json file of the model.
 #    - multilabel_prefix: A prefix to distinguish between different types of labels in multi-label models.
 #
 # To include your own model, add a new entry to this dictionary following the above format.
 
 MODELS = {
-    "clin_ct_lungs": {
+    "clin_ct_lungs_v2": {
         "nnunet_version": "v2",
         "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/clin_ct_lungs_24062023.zip",
         "filename": "Dataset333_HMS3dlungs.zip",
         "directory": "Dataset333_HMS3dlungs",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Lungs_",
         "model_type": None,
         "fold": None,
     },
-    "clin_ct_organs": {
+    "clin_ct_organs_v2": {
         "nnunet_version": "v2",
         "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/MOOSEv2_bspline_organs23062023.zip",
         "filename": "Dataset123_Organs.zip",
         "directory": "Dataset123_Organs",
         "trainer": "nnUNetTrainer_2000epochs_NoMirroring",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Organs_",
         "model_type": None,
         "fold": None,
     },
-    "clin_pt_fdg_tumor": {
+    "clin_pt_fdg_tumor_v2": {
         "nnunet_version": "v2",
         "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/Dataset789_Tumors.zip",
         "filename": "Dataset789_Tumors.zip",
         "directory": "Dataset789_Tumors",
         "trainer": "nnUNetTrainerDA5",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "PT_FDG_Tumor_",
         "model_type": None,
         "fold": None,
     },
-    "preclin_mr_all": {
+    "preclin_mr_all_v2": {
         "nnunet_version": "v2",
         "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/preclin_mr_14062023.zip",
         "filename": "Dataset234_Preclin.zip",
         "directory": "Dataset234_Preclin",
         "trainer": "nnUNetTrainerNoMirroring",
         "voxel_spacing": [0.15, 0.15, 0.15],
         "multilabel_prefix": "Preclin_MR_all_",
         "model_type": None,
         "fold": None,
     },
-    "clin_ct_body": {
+    "clin_ct_body_v2": {
         "nnunet_version": "v2",
         "url": "https://moose-files.s3.eu-de.cloud-object-storage.appdomain.cloud/Dataset696_BodyContour.zip",
         "filename": "Dataset696_BodyContour.zip",
         "directory": "Dataset696_BodyContour",
         "trainer": "nnUNetTrainer",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "CT_Body_",
```

### Comparing `moosez-2.2.6/moosez.egg-info/PKG-INFO` & `moosez-2.2.7/moosez.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.2.6
+Version: 2.2.7
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.2.6/setup.py` & `moosez-2.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='moosez',
-    version='2.2.6',
+    version='2.2.7',
     author='Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
```

