# Comparing `tmp/vegafusion-1.4.0rc3.tar.gz` & `tmp/vegafusion-1.4.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegafusion-1.4.0rc3.tar", last modified: Thu Jul 20 16:58:31 2023, max compression
+gzip compressed data, was "vegafusion-1.4.0rc4.tar", last modified: Mon Jul 24 20:44:45 2023, max compression
```

## Comparing `vegafusion-1.4.0rc3.tar` & `vegafusion-1.4.0rc4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:58:31.629995 vegafusion-1.4.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_conext_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_input_utc.py
--rw-r--r--   0 runner    (1001) docker     (123)    43916 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_pretransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_pretransform_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_row_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_transformed_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/tests/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/vegafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/compilers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/vegafusion/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/connection/duckdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/vegafusion/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/dataset/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/dataset/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/dataset/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/local_tz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/vegafusion/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63111 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/proto/datafusion_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23574 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-20 16:57:29.000000 vegafusion-1.4.0rc3/vegafusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:58:31.633995 vegafusion-1.4.0rc3/vegafusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-20 16:58:31.000000 vegafusion-1.4.0rc3/vegafusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-20 16:58:31.000000 vegafusion-1.4.0rc3/vegafusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:58:31.000000 vegafusion-1.4.0rc3/vegafusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-20 16:58:31.000000 vegafusion-1.4.0rc3/vegafusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 16:58:31.000000 vegafusion-1.4.0rc3/vegafusion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:44:45.355482 vegafusion-1.4.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-24 20:44:45.355482 vegafusion-1.4.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-24 20:44:45.355482 vegafusion-1.4.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:44:45.351482 vegafusion-1.4.0rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/tests/test_conext_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/tests/test_input_utc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45595 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/tests/test_pretransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/tests/test_pretransform_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/tests/test_row_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/tests/test_transformed_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:44:45.355482 vegafusion-1.4.0rc4/vegafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/compilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:44:45.355482 vegafusion-1.4.0rc4/vegafusion/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/connection/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:44:45.355482 vegafusion-1.4.0rc4/vegafusion/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/dataset/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/dataset/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/dataset/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/local_tz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:44:45.355482 vegafusion-1.4.0rc4/vegafusion/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63111 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/proto/datafusion_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27356 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-24 20:43:46.000000 vegafusion-1.4.0rc4/vegafusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:44:45.355482 vegafusion-1.4.0rc4/vegafusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-24 20:44:45.000000 vegafusion-1.4.0rc4/vegafusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-24 20:44:45.000000 vegafusion-1.4.0rc4/vegafusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:44:45.000000 vegafusion-1.4.0rc4/vegafusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-24 20:44:45.000000 vegafusion-1.4.0rc4/vegafusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 20:44:45.000000 vegafusion-1.4.0rc4/vegafusion.egg-info/top_level.txt
```

### Comparing `vegafusion-1.4.0rc3/LICENSE.txt` & `vegafusion-1.4.0rc4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/PKG-INFO` & `vegafusion-1.4.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.4.0rc3
+Version: 1.4.0rc4
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.4.0rc3/README.md` & `vegafusion-1.4.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/setup.cfg` & `vegafusion-1.4.0rc4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [bdist_wheel]
 universal = 0
 
 [metadata]
 name = vegafusion
 description = Core tools for using VegaFusion from Python
-version = 1.4.0-rc3
+version = 1.4.0-rc4
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = vega, altair, vegafusion, arrow
 license = BSD-3-Clause
 license_file = LICENSE.txt
 python = "^3.7"
 homepage = "https://vegafusion.io"
@@ -31,14 +31,14 @@
 	pyarrow>=5
 	pandas
 	psutil
 	protobuf
 
 [options.extras_require]
 embed = 
-	vegafusion-python-embed==1.4.0-rc3
+	vegafusion-python-embed==1.4.0-rc4
 	vl-convert-python>=0.7.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vegafusion-1.4.0rc3/tests/test_conext_manager.py` & `vegafusion-1.4.0rc4/tests/test_conext_manager.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/tests/test_input_utc.py` & `vegafusion-1.4.0rc4/tests/test_input_utc.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/tests/test_pretransform.py` & `vegafusion-1.4.0rc4/tests/test_pretransform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import pandas as pd
 import pytest
 from pandas import Timestamp, NaT
+import pyarrow as pa
 import vegafusion as vf
 import json
 import polars as pl
 from datetime import date
 import decimal
-
+import base64
 
 def setup_module(module):
     vf.set_local_tz("UTC")
 
 
 def get_connections():
     connections = ["datafusion"]
@@ -1639,7 +1640,55 @@
     assert len(tx_spec.get("signals", [])) == 2
     sig0 = tx_spec["signals"][0]
     sig1 = tx_spec["signals"][1]
     [sig0, sig1] = sorted([sig0, sig1], key=lambda v: v["name"])
     assert sig0["name"] == "layer_0_layer_0_bin_maxbins_10_IMDB_Rating_bins"
     assert sig1["name"] == "layer_0_layer_0_bin_maxbins_10_IMDB_Rating_extent"
     assert sig1["value"] == [1.4, 9.2]
+
+
+def test_pre_transform_spec_encoded_datasets():
+    # Pre-transform with supported aggregate function should result in no warnings
+    vega_spec = movies_histogram_spec()
+
+    # default list of dict format
+    tx_spec, warnings = vf.runtime.pre_transform_spec(
+        vega_spec, data_encoding_threshold=10, data_encoding_format="pyarrow"
+    )
+
+    values = tx_spec["data"][0]["values"]
+    assert isinstance(values, list)
+    assert len(values) == 9
+
+    # pyarrow format
+    tx_spec, warnings = vf.runtime.pre_transform_spec(
+        vega_spec, data_encoding_threshold=0, data_encoding_format="pyarrow"
+    )
+
+    values = tx_spec["data"][0]["values"]
+    assert isinstance(values, pa.Table)
+    values_df = values.to_pandas()
+    assert len(values_df) == 9
+    assert values_df.columns[0] == "bin_maxbins_10_IMDB Rating"
+
+    # arrow-ipc format
+    tx_spec, warnings = vf.runtime.pre_transform_spec(
+        vega_spec, data_encoding_threshold=0, data_encoding_format="arrow-ipc"
+    )
+
+    values = tx_spec["data"][0]["values"]
+    assert isinstance(values, bytes)
+    values_df = pa.ipc.deserialize_pandas(values)
+    assert len(values_df) == 9
+    assert values_df.columns[0] == "bin_maxbins_10_IMDB Rating"
+
+    # arrow-ipc-base64 format
+    tx_spec, warnings = vf.runtime.pre_transform_spec(
+        vega_spec, data_encoding_threshold=0, data_encoding_format="arrow-ipc-base64"
+    )
+
+    values = tx_spec["data"][0]["values"]
+    assert isinstance(values, str)
+    values_df = pa.ipc.deserialize_pandas(base64.standard_b64decode(values))
+    assert len(values_df) == 9
+    assert values_df.columns[0] == "bin_maxbins_10_IMDB Rating"
+
```

### Comparing `vegafusion-1.4.0rc3/tests/test_pretransform_specs.py` & `vegafusion-1.4.0rc4/tests/test_pretransform_specs.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/tests/test_row_limit.py` & `vegafusion-1.4.0rc4/tests/test_row_limit.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/tests/test_save.py` & `vegafusion-1.4.0rc4/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/tests/test_transformed_data.py` & `vegafusion-1.4.0rc4/tests/test_transformed_data.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/tests/test_transformer.py` & `vegafusion-1.4.0rc4/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion/__init__.py` & `vegafusion-1.4.0rc4/vegafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion/compilers.py` & `vegafusion-1.4.0rc4/vegafusion/compilers.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion/connection/__init__.py` & `vegafusion-1.4.0rc4/vegafusion/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion/connection/duckdb.py` & `vegafusion-1.4.0rc4/vegafusion/connection/duckdb.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion/dataset/dataframe.py` & `vegafusion-1.4.0rc4/vegafusion/dataset/dataframe.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion/dataset/duckdb.py` & `vegafusion-1.4.0rc4/vegafusion/dataset/duckdb.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion/dataset/sql.py` & `vegafusion-1.4.0rc4/vegafusion/dataset/sql.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion/evaluation.py` & `vegafusion-1.4.0rc4/vegafusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion/local_tz.py` & `vegafusion-1.4.0rc4/vegafusion/local_tz.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion/proto/datafusion_pb2.py` & `vegafusion-1.4.0rc4/vegafusion/proto/datafusion_pb2.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion/renderer.py` & `vegafusion-1.4.0rc4/vegafusion/renderer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion/runtime.py` & `vegafusion-1.4.0rc4/vegafusion/runtime.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import pandas as pd
 import psutil
 import pyarrow as pa
 from typing import Union
 from .connection import SqlConnection
 from .dataset import SqlDataset, DataFrameDataset
+from .evaluation import get_mark_group_for_scope
 from .transformer import import_pyarrow_interchange, to_arrow_table
 from .local_tz import get_local_tz
 
 try:
     from duckdb import DuckDBPyConnection
 except ImportError:
     DuckDBPyConnection = None
@@ -181,14 +182,16 @@
         local_tz=None,
         default_input_tz=None,
         row_limit=None,
         preserve_interactivity=True,
         inline_datasets=None,
         keep_signals=None,
         keep_datasets=None,
+        data_encoding_threshold=None,
+        data_encoding_format="pyarrow",
     ):
         """
         Evaluate supported transforms in an input Vega specification and produce a new
         specification with pre-transformed datasets included inline.
 
         :param spec: A Vega specification dict or JSON string
         :param local_tz: Name of timezone to be considered local. E.g. 'America/New_York'.
@@ -214,14 +217,26 @@
               - A two-element tuple where the first element is the name of a signal as a string
                 and the second element is the nested scope of the dataset as a list of integers
         :param keep_datasets: Datasets from the input spec that must be included in the
             pre-transformed spec. A list with elements that are either:
               - The name of a top-level dataset as a string
               - A two-element tuple where the first element is the name of a dataset as a string
                 and the second element is the nested scope of the dataset as a list of integers
+        :param data_encoding_threshold: threshold for encoding datasets
+            When length of pre-transformed datasets exceeds data_encoding_threshold, datasets
+            are encoded into an alternative format (as determined by the data_encoding_format
+            argument). When None (the default), pre-transformed datasets are never encoded and
+            are always included as JSON compatible lists of dictionaries.
+        :param data_encoding_format: format of encoded datasets
+            Format to use to encode datasets with length exceeding the data_encoding_threshold
+            argument.
+                - "pyarrow": Encode datasets as pyarrow Tables. Not JSON compatible.
+                - "arrow-ipc": Encode datasets as bytes in Arrow IPC format. Not JSON compatible.
+                - "arrow-ipc-base64": Encode datasets as strings in base64 encoded Arrow IPC format.
+                    JSON compatible.
         :return:
             Two-element tuple:
                 0. A string containing the JSON representation of a Vega specification
                    with pre-transformed datasets included inline
                 1. A list of warnings as dictionaries. Each warning dict has a 'type'
                    key indicating the warning type, and a 'message' key containing
                    a description of the warning. Potential warning types include:
@@ -238,24 +253,46 @@
             local_tz = local_tz or get_local_tz()
             imported_inline_dataset = self._import_or_register_inline_datasets(inline_datasets)
 
             # Parse input keep signals and datasets
             keep_signals = parse_variables(keep_signals)
             keep_datasets = parse_variables(keep_datasets)
             try:
-                new_spec, warnings = self.embedded_runtime.pre_transform_spec(
-                    spec,
-                    local_tz=local_tz,
-                    default_input_tz=default_input_tz,
-                    row_limit=row_limit,
-                    preserve_interactivity=preserve_interactivity,
-                    inline_datasets=imported_inline_dataset,
-                    keep_signals=keep_signals,
-                    keep_datasets=keep_datasets,
-                )
+                if data_encoding_threshold is None:
+                    new_spec, warnings = self.embedded_runtime.pre_transform_spec(
+                        spec,
+                        local_tz=local_tz,
+                        default_input_tz=default_input_tz,
+                        row_limit=row_limit,
+                        preserve_interactivity=preserve_interactivity,
+                        inline_datasets=imported_inline_dataset,
+                        keep_signals=keep_signals,
+                        keep_datasets=keep_datasets,
+                    )
+                else:
+                    # Use pre_transform_extract to extract large datasets
+                    new_spec, datasets, warnings = self.embedded_runtime.pre_transform_extract(
+                        spec,
+                        local_tz=local_tz,
+                        default_input_tz=default_input_tz,
+                        preserve_interactivity=preserve_interactivity,
+                        extract_threshold=data_encoding_threshold,
+                        extracted_format=data_encoding_format,
+                        inline_datasets=imported_inline_dataset,
+                        keep_signals=keep_signals,
+                        keep_datasets=keep_datasets,
+                    )
+
+                    # Insert encoded datasets back into spec
+                    for (name, scope, tbl) in datasets:
+                        group = get_mark_group_for_scope(new_spec, scope)
+                        for data in group.get("data", []):
+                            if data.get("name", None) == name:
+                                data["values"] = tbl
+
             finally:
                 # Clean up temporary tables
                 if self._connection is not None:
                     self._connection.unregister_temporary_tables()
 
             return new_spec, warnings
 
@@ -349,15 +386,19 @@
 
     def pre_transform_extract(
         self,
         spec,
         local_tz=None,
         default_input_tz=None,
         preserve_interactivity=True,
-        inline_datasets=None
+        extract_threshold=20,
+        extracted_format="pyarrow",
+        inline_datasets=None,
+        keep_signals=None,
+        keep_datasets=None,
     ):
         """
         Evaluate supported transforms in an input Vega specification and produce a new
         specification with small pre-transformed datasets (under 100 rows) included inline
         and larger inline datasets (100 rows or more) are extracted into pyarrow tables.
 
         :param spec: A Vega specification dict or JSON string
@@ -367,18 +408,35 @@
         :param default_input_tz: Name of timezone (e.g. 'America/New_York') that naive datetime
             strings should be interpreted in. Defaults to `local_tz`.
         :param preserve_interactivity: If True (default) then the interactive behavior of
             the chart will pre preserved. This requires that all the data that participates
             in interactions be included in the resulting spec rather than being pre-transformed.
             If False, then all possible data transformations are applied even if they break
             the original interactive behavior of the chart.
+        :param extract_threshold: Datasets with length below extract_threshold will be
+            inlined
+        :param extracted_format: The format for the extracted datasets
+            The format for extracted datasets:
+                - "pyarrow": pyarrow.Table
+                - "arrow-ipc": bytes in arrow IPC format
+                - "arrow-ipc-base64": base64 encoded arrow IPC format
         :param inline_datasets: A dict from dataset names to pandas DataFrames or pyarrow
             Tables. Inline datasets may be referenced by the input specification using
             the following url syntax 'vegafusion+dataset://{dataset_name}' or
             'table://{dataset_name}'.
+        :param keep_signals: Signals from the input spec that must be included in the
+            pre-transformed spec. A list with elements that are either:
+              - The name of a top-level signal as a string
+              - A two-element tuple where the first element is the name of a signal as a string
+                and the second element is the nested scope of the dataset as a list of integers
+        :param keep_datasets: Datasets from the input spec that must be included in the
+            pre-transformed spec. A list with elements that are either:
+              - The name of a top-level dataset as a string
+              - A two-element tuple where the first element is the name of a dataset as a string
+                and the second element is the nested scope of the dataset as a list of integers
         :return:
             Three-element tuple:
                 0. A dict containing the JSON representation of the pre-transformed Vega
                    specification without pre-transformed datasets included inline
                 1. Extracted datasets as a list of three element tuples
                     0. dataset name
                     1. dataset scope
@@ -396,15 +454,19 @@
             inline_arrow_dataset = self._import_or_register_inline_datasets(inline_datasets)
             try:
                 new_spec, datasets, warnings = self.embedded_runtime.pre_transform_extract(
                     spec,
                     local_tz=local_tz,
                     default_input_tz=default_input_tz,
                     preserve_interactivity=preserve_interactivity,
-                    inline_datasets=inline_arrow_dataset
+                    extract_threshold=extract_threshold,
+                    extracted_format=extracted_format,
+                    inline_datasets=inline_arrow_dataset,
+                    keep_signals=keep_signals,
+                    keep_datasets=keep_datasets,
                 )
             finally:
                 # Clean up temporary tables
                 if self._connection is not None:
                     self._connection.unregister_temporary_tables()
 
             return new_spec, datasets, warnings
```

### Comparing `vegafusion-1.4.0rc3/vegafusion/save.py` & `vegafusion-1.4.0rc4/vegafusion/save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion/transformer.py` & `vegafusion-1.4.0rc4/vegafusion/transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion/utils.py` & `vegafusion-1.4.0rc4/vegafusion/utils.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.4.0rc3/vegafusion.egg-info/PKG-INFO` & `vegafusion-1.4.0rc4/vegafusion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.4.0rc3
+Version: 1.4.0rc4
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.4.0rc3/vegafusion.egg-info/SOURCES.txt` & `vegafusion-1.4.0rc4/vegafusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

