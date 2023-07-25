# Comparing `tmp/unstructured_inference-0.5.6.tar.gz` & `tmp/unstructured_inference-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_inference-0.5.6.tar", last modified: Mon Jul 24 19:17:08 2023, max compression
+gzip compressed data, was "unstructured_inference-0.5.7.tar", last modified: Tue Jul 25 18:24:53 2023, max compression
```

## Comparing `unstructured_inference-0.5.6.tar` & `unstructured_inference-0.5.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:17:08.136584 unstructured_inference-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-24 19:17:08.136584 unstructured_inference-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:17:08.116584 unstructured_inference-0.5.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-24 19:17:08.140585 unstructured_inference-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:17:08.120584 unstructured_inference-0.5.6/unstructured_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:17:08.128584 unstructured_inference-0.5.6/unstructured_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/inference/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/inference/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/inference/layoutelement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/inference/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:17:08.136584 unstructured_inference-0.5.6/unstructured_inference/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/chipper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/detectron2onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/donut.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/paddle_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    24262 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/table_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/tesseract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/unstructuredmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/models/yolox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:17:08.136584 unstructured_inference-0.5.6/unstructured_inference/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/patches/pdfminer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-24 19:14:51.000000 unstructured_inference-0.5.6/unstructured_inference/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:17:08.124584 unstructured_inference-0.5.6/unstructured_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-24 19:17:07.000000 unstructured_inference-0.5.6/unstructured_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-24 19:17:08.000000 unstructured_inference-0.5.6/unstructured_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:17:07.000000 unstructured_inference-0.5.6/unstructured_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-24 19:17:07.000000 unstructured_inference-0.5.6/unstructured_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 19:17:07.000000 unstructured_inference-0.5.6/unstructured_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:53.406677 unstructured_inference-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-25 18:24:53.406677 unstructured_inference-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:53.402677 unstructured_inference-0.5.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-25 18:24:53.410677 unstructured_inference-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:53.402677 unstructured_inference-0.5.7/unstructured_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:53.402677 unstructured_inference-0.5.7/unstructured_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/inference/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/inference/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/inference/layoutelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/inference/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:53.406677 unstructured_inference-0.5.7/unstructured_inference/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/models/chipper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/models/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/models/detectron2onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/models/donut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/models/paddle_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24262 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/models/table_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/models/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/models/tesseract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/models/unstructuredmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/models/yolox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:53.406677 unstructured_inference-0.5.7/unstructured_inference/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/patches/pdfminer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-25 18:22:56.000000 unstructured_inference-0.5.7/unstructured_inference/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:53.402677 unstructured_inference-0.5.7/unstructured_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-25 18:24:53.000000 unstructured_inference-0.5.7/unstructured_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-25 18:24:53.000000 unstructured_inference-0.5.7/unstructured_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:24:53.000000 unstructured_inference-0.5.7/unstructured_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-25 18:24:53.000000 unstructured_inference-0.5.7/unstructured_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 18:24:53.000000 unstructured_inference-0.5.7/unstructured_inference.egg-info/top_level.txt
```

### Comparing `unstructured_inference-0.5.6/PKG-INFO` & `unstructured_inference-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured_inference
-Version: 0.5.6
+Version: 0.5.7
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.5.6/README.md` & `unstructured_inference-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/setup.py` & `unstructured_inference-0.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/inference/elements.py` & `unstructured_inference-0.5.7/unstructured_inference/inference/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/inference/layout.py` & `unstructured_inference-0.5.7/unstructured_inference/inference/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -466,10 +466,12 @@
 def create_image_output_dir(
     filename: Union[str, PurePath],
 ) -> Union[str, PurePath]:
     """Creates a directory to store the converted images from the pdf pages and returns the
     directory path"""
     parent_dir = os.path.abspath(os.path.dirname(filename))
     f_name_without_extension = os.path.splitext(os.path.basename(filename))[0]
-    output_dir = os.path.join(parent_dir, f_name_without_extension)
+
+    # Add a suffix to avoid conflicts in case original file doesn't have an extension
+    output_dir = os.path.join(parent_dir, f"{f_name_without_extension}_images")
     os.makedirs(output_dir, exist_ok=True)
     return output_dir
```

### Comparing `unstructured_inference-0.5.6/unstructured_inference/inference/layoutelement.py` & `unstructured_inference-0.5.7/unstructured_inference/inference/layoutelement.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/inference/ordering.py` & `unstructured_inference-0.5.7/unstructured_inference/inference/ordering.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/logger.py` & `unstructured_inference-0.5.7/unstructured_inference/logger.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/models/base.py` & `unstructured_inference-0.5.7/unstructured_inference/models/base.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/models/chipper.py` & `unstructured_inference-0.5.7/unstructured_inference/models/chipper.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/models/detectron2.py` & `unstructured_inference-0.5.7/unstructured_inference/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/models/detectron2onnx.py` & `unstructured_inference-0.5.7/unstructured_inference/models/detectron2onnx.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/models/donut.py` & `unstructured_inference-0.5.7/unstructured_inference/models/donut.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/models/table_postprocess.py` & `unstructured_inference-0.5.7/unstructured_inference/models/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/models/tables.py` & `unstructured_inference-0.5.7/unstructured_inference/models/tables.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/models/tesseract.py` & `unstructured_inference-0.5.7/unstructured_inference/models/tesseract.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/models/unstructuredmodel.py` & `unstructured_inference-0.5.7/unstructured_inference/models/unstructuredmodel.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/models/yolox.py` & `unstructured_inference-0.5.7/unstructured_inference/models/yolox.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/patches/pdfminer.py` & `unstructured_inference-0.5.7/unstructured_inference/patches/pdfminer.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/utils.py` & `unstructured_inference-0.5.7/unstructured_inference/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference/visualize.py` & `unstructured_inference-0.5.7/unstructured_inference/visualize.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.6/unstructured_inference.egg-info/PKG-INFO` & `unstructured_inference-0.5.7/unstructured_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured-inference
-Version: 0.5.6
+Version: 0.5.7
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.5.6/unstructured_inference.egg-info/SOURCES.txt` & `unstructured_inference-0.5.7/unstructured_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

