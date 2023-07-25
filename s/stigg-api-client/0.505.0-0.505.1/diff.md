# Comparing `tmp/stigg_api_client-0.505.0.tar.gz` & `tmp/stigg_api_client-0.505.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.505.0.tar", max compression
+gzip compressed data, was "stigg_api_client-0.505.1.tar", max compression
```

## Comparing `stigg_api_client-0.505.0.tar` & `stigg_api_client-0.505.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-07-25 15:32:58.059762 stigg_api_client-0.505.0/README.md
--rw-r--r--   0        0        0      460 2023-07-25 15:33:51.737270 stigg_api_client-0.505.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-25 15:32:58.059762 stigg_api_client-0.505.0/stigg/__init__.py
--rw-r--r--   0        0        0     1141 2023-07-25 15:32:58.059762 stigg_api_client-0.505.0/stigg/client.py
--rw-r--r--   0        0        0        0 2023-07-25 15:33:49.209197 stigg_api_client-0.505.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    49504 2023-07-25 15:33:49.757212 stigg_api_client-0.505.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   465793 2023-07-25 15:33:49.553207 stigg_api_client-0.505.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 stigg_api_client-0.505.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-07-25 16:15:50.595696 stigg_api_client-0.505.1/README.md
+-rw-r--r--   0        0        0      460 2023-07-25 16:16:40.304018 stigg_api_client-0.505.1/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-25 16:15:50.595696 stigg_api_client-0.505.1/stigg/__init__.py
+-rw-r--r--   0        0        0     1141 2023-07-25 16:15:50.595696 stigg_api_client-0.505.1/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-07-25 16:16:37.868003 stigg_api_client-0.505.1/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    49504 2023-07-25 16:16:38.388006 stigg_api_client-0.505.1/stigg/generated/operations.py
+-rw-r--r--   0        0        0   465924 2023-07-25 16:16:38.176005 stigg_api_client-0.505.1/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 stigg_api_client-0.505.1/PKG-INFO
```

### Comparing `stigg_api_client-0.505.0/README.md` & `stigg_api_client-0.505.1/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.505.0/stigg/client.py` & `stigg_api_client-0.505.1/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.505.0/stigg/generated/operations.py` & `stigg_api_client-0.505.1/stigg/generated/operations.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.505.0/stigg/generated/schema.py` & `stigg_api_client-0.505.1/stigg/generated/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -3195,17 +3195,18 @@
     reset_period = sgqlc.types.Field(EntitlementResetPeriod, graphql_name='resetPeriod')
     usage_limit = sgqlc.types.Field(Float, graphql_name='usageLimit')
     weekly_reset_period_configuration = sgqlc.types.Field('WeeklyResetPeriodConfigInput', graphql_name='weeklyResetPeriodConfiguration')
 
 
 class UpdateSubscriptionInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'addons', 'billable_features', 'billing_period', 'environment_id', 'promotion_code', 'ref_id', 'subscription_entitlements', 'subscription_id', 'trial_end_date', 'unit_quantity')
+    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billable_features', 'billing_period', 'environment_id', 'promotion_code', 'ref_id', 'subscription_entitlements', 'subscription_id', 'trial_end_date', 'unit_quantity')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(SubscriptionAddonInput)), graphql_name='addons')
+    await_payment_confirmation = sgqlc.types.Field(Boolean, graphql_name='awaitPaymentConfirmation')
     billable_features = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(BillableFeatureInput)), graphql_name='billableFeatures')
     billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     promotion_code = sgqlc.types.Field(String, graphql_name='promotionCode')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
     subscription_entitlements = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(UpdateSubscriptionEntitlementInput)), graphql_name='subscriptionEntitlements')
     subscription_id = sgqlc.types.Field(String, graphql_name='subscriptionId')
```

### Comparing `stigg_api_client-0.505.0/PKG-INFO` & `stigg_api_client-0.505.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.505.0
+Version: 0.505.1
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

