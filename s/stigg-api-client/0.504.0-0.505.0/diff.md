# Comparing `tmp/stigg_api_client-0.504.0.tar.gz` & `tmp/stigg_api_client-0.505.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.504.0.tar", max compression
+gzip compressed data, was "stigg_api_client-0.505.0.tar", max compression
```

## Comparing `stigg_api_client-0.504.0.tar` & `stigg_api_client-0.505.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-07-25 10:54:05.022805 stigg_api_client-0.504.0/README.md
--rw-r--r--   0        0        0      460 2023-07-25 10:54:52.695342 stigg_api_client-0.504.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-25 10:54:05.022805 stigg_api_client-0.504.0/stigg/__init__.py
--rw-r--r--   0        0        0     1141 2023-07-25 10:54:05.022805 stigg_api_client-0.504.0/stigg/client.py
--rw-r--r--   0        0        0        0 2023-07-25 10:54:50.731320 stigg_api_client-0.504.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    49504 2023-07-25 10:54:51.187325 stigg_api_client-0.504.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   465775 2023-07-25 10:54:51.023323 stigg_api_client-0.504.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 stigg_api_client-0.504.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-07-25 15:32:58.059762 stigg_api_client-0.505.0/README.md
+-rw-r--r--   0        0        0      460 2023-07-25 15:33:51.737270 stigg_api_client-0.505.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-25 15:32:58.059762 stigg_api_client-0.505.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1141 2023-07-25 15:32:58.059762 stigg_api_client-0.505.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-07-25 15:33:49.209197 stigg_api_client-0.505.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    49504 2023-07-25 15:33:49.757212 stigg_api_client-0.505.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   465793 2023-07-25 15:33:49.553207 stigg_api_client-0.505.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 stigg_api_client-0.505.0/PKG-INFO
```

### Comparing `stigg_api_client-0.504.0/README.md` & `stigg_api_client-0.505.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.504.0/stigg/client.py` & `stigg_api_client-0.505.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.504.0/stigg/generated/operations.py` & `stigg_api_client-0.505.0/stigg/generated/operations.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.504.0/stigg/generated/schema.py` & `stigg_api_client-0.505.0/stigg/generated/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
 class SubscriptionPriceSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('billingModel', 'createdAt', 'featureId', 'id', 'updatedAt', 'usageLimit')
 
 
 class SubscriptionScheduleStatus(sgqlc.types.Enum):
     __schema__ = schema
-    __choices__ = ('Canceled', 'Done', 'Failed', 'Scheduled')
+    __choices__ = ('Canceled', 'Done', 'Failed', 'PendingPayment', 'Scheduled')
 
 
 class SubscriptionScheduleType(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('BillingPeriod', 'Downgrade', 'MigrateToLatest', 'UnitAmount')
```

### Comparing `stigg_api_client-0.504.0/PKG-INFO` & `stigg_api_client-0.505.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.504.0
+Version: 0.505.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

