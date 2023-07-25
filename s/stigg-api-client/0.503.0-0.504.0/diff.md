# Comparing `tmp/stigg_api_client-0.503.0.tar.gz` & `tmp/stigg_api_client-0.504.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.503.0.tar", max compression
+gzip compressed data, was "stigg_api_client-0.504.0.tar", max compression
```

## Comparing `stigg_api_client-0.503.0.tar` & `stigg_api_client-0.504.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-07-25 06:51:35.612858 stigg_api_client-0.503.0/README.md
--rw-r--r--   0        0        0      460 2023-07-25 06:52:11.427219 stigg_api_client-0.503.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-25 06:51:35.612858 stigg_api_client-0.503.0/stigg/__init__.py
--rw-r--r--   0        0        0     1141 2023-07-25 06:51:35.612858 stigg_api_client-0.503.0/stigg/client.py
--rw-r--r--   0        0        0        0 2023-07-25 06:52:09.367084 stigg_api_client-0.503.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    49477 2023-07-25 06:52:09.819114 stigg_api_client-0.503.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   465775 2023-07-25 06:52:09.651102 stigg_api_client-0.503.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 stigg_api_client-0.503.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-07-25 10:54:05.022805 stigg_api_client-0.504.0/README.md
+-rw-r--r--   0        0        0      460 2023-07-25 10:54:52.695342 stigg_api_client-0.504.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-25 10:54:05.022805 stigg_api_client-0.504.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1141 2023-07-25 10:54:05.022805 stigg_api_client-0.504.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:54:50.731320 stigg_api_client-0.504.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    49504 2023-07-25 10:54:51.187325 stigg_api_client-0.504.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   465775 2023-07-25 10:54:51.023323 stigg_api_client-0.504.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 stigg_api_client-0.504.0/PKG-INFO
```

### Comparing `stigg_api_client-0.503.0/README.md` & `stigg_api_client-0.504.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.503.0/stigg/client.py` & `stigg_api_client-0.504.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.503.0/stigg/generated/operations.py` & `stigg_api_client-0.504.0/stigg/generated/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 def fragment_plan_fragment():
     _frag = sgqlc.operation.Fragment(_schema.Plan, 'PlanFragment')
     _frag.id()
     _frag.ref_id()
     _frag.display_name()
     _frag.description()
     _frag.billing_id()
+    _frag.version_number()
     _frag.additional_meta_data()
     _frag_product = _frag.product()
     _frag_product.__fragment__(fragment_product_fragment())
     _frag_base_plan = _frag.base_plan()
     _frag_base_plan.ref_id()
     _frag_base_plan.display_name()
     _frag_entitlements = _frag.entitlements()
```

### Comparing `stigg_api_client-0.503.0/stigg/generated/schema.py` & `stigg_api_client-0.504.0/stigg/generated/schema.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.503.0/PKG-INFO` & `stigg_api_client-0.504.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.503.0
+Version: 0.504.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

