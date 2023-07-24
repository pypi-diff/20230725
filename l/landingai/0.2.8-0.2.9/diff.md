# Comparing `tmp/landingai-0.2.8.tar.gz` & `tmp/landingai-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingai-0.2.8.tar", max compression
+gzip compressed data, was "landingai-0.2.9.tar", max compression
```

## Comparing `landingai-0.2.8.tar` & `landingai-0.2.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1063 2023-07-19 00:57:21.427837 landingai-0.2.8/LICENSE.md
--rw-r--r--   0        0        0     6743 2023-07-19 00:57:21.427837 landingai-0.2.8/README.md
--rw-r--r--   0        0        0      354 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/__init__.py
--rw-r--r--   0        0        0     6451 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/common.py
--rw-r--r--   0        0        0       72 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/data_management/__init__.py
--rw-r--r--   0        0        0     8714 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/data_management/client.py
--rw-r--r--   0        0        0    21178 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/data_management/media.py
--rw-r--r--   0        0        0     4722 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/data_management/metadata.py
--rw-r--r--   0        0        0     2188 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/data_management/utils.py
--rw-r--r--   0        0        0     9730 2023-07-19 00:57:21.455837 landingai-0.2.8/landingai/exceptions.py
--rw-r--r--   0        0        0  1594400 2023-07-19 00:57:21.463837 landingai-0.2.8/landingai/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     5915 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/image_source_ops.py
--rw-r--r--   0        0        0     1502 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/notebook_utils.py
--rw-r--r--   0        0        0      420 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/pipeline/__init__.py
--rw-r--r--   0        0        0    16449 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/pipeline/frameset.py
--rw-r--r--   0        0        0    11810 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/pipeline/image_source.py
--rw-r--r--   0        0        0     1339 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/pipeline/postprocessing.py
--rw-r--r--   0        0        0     8389 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/postprocess.py
--rw-r--r--   0        0        0    25677 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/predict.py
--rw-r--r--   0        0        0     6462 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/st_utils.py
--rw-r--r--   0        0        0       40 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/storage/__init__.py
--rw-r--r--   0        0        0     4439 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/storage/data_access.py
--rw-r--r--   0        0        0     4340 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/storage/snowflake.py
--rw-r--r--   0        0        0     1503 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/telemetry.py
--rw-r--r--   0        0        0     5869 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/timer.py
--rw-r--r--   0        0        0     1685 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/transform.py
--rw-r--r--   0        0        0     2812 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/utils.py
--rw-r--r--   0        0        0    13403 2023-07-19 00:57:21.467837 landingai-0.2.8/landingai/visualize.py
--rw-r--r--   0        0        0     2606 2023-07-19 00:57:22.255844 landingai-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     7988 1970-01-01 00:00:00.000000 landingai-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-19 21:47:22.420853 landingai-0.2.9/LICENSE.md
+-rw-r--r--   0        0        0     6743 2023-07-19 21:47:22.420853 landingai-0.2.9/README.md
+-rw-r--r--   0        0        0      354 2023-07-19 21:47:22.452853 landingai-0.2.9/landingai/__init__.py
+-rw-r--r--   0        0        0     6451 2023-07-19 21:47:22.452853 landingai-0.2.9/landingai/common.py
+-rw-r--r--   0        0        0       72 2023-07-19 21:47:22.452853 landingai-0.2.9/landingai/data_management/__init__.py
+-rw-r--r--   0        0        0     8714 2023-07-19 21:47:22.452853 landingai-0.2.9/landingai/data_management/client.py
+-rw-r--r--   0        0        0    21178 2023-07-19 21:47:22.452853 landingai-0.2.9/landingai/data_management/media.py
+-rw-r--r--   0        0        0     4722 2023-07-19 21:47:22.452853 landingai-0.2.9/landingai/data_management/metadata.py
+-rw-r--r--   0        0        0     2188 2023-07-19 21:47:22.452853 landingai-0.2.9/landingai/data_management/utils.py
+-rw-r--r--   0        0        0     9730 2023-07-19 21:47:22.452853 landingai-0.2.9/landingai/exceptions.py
+-rw-r--r--   0        0        0  1594400 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     5915 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/image_source_ops.py
+-rw-r--r--   0        0        0     1502 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/notebook_utils.py
+-rw-r--r--   0        0        0      420 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/pipeline/__init__.py
+-rw-r--r--   0        0        0    16449 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/pipeline/frameset.py
+-rw-r--r--   0        0        0    11810 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/pipeline/image_source.py
+-rw-r--r--   0        0        0     1339 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/pipeline/postprocessing.py
+-rw-r--r--   0        0        0     8389 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/postprocess.py
+-rw-r--r--   0        0        0    25677 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/predict.py
+-rw-r--r--   0        0        0     6462 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/st_utils.py
+-rw-r--r--   0        0        0       40 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/storage/__init__.py
+-rw-r--r--   0        0        0     4439 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/storage/data_access.py
+-rw-r--r--   0        0        0     4340 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/storage/snowflake.py
+-rw-r--r--   0        0        0     1503 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/telemetry.py
+-rw-r--r--   0        0        0     5869 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/timer.py
+-rw-r--r--   0        0        0     1685 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/transform.py
+-rw-r--r--   0        0        0     2998 2023-07-19 21:47:22.464853 landingai-0.2.9/landingai/utils.py
+-rw-r--r--   0        0        0    13403 2023-07-19 21:47:22.468853 landingai-0.2.9/landingai/visualize.py
+-rw-r--r--   0        0        0     2606 2023-07-19 21:47:23.124856 landingai-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     7988 1970-01-01 00:00:00.000000 landingai-0.2.9/PKG-INFO
```

### Comparing `landingai-0.2.8/LICENSE.md` & `landingai-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/README.md` & `landingai-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/common.py` & `landingai-0.2.9/landingai/common.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/data_management/client.py` & `landingai-0.2.9/landingai/data_management/client.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/data_management/media.py` & `landingai-0.2.9/landingai/data_management/media.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/data_management/metadata.py` & `landingai-0.2.9/landingai/data_management/metadata.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/data_management/utils.py` & `landingai-0.2.9/landingai/data_management/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/exceptions.py` & `landingai-0.2.9/landingai/exceptions.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/fonts/default_font_ch_en.ttf` & `landingai-0.2.9/landingai/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/image_source_ops.py` & `landingai-0.2.9/landingai/image_source_ops.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/notebook_utils.py` & `landingai-0.2.9/landingai/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/pipeline/frameset.py` & `landingai-0.2.9/landingai/pipeline/frameset.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/pipeline/image_source.py` & `landingai-0.2.9/landingai/pipeline/image_source.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/pipeline/postprocessing.py` & `landingai-0.2.9/landingai/pipeline/postprocessing.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/postprocess.py` & `landingai-0.2.9/landingai/postprocess.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/predict.py` & `landingai-0.2.9/landingai/predict.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/st_utils.py` & `landingai-0.2.9/landingai/st_utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/storage/data_access.py` & `landingai-0.2.9/landingai/storage/data_access.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/storage/snowflake.py` & `landingai-0.2.9/landingai/storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/telemetry.py` & `landingai-0.2.9/landingai/telemetry.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/timer.py` & `landingai-0.2.9/landingai/timer.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/transform.py` & `landingai-0.2.9/landingai/transform.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/landingai/utils.py` & `landingai-0.2.9/landingai/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,23 +22,26 @@
 
 @Timer(name="serialize_image", log_fn=_LOGGER.info)
 def serialize_image(image: Union[np.ndarray, PIL.Image.Image]) -> bytes:
     """Serialize the input image into bytes of an image file.
 
     The image file encoding format is set to "JPEG" for optimal latency.
     For RGBA images, the encoding format will be `PNG` to preserve transparency.
+    For palettized image, i.e. mode `P` or `PA`, the image will be converted to RGB before encoding.
     In addition, the image file encoding format can be overwritten by the environment variable `DEFAULT_IMAGE_SERIALIZATION_FORMAT`.
     Supported image serialization formats are: JPEG, PNG, BMP.
     """
     if image is None or (isinstance(image, np.ndarray) and len(image) == 0):
         raise ValueError(f"Input image must be non-emtpy, but got: {image}")
     format = _resolve_serialization_format(image)
     _LOGGER.debug("Use %s as the serialization format.", format)
     if isinstance(image, np.ndarray):
         image = PIL.Image.fromarray(image)
+    if image.mode == "P" or image.mode == "PA":
+        image = image.convert("RGB")
     img_buffer = io.BytesIO()
     image.save(img_buffer, format=format)
     buffer_bytes = img_buffer.getvalue()
     img_buffer.close()
     return buffer_bytes
```

### Comparing `landingai-0.2.8/landingai/visualize.py` & `landingai-0.2.9/landingai/visualize.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.8/pyproject.toml` & `landingai-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "landingai"
-version = "0.2.8"
+version = "0.2.9"
 description = "Helper library for interacting with Landing AI LandingLens"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "landingai"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `landingai-0.2.8/PKG-INFO` & `landingai-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingai
-Version: 0.2.8
+Version: 0.2.9
 Summary: Helper library for interacting with Landing AI LandingLens
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

