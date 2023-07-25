# Comparing `tmp/stigg_api_client_v2-0.504.0.tar.gz` & `tmp/stigg_api_client_v2-0.505.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.504.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.505.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.504.0.tar` & `stigg_api_client_v2-0.505.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1644 2023-07-25 10:54:06.737942 stigg_api_client_v2-0.504.0/README.md
--rw-r--r--   0        0        0      432 2023-07-25 10:55:05.954953 stigg_api_client_v2-0.504.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-25 10:54:06.737942 stigg_api_client_v2-0.504.0/stigg/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-25 10:54:06.737942 stigg_api_client_v2-0.504.0/stigg/client.py
--rw-r--r--   0        0        0    40274 2023-07-25 10:55:04.338983 stigg_api_client_v2-0.504.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0      460 2023-07-25 10:55:02.986975 stigg_api_client_v2-0.504.0/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0     7303 2023-07-25 10:55:03.854990 stigg_api_client_v2-0.504.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    68314 2023-07-25 10:55:04.074989 stigg_api_client_v2-0.504.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-25 10:54:58.898902 stigg_api_client_v2-0.504.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-25 10:55:03.854990 stigg_api_client_v2-0.504.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-25 10:55:02.934974 stigg_api_client_v2-0.504.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-25 10:55:02.950974 stigg_api_client_v2-0.504.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    67887 2023-07-25 10:54:59.114906 stigg_api_client_v2-0.504.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-25 10:55:02.974974 stigg_api_client_v2-0.504.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24160 2023-07-25 10:55:00.666933 stigg_api_client_v2-0.504.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-25 10:55:02.942974 stigg_api_client_v2-0.504.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-25 10:55:02.946974 stigg_api_client_v2-0.504.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-25 10:55:03.854990 stigg_api_client_v2-0.504.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    56347 2023-07-25 10:55:03.854990 stigg_api_client_v2-0.504.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-25 10:55:03.002975 stigg_api_client_v2-0.504.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-25 10:55:03.010975 stigg_api_client_v2-0.504.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-25 10:55:02.994975 stigg_api_client_v2-0.504.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-25 10:55:03.046975 stigg_api_client_v2-0.504.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-25 10:55:03.026975 stigg_api_client_v2-0.504.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-25 10:55:03.018975 stigg_api_client_v2-0.504.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-25 10:55:03.054976 stigg_api_client_v2-0.504.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-25 10:55:03.014975 stigg_api_client_v2-0.504.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-25 10:55:03.030975 stigg_api_client_v2-0.504.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-25 10:55:03.042976 stigg_api_client_v2-0.504.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-25 10:55:02.902973 stigg_api_client_v2-0.504.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-25 10:55:02.894973 stigg_api_client_v2-0.504.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-25 10:55:02.922973 stigg_api_client_v2-0.504.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   126973 2023-07-25 10:55:02.878973 stigg_api_client_v2-0.504.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-25 10:55:02.982974 stigg_api_client_v2-0.504.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-25 10:55:02.890973 stigg_api_client_v2-0.504.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-25 10:55:02.918973 stigg_api_client_v2-0.504.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-25 10:55:02.970974 stigg_api_client_v2-0.504.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-25 10:55:02.966974 stigg_api_client_v2-0.504.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-25 10:55:02.958974 stigg_api_client_v2-0.504.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-25 10:55:03.862990 stigg_api_client_v2-0.504.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-25 10:55:02.906973 stigg_api_client_v2-0.504.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-25 10:55:02.926973 stigg_api_client_v2-0.504.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-25 10:55:03.062976 stigg_api_client_v2-0.504.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.504.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-25 15:32:57.775076 stigg_api_client_v2-0.505.0/README.md
+-rw-r--r--   0        0        0      432 2023-07-25 15:34:13.830574 stigg_api_client_v2-0.505.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-25 15:32:57.779076 stigg_api_client_v2-0.505.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-25 15:32:57.779076 stigg_api_client_v2-0.505.0/stigg/client.py
+-rw-r--r--   0        0        0    40274 2023-07-25 15:34:11.722478 stigg_api_client_v2-0.505.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-25 15:34:09.918394 stigg_api_client_v2-0.505.0/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-07-25 15:34:11.094448 stigg_api_client_v2-0.505.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    68314 2023-07-25 15:34:11.378462 stigg_api_client_v2-0.505.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-25 15:34:04.402140 stigg_api_client_v2-0.505.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-25 15:34:11.094448 stigg_api_client_v2-0.505.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-25 15:34:09.846391 stigg_api_client_v2-0.505.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-25 15:34:09.870392 stigg_api_client_v2-0.505.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    67887 2023-07-25 15:34:04.690154 stigg_api_client_v2-0.505.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-25 15:34:09.902394 stigg_api_client_v2-0.505.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24198 2023-07-25 15:34:06.738248 stigg_api_client_v2-0.505.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-25 15:34:09.854391 stigg_api_client_v2-0.505.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-25 15:34:09.862392 stigg_api_client_v2-0.505.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-25 15:34:11.094448 stigg_api_client_v2-0.505.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    56347 2023-07-25 15:34:11.090448 stigg_api_client_v2-0.505.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-25 15:34:09.934395 stigg_api_client_v2-0.505.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-25 15:34:09.946396 stigg_api_client_v2-0.505.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-25 15:34:09.926395 stigg_api_client_v2-0.505.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-25 15:34:09.998398 stigg_api_client_v2-0.505.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-25 15:34:09.966397 stigg_api_client_v2-0.505.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-25 15:34:09.962396 stigg_api_client_v2-0.505.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-25 15:34:10.014399 stigg_api_client_v2-0.505.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-25 15:34:09.954396 stigg_api_client_v2-0.505.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-25 15:34:09.978397 stigg_api_client_v2-0.505.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-25 15:34:09.990398 stigg_api_client_v2-0.505.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-25 15:34:09.798389 stigg_api_client_v2-0.505.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-25 15:34:09.790388 stigg_api_client_v2-0.505.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-25 15:34:09.830390 stigg_api_client_v2-0.505.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   126973 2023-07-25 15:34:09.766387 stigg_api_client_v2-0.505.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-25 15:34:09.910394 stigg_api_client_v2-0.505.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-25 15:34:09.782388 stigg_api_client_v2-0.505.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-25 15:34:09.826390 stigg_api_client_v2-0.505.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-25 15:34:09.894393 stigg_api_client_v2-0.505.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-25 15:34:09.886393 stigg_api_client_v2-0.505.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-25 15:34:09.882393 stigg_api_client_v2-0.505.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-25 15:34:11.098449 stigg_api_client_v2-0.505.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-25 15:34:09.810389 stigg_api_client_v2-0.505.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-25 15:34:09.838391 stigg_api_client_v2-0.505.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-25 15:34:10.018399 stigg_api_client_v2-0.505.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.505.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.504.0/README.md` & `stigg_api_client_v2-0.505.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.504.0/stigg/client.py` & `stigg_api_client_v2-0.505.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.505.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 
 from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.505.0/stigg/generated/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.505.0/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.505.0/stigg/generated/base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:54
+# Generated by ariadne-codegen on 2023-07-25 15:34
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.505.0/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.505.0/stigg/generated/cancel_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/client.py` & `stigg_api_client_v2-0.505.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:54
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.505.0/stigg/generated/create_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.505.0/stigg/generated/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerIsArchived = "CustomerIsArchived"
@@ -780,14 +780,15 @@
     usageLimit = "usageLimit"
 
 
 class SubscriptionScheduleStatus(str, Enum):
     Canceled = "Canceled"
     Done = "Done"
     Failed = "Failed"
+    PendingPayment = "PendingPayment"
     Scheduled = "Scheduled"
 
 
 class SubscriptionScheduleType(str, Enum):
     BillingPeriod = "BillingPeriod"
     Downgrade = "Downgrade"
     MigrateToLatest = "MigrateToLatest"
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.505.0/stigg/generated/estimate_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.505.0/stigg/generated/estimate_subscription_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.505.0/stigg/generated/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.505.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -32,14 +32,36 @@
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
     experimentGroupType,
 )
 
 
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
 class PriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -56,36 +78,14 @@
     ref_id: str = Field(alias="refId")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
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
 class AddonFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     billing_id: Optional[str] = Field(alias="billingId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -125,14 +125,25 @@
     status: SyncStatus
 
 
 class CouponFragmentCustomers(BaseModel):
     id: str
 
 
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
 class PromotionalEntitlementFragment(BaseModel):
     status: PromotionalEntitlementStatus
     usage_limit: Optional[float] = Field(alias="usageLimit")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -147,25 +158,14 @@
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     ref_id: str = Field(alias="refId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
 
 
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
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -342,14 +342,41 @@
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     usage_limit: Optional[float] = Field(alias="usageLimit")
     period: PromotionalEntitlementPeriod
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
 
 
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
+    display_name: str = Field(alias="displayName")
+    quantity: int
+
+
+class CustomerPortalSubscriptionPriceFragment(BaseModel):
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    billing_model: Optional[BillingModel] = Field(alias="billingModel")
+    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
+    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
+
+
+class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+
+
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional[
@@ -394,41 +421,14 @@
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
-    display_name: str = Field(alias="displayName")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-
-
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
-    display_name: str = Field(alias="displayName")
-    quantity: int
-
-
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing_type: PricingType = Field(alias="pricingType")
     prices: List["CustomerPortalSubscriptionFragmentPrices"]
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
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
 class SubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
@@ -599,29 +614,14 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
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
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -845,34 +845,14 @@
 class LayoutConfigurationFragment(BaseModel):
     alignment: Optional[Alignment]
     plan_width: Optional[float] = Field(alias="planWidth")
     plan_margin: Optional[float] = Field(alias="planMargin")
     plan_padding: Optional[float] = Field(alias="planPadding")
 
 
-class MockPaywallPackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
-
-
-class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
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
 class MockPaywallPriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -888,14 +868,34 @@
 class MockPaywallPriceFragmentFeature(BaseModel):
     ref_id: str = Field(alias="refId")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
 
 
+class MockPaywallPackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
+
+
+class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
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
 class MockPaywallAddonFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     billing_id: Optional[str] = Field(alias="billingId")
     entitlements: List["MockPaywallAddonFragmentEntitlements"]
@@ -1342,28 +1342,28 @@
 
 class UsageHistoryFragmentUsageMeasurements(BaseModel):
     date: Any
     value: float
     is_reset_point: Optional[bool] = Field(alias="isResetPoint")
 
 
+PackageEntitlementFragment.update_forward_refs()
+PackageEntitlementFragmentFeature.update_forward_refs()
 PriceFragment.update_forward_refs()
 PriceFragmentPrice.update_forward_refs()
 PriceFragmentFeature.update_forward_refs()
-PackageEntitlementFragment.update_forward_refs()
-PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
+SlimCustomerFragment.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
 PromotionalEntitlementFragmentFeature.update_forward_refs()
-SlimCustomerFragment.update_forward_refs()
 CustomerFragment.update_forward_refs()
 CustomerFragmentTrialedPlans.update_forward_refs()
 CustomerFragmentExperimentInfo.update_forward_refs()
 CustomerFragmentCoupon.update_forward_refs()
 CustomerFragmentEligibleForTrial.update_forward_refs()
 CustomerFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalBillingInformation.update_forward_refs()
@@ -1379,23 +1379,23 @@
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
 CustomerResourceFragment.update_forward_refs()
 CustomerPortalPromotionalEntitlement.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
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
-CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
@@ -1407,22 +1407,22 @@
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
 SubscriptionScheduledUpdateData.update_forward_refs()
 SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-TotalPriceFragment.update_forward_refs()
-TotalPriceFragmentSubTotal.update_forward_refs()
-TotalPriceFragmentTotal.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
@@ -1449,19 +1449,19 @@
 UsageUpdatedFragment.update_forward_refs()
 EntitlementUsageUpdated.update_forward_refs()
 EntitlementUsageUpdatedUsage.update_forward_refs()
 EntitlementUsageUpdatedEntitlement.update_forward_refs()
 EntitlementsUpdatedPayload.update_forward_refs()
 EntitlementsUpdatedPayloadEntitlements.update_forward_refs()
 LayoutConfigurationFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallPriceFragment.update_forward_refs()
 MockPaywallPriceFragmentPrice.update_forward_refs()
 MockPaywallPriceFragmentFeature.update_forward_refs()
+MockPaywallPackageEntitlementFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallAddonFragment.update_forward_refs()
 MockPaywallAddonFragmentEntitlements.update_forward_refs()
 MockPaywallAddonFragmentPrices.update_forward_refs()
 MockPaywallPlanFragment.update_forward_refs()
 MockPaywallPlanFragmentProduct.update_forward_refs()
 MockPaywallPlanFragmentBasePlan.update_forward_refs()
 MockPaywallPlanFragmentEntitlements.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.505.0/stigg/generated/get_active_subscriptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.505.0/stigg/generated/get_coupons.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.505.0/stigg/generated/get_customer_by_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.505.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.505.0/stigg/generated/get_mock_paywall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.505.0/stigg/generated/get_products.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.505.0/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.505.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.505.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.505.0/stigg/generated/provision_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.505.0/stigg/generated/provision_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.505.0/stigg/generated/report_usage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.504.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.505.0/stigg/generated/update_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 10:55
+# Generated by ariadne-codegen on 2023-07-25 15:34
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.504.0/PKG-INFO` & `stigg_api_client_v2-0.505.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.504.0
+Version: 0.505.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

