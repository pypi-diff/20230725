# Comparing `tmp/stigg_api_client-0.502.0.tar.gz` & `tmp/stigg_api_client-0.503.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.502.0.tar", max compression
+gzip compressed data, was "stigg_api_client-0.503.0.tar", max compression
```

## Comparing `stigg_api_client-0.502.0.tar` & `stigg_api_client-0.503.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-07-23 16:25:27.250014 stigg_api_client-0.502.0/README.md
--rw-r--r--   0        0        0      460 2023-07-23 16:26:00.458070 stigg_api_client-0.502.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-23 16:25:27.250014 stigg_api_client-0.502.0/stigg/__init__.py
--rw-r--r--   0        0        0     1141 2023-07-23 16:25:27.250014 stigg_api_client-0.502.0/stigg/client.py
--rw-r--r--   0        0        0        0 2023-07-23 16:25:58.542063 stigg_api_client-0.502.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    49477 2023-07-23 16:25:58.954065 stigg_api_client-0.502.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   465343 2023-07-23 16:25:58.802064 stigg_api_client-0.502.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 stigg_api_client-0.502.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-07-25 06:51:35.612858 stigg_api_client-0.503.0/README.md
+-rw-r--r--   0        0        0      460 2023-07-25 06:52:11.427219 stigg_api_client-0.503.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-25 06:51:35.612858 stigg_api_client-0.503.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1141 2023-07-25 06:51:35.612858 stigg_api_client-0.503.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-07-25 06:52:09.367084 stigg_api_client-0.503.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    49477 2023-07-25 06:52:09.819114 stigg_api_client-0.503.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   465775 2023-07-25 06:52:09.651102 stigg_api_client-0.503.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 stigg_api_client-0.503.0/PKG-INFO
```

### Comparing `stigg_api_client-0.502.0/README.md` & `stigg_api_client-0.503.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.502.0/stigg/client.py` & `stigg_api_client-0.503.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.502.0/stigg/generated/operations.py` & `stigg_api_client-0.503.0/stigg/generated/operations.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.502.0/stigg/generated/schema.py` & `stigg_api_client-0.503.0/stigg/generated/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -2948,14 +2948,20 @@
 class SubscriptionUpdateScheduleCancellationInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('environment_id', 'subscription_id')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     subscription_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='subscriptionId')
 
 
+class SyncTaxRatesInput(sgqlc.types.Input):
+    __schema__ = schema
+    __field_names__ = ('environment_id',)
+    environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
+
+
 class TaskStatusFilterComparison(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('eq', 'gt', 'gte', 'i_like', 'in_', 'is_', 'is_not', 'like', 'lt', 'lte', 'neq', 'not_ilike', 'not_in', 'not_like')
     eq = sgqlc.types.Field(TaskStatus, graphql_name='eq')
     gt = sgqlc.types.Field(TaskStatus, graphql_name='gt')
     gte = sgqlc.types.Field(TaskStatus, graphql_name='gte')
     i_like = sgqlc.types.Field(TaskStatus, graphql_name='iLike')
@@ -5194,15 +5200,15 @@
     __schema__ = schema
     __field_names__ = ('monthly_according_to',)
     monthly_according_to = sgqlc.types.Field(MonthlyAccordingTo, graphql_name='monthlyAccordingTo')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('add_compatible_addons_to_plan', 'archive_customer', 'archive_one_coupon', 'archive_plan', 'attach_customer_payment_method', 'cancel_schedule', 'cancel_subscription', 'create_account', 'create_addon_draft', 'create_feature', 'create_many_package_entitlements', 'create_many_promotional_entitlements', 'create_one_addon', 'create_one_coupon', 'create_one_customer', 'create_one_environment', 'create_one_experiment', 'create_one_feature', 'create_one_hook', 'create_one_integration', 'create_one_plan', 'create_one_product', 'create_plan_draft', 'create_subscription', 'create_usage_measurement', 'delete_environment', 'delete_feature', 'delete_one_addon', 'delete_one_environment', 'delete_one_feature', 'delete_one_hook', 'delete_one_integration', 'delete_one_package_entitlement', 'delete_one_price', 'delete_one_product', 'delete_one_promotional_entitlement', 'estimate_subscription', 'estimate_subscription_update', 'hide_getting_started_page', 'import_customers_bulk', 'import_one_customer', 'import_subscriptions_bulk', 'init_add_stripe_customer_payment_method', 'invite_members', 'migrate_subscription_to_latest', 'provision_customer', 'provision_sandbox', 'provision_subscription', 'provision_subscription_v2', 'publish_addon', 'publish_plan', 'purge_customer_cache', 'recalculate_entitlements', 'register_member', 'remove_addon_draft', 'remove_base_plan_from_plan', 'remove_compatible_addons_from_plan', 'remove_coupon_from_customer', 'remove_coupon_from_customer_subscription', 'remove_experiment_from_customer', 'remove_experiment_from_customer_subscription', 'remove_member', 'remove_plan_draft', 'report_entitlement_check_requested', 'report_event', 'report_usage', 'resend_email_verification', 'resync_integration', 'set_base_plan_on_plan', 'set_compatible_addons_on_plan', 'set_coupon_on_customer', 'set_coupon_on_customer_subscription', 'set_experiment_on_customer', 'set_experiment_on_customer_subscription', 'set_package_pricing', 'set_widget_configuration', 'start_experiment', 'stop_experiment', 'trigger_import_catalog', 'trigger_import_customers', 'update_account', 'update_entitlements_order', 'update_feature', 'update_one_addon', 'update_one_coupon', 'update_one_customer', 'update_one_environment', 'update_one_experiment', 'update_one_feature', 'update_one_hook', 'update_one_integration', 'update_one_package_entitlement', 'update_one_plan', 'update_one_product', 'update_one_promotional_entitlement', 'update_one_subscription', 'update_user')
+    __field_names__ = ('add_compatible_addons_to_plan', 'archive_customer', 'archive_one_coupon', 'archive_plan', 'attach_customer_payment_method', 'cancel_schedule', 'cancel_subscription', 'create_account', 'create_addon_draft', 'create_feature', 'create_many_package_entitlements', 'create_many_promotional_entitlements', 'create_one_addon', 'create_one_coupon', 'create_one_customer', 'create_one_environment', 'create_one_experiment', 'create_one_feature', 'create_one_hook', 'create_one_integration', 'create_one_plan', 'create_one_product', 'create_plan_draft', 'create_subscription', 'create_usage_measurement', 'delete_environment', 'delete_feature', 'delete_one_addon', 'delete_one_environment', 'delete_one_feature', 'delete_one_hook', 'delete_one_integration', 'delete_one_package_entitlement', 'delete_one_price', 'delete_one_product', 'delete_one_promotional_entitlement', 'estimate_subscription', 'estimate_subscription_update', 'hide_getting_started_page', 'import_customers_bulk', 'import_one_customer', 'import_subscriptions_bulk', 'init_add_stripe_customer_payment_method', 'invite_members', 'migrate_subscription_to_latest', 'provision_customer', 'provision_sandbox', 'provision_subscription', 'provision_subscription_v2', 'publish_addon', 'publish_plan', 'purge_customer_cache', 'recalculate_entitlements', 'register_member', 'remove_addon_draft', 'remove_base_plan_from_plan', 'remove_compatible_addons_from_plan', 'remove_coupon_from_customer', 'remove_coupon_from_customer_subscription', 'remove_experiment_from_customer', 'remove_experiment_from_customer_subscription', 'remove_member', 'remove_plan_draft', 'report_entitlement_check_requested', 'report_event', 'report_usage', 'resend_email_verification', 'resync_integration', 'set_base_plan_on_plan', 'set_compatible_addons_on_plan', 'set_coupon_on_customer', 'set_coupon_on_customer_subscription', 'set_experiment_on_customer', 'set_experiment_on_customer_subscription', 'set_package_pricing', 'set_widget_configuration', 'start_experiment', 'stop_experiment', 'sync_tax_rates', 'trigger_import_catalog', 'trigger_import_customers', 'update_account', 'update_entitlements_order', 'update_feature', 'update_one_addon', 'update_one_coupon', 'update_one_customer', 'update_one_environment', 'update_one_experiment', 'update_one_feature', 'update_one_hook', 'update_one_integration', 'update_one_package_entitlement', 'update_one_plan', 'update_one_product', 'update_one_promotional_entitlement', 'update_one_subscription', 'update_user')
     add_compatible_addons_to_plan = sgqlc.types.Field(sgqlc.types.non_null('Plan'), graphql_name='addCompatibleAddonsToPlan', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(AddCompatibleAddonsToPlanInput), graphql_name='input', default=None)),
 ))
     )
     archive_customer = sgqlc.types.Field(sgqlc.types.non_null(Customer), graphql_name='archiveCustomer', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(ArchiveCustomerInput), graphql_name='input', default=None)),
 ))
@@ -5501,14 +5507,18 @@
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(StartExperimentInput), graphql_name='input', default=None)),
 ))
     )
     stop_experiment = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='stopExperiment', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(StopExperimentInput), graphql_name='input', default=None)),
 ))
     )
+    sync_tax_rates = sgqlc.types.Field(String, graphql_name='syncTaxRates', args=sgqlc.types.ArgDict((
+        ('input', sgqlc.types.Arg(sgqlc.types.non_null(SyncTaxRatesInput), graphql_name='input', default=None)),
+))
+    )
     trigger_import_catalog = sgqlc.types.Field(sgqlc.types.non_null(AsyncTaskResult), graphql_name='triggerImportCatalog', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(ImportIntegrationCatalogInput), graphql_name='input', default=None)),
 ))
     )
     trigger_import_customers = sgqlc.types.Field(sgqlc.types.non_null(AsyncTaskResult), graphql_name='triggerImportCustomers', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(ImportIntegrationCustomersInput), graphql_name='input', default=None)),
 ))
```

### Comparing `stigg_api_client-0.502.0/PKG-INFO` & `stigg_api_client-0.503.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.502.0
+Version: 0.503.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

