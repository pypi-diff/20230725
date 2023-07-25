# Comparing `tmp/stigg_api_client_v2-0.505.0.tar.gz` & `tmp/stigg_api_client_v2-0.505.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.505.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.505.1.tar", max compression
```

## Comparing `stigg_api_client_v2-0.505.0.tar` & `stigg_api_client_v2-0.505.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1644 2023-07-25 15:32:57.775076 stigg_api_client_v2-0.505.0/README.md
--rw-r--r--   0        0        0      432 2023-07-25 15:34:13.830574 stigg_api_client_v2-0.505.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-25 15:32:57.779076 stigg_api_client_v2-0.505.0/stigg/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-25 15:32:57.779076 stigg_api_client_v2-0.505.0/stigg/client.py
--rw-r--r--   0        0        0    40274 2023-07-25 15:34:11.722478 stigg_api_client_v2-0.505.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0      460 2023-07-25 15:34:09.918394 stigg_api_client_v2-0.505.0/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0     7303 2023-07-25 15:34:11.094448 stigg_api_client_v2-0.505.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    68314 2023-07-25 15:34:11.378462 stigg_api_client_v2-0.505.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-25 15:34:04.402140 stigg_api_client_v2-0.505.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-25 15:34:11.094448 stigg_api_client_v2-0.505.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-25 15:34:09.846391 stigg_api_client_v2-0.505.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-25 15:34:09.870392 stigg_api_client_v2-0.505.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    67887 2023-07-25 15:34:04.690154 stigg_api_client_v2-0.505.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-25 15:34:09.902394 stigg_api_client_v2-0.505.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24198 2023-07-25 15:34:06.738248 stigg_api_client_v2-0.505.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-25 15:34:09.854391 stigg_api_client_v2-0.505.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-25 15:34:09.862392 stigg_api_client_v2-0.505.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-25 15:34:11.094448 stigg_api_client_v2-0.505.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    56347 2023-07-25 15:34:11.090448 stigg_api_client_v2-0.505.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-25 15:34:09.934395 stigg_api_client_v2-0.505.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-25 15:34:09.946396 stigg_api_client_v2-0.505.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-25 15:34:09.926395 stigg_api_client_v2-0.505.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-25 15:34:09.998398 stigg_api_client_v2-0.505.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-25 15:34:09.966397 stigg_api_client_v2-0.505.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-25 15:34:09.962396 stigg_api_client_v2-0.505.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-25 15:34:10.014399 stigg_api_client_v2-0.505.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-25 15:34:09.954396 stigg_api_client_v2-0.505.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-25 15:34:09.978397 stigg_api_client_v2-0.505.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-25 15:34:09.990398 stigg_api_client_v2-0.505.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-25 15:34:09.798389 stigg_api_client_v2-0.505.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-25 15:34:09.790388 stigg_api_client_v2-0.505.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-25 15:34:09.830390 stigg_api_client_v2-0.505.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   126973 2023-07-25 15:34:09.766387 stigg_api_client_v2-0.505.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-25 15:34:09.910394 stigg_api_client_v2-0.505.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-25 15:34:09.782388 stigg_api_client_v2-0.505.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-25 15:34:09.826390 stigg_api_client_v2-0.505.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-25 15:34:09.894393 stigg_api_client_v2-0.505.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-25 15:34:09.886393 stigg_api_client_v2-0.505.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-25 15:34:09.882393 stigg_api_client_v2-0.505.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-25 15:34:11.098449 stigg_api_client_v2-0.505.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-25 15:34:09.810389 stigg_api_client_v2-0.505.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-25 15:34:09.838391 stigg_api_client_v2-0.505.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-25 15:34:10.018399 stigg_api_client_v2-0.505.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.505.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-25 16:15:51.201603 stigg_api_client_v2-0.505.1/README.md
+-rw-r--r--   0        0        0      432 2023-07-25 16:16:45.537880 stigg_api_client_v2-0.505.1/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-25 16:15:51.201603 stigg_api_client_v2-0.505.1/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-25 16:15:51.201603 stigg_api_client_v2-0.505.1/stigg/client.py
+-rw-r--r--   0        0        0    40274 2023-07-25 16:16:43.621872 stigg_api_client_v2-0.505.1/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-25 16:16:42.009865 stigg_api_client_v2-0.505.1/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-07-25 16:16:43.065869 stigg_api_client_v2-0.505.1/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    68314 2023-07-25 16:16:43.321870 stigg_api_client_v2-0.505.1/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-25 16:16:37.149844 stigg_api_client_v2-0.505.1/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-25 16:16:43.065869 stigg_api_client_v2-0.505.1/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-25 16:16:41.941864 stigg_api_client_v2-0.505.1/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-25 16:16:41.965865 stigg_api_client_v2-0.505.1/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    67887 2023-07-25 16:16:37.393845 stigg_api_client_v2-0.505.1/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-25 16:16:41.993865 stigg_api_client_v2-0.505.1/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24198 2023-07-25 16:16:39.161853 stigg_api_client_v2-0.505.1/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-25 16:16:41.949864 stigg_api_client_v2-0.505.1/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-25 16:16:41.957865 stigg_api_client_v2-0.505.1/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-25 16:16:43.065869 stigg_api_client_v2-0.505.1/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    56347 2023-07-25 16:16:43.061869 stigg_api_client_v2-0.505.1/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-25 16:16:42.029865 stigg_api_client_v2-0.505.1/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-25 16:16:42.037865 stigg_api_client_v2-0.505.1/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-25 16:16:42.017865 stigg_api_client_v2-0.505.1/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-25 16:16:42.089865 stigg_api_client_v2-0.505.1/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-25 16:16:42.057865 stigg_api_client_v2-0.505.1/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-25 16:16:42.053865 stigg_api_client_v2-0.505.1/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-25 16:16:42.101865 stigg_api_client_v2-0.505.1/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-25 16:16:42.045865 stigg_api_client_v2-0.505.1/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-25 16:16:42.069865 stigg_api_client_v2-0.505.1/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-25 16:16:42.081865 stigg_api_client_v2-0.505.1/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-25 16:16:41.897864 stigg_api_client_v2-0.505.1/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-25 16:16:41.889864 stigg_api_client_v2-0.505.1/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-25 16:16:41.925864 stigg_api_client_v2-0.505.1/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   127090 2023-07-25 16:16:41.869864 stigg_api_client_v2-0.505.1/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-25 16:16:42.001865 stigg_api_client_v2-0.505.1/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-25 16:16:41.885864 stigg_api_client_v2-0.505.1/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-25 16:16:41.921864 stigg_api_client_v2-0.505.1/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-25 16:16:41.985865 stigg_api_client_v2-0.505.1/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-25 16:16:41.981865 stigg_api_client_v2-0.505.1/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-25 16:16:41.973865 stigg_api_client_v2-0.505.1/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-25 16:16:43.069869 stigg_api_client_v2-0.505.1/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-25 16:16:41.909864 stigg_api_client_v2-0.505.1/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-25 16:16:41.933864 stigg_api_client_v2-0.505.1/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-25 16:16:42.109865 stigg_api_client_v2-0.505.1/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.505.1/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.505.0/README.md` & `stigg_api_client_v2-0.505.1/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.505.0/stigg/client.py` & `stigg_api_client_v2-0.505.1/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.505.1/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 
 from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.505.1/stigg/generated/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.505.1/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.505.1/stigg/generated/base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.505.1/stigg/generated/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.505.1/stigg/generated/cancel_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/client.py` & `stigg_api_client_v2-0.505.1/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.505.1/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerIsArchived = "CustomerIsArchived"
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.505.1/stigg/generated/estimate_subscription_update.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
 
 
-class EstimateSubscription(BaseModel):
-    estimate_subscription: "EstimateSubscriptionEstimateSubscription" = Field(
-        alias="estimateSubscription"
+class EstimateSubscriptionUpdate(BaseModel):
+    estimate_subscription_update: "EstimateSubscriptionUpdateEstimateSubscriptionUpdate" = Field(
+        alias="estimateSubscriptionUpdate"
     )
 
 
-class EstimateSubscriptionEstimateSubscription(SubscriptionPreviewFragment):
+class EstimateSubscriptionUpdateEstimateSubscriptionUpdate(SubscriptionPreviewFragment):
     pass
 
 
-EstimateSubscription.update_forward_refs()
-EstimateSubscriptionEstimateSubscription.update_forward_refs()
+EstimateSubscriptionUpdate.update_forward_refs()
+EstimateSubscriptionUpdateEstimateSubscriptionUpdate.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.505.1/stigg/generated/estimate_subscription.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
 
 
-class EstimateSubscriptionUpdate(BaseModel):
-    estimate_subscription_update: "EstimateSubscriptionUpdateEstimateSubscriptionUpdate" = Field(
-        alias="estimateSubscriptionUpdate"
+class EstimateSubscription(BaseModel):
+    estimate_subscription: "EstimateSubscriptionEstimateSubscription" = Field(
+        alias="estimateSubscription"
     )
 
 
-class EstimateSubscriptionUpdateEstimateSubscriptionUpdate(SubscriptionPreviewFragment):
+class EstimateSubscriptionEstimateSubscription(SubscriptionPreviewFragment):
     pass
 
 
-EstimateSubscriptionUpdate.update_forward_refs()
-EstimateSubscriptionUpdateEstimateSubscriptionUpdate.update_forward_refs()
+EstimateSubscription.update_forward_refs()
+EstimateSubscriptionEstimateSubscription.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.505.1/stigg/generated/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.505.1/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -333,23 +333,14 @@
     pass
 
 
 class CustomerResourceFragment(BaseModel):
     resource_id: str = Field(alias="resourceId")
 
 
-class CustomerPortalPromotionalEntitlement(BaseModel):
-    display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
-
-
 class CustomerPortalSubscriptionAddon(BaseModel):
     addon_id: str = Field(alias="addonId")
     description: Optional[str]
     display_name: str = Field(alias="displayName")
     quantity: int
 
 
@@ -506,14 +497,23 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
+class CustomerPortalPromotionalEntitlement(BaseModel):
+    display_name: str = Field(alias="displayName")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
+
+
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -548,29 +548,14 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
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
@@ -614,14 +599,29 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
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
 
@@ -1378,15 +1378,14 @@
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
 CustomerResourceFragment.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionPriceFragment.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
@@ -1400,29 +1399,30 @@
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
-TotalPriceFragment.update_forward_refs()
-TotalPriceFragmentSubTotal.update_forward_refs()
-TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionScheduledUpdateData.update_forward_refs()
 SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
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
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.505.1/stigg/generated/get_active_subscriptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.505.1/stigg/generated/get_coupons.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.505.1/stigg/generated/get_customer_by_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.505.1/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.505.1/stigg/generated/get_mock_paywall.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.505.1/stigg/generated/get_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.505.1/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.505.1/stigg/generated/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -2612,14 +2612,17 @@
         alias="weeklyResetPeriodConfiguration"
     )
 
 
 class UpdateSubscriptionInput(BaseModel):
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     addons: Optional[List["SubscriptionAddonInput"]]
+    await_payment_confirmation: Optional[bool] = Field(
+        alias="awaitPaymentConfirmation", default=True
+    )
     billable_features: Optional[List["BillableFeatureInput"]] = Field(
         alias="billableFeatures"
     )
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     environment_id: Optional[str] = Field(alias="environmentId")
     promotion_code: Optional[str] = Field(alias="promotionCode")
     ref_id: Optional[str] = Field(alias="refId")
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.505.1/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.505.1/stigg/generated/provision_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.505.1/stigg/generated/provision_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.505.1/stigg/generated/report_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.505.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.505.1/stigg/generated/update_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 15:34
+# Generated by ariadne-codegen on 2023-07-25 16:16
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.505.0/PKG-INFO` & `stigg_api_client_v2-0.505.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.505.0
+Version: 0.505.1
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

