# Comparing `tmp/chift-0.1.0.tar.gz` & `tmp/chift-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chift-0.1.0.tar", last modified: Thu Jul 20 12:08:43 2023, max compression
+gzip compressed data, was "chift-0.1.1.tar", last modified: Tue Jul 25 14:01:14 2023, max compression
```

## Comparing `chift-0.1.0.tar` & `chift-0.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.036389 chift-0.1.0/
--rw-r--r--   0 thomas     (501) staff       (20)     1316 2023-07-20 12:08:43.036164 chift-0.1.0/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)     1157 2023-07-20 10:27:56.000000 chift-0.1.0/README.md
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.005282 chift-0.1.0/chift/
--rw-r--r--   0 thomas     (501) staff       (20)      188 2023-07-05 10:38:21.000000 chift-0.1.0/chift/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.012030 chift-0.1.0/chift/api/
--rw-r--r--   0 thomas     (501) staff       (20)        0 2023-06-23 14:17:04.000000 chift-0.1.0/chift/api/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     7230 2023-07-12 10:48:09.000000 chift-0.1.0/chift/api/client.py
--rw-r--r--   0 thomas     (501) staff       (20)      346 2023-06-23 14:18:46.000000 chift-0.1.0/chift/api/exceptions.py
--rw-r--r--   0 thomas     (501) staff       (20)     3514 2023-07-17 10:17:00.000000 chift-0.1.0/chift/api/mixins.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.012668 chift-0.1.0/chift/models/
--rw-r--r--   0 thomas     (501) staff       (20)      315 2023-06-28 06:40:31.000000 chift-0.1.0/chift/models/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.014143 chift-0.1.0/chift/models/consumers/
--rw-r--r--   0 thomas     (501) staff       (20)       31 2023-06-23 14:18:46.000000 chift-0.1.0/chift/models/consumers/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.014724 chift-0.1.0/chift/models/consumers/accounting/
--rw-r--r--   0 thomas     (501) staff       (20)     2851 2023-07-12 10:48:09.000000 chift-0.1.0/chift/models/consumers/accounting/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.015506 chift-0.1.0/chift/models/consumers/commerce/
--rw-r--r--   0 thomas     (501) staff       (20)     1520 2023-07-18 13:46:49.000000 chift-0.1.0/chift/models/consumers/commerce/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.016025 chift-0.1.0/chift/models/consumers/connection/
--rw-r--r--   0 thomas     (501) staff       (20)      465 2023-07-03 09:04:37.000000 chift-0.1.0/chift/models/consumers/connection/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)      619 2023-07-05 13:17:47.000000 chift-0.1.0/chift/models/consumers/consumer.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.016553 chift-0.1.0/chift/models/consumers/data/
--rw-r--r--   0 thomas     (501) staff       (20)      752 2023-07-11 12:35:08.000000 chift-0.1.0/chift/models/consumers/data/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.017093 chift-0.1.0/chift/models/consumers/invoicing/
--rw-r--r--   0 thomas     (501) staff       (20)     1865 2023-07-03 09:48:13.000000 chift-0.1.0/chift/models/consumers/invoicing/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.018576 chift-0.1.0/chift/models/consumers/log/
--rw-r--r--   0 thomas     (501) staff       (20)      518 2023-07-05 12:19:54.000000 chift-0.1.0/chift/models/consumers/log/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.019331 chift-0.1.0/chift/models/consumers/pos/
--rw-r--r--   0 thomas     (501) staff       (20)     2134 2023-07-12 08:16:34.000000 chift-0.1.0/chift/models/consumers/pos/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.020887 chift-0.1.0/chift/models/consumers/sync/
--rw-r--r--   0 thomas     (501) staff       (20)      404 2023-07-03 09:04:37.000000 chift-0.1.0/chift/models/consumers/sync/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.022459 chift-0.1.0/chift/models/datastores/
--rw-r--r--   0 thomas     (501) staff       (20)      425 2023-07-03 10:30:44.000000 chift-0.1.0/chift/models/datastores/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.023025 chift-0.1.0/chift/models/integrations/
--rw-r--r--   0 thomas     (501) staff       (20)      438 2023-07-03 10:30:47.000000 chift-0.1.0/chift/models/integrations/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.023544 chift-0.1.0/chift/models/syncs/
--rw-r--r--   0 thomas     (501) staff       (20)     1703 2023-07-20 09:05:25.000000 chift-0.1.0/chift/models/syncs/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.024632 chift-0.1.0/chift/models/webhooks/
--rw-r--r--   0 thomas     (501) staff       (20)      985 2023-07-03 10:34:42.000000 chift-0.1.0/chift/models/webhooks/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.026135 chift-0.1.0/chift/openapi/
--rw-r--r--   0 thomas     (501) staff       (20)        0 2023-06-23 14:17:04.000000 chift-0.1.0/chift/openapi/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     5941 2023-07-20 09:05:25.000000 chift-0.1.0/chift/openapi/models.py
--rw-r--r--   0 thomas     (501) staff       (20)   107768 2023-07-20 09:05:26.000000 chift-0.1.0/chift/openapi/openapi.py
--rw-r--r--   0 thomas     (501) staff       (20)       18 2023-07-20 12:08:19.000000 chift-0.1.0/chift/version.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.009840 chift-0.1.0/chift.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)     1316 2023-07-20 12:08:42.000000 chift-0.1.0/chift.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)     1176 2023-07-20 12:08:42.000000 chift-0.1.0/chift.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2023-07-20 12:08:42.000000 chift-0.1.0/chift.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       53 2023-07-20 12:08:42.000000 chift-0.1.0/chift.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)        6 2023-07-20 12:08:42.000000 chift-0.1.0/chift.egg-info/top_level.txt
--rw-r--r--   0 thomas     (501) staff       (20)       38 2023-07-20 12:08:43.036464 chift-0.1.0/setup.cfg
--rw-r--r--   0 thomas     (501) staff       (20)      793 2023-07-20 12:07:15.000000 chift-0.1.0/setup.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-20 12:08:43.035616 chift-0.1.0/tests/
--rw-r--r--   0 thomas     (501) staff       (20)     1919 2023-07-20 09:26:58.000000 chift-0.1.0/tests/test_accounting.py
--rw-r--r--   0 thomas     (501) staff       (20)      595 2023-07-05 13:36:56.000000 chift-0.1.0/tests/test_client.py
--rw-r--r--   0 thomas     (501) staff       (20)     1146 2023-07-20 10:01:24.000000 chift-0.1.0/tests/test_commerce.py
--rw-r--r--   0 thomas     (501) staff       (20)     1458 2023-07-20 09:31:02.000000 chift-0.1.0/tests/test_connection.py
--rw-r--r--   0 thomas     (501) staff       (20)      178 2023-07-20 09:20:49.000000 chift-0.1.0/tests/test_datastore.py
--rw-r--r--   0 thomas     (501) staff       (20)      169 2023-07-20 09:21:39.000000 chift-0.1.0/tests/test_integration.py
--rw-r--r--   0 thomas     (501) staff       (20)     4156 2023-07-20 09:29:50.000000 chift-0.1.0/tests/test_invoicing.py
--rw-r--r--   0 thomas     (501) staff       (20)      622 2023-07-20 09:31:04.000000 chift-0.1.0/tests/test_log.py
--rw-r--r--   0 thomas     (501) staff       (20)     2342 2023-07-20 09:31:07.000000 chift-0.1.0/tests/test_pos.py
--rw-r--r--   0 thomas     (501) staff       (20)     8473 2023-07-20 09:05:25.000000 chift-0.1.0/tests/test_sync.py
--rw-r--r--   0 thomas     (501) staff       (20)      329 2023-06-28 06:33:15.000000 chift-0.1.0/tests/test_webhook.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.452555 chift-0.1.1/
+-rw-r--r--   0 thomas     (501) staff       (20)     1316 2023-07-25 14:01:14.452355 chift-0.1.1/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)     1157 2023-07-20 10:27:56.000000 chift-0.1.1/README.md
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.391172 chift-0.1.1/chift/
+-rw-r--r--   0 thomas     (501) staff       (20)      188 2023-07-05 10:38:21.000000 chift-0.1.1/chift/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.395997 chift-0.1.1/chift/api/
+-rw-r--r--   0 thomas     (501) staff       (20)        0 2023-06-23 14:17:04.000000 chift-0.1.1/chift/api/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)     7230 2023-07-12 10:48:09.000000 chift-0.1.1/chift/api/client.py
+-rw-r--r--   0 thomas     (501) staff       (20)      346 2023-06-23 14:18:46.000000 chift-0.1.1/chift/api/exceptions.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3514 2023-07-17 10:17:00.000000 chift-0.1.1/chift/api/mixins.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.396564 chift-0.1.1/chift/models/
+-rw-r--r--   0 thomas     (501) staff       (20)      315 2023-06-28 06:40:31.000000 chift-0.1.1/chift/models/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.399049 chift-0.1.1/chift/models/consumers/
+-rw-r--r--   0 thomas     (501) staff       (20)       31 2023-06-23 14:18:46.000000 chift-0.1.1/chift/models/consumers/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.405809 chift-0.1.1/chift/models/consumers/accounting/
+-rw-r--r--   0 thomas     (501) staff       (20)     3208 2023-07-25 13:49:53.000000 chift-0.1.1/chift/models/consumers/accounting/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.408617 chift-0.1.1/chift/models/consumers/commerce/
+-rw-r--r--   0 thomas     (501) staff       (20)     1520 2023-07-18 13:46:49.000000 chift-0.1.1/chift/models/consumers/commerce/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.409242 chift-0.1.1/chift/models/consumers/connection/
+-rw-r--r--   0 thomas     (501) staff       (20)      465 2023-07-03 09:04:37.000000 chift-0.1.1/chift/models/consumers/connection/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)      619 2023-07-05 13:17:47.000000 chift-0.1.1/chift/models/consumers/consumer.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.409780 chift-0.1.1/chift/models/consumers/data/
+-rw-r--r--   0 thomas     (501) staff       (20)      752 2023-07-11 12:35:08.000000 chift-0.1.1/chift/models/consumers/data/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.412046 chift-0.1.1/chift/models/consumers/invoicing/
+-rw-r--r--   0 thomas     (501) staff       (20)     1865 2023-07-03 09:48:13.000000 chift-0.1.1/chift/models/consumers/invoicing/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.412656 chift-0.1.1/chift/models/consumers/log/
+-rw-r--r--   0 thomas     (501) staff       (20)      518 2023-07-05 12:19:54.000000 chift-0.1.1/chift/models/consumers/log/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.418460 chift-0.1.1/chift/models/consumers/pos/
+-rw-r--r--   0 thomas     (501) staff       (20)     2134 2023-07-12 08:16:34.000000 chift-0.1.1/chift/models/consumers/pos/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.419316 chift-0.1.1/chift/models/consumers/sync/
+-rw-r--r--   0 thomas     (501) staff       (20)      404 2023-07-03 09:04:37.000000 chift-0.1.1/chift/models/consumers/sync/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.419973 chift-0.1.1/chift/models/datastores/
+-rw-r--r--   0 thomas     (501) staff       (20)      425 2023-07-03 10:30:44.000000 chift-0.1.1/chift/models/datastores/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.421449 chift-0.1.1/chift/models/integrations/
+-rw-r--r--   0 thomas     (501) staff       (20)      438 2023-07-03 10:30:47.000000 chift-0.1.1/chift/models/integrations/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.422751 chift-0.1.1/chift/models/syncs/
+-rw-r--r--   0 thomas     (501) staff       (20)     1703 2023-07-20 09:05:25.000000 chift-0.1.1/chift/models/syncs/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.431066 chift-0.1.1/chift/models/webhooks/
+-rw-r--r--   0 thomas     (501) staff       (20)      985 2023-07-03 10:34:42.000000 chift-0.1.1/chift/models/webhooks/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.432875 chift-0.1.1/chift/openapi/
+-rw-r--r--   0 thomas     (501) staff       (20)        0 2023-06-23 14:17:04.000000 chift-0.1.1/chift/openapi/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)     5610 2023-07-25 13:49:53.000000 chift-0.1.1/chift/openapi/models.py
+-rw-r--r--   0 thomas     (501) staff       (20)   107973 2023-07-25 13:49:53.000000 chift-0.1.1/chift/openapi/openapi.py
+-rw-r--r--   0 thomas     (501) staff       (20)       19 2023-07-25 13:49:53.000000 chift-0.1.1/chift/version.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.393422 chift-0.1.1/chift.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)     1316 2023-07-25 14:01:14.000000 chift-0.1.1/chift.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)     1176 2023-07-25 14:01:14.000000 chift-0.1.1/chift.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2023-07-25 14:01:14.000000 chift-0.1.1/chift.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       53 2023-07-25 14:01:14.000000 chift-0.1.1/chift.egg-info/requires.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        6 2023-07-25 14:01:14.000000 chift-0.1.1/chift.egg-info/top_level.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       38 2023-07-25 14:01:14.452606 chift-0.1.1/setup.cfg
+-rw-r--r--   0 thomas     (501) staff       (20)      793 2023-07-20 12:07:15.000000 chift-0.1.1/setup.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-07-25 14:01:14.451496 chift-0.1.1/tests/
+-rw-r--r--   0 thomas     (501) staff       (20)     2266 2023-07-25 13:49:53.000000 chift-0.1.1/tests/test_accounting.py
+-rw-r--r--   0 thomas     (501) staff       (20)      595 2023-07-05 13:36:56.000000 chift-0.1.1/tests/test_client.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1146 2023-07-20 10:01:24.000000 chift-0.1.1/tests/test_commerce.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1458 2023-07-20 09:31:02.000000 chift-0.1.1/tests/test_connection.py
+-rw-r--r--   0 thomas     (501) staff       (20)      178 2023-07-20 09:20:49.000000 chift-0.1.1/tests/test_datastore.py
+-rw-r--r--   0 thomas     (501) staff       (20)      169 2023-07-20 09:21:39.000000 chift-0.1.1/tests/test_integration.py
+-rw-r--r--   0 thomas     (501) staff       (20)     4156 2023-07-20 09:29:50.000000 chift-0.1.1/tests/test_invoicing.py
+-rw-r--r--   0 thomas     (501) staff       (20)      622 2023-07-20 09:31:04.000000 chift-0.1.1/tests/test_log.py
+-rw-r--r--   0 thomas     (501) staff       (20)     2342 2023-07-20 09:31:07.000000 chift-0.1.1/tests/test_pos.py
+-rw-r--r--   0 thomas     (501) staff       (20)     8473 2023-07-25 13:44:46.000000 chift-0.1.1/tests/test_sync.py
+-rw-r--r--   0 thomas     (501) staff       (20)      329 2023-06-28 06:33:15.000000 chift-0.1.1/tests/test_webhook.py
```

### Comparing `chift-0.1.0/PKG-INFO` & `chift-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chift
-Version: 0.1.0
+Version: 0.1.1
 Summary: Chift API client
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Chift Python Library
```

### Comparing `chift-0.1.0/README.md` & `chift-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/chift/api/client.py` & `chift-0.1.1/chift/api/client.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/chift/api/mixins.py` & `chift-0.1.1/chift/api/mixins.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/chift/models/consumers/accounting/__init__.py` & `chift-0.1.1/chift/models/consumers/accounting/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 from chift.openapi.models import Account as AccountModel
 from chift.openapi.models import AnalyticPlan as AnalyticPlanModel
 from chift.openapi.models import Client as ClientModel
 from chift.openapi.models import InvoiceAccounting as InvoiceAccountingModel
 from chift.openapi.models import MiscellaneousOperation as MiscellaneousOperationModel
 from chift.openapi.models import Supplier as SupplierModel
 from chift.openapi.models import TaxAccounting as TaxAccountingModel
+from chift.openapi.models import JournalEntry as JournalEntryModel
 
 
 class AccountingRouter:
     def __init__(self, consumer_id, connection_id):
         self.AnalyticPlan = AnalyticPlan(consumer_id, connection_id)
         self.Tax = Tax(consumer_id, connection_id)
         self.Account = Account(consumer_id, connection_id)
         self.MiscellaneousOperation = MiscellaneousOperation(consumer_id, connection_id)
         self.Client = Client(consumer_id, connection_id)
         self.Supplier = Supplier(consumer_id, connection_id)
         self.Invoice = Invoice(consumer_id, connection_id)
+        self.JournalEntry = JournalEntry(consumer_id, connection_id)
 
 
 class AnalyticPlan(PaginationMixin[AnalyticPlanModel]):
     chift_vertical: ClassVar = "accounting"
     chift_model: ClassVar = "analytic-plans"
     model = AnalyticPlanModel
 
@@ -81,7 +83,16 @@
     chift_vertical: ClassVar = "accounting"
     chift_model: ClassVar = "invoices"
     model = InvoiceAccountingModel
 
     def all(self, invoice_type, limit=None, client=None):
         self.extra_path = f"type/{invoice_type}"
         return super().all(limit=limit, client=client)
+
+
+class JournalEntry(
+    PaginationMixin[JournalEntryModel],
+    CreateMixin[JournalEntryModel],
+):
+    chift_vertical: ClassVar = "accounting"
+    chift_model: ClassVar = "journal/entries"
+    model = JournalEntryModel
```

### Comparing `chift-0.1.0/chift/models/consumers/commerce/__init__.py` & `chift-0.1.1/chift/models/consumers/commerce/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/chift/models/consumers/consumer.py` & `chift-0.1.1/chift/models/consumers/consumer.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/chift/models/consumers/data/__init__.py` & `chift-0.1.1/chift/models/consumers/data/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/chift/models/consumers/invoicing/__init__.py` & `chift-0.1.1/chift/models/consumers/invoicing/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/chift/models/consumers/log/__init__.py` & `chift-0.1.1/chift/models/consumers/log/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/chift/models/consumers/pos/__init__.py` & `chift-0.1.1/chift/models/consumers/pos/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/chift/models/syncs/__init__.py` & `chift-0.1.1/chift/models/syncs/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/chift/models/webhooks/__init__.py` & `chift-0.1.1/chift/models/webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/chift/openapi/models.py` & `chift-0.1.1/chift/openapi/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 from enum import Enum
-from typing import List, Optional, Union
+from typing import List, Optional
 
 from pydantic import BaseModel, Extra
 
 from .openapi import (
     AccountItem,
     AnalyticAccountItemOut,
     BackboneBackboneApiAppRoutersAccountingVatCode,
@@ -35,14 +35,15 @@
     ReadFlowItem,
     SalesItem,
     SupplierItemOut,
     SyncConsumerItem,
     SyncItem,
     WebhookInstanceGetItem,
     WebhookItem,
+    JournalEntryMultiAnalyticPlan,
 )
 
 # UNPUBLISHED MODELS
 
 
 class DatastoreColumn(BaseModel):
     name: str
@@ -93,44 +94,26 @@
     id: str
 
 
 class FlowTriggerTimer(BaseModel):
     cronschedule: str = "*/5 * * * *"
 
 
-class FlowExecution(BaseModel):
-    type: ExecutionType
-    data: Union[Optional[FlowExecutionChain], Optional[FlowExecutionCode]]
-
-
 class FlowTrigger(BaseModel):
     type: TriggerType
     data: Optional[FlowTriggerTimer]
 
 
 class FlowConfig(BaseModel):
     definitionFields: Optional[List[dict]]
     doorkeyFields: Optional[List[dict]]
     customFields: Optional[List[dict]]
     datastores: Optional[List[Datastore]] = []
 
 
-class FlowItem(BaseModel):
-    name: str
-    description: Optional[str]
-    trigger: Optional[FlowTrigger] = None
-    execution: Optional[FlowExecution] = None
-    config: Optional[FlowConfig] = FlowConfig()
-    values: Optional[dict] = None
-
-
-class ReadFlowItem(FlowItem):
-    id: str
-
-
 # consumers
 
 
 class Consumer(ConsumerItem, extra=Extra.allow):
     connectionid: str = None
 
     @property
@@ -292,14 +275,18 @@
     pass
 
 
 class InvoiceAccounting(InvoiceItemOutMonoAnalyticPlan):
     pass
 
 
+class JournalEntry(JournalEntryMultiAnalyticPlan):
+    pass
+
+
 # log
 class Log(ConsumerLog):
     pass
 
 
 # pos
 class Customer(POSCustomerItem):
```

### Comparing `chift-0.1.0/chift/openapi/openapi.py` & `chift-0.1.1/chift/openapi/openapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-07-18T12:14:57+00:00
+#   timestamp: 2023-07-25T13:24:49+00:00
 
 from __future__ import annotations
 
 from datetime import date, datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
@@ -2202,24 +2202,31 @@
     variant_images: Optional[List[ImageItem]] = Field(
         [],
         description="List of images that are specific to the variant of the product.",
         title="Variant Images",
     )
 
 
+class ReadFlowConsumerItem(BaseModel):
+    name: str = Field(..., title="Name")
+    description: Optional[str] = Field(None, title="Description")
+    id: str = Field(..., title="Id")
+    config: FlowConfig
+    values: Dict[str, Any] = Field(..., title="Values")
+
+
 class ReadFlowItem(BaseModel):
     name: str = Field(..., title="Name")
     description: Optional[str] = Field(None, title="Description")
-    trigger: Optional[FlowTrigger] = None
+    id: str = Field(..., title="Id")
     execution: Optional[FlowExecution] = None
     config: Optional[FlowConfig] = Field(
         default_factory=lambda: FlowConfig.parse_obj({"datastores": []}), title="Config"
     )
-    values: Optional[Dict[str, Any]] = Field(None, title="Values")
-    id: str = Field(..., title="Id")
+    trigger: Optional[FlowTrigger] = None
 
 
 class SalesItem(BaseModel):
     total: float = Field(..., title="Total")
     tax_amount: float = Field(..., title="Tax Amount")
     taxes: Optional[List[TotalTaxItem]] = Field(None, title="Taxes")
 
@@ -2401,15 +2408,15 @@
         title="Link Createdon",
     )
     link_mappings: Optional[List[SyncMappingItem]] = Field(
         None,
         description="Values of the mappings requested for the sync for the specific consumer",
         title="Link Mappings",
     )
-    enabled_flows: Optional[List[ReadFlowItem]] = Field(
+    enabled_flows: Optional[List[ReadFlowConsumerItem]] = Field(
         None,
         description="List of flows that the consumer has enabled",
         title="Enabled Flows",
     )
 
 
 class SyncItem(BaseModel):
```

### Comparing `chift-0.1.0/chift.egg-info/PKG-INFO` & `chift-0.1.1/chift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chift
-Version: 0.1.0
+Version: 0.1.1
 Summary: Chift API client
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Chift Python Library
```

### Comparing `chift-0.1.0/chift.egg-info/SOURCES.txt` & `chift-0.1.1/chift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/setup.py` & `chift-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/tests/test_accounting.py` & `chift-0.1.1/tests/test_accounting.py`

 * *Files 20% similar despite different names*

```diff
@@ -82,7 +82,23 @@
 
     assert invoices
 
     for invoice in invoices:
         expected_invoice = consumer.accounting.Invoice.get(invoice.id)
 
         assert invoice == expected_invoice
+
+
+def test_journal_entries(odoo_consumer: Consumer):
+    consumer = odoo_consumer
+
+    entries = consumer.accounting.JournalEntry.all(
+        {
+            "unposted_allowed": "false",
+            "date_from": "2023-03-01",
+            "date_to": "2023-06-01",
+            "journal_id": "7",
+        },
+        limit=2,
+    )
+
+    assert entries
```

### Comparing `chift-0.1.0/tests/test_client.py` & `chift-0.1.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/tests/test_commerce.py` & `chift-0.1.1/tests/test_commerce.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/tests/test_connection.py` & `chift-0.1.1/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/tests/test_invoicing.py` & `chift-0.1.1/tests/test_invoicing.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/tests/test_log.py` & `chift-0.1.1/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/tests/test_pos.py` & `chift-0.1.1/tests/test_pos.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.0/tests/test_sync.py` & `chift-0.1.1/tests/test_sync.py`

 * *Files identical despite different names*

