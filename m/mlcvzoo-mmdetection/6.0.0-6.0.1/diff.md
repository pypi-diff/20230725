# Comparing `tmp/mlcvzoo_mmdetection-6.0.0.tar.gz` & `tmp/mlcvzoo_mmdetection-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_mmdetection-6.0.0.tar", max compression
+gzip compressed data, was "mlcvzoo_mmdetection-6.0.1.tar", max compression
```

## Comparing `mlcvzoo_mmdetection-6.0.0.tar` & `mlcvzoo_mmdetection-6.0.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    11412 2023-06-12 09:08:46.196127 mlcvzoo_mmdetection-6.0.0/LICENSE
--rw-r--r--   0        0        0      423 2023-06-12 09:08:46.196127 mlcvzoo_mmdetection-6.0.0/README.md
--rw-r--r--   0        0        0      244 2023-06-13 14:54:27.168223 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/__init__.py
--rw-r--r--   0        0        0     5716 2023-06-13 09:14:59.550114 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/configuration.py
--rw-r--r--   0        0        0     6817 2023-06-13 09:14:59.550114 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py
--rw-r--r--   0        0        0    13641 2023-06-13 09:14:59.550114 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/model.py
--rw-r--r--   0        0        0     7394 2023-06-12 09:08:46.196127 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/object_detection_model.py
--rw-r--r--   0        0        0      196 2023-06-12 09:08:46.196127 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/py.typed
--rw-r--r--   0        0        0    10928 2023-06-13 09:14:59.550114 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/segmentation_model.py
--rw-r--r--   0        0        0     1938 2023-06-13 09:14:59.550114 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/utils.py
--rw-r--r--   0        0        0     4294 2023-06-13 14:54:27.172223 mlcvzoo_mmdetection-6.0.0/pyproject.toml
--rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-6.0.0/setup.py
--rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11412 2023-07-25 09:11:15.684266 mlcvzoo_mmdetection-6.0.1/LICENSE
+-rw-r--r--   0        0        0      423 2023-07-25 09:11:15.684266 mlcvzoo_mmdetection-6.0.1/README.md
+-rw-r--r--   0        0        0      244 2023-07-25 11:03:15.993091 mlcvzoo_mmdetection-6.0.1/mlcvzoo_mmdetection/__init__.py
+-rw-r--r--   0        0        0     5716 2023-07-25 09:11:15.688266 mlcvzoo_mmdetection-6.0.1/mlcvzoo_mmdetection/configuration.py
+-rw-r--r--   0        0        0     6948 2023-07-25 11:03:15.993091 mlcvzoo_mmdetection-6.0.1/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py
+-rw-r--r--   0        0        0    13641 2023-07-25 09:11:15.688266 mlcvzoo_mmdetection-6.0.1/mlcvzoo_mmdetection/model.py
+-rw-r--r--   0        0        0     7394 2023-07-25 09:11:15.688266 mlcvzoo_mmdetection-6.0.1/mlcvzoo_mmdetection/object_detection_model.py
+-rw-r--r--   0        0        0      196 2023-07-25 09:11:15.688266 mlcvzoo_mmdetection-6.0.1/mlcvzoo_mmdetection/py.typed
+-rw-r--r--   0        0        0    10928 2023-07-25 09:11:15.688266 mlcvzoo_mmdetection-6.0.1/mlcvzoo_mmdetection/segmentation_model.py
+-rw-r--r--   0        0        0     1938 2023-07-25 09:11:15.688266 mlcvzoo_mmdetection-6.0.1/mlcvzoo_mmdetection/utils.py
+-rw-r--r--   0        0        0     4294 2023-07-25 11:03:15.997091 mlcvzoo_mmdetection-6.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-6.0.1/PKG-INFO
```

### Comparing `mlcvzoo_mmdetection-6.0.0/LICENSE` & `mlcvzoo_mmdetection-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/configuration.py` & `mlcvzoo_mmdetection-6.0.1/mlcvzoo_mmdetection/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py` & `mlcvzoo_mmdetection-6.0.1/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,52 +94,53 @@
             annotation_handler = AnnotationHandler(
                 configuration=configuration,
             )
             # Load annotations and model classes from annotation handler
             self.annotations = annotation_handler.parse_training_annotations()
             self.CLASSES = annotation_handler.mapper.get_model_class_names()
 
-        self._with_bbox: bool = True
-        self._with_mask: bool = True
+        self._with_bbox: bool = False
+        self._with_mask: bool = False
         pipeline = kwargs.get("pipeline")
         if pipeline is not None:
             annotation_pipelines = [
                 p for p in pipeline if p["type"] == "LoadAnnotations"
             ]
 
             # Handle with_seg if we need to train panoptic segmentation models
             # self.with_seg: bool
             if len(annotation_pipelines) > 0:
-                _with_mask: Optional[bool] = annotation_pipelines[0].get("with_mask")
-                if _with_mask is not None:
-                    self._with_bbox = _with_mask
                 _with_bbox: Optional[bool] = annotation_pipelines[0].get("with_bbox")
                 if _with_bbox is not None:
-                    self._with_mask = _with_bbox
+                    self._with_bbox = _with_bbox
+                _with_mask: Optional[bool] = annotation_pipelines[0].get("with_mask")
+                if _with_mask is not None:
+                    self._with_mask = _with_mask
 
         BaseDetDataset.__init__(self, *args, **kwargs)
 
     def load_data_list(self) -> List[Dict[str, Any]]:
         data_list: List[Dict[str, Any]] = []
 
+        # TODO: Handle ignore flag if present in kwargs
         for img_id, annotation in enumerate(self.annotations):
             instances: List[Dict[str, Any]] = []
-            # TODO: Handle ignore flag if present in kwargs
             if self._with_bbox and not self._with_mask:
                 # Object detection training - train only on bounding boxes
                 for bounding_box in annotation.bounding_boxes:
                     instances.append(
                         {
                             "ignore_flag": 0,
                             "ignore": 0,
                             "bbox_label": bounding_box.class_id,
                             "bbox": bounding_box.box.to_list(dst_type=float),
                         }
                     )
-
+            # TODO: Allow to use bbox and mask for segmentation training?!
+            # elif if self._with_bbox and self._with_mask:
             elif self._with_mask:
                 # Segmentation training - train with masks and bounding boxes
                 for segmentation in annotation.segmentations:
                     if segmentation.box is None:
                         box = segmentation.to_bounding_box().box
                     else:
                         box = segmentation.box
```

### Comparing `mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/model.py` & `mlcvzoo_mmdetection-6.0.1/mlcvzoo_mmdetection/model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/object_detection_model.py` & `mlcvzoo_mmdetection-6.0.1/mlcvzoo_mmdetection/object_detection_model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/segmentation_model.py` & `mlcvzoo_mmdetection-6.0.1/mlcvzoo_mmdetection/segmentation_model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/utils.py` & `mlcvzoo_mmdetection-6.0.1/mlcvzoo_mmdetection/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-6.0.0/pyproject.toml` & `mlcvzoo_mmdetection-6.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mlcvzoo_mmdetection"
 description = "MLCVZoo MMDetection Package"
-version = "6.0.0"
+version = "6.0.1"
 license = "Open Logistics Foundation License 1.3"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `mlcvzoo_mmdetection-6.0.0/PKG-INFO` & `mlcvzoo_mmdetection-6.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-mmdetection
-Version: 6.0.0
+Version: 6.0.1
 Summary: MLCVZoo MMDetection Package
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 License: Open Logistics Foundation License 1.3
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

