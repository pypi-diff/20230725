# Comparing `tmp/eodc_faas_force-2023.6.2.tar.gz` & `tmp/eodc_faas_force-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_force-2023.6.2.tar", max compression
+gzip compressed data, was "eodc_faas_force-2023.7.0.tar", max compression
```

## Comparing `eodc_faas_force-2023.6.2.tar` & `eodc_faas_force-2023.7.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       24 2023-05-04 07:19:47.663253 eodc_faas_force-2023.6.2/README.md
--rw-r--r--   0        0        0       93 2023-06-15 09:56:41.391253 eodc_faas_force-2023.6.2/force_processor_bindings/__init__.py
--rw-r--r--   0        0        0     2952 2023-06-15 09:39:13.387253 eodc_faas_force-2023.6.2/force_processor_bindings/model.py
--rw-r--r--   0        0        0      610 2023-06-15 09:56:41.391253 eodc_faas_force-2023.6.2/pyproject.toml
--rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 eodc_faas_force-2023.6.2/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-05-04 07:19:47.663253 eodc_faas_force-2023.7.0/README.md
+-rw-r--r--   0        0        0       93 2023-07-25 13:10:32.840000 eodc_faas_force-2023.7.0/force_processor_bindings/__init__.py
+-rw-r--r--   0        0        0     3352 2023-07-25 08:54:20.680000 eodc_faas_force-2023.7.0/force_processor_bindings/model.py
+-rw-r--r--   0        0        0      610 2023-07-25 13:10:32.840000 eodc_faas_force-2023.7.0/pyproject.toml
+-rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 eodc_faas_force-2023.7.0/PKG-INFO
```

### Comparing `eodc_faas_force-2023.6.2/force_processor_bindings/model.py` & `eodc_faas_force-2023.7.0/force_processor_bindings/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from enum import Enum
 from pathlib import Path
+from typing import Optional, Union
 
 from pydantic import BaseModel, Field, validator
 
 logger = logging.getLogger(__name__)
 
 
 class ForceResMergeOptions(Enum):
@@ -18,15 +19,24 @@
         the value, without the enum name"""
         return str(self.value)
 
 
 class ForceParameters(BaseModel):
     """Pydantic model of force supported parameters."""
 
-    input_files: list[str]
+    stac_url: Optional[str]
+    collection_id: Optional[str]
+
+    # Specify bounding box in Lon/Lat.
+    bbox: Optional[Union[tuple[float, ...], list[float], str]]
+
+    # datetime needs to be formatted as required by
+    # https://pystac-client.readthedocs.io/en/latest/api.html#pystac_client.Client.search
+    datetime: Optional[str]
+    input_files: list[str] = Field(default_factory=list)
     user_workspace: Path
     dem_file: str
     dem_nodata: int = Field(default=-9999)
     do_atmo: bool = Field(default="TRUE")
     do_topo: bool = Field(default="TRUE")
     do_brdf: bool = Field(default="TRUE")
     adjacency_effect: bool = Field(default="TRUE")
```

### Comparing `eodc_faas_force-2023.6.2/pyproject.toml` & `eodc_faas_force-2023.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-faas-force"
-version = "2023.6.2"
+version = "2023.7.0"
 description = "Bindings for the FORCE processor exposed at EODC"
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Valentina Hutter <valentina.hutter@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "force_processor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `eodc_faas_force-2023.6.2/PKG-INFO` & `eodc_faas_force-2023.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc-faas-force
-Version: 2023.6.2
+Version: 2023.7.0
 Summary: Bindings for the FORCE processor exposed at EODC
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

