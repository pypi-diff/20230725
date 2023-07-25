# Comparing `tmp/warpzone_sdk-8.3.4.tar.gz` & `tmp/warpzone_sdk-8.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warpzone_sdk-8.3.4.tar", max compression
+gzip compressed data, was "warpzone_sdk-8.3.5.tar", max compression
```

## Comparing `warpzone_sdk-8.3.4.tar` & `warpzone_sdk-8.3.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1093 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/pyproject.toml
--rw-r--r--   0        0        0     1330 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/__init__.py
--rw-r--r--   0        0        0       21 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/blobstorage/__init__.py
--rw-r--r--   0        0        0     2844 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/blobstorage/client.py
--rw-r--r--   0        0        0       24 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/enums/__init__.py
--rw-r--r--   0        0        0      213 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/enums/topicenum.py
--rw-r--r--   0        0        0       35 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/__init__.py
--rw-r--r--   0        0        0     1018 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/checks.py
--rw-r--r--   0        0        0     2108 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/functionize.py
--rw-r--r--   0        0        0     3840 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/integrations.py
--rw-r--r--   0        0        0     2223 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/monitor.py
--rw-r--r--   0        0        0     2105 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/process.py
--rw-r--r--   0        0        0       46 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/processors/__init__.py
--rw-r--r--   0        0        0      781 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/processors/dependencies.py
--rw-r--r--   0        0        0     2067 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/processors/outputs.py
--rw-r--r--   0        0        0     1727 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/processors/triggers.py
--rw-r--r--   0        0        0     2268 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/signature.py
--rw-r--r--   0        0        0      547 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/function/types.py
--rw-r--r--   0        0        0     2108 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/healthchecks/__init__.py
--rw-r--r--   0        0        0     1112 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/healthchecks/model.py
--rw-r--r--   0        0        0       87 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/monitor/__init__.py
--rw-r--r--   0        0        0     1650 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/monitor/logs.py
--rw-r--r--   0        0        0     4781 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/monitor/traces.py
--rw-r--r--   0        0        0       21 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/servicebus/data/__init__.py
--rw-r--r--   0        0        0     5636 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/servicebus/data/client.py
--rw-r--r--   0        0        0       21 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/servicebus/events/__init__.py
--rw-r--r--   0        0        0     4250 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/servicebus/events/client.py
--rw-r--r--   0        0        0       21 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/db/__init__.py
--rw-r--r--   0        0        0     1522 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/db/base_client.py
--rw-r--r--   0        0        0     1960 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/db/client.py
--rw-r--r--   0        0        0     1704 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/db/client_async.py
--rw-r--r--   0        0        0       47 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/tables/__init__.py
--rw-r--r--   0        0        0     2916 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/tables/client.py
--rw-r--r--   0        0        0     2516 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/tables/client_async.py
--rw-r--r--   0        0        0      521 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/tables/helpers.py
--rw-r--r--   0        0        0     2470 2023-07-21 13:08:40.015096 warpzone_sdk-8.3.4/warpzone/tablestorage/tables/operations.py
--rw-r--r--   0        0        0      248 2023-07-21 13:08:40.019096 warpzone_sdk-8.3.4/warpzone/testing/__init__.py
--rw-r--r--   0        0        0     3661 2023-07-21 13:08:40.019096 warpzone_sdk-8.3.4/warpzone/testing/assertions.py
--rw-r--r--   0        0        0     3661 2023-07-21 13:08:40.019096 warpzone_sdk-8.3.4/warpzone/testing/data.py
--rw-r--r--   0        0        0       27 2023-07-21 13:08:40.019096 warpzone_sdk-8.3.4/warpzone/transform/__init__.py
--rw-r--r--   0        0        0     1641 2023-07-21 13:08:40.019096 warpzone_sdk-8.3.4/warpzone/transform/data.py
--rw-r--r--   0        0        0     1968 2023-07-21 13:08:40.019096 warpzone_sdk-8.3.4/warpzone/transform/schema.py
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 warpzone_sdk-8.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-07-25 11:01:05.089434 warpzone_sdk-8.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1397 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/__init__.py
+-rw-r--r--   0        0        0       21 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/blobstorage/__init__.py
+-rw-r--r--   0        0        0     2844 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/blobstorage/client.py
+-rw-r--r--   0        0        0       24 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/enums/__init__.py
+-rw-r--r--   0        0        0      213 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/enums/topicenum.py
+-rw-r--r--   0        0        0       35 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/function/__init__.py
+-rw-r--r--   0        0        0     1018 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/function/checks.py
+-rw-r--r--   0        0        0     2108 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/function/functionize.py
+-rw-r--r--   0        0        0     3840 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/function/integrations.py
+-rw-r--r--   0        0        0     2223 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/function/monitor.py
+-rw-r--r--   0        0        0     2105 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/function/process.py
+-rw-r--r--   0        0        0       46 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/function/processors/__init__.py
+-rw-r--r--   0        0        0      781 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/function/processors/dependencies.py
+-rw-r--r--   0        0        0     2067 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/function/processors/outputs.py
+-rw-r--r--   0        0        0     1727 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/function/processors/triggers.py
+-rw-r--r--   0        0        0     2268 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/function/signature.py
+-rw-r--r--   0        0        0      547 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/function/types.py
+-rw-r--r--   0        0        0     2108 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/healthchecks/__init__.py
+-rw-r--r--   0        0        0     1112 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/healthchecks/model.py
+-rw-r--r--   0        0        0       87 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/monitor/__init__.py
+-rw-r--r--   0        0        0     1650 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/monitor/logs.py
+-rw-r--r--   0        0        0     4781 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/monitor/traces.py
+-rw-r--r--   0        0        0       21 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/servicebus/data/__init__.py
+-rw-r--r--   0        0        0     5636 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/servicebus/data/client.py
+-rw-r--r--   0        0        0       21 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/servicebus/events/__init__.py
+-rw-r--r--   0        0        0     4250 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/servicebus/events/client.py
+-rw-r--r--   0        0        0       21 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/tablestorage/db/__init__.py
+-rw-r--r--   0        0        0     1522 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/tablestorage/db/base_client.py
+-rw-r--r--   0        0        0     1960 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/tablestorage/db/client.py
+-rw-r--r--   0        0        0     1704 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/tablestorage/db/client_async.py
+-rw-r--r--   0        0        0       94 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/tablestorage/tables/__init__.py
+-rw-r--r--   0        0        0     2916 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/tablestorage/tables/client.py
+-rw-r--r--   0        0        0     2516 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/tablestorage/tables/client_async.py
+-rw-r--r--   0        0        0      932 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/tablestorage/tables/helpers.py
+-rw-r--r--   0        0        0     2689 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/tablestorage/tables/operations.py
+-rw-r--r--   0        0        0      248 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/testing/__init__.py
+-rw-r--r--   0        0        0     3661 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/testing/assertions.py
+-rw-r--r--   0        0        0     3661 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/testing/data.py
+-rw-r--r--   0        0        0       27 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/transform/__init__.py
+-rw-r--r--   0        0        0     1641 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/transform/data.py
+-rw-r--r--   0        0        0     1968 2023-07-25 11:01:05.093433 warpzone_sdk-8.3.5/warpzone/transform/schema.py
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 warpzone_sdk-8.3.5/PKG-INFO
```

### Comparing `warpzone_sdk-8.3.4/pyproject.toml` & `warpzone_sdk-8.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "warpzone-sdk"
-version = "8.3.4"
+version = "8.3.5"
 description = "The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "warpzone" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `warpzone_sdk-8.3.4/warpzone/__init__.py` & `warpzone_sdk-8.3.5/warpzone/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from warpzone.function.processors import dependencies, outputs, triggers
 from warpzone.healthchecks import HealthCheckResult, HealthStatus
 from warpzone.monitor import get_logger, get_tracer
 from warpzone.servicebus.data.client import DataMessage, WarpzoneDataClient
 from warpzone.servicebus.events.client import EventMessage, WarpzoneEventClient
 from warpzone.tablestorage.db.client import WarpzoneDatabaseClient
 from warpzone.tablestorage.db.client_async import WarpzoneDatabaseClientAsync
+from warpzone.tablestorage.tables import generate_valid_table_keys
 from warpzone.tablestorage.tables.client import WarpzoneTableClient
 from warpzone.tablestorage.tables.client_async import WarpzoneTableClientAsync
 from warpzone.tablestorage.tables.operations import TableOperations
 from warpzone.transform.data import (
     arrow_to_pandas,
     arrow_to_parquet,
     pandas_to_arrow,
```

### Comparing `warpzone_sdk-8.3.4/warpzone/blobstorage/client.py` & `warpzone_sdk-8.3.5/warpzone/blobstorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/function/checks.py` & `warpzone_sdk-8.3.5/warpzone/function/checks.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/function/functionize.py` & `warpzone_sdk-8.3.5/warpzone/function/functionize.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/function/integrations.py` & `warpzone_sdk-8.3.5/warpzone/function/integrations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/function/monitor.py` & `warpzone_sdk-8.3.5/warpzone/function/monitor.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/function/process.py` & `warpzone_sdk-8.3.5/warpzone/function/process.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/function/processors/dependencies.py` & `warpzone_sdk-8.3.5/warpzone/function/processors/dependencies.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/function/processors/outputs.py` & `warpzone_sdk-8.3.5/warpzone/function/processors/outputs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/function/processors/triggers.py` & `warpzone_sdk-8.3.5/warpzone/function/processors/triggers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/function/signature.py` & `warpzone_sdk-8.3.5/warpzone/function/signature.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/function/types.py` & `warpzone_sdk-8.3.5/warpzone/function/types.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/healthchecks/__init__.py` & `warpzone_sdk-8.3.5/warpzone/healthchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/healthchecks/model.py` & `warpzone_sdk-8.3.5/warpzone/healthchecks/model.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/monitor/logs.py` & `warpzone_sdk-8.3.5/warpzone/monitor/logs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/monitor/traces.py` & `warpzone_sdk-8.3.5/warpzone/monitor/traces.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/servicebus/data/client.py` & `warpzone_sdk-8.3.5/warpzone/servicebus/data/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/servicebus/events/client.py` & `warpzone_sdk-8.3.5/warpzone/servicebus/events/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/tablestorage/db/base_client.py` & `warpzone_sdk-8.3.5/warpzone/tablestorage/db/base_client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/tablestorage/db/client.py` & `warpzone_sdk-8.3.5/warpzone/tablestorage/db/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/tablestorage/db/client_async.py` & `warpzone_sdk-8.3.5/warpzone/tablestorage/db/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/tablestorage/tables/client.py` & `warpzone_sdk-8.3.5/warpzone/tablestorage/tables/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/tablestorage/tables/client_async.py` & `warpzone_sdk-8.3.5/warpzone/tablestorage/tables/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/tablestorage/tables/operations.py` & `warpzone_sdk-8.3.5/warpzone/tablestorage/tables/operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import defaultdict
 
 import pandas as pd
 
-from .helpers import chunkify
+from .helpers import chunkify, generate_valid_table_keys
 
 
 class TableOperations:
     def __init__(self, max_chunk_size: int = 100) -> None:
         self._max_chunk_size = max_chunk_size
         self._partitions = defaultdict(list)
 
@@ -47,16 +47,26 @@
     ):
         datetime_columns = df.select_dtypes(["datetime", "datetimetz"]).columns
 
         for column in datetime_columns:
             df[column] = df[column].dt.strftime("%Y-%m-%dT%H:%M:%SZ")
             df[f"{column}@odata.type"] = "Edm.DateTime"
 
-        df["PartitionKey"] = df[partition_keys].astype(str).agg("_".join, axis=1)
-        df["RowKey"] = df[row_keys].astype(str).agg("_".join, axis=1)
+        df["PartitionKey"] = (
+            df[partition_keys]
+            .astype(str)
+            .agg("_".join, axis=1)
+            .apply(generate_valid_table_keys)
+        )
+        df["RowKey"] = (
+            df[row_keys]
+            .astype(str)
+            .agg("_".join, axis=1)
+            .apply(generate_valid_table_keys)
+        )
 
         operations = cls()
         for _, partition_group in df.groupby(partition_keys):
             entities = partition_group.to_dict("records")
             operations.add(entities, operation_type)
 
         return operations
```

### Comparing `warpzone_sdk-8.3.4/warpzone/testing/assertions.py` & `warpzone_sdk-8.3.5/warpzone/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/testing/data.py` & `warpzone_sdk-8.3.5/warpzone/testing/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/transform/data.py` & `warpzone_sdk-8.3.5/warpzone/transform/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/warpzone/transform/schema.py` & `warpzone_sdk-8.3.5/warpzone/transform/schema.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.4/PKG-INFO` & `warpzone_sdk-8.3.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warpzone-sdk
-Version: 8.3.4
+Version: 8.3.5
 Summary: The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage
 Author: Mikkel Ladekarl Folmersen Nygaard
 Author-email: mny@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

