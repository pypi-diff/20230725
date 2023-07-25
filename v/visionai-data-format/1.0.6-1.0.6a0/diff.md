# Comparing `tmp/visionai-data-format-1.0.6.tar.gz` & `tmp/visionai-data-format-1.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionai-data-format-1.0.6.tar", last modified: Thu Jul 20 06:18:07 2023, max compression
+gzip compressed data, was "visionai-data-format-1.0.6a0.tar", last modified: Tue Jul 25 08:40:44 2023, max compression
```

## Comparing `visionai-data-format-1.0.6.tar` & `visionai-data-format-1.0.6a0.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-07-20 06:18:07.639571 visionai-data-format-1.0.6/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    17296 2023-07-20 06:18:07.639429 visionai-data-format-1.0.6/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    17066 2023-07-19 07:41:15.000000 visionai-data-format-1.0.6/README.md
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2023-07-20 06:18:07.639603 visionai-data-format-1.0.6/setup.cfg
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      753 2023-07-19 07:30:08.000000 visionai-data-format-1.0.6/setup.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-07-20 06:18:07.634378 visionai-data-format-1.0.6/tests/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     2176 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/tests/test_schemas.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     4731 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/tests/test_validators.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-07-20 06:18:07.635835 visionai-data-format-1.0.6/visionai_data_format/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     3180 2023-07-19 08:21:36.000000 visionai-data-format-1.0.6/visionai_data_format/bdd_to_vai.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     7775 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/coco_to_vai.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-07-20 06:18:07.637307 visionai-data-format-1.0.6/visionai_data_format/schemas/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/schemas/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     2581 2023-07-19 05:41:21.000000 visionai-data-format-1.0.6/visionai_data_format/schemas/bdd_schema.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      679 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/schemas/coco_schema.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1657 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/schemas/common.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      994 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/schemas/ontology.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-07-20 06:18:07.637594 visionai-data-format-1.0.6/visionai_data_format/schemas/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/schemas/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    40508 2023-07-18 08:05:51.000000 visionai-data-format-1.0.6/visionai_data_format/schemas/utils/validators.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    27992 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/schemas/visionai_schema.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-07-20 06:18:07.639263 visionai-data-format-1.0.6/visionai_data_format/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      494 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/utils/calculation.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    10506 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/utils/checker.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      761 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/utils/classes.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      335 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/utils/common.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    14161 2023-07-19 08:23:02.000000 visionai-data-format-1.0.6/visionai_data_format/utils/converter.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     4059 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/utils/resize.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1991 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/utils/validator.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     2308 2023-07-13 07:05:34.000000 visionai-data-format-1.0.6/visionai_data_format/vai_to_bdd.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5917 2023-07-06 06:50:32.000000 visionai-data-format-1.0.6/visionai_data_format/vai_to_bdd_v2.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     6237 2023-07-05 08:54:57.000000 visionai-data-format-1.0.6/visionai_data_format/vai_to_coco.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-07-20 06:18:07.636419 visionai-data-format-1.0.6/visionai_data_format.egg-info/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    17296 2023-07-20 06:18:07.000000 visionai-data-format-1.0.6/visionai_data_format.egg-info/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1160 2023-07-20 06:18:07.000000 visionai-data-format-1.0.6/visionai_data_format.egg-info/SOURCES.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2023-07-20 06:18:07.000000 visionai-data-format-1.0.6/visionai_data_format.egg-info/dependency_links.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       45 2023-07-20 06:18:07.000000 visionai-data-format-1.0.6/visionai_data_format.egg-info/requires.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       21 2023-07-20 06:18:07.000000 visionai-data-format-1.0.6/visionai_data_format.egg-info/top_level.txt
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-25 08:40:44.958998 visionai-data-format-1.0.6a0/
+-rw-r--r--   0 christian   (501) staff       (20)    17298 2023-07-25 08:40:44.958372 visionai-data-format-1.0.6a0/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)    17066 2023-07-25 08:38:17.000000 visionai-data-format-1.0.6a0/README.md
+-rw-r--r--   0 christian   (501) staff       (20)       38 2023-07-25 08:40:44.959056 visionai-data-format-1.0.6a0/setup.cfg
+-rw-r--r--   0 christian   (501) staff       (20)      755 2023-07-25 08:40:19.000000 visionai-data-format-1.0.6a0/setup.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-25 08:40:44.945729 visionai-data-format-1.0.6a0/tests/
+-rw-r--r--   0 christian   (501) staff       (20)     2176 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/tests/test_schemas.py
+-rw-r--r--   0 christian   (501) staff       (20)     4731 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/tests/test_validators.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-25 08:40:44.948486 visionai-data-format-1.0.6a0/visionai_data_format/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     3180 2023-07-25 08:38:17.000000 visionai-data-format-1.0.6a0/visionai_data_format/bdd_to_vai.py
+-rw-r--r--   0 christian   (501) staff       (20)     7775 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/coco_to_vai.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-25 08:40:44.953929 visionai-data-format-1.0.6a0/visionai_data_format/schemas/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/schemas/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     2581 2023-07-25 08:38:17.000000 visionai-data-format-1.0.6a0/visionai_data_format/schemas/bdd_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)      679 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/schemas/coco_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)     1657 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/schemas/common.py
+-rw-r--r--   0 christian   (501) staff       (20)      994 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/schemas/ontology.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-25 08:40:44.955415 visionai-data-format-1.0.6a0/visionai_data_format/schemas/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/schemas/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)    40508 2023-07-25 08:39:08.000000 visionai-data-format-1.0.6a0/visionai_data_format/schemas/utils/validators.py
+-rw-r--r--   0 christian   (501) staff       (20)    27992 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/schemas/visionai_schema.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-25 08:40:44.958125 visionai-data-format-1.0.6a0/visionai_data_format/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)      494 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/utils/calculation.py
+-rw-r--r--   0 christian   (501) staff       (20)    10506 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/utils/checker.py
+-rw-r--r--   0 christian   (501) staff       (20)      761 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/utils/classes.py
+-rw-r--r--   0 christian   (501) staff       (20)      335 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/utils/common.py
+-rw-r--r--   0 christian   (501) staff       (20)    14161 2023-07-25 08:38:17.000000 visionai-data-format-1.0.6a0/visionai_data_format/utils/converter.py
+-rw-r--r--   0 christian   (501) staff       (20)     4059 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/utils/resize.py
+-rw-r--r--   0 christian   (501) staff       (20)     1991 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/utils/validator.py
+-rw-r--r--   0 christian   (501) staff       (20)     2308 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/vai_to_bdd.py
+-rw-r--r--   0 christian   (501) staff       (20)     6237 2023-07-17 04:56:18.000000 visionai-data-format-1.0.6a0/visionai_data_format/vai_to_coco.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-25 08:40:44.950532 visionai-data-format-1.0.6a0/visionai_data_format.egg-info/
+-rw-r--r--   0 christian   (501) staff       (20)    17298 2023-07-25 08:40:44.000000 visionai-data-format-1.0.6a0/visionai_data_format.egg-info/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)     1122 2023-07-25 08:40:44.000000 visionai-data-format-1.0.6a0/visionai_data_format.egg-info/SOURCES.txt
+-rw-r--r--   0 christian   (501) staff       (20)        1 2023-07-25 08:40:44.000000 visionai-data-format-1.0.6a0/visionai_data_format.egg-info/dependency_links.txt
+-rw-r--r--   0 christian   (501) staff       (20)       45 2023-07-25 08:40:44.000000 visionai-data-format-1.0.6a0/visionai_data_format.egg-info/requires.txt
+-rw-r--r--   0 christian   (501) staff       (20)       21 2023-07-25 08:40:44.000000 visionai-data-format-1.0.6a0/visionai_data_format.egg-info/top_level.txt
```

### Comparing `visionai-data-format-1.0.6/PKG-INFO` & `visionai-data-format-1.0.6a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionai-data-format
-Version: 1.0.6
+Version: 1.0.6a0
 Summary: converter tool for visionai format
 Home-page: 
 Author: LinkerVision
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `visionai-data-format-1.0.6/README.md` & `visionai-data-format-1.0.6a0/README.md`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/setup.py` & `visionai-data-format-1.0.6a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "visionai-data-format"
-PACKAGE_VERSION = "1.0.6"
+PACKAGE_VERSION = "1.0.6a0"
 DESC = "converter tool for visionai format"
 REQUIRED = ["pydantic==1.*"]
 REQUIRES_PYTHON = ">=3.7, <4"
 EXTRAS = {
     "test": [
         "pytest",
         "mock",
```

### Comparing `visionai-data-format-1.0.6/tests/test_schemas.py` & `visionai-data-format-1.0.6a0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/tests/test_validators.py` & `visionai-data-format-1.0.6a0/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format/bdd_to_vai.py` & `visionai-data-format-1.0.6a0/visionai_data_format/bdd_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format/coco_to_vai.py` & `visionai-data-format-1.0.6a0/visionai_data_format/coco_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format/schemas/bdd_schema.py` & `visionai-data-format-1.0.6a0/visionai_data_format/schemas/bdd_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format/schemas/coco_schema.py` & `visionai-data-format-1.0.6a0/visionai_data_format/schemas/coco_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format/schemas/common.py` & `visionai-data-format-1.0.6a0/visionai_data_format/schemas/common.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format/schemas/ontology.py` & `visionai-data-format-1.0.6a0/visionai_data_format/schemas/ontology.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format/schemas/utils/validators.py` & `visionai-data-format-1.0.6a0/visionai_data_format/schemas/utils/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -818,19 +818,19 @@
     data_pointers_keys: Set[Tuple[str, str]] = (
         set() if not data_pointers else set(data_pointers.keys())
     )
 
     # validate if combinations of static and dynamic equals to data pointers
     combination_attrs = static_attrs_keys | dynamic_attrs_keys
     if combination_attrs ^ data_pointers_keys:
-        extra_attributes_name: Set[str] = combination_attrs - data_pointers_keys
-        missing_attributes_name: Set[str] = data_pointers_keys - combination_attrs
+        extra_attribute_names: Set[str] = combination_attrs - data_pointers_keys
+        missing_attribute_names: Set[str] = data_pointers_keys - combination_attrs
         msg: str = generate_missing_attributes_error_message(
-            extra_attributes_name=extra_attributes_name,
-            missing_attributes_name=missing_attributes_name,
+            extra_attribute_names=extra_attribute_names,
+            missing_attribute_names=missing_attribute_names,
             dynamic_attrs=dynamic_attrs,
         )
 
         return False, msg
 
     # retrieve frame numbers
     frame_numbers = [int(frame_num) for frame_num in frames.keys()]
```

### Comparing `visionai-data-format-1.0.6/visionai_data_format/schemas/visionai_schema.py` & `visionai-data-format-1.0.6a0/visionai_data_format/schemas/visionai_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format/utils/checker.py` & `visionai-data-format-1.0.6a0/visionai_data_format/utils/checker.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format/utils/classes.py` & `visionai-data-format-1.0.6a0/visionai_data_format/utils/classes.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format/utils/converter.py` & `visionai-data-format-1.0.6a0/visionai_data_format/utils/converter.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format/utils/resize.py` & `visionai-data-format-1.0.6a0/visionai_data_format/utils/resize.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format/utils/validator.py` & `visionai-data-format-1.0.6a0/visionai_data_format/utils/validator.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format/vai_to_bdd.py` & `visionai-data-format-1.0.6a0/visionai_data_format/vai_to_bdd.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format/vai_to_coco.py` & `visionai-data-format-1.0.6a0/visionai_data_format/vai_to_coco.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.6/visionai_data_format.egg-info/PKG-INFO` & `visionai-data-format-1.0.6a0/visionai_data_format.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionai-data-format
-Version: 1.0.6
+Version: 1.0.6a0
 Summary: converter tool for visionai format
 Home-page: 
 Author: LinkerVision
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `visionai-data-format-1.0.6/visionai_data_format.egg-info/SOURCES.txt` & `visionai-data-format-1.0.6a0/visionai_data_format.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 setup.py
 tests/test_schemas.py
 tests/test_validators.py
 visionai_data_format/__init__.py
 visionai_data_format/bdd_to_vai.py
 visionai_data_format/coco_to_vai.py
 visionai_data_format/vai_to_bdd.py
-visionai_data_format/vai_to_bdd_v2.py
 visionai_data_format/vai_to_coco.py
 visionai_data_format.egg-info/PKG-INFO
 visionai_data_format.egg-info/SOURCES.txt
 visionai_data_format.egg-info/dependency_links.txt
 visionai_data_format.egg-info/requires.txt
 visionai_data_format.egg-info/top_level.txt
 visionai_data_format/schemas/__init__.py
```

