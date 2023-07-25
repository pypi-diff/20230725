# Comparing `tmp/stigg_api_client_v2-0.502.0.tar.gz` & `tmp/stigg_api_client_v2-0.503.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.502.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.503.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.502.0.tar` & `stigg_api_client_v2-0.503.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1644 2023-07-23 16:25:30.247952 stigg_api_client_v2-0.502.0/README.md
--rw-r--r--   0        0        0      432 2023-07-23 16:26:35.519321 stigg_api_client_v2-0.502.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-23 16:25:30.247952 stigg_api_client_v2-0.502.0/stigg/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-23 16:25:30.247952 stigg_api_client_v2-0.502.0/stigg/client.py
--rw-r--r--   0        0        0    40226 2023-07-23 16:26:32.823344 stigg_api_client_v2-0.502.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0      460 2023-07-23 16:26:30.739362 stigg_api_client_v2-0.502.0/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0     7303 2023-07-23 16:26:32.215350 stigg_api_client_v2-0.502.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    68230 2023-07-23 16:26:32.571347 stigg_api_client_v2-0.502.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-23 16:26:23.931429 stigg_api_client_v2-0.502.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-23 16:26:32.215350 stigg_api_client_v2-0.502.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-23 16:26:30.647363 stigg_api_client_v2-0.502.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-23 16:26:30.679363 stigg_api_client_v2-0.502.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    67803 2023-07-23 16:26:24.247426 stigg_api_client_v2-0.502.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-23 16:26:30.719363 stigg_api_client_v2-0.502.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24160 2023-07-23 16:26:26.839400 stigg_api_client_v2-0.502.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-23 16:26:30.659363 stigg_api_client_v2-0.502.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-23 16:26:30.675363 stigg_api_client_v2-0.502.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-23 16:26:32.215350 stigg_api_client_v2-0.502.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    56292 2023-07-23 16:26:32.211350 stigg_api_client_v2-0.502.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-23 16:26:30.763362 stigg_api_client_v2-0.502.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-23 16:26:30.775362 stigg_api_client_v2-0.502.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-23 16:26:30.751362 stigg_api_client_v2-0.502.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-23 16:26:30.839362 stigg_api_client_v2-0.502.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-23 16:26:30.799362 stigg_api_client_v2-0.502.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-23 16:26:30.791362 stigg_api_client_v2-0.502.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-23 16:26:30.851361 stigg_api_client_v2-0.502.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-23 16:26:30.783362 stigg_api_client_v2-0.502.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-23 16:26:30.811362 stigg_api_client_v2-0.502.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-23 16:26:30.827361 stigg_api_client_v2-0.502.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-23 16:26:30.583364 stigg_api_client_v2-0.502.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-23 16:26:30.575364 stigg_api_client_v2-0.502.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-23 16:26:30.623363 stigg_api_client_v2-0.502.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   126830 2023-07-23 16:26:30.551364 stigg_api_client_v2-0.502.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-23 16:26:30.731362 stigg_api_client_v2-0.502.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-23 16:26:30.567364 stigg_api_client_v2-0.502.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-23 16:26:30.611364 stigg_api_client_v2-0.502.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-23 16:26:30.707363 stigg_api_client_v2-0.502.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-23 16:26:30.703363 stigg_api_client_v2-0.502.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-23 16:26:30.695363 stigg_api_client_v2-0.502.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-23 16:26:32.219349 stigg_api_client_v2-0.502.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-23 16:26:30.591364 stigg_api_client_v2-0.502.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-23 16:26:30.635363 stigg_api_client_v2-0.502.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-23 16:26:30.863361 stigg_api_client_v2-0.502.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.502.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-25 06:51:36.042290 stigg_api_client_v2-0.503.0/README.md
+-rw-r--r--   0        0        0      432 2023-07-25 06:52:30.769405 stigg_api_client_v2-0.503.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-25 06:51:36.042290 stigg_api_client_v2-0.503.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-25 06:51:36.042290 stigg_api_client_v2-0.503.0/stigg/client.py
+-rw-r--r--   0        0        0    40274 2023-07-25 06:52:28.713289 stigg_api_client_v2-0.503.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-25 06:52:27.197203 stigg_api_client_v2-0.503.0/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-07-25 06:52:28.257263 stigg_api_client_v2-0.503.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    68230 2023-07-25 06:52:28.521278 stigg_api_client_v2-0.503.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-25 06:52:22.180918 stigg_api_client_v2-0.503.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-25 06:52:28.261263 stigg_api_client_v2-0.503.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-25 06:52:27.129199 stigg_api_client_v2-0.503.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-25 06:52:27.153200 stigg_api_client_v2-0.503.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    67803 2023-07-25 06:52:22.448933 stigg_api_client_v2-0.503.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-25 06:52:27.181202 stigg_api_client_v2-0.503.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24160 2023-07-25 06:52:24.397044 stigg_api_client_v2-0.503.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-25 06:52:27.137199 stigg_api_client_v2-0.503.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-25 06:52:27.145200 stigg_api_client_v2-0.503.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-25 06:52:28.261263 stigg_api_client_v2-0.503.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    56292 2023-07-25 06:52:28.257263 stigg_api_client_v2-0.503.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-25 06:52:27.213204 stigg_api_client_v2-0.503.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-25 06:52:27.225205 stigg_api_client_v2-0.503.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-25 06:52:27.205203 stigg_api_client_v2-0.503.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-25 06:52:27.273207 stigg_api_client_v2-0.503.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-25 06:52:27.245206 stigg_api_client_v2-0.503.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-25 06:52:27.237205 stigg_api_client_v2-0.503.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-25 06:52:27.281208 stigg_api_client_v2-0.503.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-25 06:52:27.233205 stigg_api_client_v2-0.503.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-25 06:52:27.253206 stigg_api_client_v2-0.503.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-25 06:52:27.265207 stigg_api_client_v2-0.503.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-25 06:52:27.089197 stigg_api_client_v2-0.503.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-25 06:52:27.081196 stigg_api_client_v2-0.503.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-25 06:52:27.117199 stigg_api_client_v2-0.503.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   126973 2023-07-25 06:52:27.061195 stigg_api_client_v2-0.503.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-25 06:52:27.189203 stigg_api_client_v2-0.503.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-25 06:52:27.077196 stigg_api_client_v2-0.503.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-25 06:52:27.109198 stigg_api_client_v2-0.503.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-25 06:52:27.173202 stigg_api_client_v2-0.503.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-25 06:52:27.169201 stigg_api_client_v2-0.503.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-25 06:52:27.161201 stigg_api_client_v2-0.503.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-25 06:52:28.265264 stigg_api_client_v2-0.503.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-25 06:52:27.097197 stigg_api_client_v2-0.503.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-25 06:52:27.121199 stigg_api_client_v2-0.503.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-25 06:52:27.289208 stigg_api_client_v2-0.503.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.503.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.502.0/README.md` & `stigg_api_client_v2-0.503.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.502.0/stigg/client.py` & `stigg_api_client_v2-0.503.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.503.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 
 from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
@@ -542,14 +542,15 @@
     SubscriptionMigrationTaskSort,
     SubscriptionPriceFilter,
     SubscriptionPriceFilterCustomerSubscriptionFilter,
     SubscriptionPriceFilterPriceFilter,
     SubscriptionPriceSort,
     SubscriptionStatusFilterComparison,
     SubscriptionUpdateScheduleCancellationInput,
+    SyncTaxRatesInput,
     TaskStatusFilterComparison,
     TaskTypeFilterComparison,
     TaxExempt,
     TestHookInput,
     TypographyConfigurationInput,
     UpdateAccountInput,
     UpdateCouponInput,
@@ -1125,14 +1126,15 @@
     "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
     "SubscriptionScheduledUpdateDataTargetPackage",
     "SubscriptionStartSetup",
     "SubscriptionStatus",
     "SubscriptionStatusFilterComparison",
     "SubscriptionUpdateScheduleCancellationInput",
     "SyncStatus",
+    "SyncTaxRatesInput",
     "TaskStatus",
     "TaskStatusFilterComparison",
     "TaskType",
     "TaskTypeFilterComparison",
     "TaxExempt",
     "TestHookInput",
     "TotalPriceFragment",
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.503.0/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.503.0/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.503.0/stigg/generated/base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.503.0/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.503.0/stigg/generated/cancel_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/client.py` & `stigg_api_client_v2-0.503.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.503.0/stigg/generated/create_subscription.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.503.0/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerIsArchived = "CustomerIsArchived"
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.503.0/stigg/generated/estimate_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.503.0/stigg/generated/estimate_subscription_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.503.0/stigg/generated/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.503.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -32,36 +32,14 @@
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
     experimentGroupType,
 )
 
 
-class PackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    feature_id: str = Field(alias="featureId")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    is_custom: Optional[bool] = Field(alias="isCustom")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: "PackageEntitlementFragmentFeature"
-
-
-class PackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class PriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -78,14 +56,36 @@
     ref_id: str = Field(alias="refId")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
+class PackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    feature_id: str = Field(alias="featureId")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    is_custom: Optional[bool] = Field(alias="isCustom")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: "PackageEntitlementFragmentFeature"
+
+
+class PackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class AddonFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     billing_id: Optional[str] = Field(alias="billingId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -125,25 +125,14 @@
     status: SyncStatus
 
 
 class CouponFragmentCustomers(BaseModel):
     id: str
 
 
-class SlimCustomerFragment(BaseModel):
-    id: str
-    name: Optional[str]
-    email: Optional[str]
-    created_at: Optional[Any] = Field(alias="createdAt")
-    updated_at: Any = Field(alias="updatedAt")
-    ref_id: str = Field(alias="refId")
-    billing_id: Optional[str] = Field(alias="billingId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class PromotionalEntitlementFragment(BaseModel):
     status: PromotionalEntitlementStatus
     usage_limit: Optional[float] = Field(alias="usageLimit")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -158,14 +147,25 @@
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     ref_id: str = Field(alias="refId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
 
 
+class SlimCustomerFragment(BaseModel):
+    id: str
+    name: Optional[str]
+    email: Optional[str]
+    created_at: Optional[Any] = Field(alias="createdAt")
+    updated_at: Any = Field(alias="updatedAt")
+    ref_id: str = Field(alias="refId")
+    billing_id: Optional[str] = Field(alias="billingId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -338,23 +338,32 @@
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     usage_limit: Optional[float] = Field(alias="usageLimit")
     period: PromotionalEntitlementPeriod
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
 
 
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
+class CustomerPortalSubscriptionPriceFragment(BaseModel):
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    billing_model: Optional[BillingModel] = Field(alias="billingModel")
+    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
+    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
 
 
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
+class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
-    quantity: int
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
 
 
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
@@ -401,32 +410,19 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
-class CustomerPortalSubscriptionPriceFragment(BaseModel):
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    billing_model: Optional[BillingModel] = Field(alias="billingModel")
-    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
-    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
-
-
-class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
     display_name: str = Field(alias="displayName")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    quantity: int
 
 
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing_type: PricingType = Field(alias="pricingType")
     prices: List["CustomerPortalSubscriptionFragmentPrices"]
@@ -506,14 +502,18 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -548,14 +548,29 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
+class TotalPriceFragment(BaseModel):
+    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
+    total: "TotalPriceFragmentTotal"
+
+
+class TotalPriceFragmentSubTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class TotalPriceFragmentTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -620,29 +635,14 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
-class TotalPriceFragment(BaseModel):
-    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
-    total: "TotalPriceFragmentTotal"
-
-
-class TotalPriceFragmentSubTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class TotalPriceFragmentTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
 class SubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
@@ -1341,28 +1341,28 @@
 
 class UsageHistoryFragmentUsageMeasurements(BaseModel):
     date: Any
     value: float
     is_reset_point: Optional[bool] = Field(alias="isResetPoint")
 
 
-PackageEntitlementFragment.update_forward_refs()
-PackageEntitlementFragmentFeature.update_forward_refs()
 PriceFragment.update_forward_refs()
 PriceFragmentPrice.update_forward_refs()
 PriceFragmentFeature.update_forward_refs()
+PackageEntitlementFragment.update_forward_refs()
+PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
-SlimCustomerFragment.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
 PromotionalEntitlementFragmentFeature.update_forward_refs()
+SlimCustomerFragment.update_forward_refs()
 CustomerFragment.update_forward_refs()
 CustomerFragmentTrialedPlans.update_forward_refs()
 CustomerFragmentExperimentInfo.update_forward_refs()
 CustomerFragmentCoupon.update_forward_refs()
 CustomerFragmentEligibleForTrial.update_forward_refs()
 CustomerFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalBillingInformation.update_forward_refs()
@@ -1377,57 +1377,57 @@
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
 CustomerPortalPromotionalEntitlement.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
+CustomerPortalSubscriptionPriceFragment.update_forward_refs()
+CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
+CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-CustomerPortalSubscriptionPriceFragment.update_forward_refs()
-CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
-CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
+TotalPriceFragment.update_forward_refs()
+TotalPriceFragmentSubTotal.update_forward_refs()
+TotalPriceFragmentTotal.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
 PlanFragmentInheritedEntitlements.update_forward_refs()
 PlanFragmentCompatibleAddons.update_forward_refs()
 PlanFragmentPrices.update_forward_refs()
 PlanFragmentDefaultTrialConfig.update_forward_refs()
-TotalPriceFragment.update_forward_refs()
-TotalPriceFragmentSubTotal.update_forward_refs()
-TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionScheduledUpdateData.update_forward_refs()
 SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.503.0/stigg/generated/get_active_subscriptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.503.0/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.503.0/stigg/generated/get_customer_by_id.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.503.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.503.0/stigg/generated/get_mock_paywall.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.503.0/stigg/generated/get_products.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.503.0/stigg/generated/get_sdk_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.503.0/stigg/generated/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -2398,14 +2398,18 @@
 
 
 class SubscriptionUpdateScheduleCancellationInput(BaseModel):
     environment_id: Optional[str] = Field(alias="environmentId")
     subscription_id: str = Field(alias="subscriptionId")
 
 
+class SyncTaxRatesInput(BaseModel):
+    environment_id: Optional[str] = Field(alias="environmentId")
+
+
 class TaskStatusFilterComparison(BaseModel):
     eq: Optional[TaskStatus]
     gt: Optional[TaskStatus]
     gte: Optional[TaskStatus]
     i_like: Optional[TaskStatus] = Field(alias="iLike")
     in_: Optional[List[TaskStatus]] = Field(alias="in")
     is_: Optional[bool] = Field(alias="is")
@@ -2981,14 +2985,15 @@
 SubscriptionMigrationTaskSort.update_forward_refs()
 SubscriptionPriceFilter.update_forward_refs()
 SubscriptionPriceFilterCustomerSubscriptionFilter.update_forward_refs()
 SubscriptionPriceFilterPriceFilter.update_forward_refs()
 SubscriptionPriceSort.update_forward_refs()
 SubscriptionStatusFilterComparison.update_forward_refs()
 SubscriptionUpdateScheduleCancellationInput.update_forward_refs()
+SyncTaxRatesInput.update_forward_refs()
 TaskStatusFilterComparison.update_forward_refs()
 TaskTypeFilterComparison.update_forward_refs()
 TaxExempt.update_forward_refs()
 TestHookInput.update_forward_refs()
 TypographyConfigurationInput.update_forward_refs()
 UpdateAccountInput.update_forward_refs()
 UpdateCouponInput.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.503.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.503.0/stigg/generated/provision_customer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.503.0/stigg/generated/provision_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.502.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.503.0/stigg/generated/update_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-23 16:26
+# Generated by ariadne-codegen on 2023-07-25 06:52
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.502.0/PKG-INFO` & `stigg_api_client_v2-0.503.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.502.0
+Version: 0.503.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

