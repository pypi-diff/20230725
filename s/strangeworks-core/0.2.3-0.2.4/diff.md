# Comparing `tmp/strangeworks_core-0.2.3.tar.gz` & `tmp/strangeworks_core-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_core-0.2.3.tar", max compression
+gzip compressed data, was "strangeworks_core-0.2.4.tar", max compression
```

## Comparing `strangeworks_core-0.2.3.tar` & `strangeworks_core-0.2.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      655 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/README.md
--rw-r--r--   0        0        0      914 2023-07-14 19:18:43.994335 strangeworks_core-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      109 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/__init__.py
--rw-r--r--   0        0        0       19 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/batch/__init__.py
--rw-r--r--   0        0        0    13255 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/batch/utils.py
--rw-r--r--   0        0        0       19 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/config/__init__.py
--rw-r--r--   0        0        0      647 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/config/base.py
--rw-r--r--   0        0        0     3340 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/config/config.py
--rw-r--r--   0        0        0      874 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/config/defaults.py
--rw-r--r--   0        0        0     1846 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/config/env.py
--rw-r--r--   0        0        0     6262 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/config/file.py
--rw-r--r--   0        0        0       19 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/errors/__init__.py
--rw-r--r--   0        0        0     2613 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/errors/error.py
--rw-r--r--   0        0        0       19 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/platform/__init__.py
--rw-r--r--   0        0        0     2457 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/platform/auth.py
--rw-r--r--   0        0        0     4880 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/platform/gql.py
--rw-r--r--   0        0        0    10844 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/platform/rest_client.py
--rw-r--r--   0        0        0     3275 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/platform/transport.py
--rw-r--r--   0        0        0       19 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/types/__init__.py
--rw-r--r--   0        0        0     3572 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/types/backend.py
--rw-r--r--   0        0        0     2024 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/types/file.py
--rw-r--r--   0        0        0      647 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/types/func.py
--rw-r--r--   0        0        0     6749 2023-07-14 19:18:26.521322 strangeworks_core-0.2.3/strangeworks_core/types/job.py
--rw-r--r--   0        0        0      760 2023-07-14 19:18:26.521322 strangeworks_core-0.2.3/strangeworks_core/types/machine.py
--rw-r--r--   0        0        0     1088 2023-07-14 19:18:26.521322 strangeworks_core-0.2.3/strangeworks_core/types/product.py
--rw-r--r--   0        0        0     2732 2023-07-14 19:18:26.521322 strangeworks_core-0.2.3/strangeworks_core/types/resource.py
--rw-r--r--   0        0        0      553 2023-07-14 19:18:26.521322 strangeworks_core-0.2.3/strangeworks_core/utils.py
--rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 strangeworks_core-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      655 2023-07-25 15:12:12.228810 strangeworks_core-0.2.4/README.md
+-rw-r--r--   0        0        0      914 2023-07-25 15:12:29.777008 strangeworks_core-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/batch/__init__.py
+-rw-r--r--   0        0        0    13604 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/batch/utils.py
+-rw-r--r--   0        0        0       19 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/config/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/config/base.py
+-rw-r--r--   0        0        0     3340 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/config/config.py
+-rw-r--r--   0        0        0      874 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/config/defaults.py
+-rw-r--r--   0        0        0     1846 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/config/env.py
+-rw-r--r--   0        0        0     6262 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/config/file.py
+-rw-r--r--   0        0        0       19 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/errors/__init__.py
+-rw-r--r--   0        0        0     2613 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/errors/error.py
+-rw-r--r--   0        0        0       19 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/platform/__init__.py
+-rw-r--r--   0        0        0     2457 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/platform/auth.py
+-rw-r--r--   0        0        0     4880 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/platform/gql.py
+-rw-r--r--   0        0        0    10844 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/platform/rest_client.py
+-rw-r--r--   0        0        0     3275 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/platform/transport.py
+-rw-r--r--   0        0        0       19 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/__init__.py
+-rw-r--r--   0        0        0     3572 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/backend.py
+-rw-r--r--   0        0        0      558 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/batch.py
+-rw-r--r--   0        0        0     2024 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/file.py
+-rw-r--r--   0        0        0      647 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/func.py
+-rw-r--r--   0        0        0     6749 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/job.py
+-rw-r--r--   0        0        0      760 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/machine.py
+-rw-r--r--   0        0        0     1088 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/product.py
+-rw-r--r--   0        0        0     2732 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/resource.py
+-rw-r--r--   0        0        0      553 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/utils.py
+-rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 strangeworks_core-0.2.4/PKG-INFO
```

### Comparing `strangeworks_core-0.2.3/README.md` & `strangeworks_core-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/pyproject.toml` & `strangeworks_core-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "strangeworks-core"
-version = "0.2.3"
+version = "0.2.4"
 
 description = "Strangeworks Core provides the infrastructure to interact with the platform."
 authors = ["Strange Devs <hello@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_core"}]
 license = "Apache-2.0"
```

### Comparing `strangeworks_core-0.2.3/strangeworks_core/batch/utils.py` & `strangeworks_core-0.2.4/strangeworks_core/batch/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 from typing import Any, Callable, Optional
 
 import dill
 import requests
 
 from strangeworks_core.errors.error import StrangeworksError
 from strangeworks_core.platform.gql import API, APIInfo, Operation
+from strangeworks_core.types.batch import Options
 from strangeworks_core.types.func import Func
 from strangeworks_core.types.machine import Accelerator, Machine
 
 
 def send_batch_request(
     api: API,
     batch_job_init_create: Operation,
     decorator_name: str,
     func: Func,
     machine: Optional[Machine] = None,
     accelerator: Optional[Accelerator] = None,
+    options: Optional[Options] = None,
     **kwargs,
 ) -> str:
     """Send batch request.
 
     Sends an initiate request to the platform to create a batch job.
     Packages up the user program and any requirements
     and stores them where the platform needs them to be.
@@ -47,14 +49,16 @@
         Decorator name.
     func : Func
         Func instance.
     machine : Optional[Machine], optional
         Machine instance, by default None
     accelerator : Optional[Accelerator], optional
         Accelerator instance, by default None
+    options: Optional[Options], optional
+        Options instance, by default None
     **kwargs
         Keyword arguments.
 
     Returns
     -------
     batch_job_slug : str
         Batch job slug.
@@ -162,21 +166,28 @@
             signed_url, data=tmp, headers={"Content-Type": "application/zip"}
         )
         res.raise_for_status()
 
     if not machine:
         machine = Machine()
 
+    if not options:
+        options = Options()
+
     final = {
         "batchJobSlug": batch_job_slug,
         "machine": {
             "Type": machine.type,
             "CPU": machine.cpu,
             "Memory": machine.memory,
         },
+        "options": {
+            "MaxRetries": options.max_retries,
+            "MaxDuration": options.max_duration,
+        },
     }
     if accelerator:
         final["machineAccelerator"] = {
             "Type": accelerator.type,
             "Count": accelerator.count,
         }
     res = api.execute(
```

### Comparing `strangeworks_core-0.2.3/strangeworks_core/config/base.py` & `strangeworks_core-0.2.4/strangeworks_core/config/base.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/config/config.py` & `strangeworks_core-0.2.4/strangeworks_core/config/config.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/config/defaults.py` & `strangeworks_core-0.2.4/strangeworks_core/config/defaults.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/config/env.py` & `strangeworks_core-0.2.4/strangeworks_core/config/env.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/config/file.py` & `strangeworks_core-0.2.4/strangeworks_core/config/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/errors/error.py` & `strangeworks_core-0.2.4/strangeworks_core/errors/error.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/platform/auth.py` & `strangeworks_core-0.2.4/strangeworks_core/platform/auth.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/platform/gql.py` & `strangeworks_core-0.2.4/strangeworks_core/platform/gql.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/platform/rest_client.py` & `strangeworks_core-0.2.4/strangeworks_core/platform/rest_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/platform/transport.py` & `strangeworks_core-0.2.4/strangeworks_core/platform/transport.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/types/backend.py` & `strangeworks_core-0.2.4/strangeworks_core/types/backend.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/types/file.py` & `strangeworks_core-0.2.4/strangeworks_core/types/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/types/func.py` & `strangeworks_core-0.2.4/strangeworks_core/types/func.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/types/job.py` & `strangeworks_core-0.2.4/strangeworks_core/types/job.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/types/machine.py` & `strangeworks_core-0.2.4/strangeworks_core/types/machine.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/types/product.py` & `strangeworks_core-0.2.4/strangeworks_core/types/product.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/types/resource.py` & `strangeworks_core-0.2.4/strangeworks_core/types/resource.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/strangeworks_core/utils.py` & `strangeworks_core-0.2.4/strangeworks_core/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.3/PKG-INFO` & `strangeworks_core-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-core
-Version: 0.2.3
+Version: 0.2.4
 Summary: Strangeworks Core provides the infrastructure to interact with the platform.
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

