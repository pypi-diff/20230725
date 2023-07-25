# Comparing `tmp/stigg_api_client_v2-0.503.0.tar.gz` & `tmp/stigg_api_client_v2-0.504.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.503.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.504.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.503.0.tar` & `stigg_api_client_v2-0.504.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1644 2023-07-25 06:51:36.042290 stigg_api_client_v2-0.503.0/README.md
--rw-r--r--   0        0        0      432 2023-07-25 06:52:30.769405 stigg_api_client_v2-0.503.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-25 06:51:36.042290 stigg_api_client_v2-0.503.0/stigg/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-25 06:51:36.042290 stigg_api_client_v2-0.503.0/stigg/client.py
--rw-r--r--   0        0        0    40274 2023-07-25 06:52:28.713289 stigg_api_client_v2-0.503.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0      460 2023-07-25 06:52:27.197203 stigg_api_client_v2-0.503.0/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0     7303 2023-07-25 06:52:28.257263 stigg_api_client_v2-0.503.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    68230 2023-07-25 06:52:28.521278 stigg_api_client_v2-0.503.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-25 06:52:22.180918 stigg_api_client_v2-0.503.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-25 06:52:28.261263 stigg_api_client_v2-0.503.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-25 06:52:27.129199 stigg_api_client_v2-0.503.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-25 06:52:27.153200 stigg_api_client_v2-0.503.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    67803 2023-07-25 06:52:22.448933 stigg_api_client_v2-0.503.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-25 06:52:27.181202 stigg_api_client_v2-0.503.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24160 2023-07-25 06:52:24.397044 stigg_api_client_v2-0.503.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-25 06:52:27.137199 stigg_api_client_v2-0.503.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-25 06:52:27.145200 stigg_api_client_v2-0.503.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-25 06:52:28.261263 stigg_api_client_v2-0.503.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    56292 2023-07-25 06:52:28.257263 stigg_api_client_v2-0.503.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-25 06:52:27.213204 stigg_api_client_v2-0.503.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-25 06:52:27.225205 stigg_api_client_v2-0.503.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-25 06:52:27.205203 stigg_api_client_v2-0.503.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-25 06:52:27.273207 stigg_api_client_v2-0.503.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-25 06:52:27.245206 stigg_api_client_v2-0.503.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-25 06:52:27.237205 stigg_api_client_v2-0.503.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-25 06:52:27.281208 stigg_api_client_v2-0.503.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-25 06:52:27.233205 stigg_api_client_v2-0.503.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-25 06:52:27.253206 stigg_api_client_v2-0.503.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-25 06:52:27.265207 stigg_api_client_v2-0.503.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-25 06:52:27.089197 stigg_api_client_v2-0.503.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-25 06:52:27.081196 stigg_api_client_v2-0.503.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-25 06:52:27.117199 stigg_api_client_v2-0.503.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   126973 2023-07-25 06:52:27.061195 stigg_api_client_v2-0.503.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-25 06:52:27.189203 stigg_api_client_v2-0.503.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-25 06:52:27.077196 stigg_api_client_v2-0.503.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-25 06:52:27.109198 stigg_api_client_v2-0.503.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-25 06:52:27.173202 stigg_api_client_v2-0.503.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-25 06:52:27.169201 stigg_api_client_v2-0.503.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-25 06:52:27.161201 stigg_api_client_v2-0.503.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-25 06:52:28.265264 stigg_api_client_v2-0.503.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-25 06:52:27.097197 stigg_api_client_v2-0.503.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-25 06:52:27.121199 stigg_api_client_v2-0.503.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-25 06:52:27.289208 stigg_api_client_v2-0.503.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.503.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-25 10:54:06.737942 stigg_api_client_v2-0.504.0/README.md
+-rw-r--r--   0        0        0      432 2023-07-25 10:55:05.954953 stigg_api_client_v2-0.504.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-25 10:54:06.737942 stigg_api_client_v2-0.504.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-25 10:54:06.737942 stigg_api_client_v2-0.504.0/stigg/client.py
+-rw-r--r--   0        0        0    40274 2023-07-25 10:55:04.338983 stigg_api_client_v2-0.504.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-25 10:55:02.986975 stigg_api_client_v2-0.504.0/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-07-25 10:55:03.854990 stigg_api_client_v2-0.504.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    68314 2023-07-25 10:55:04.074989 stigg_api_client_v2-0.504.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-25 10:54:58.898902 stigg_api_client_v2-0.504.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-25 10:55:03.854990 stigg_api_client_v2-0.504.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-25 10:55:02.934974 stigg_api_client_v2-0.504.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-25 10:55:02.950974 stigg_api_client_v2-0.504.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    67887 2023-07-25 10:54:59.114906 stigg_api_client_v2-0.504.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-25 10:55:02.974974 stigg_api_client_v2-0.504.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24160 2023-07-25 10:55:00.666933 stigg_api_client_v2-0.504.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-25 10:55:02.942974 stigg_api_client_v2-0.504.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-25 10:55:02.946974 stigg_api_client_v2-0.504.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-25 10:55:03.854990 stigg_api_client_v2-0.504.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    56347 2023-07-25 10:55:03.854990 stigg_api_client_v2-0.504.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-25 10:55:03.002975 stigg_api_client_v2-0.504.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-25 10:55:03.010975 stigg_api_client_v2-0.504.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-25 10:55:02.994975 stigg_api_client_v2-0.504.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-25 10:55:03.046975 stigg_api_client_v2-0.504.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-25 10:55:03.026975 stigg_api_client_v2-0.504.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-25 10:55:03.018975 stigg_api_client_v2-0.504.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-25 10:55:03.054976 stigg_api_client_v2-0.504.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-25 10:55:03.014975 stigg_api_client_v2-0.504.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-25 10:55:03.030975 stigg_api_client_v2-0.504.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-25 10:55:03.042976 stigg_api_client_v2-0.504.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-25 10:55:02.902973 stigg_api_client_v2-0.504.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-25 10:55:02.894973 stigg_api_client_v2-0.504.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-25 10:55:02.922973 stigg_api_client_v2-0.504.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   126973 2023-07-25 10:55:02.878973 stigg_api_client_v2-0.504.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-25 10:55:02.982974 stigg_api_client_v2-0.504.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-25 10:55:02.890973 stigg_api_client_v2-0.504.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-25 10:55:02.918973 stigg_api_client_v2-0.504.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-25 10:55:02.970974 stigg_api_client_v2-0.504.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-25 10:55:02.966974 stigg_api_client_v2-0.504.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-25 10:55:02.958974 stigg_api_client_v2-0.504.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-25 10:55:03.862990 stigg_api_client_v2-0.504.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-25 10:55:02.906973 stigg_api_client_v2-0.504.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-25 10:55:02.926973 stigg_api_client_v2-0.504.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-25 10:55:03.062976 stigg_api_client_v2-0.504.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.504.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.503.0/README.md` & `stigg_api_client_v2-0.504.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.503.0/stigg/client.py` & `stigg_api_client_v2-0.504.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.504.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 
 from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.504.0/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.504.0/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
@@ -1029,14 +1029,15 @@
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
               description
               billingId
+              versionNumber
               additionalMetaData
               product {
                 ...ProductFragment
               }
               basePlan {
                 refId
                 displayName
@@ -1266,14 +1267,15 @@
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
               description
               billingId
+              versionNumber
               additionalMetaData
               product {
                 ...ProductFragment
               }
               basePlan {
                 refId
                 displayName
@@ -1641,14 +1643,15 @@
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
               description
               billingId
+              versionNumber
               additionalMetaData
               product {
                 ...ProductFragment
               }
               basePlan {
                 refId
                 displayName
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.504.0/stigg/generated/base_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:54
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.504.0/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.504.0/stigg/generated/cancel_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/client.py` & `stigg_api_client_v2-0.504.0/stigg/generated/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:54
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
@@ -1021,14 +1021,15 @@
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
               description
               billingId
+              versionNumber
               additionalMetaData
               product {
                 ...ProductFragment
               }
               basePlan {
                 refId
                 displayName
@@ -1258,14 +1259,15 @@
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
               description
               billingId
+              versionNumber
               additionalMetaData
               product {
                 ...ProductFragment
               }
               basePlan {
                 refId
                 displayName
@@ -1633,14 +1635,15 @@
 
             fragment PlanFragment on Plan {
               id
               refId
               displayName
               description
               billingId
+              versionNumber
               additionalMetaData
               product {
                 ...ProductFragment
               }
               basePlan {
                 refId
                 displayName
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.504.0/stigg/generated/create_subscription.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.504.0/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerIsArchived = "CustomerIsArchived"
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.504.0/stigg/generated/estimate_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.504.0/stigg/generated/estimate_subscription_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.504.0/stigg/generated/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.504.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -329,43 +329,27 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
 class CustomerPortalPromotionalEntitlement(BaseModel):
     display_name: str = Field(alias="displayName")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     usage_limit: Optional[float] = Field(alias="usageLimit")
     period: PromotionalEntitlementPeriod
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
 
 
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
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional[
@@ -410,14 +394,34 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
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
 class CustomerPortalSubscriptionAddon(BaseModel):
     addon_id: str = Field(alias="addonId")
     description: Optional[str]
     display_name: str = Field(alias="displayName")
     quantity: int
 
 
@@ -502,18 +506,14 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -548,14 +548,65 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
+class SubscriptionScheduledUpdateData(BaseModel):
+    subscription_schedule_type: SubscriptionScheduleType = Field(
+        alias="subscriptionScheduleType"
+    )
+    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
+    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
+    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
+        alias="targetPackage"
+    )
+    schedule_variables: Optional[
+        Annotated[
+            Union[
+                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
+            ],
+            Field(discriminator="typename__"),
+        ]
+    ] = Field(alias="scheduleVariables")
+
+
+class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+    BaseModel
+):
+    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
+    BaseModel
+):
+    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
+    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
+    BaseModel
+):
+    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
+    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
+    feature_id: Optional[str] = Field(alias="featureId")
+
+
 class TotalPriceFragment(BaseModel):
     sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
     total: "TotalPriceFragmentTotal"
 
 
 class TotalPriceFragmentSubTotal(BaseModel):
     amount: float
@@ -588,14 +639,15 @@
 
 class PlanFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     billing_id: Optional[str] = Field(alias="billingId")
+    version_number: int = Field(alias="versionNumber")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product: "PlanFragmentProduct"
     base_plan: Optional["PlanFragmentBasePlan"] = Field(alias="basePlan")
     entitlements: Optional[List["PlanFragmentEntitlements"]]
     inherited_entitlements: Optional[List["PlanFragmentInheritedEntitlements"]] = Field(
         alias="inheritedEntitlements"
     )
@@ -635,65 +687,14 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
-class SubscriptionScheduledUpdateData(BaseModel):
-    subscription_schedule_type: SubscriptionScheduleType = Field(
-        alias="subscriptionScheduleType"
-    )
-    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
-    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
-        alias="targetPackage"
-    )
-    schedule_variables: Optional[
-        Annotated[
-            Union[
-                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
-            ],
-            Field(discriminator="typename__"),
-        ]
-    ] = Field(alias="scheduleVariables")
-
-
-class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
-    BaseModel
-):
-    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
-    BaseModel
-):
-    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
-    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
-    BaseModel
-):
-    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
-    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
-    feature_id: Optional[str] = Field(alias="featureId")
-
-
 class SubscriptionFragment(BaseModel):
     id: str
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
     trial_end_date: Optional[Any] = Field(alias="trialEndDate")
     cancellation_date: Optional[Any] = Field(alias="cancellationDate")
     effective_end_date: Optional[Any] = Field(alias="effectiveEndDate")
@@ -1376,63 +1377,63 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
 CustomerPortalPromotionalEntitlement.update_forward_refs()
-CustomerPortalSubscriptionPriceFragment.update_forward_refs()
-CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
-CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+CustomerPortalSubscriptionPriceFragment.update_forward_refs()
+CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
+CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionAddon.update_forward_refs()
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
-CustomerResourceFragment.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
+SubscriptionScheduledUpdateData.update_forward_refs()
+SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 TotalPriceFragment.update_forward_refs()
 TotalPriceFragmentSubTotal.update_forward_refs()
 TotalPriceFragmentTotal.update_forward_refs()
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
-SubscriptionScheduledUpdateData.update_forward_refs()
-SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
 SubscriptionFragmentExperimentInfo.update_forward_refs()
 SubscriptionFragmentPrices.update_forward_refs()
 SubscriptionFragmentPricesPrice.update_forward_refs()
 SubscriptionFragmentTotalPrice.update_forward_refs()
 SubscriptionFragmentPlan.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.504.0/stigg/generated/get_active_subscriptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.504.0/stigg/generated/get_coupons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.504.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
-from typing import Optional
-
 from pydantic import Field
 
 from .base_model import BaseModel
-from .fragments import CustomerWithSubscriptionsFragment
+from .fragments import CustomerPortalFragment
 
 
-class GetCustomerById(BaseModel):
-    get_customer_by_ref_id: Optional["GetCustomerByIdGetCustomerByRefId"] = Field(
-        alias="getCustomerByRefId"
+class GetCustomerPortalByRefId(BaseModel):
+    customer_portal: "GetCustomerPortalByRefIdCustomerPortal" = Field(
+        alias="customerPortal"
     )
 
 
-class GetCustomerByIdGetCustomerByRefId(CustomerWithSubscriptionsFragment):
+class GetCustomerPortalByRefIdCustomerPortal(CustomerPortalFragment):
     pass
 
 
-GetCustomerById.update_forward_refs()
-GetCustomerByIdGetCustomerByRefId.update_forward_refs()
+GetCustomerPortalByRefId.update_forward_refs()
+GetCustomerPortalByRefIdCustomerPortal.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.504.0/stigg/generated/get_mock_paywall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.504.0/stigg/generated/get_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.504.0/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.504.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.504.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.504.0/stigg/generated/provision_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.504.0/stigg/generated/provision_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.504.0/stigg/generated/report_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.503.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.504.0/stigg/generated/update_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-25 06:52
+# Generated by ariadne-codegen on 2023-07-25 10:55
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.503.0/PKG-INFO` & `stigg_api_client_v2-0.504.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.503.0
+Version: 0.504.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

