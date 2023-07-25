# Comparing `tmp/marketplace_sdk-0.4.0.tar.gz` & `tmp/marketplace_sdk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marketplace_sdk-0.4.0.tar", last modified: Tue Jun 27 09:58:40 2023, max compression
+gzip compressed data, was "marketplace_sdk-0.5.0.tar", last modified: Tue Jul 25 14:14:07 2023, max compression
```

## Comparing `marketplace_sdk-0.4.0.tar` & `marketplace_sdk-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:40.840193 marketplace_sdk-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-27 09:58:40.840193 marketplace_sdk-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:40.836193 marketplace_sdk-0.4.0/logos/
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/logos/MARVEL.png
--rw-r--r--   0 runner    (1001) docker     (123)    27591 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/logos/MarketPlace.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:40.836193 marketplace_sdk-0.4.0/marketplace/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:40.836193 marketplace_sdk-0.4.0/marketplace/app/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/app/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:40.840193 marketplace_sdk-0.4.0/marketplace/app/v0/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/app/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/app/v0/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/app/v0/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/app/v0/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/app/v0/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:40.840193 marketplace_sdk-0.4.0/marketplace/message_broker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/message_broker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/message_broker/rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/message_broker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/marketplace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:40.840193 marketplace_sdk-0.4.0/marketplace_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-27 09:58:40.000000 marketplace_sdk-0.4.0/marketplace_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-27 09:58:40.000000 marketplace_sdk-0.4.0/marketplace_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:58:40.000000 marketplace_sdk-0.4.0/marketplace_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-27 09:58:40.000000 marketplace_sdk-0.4.0/marketplace_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 09:58:40.000000 marketplace_sdk-0.4.0/marketplace_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-27 09:58:40.840193 marketplace_sdk-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 09:58:30.000000 marketplace_sdk-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:14:07.104219 marketplace_sdk-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/.env_template
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-25 14:14:07.104219 marketplace_sdk-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:14:07.100219 marketplace_sdk-0.5.0/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/logos/MARVEL.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27591 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/logos/MarketPlace.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:14:07.100219 marketplace_sdk-0.5.0/marketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:14:07.100219 marketplace_sdk-0.5.0/marketplace/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/app/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:14:07.100219 marketplace_sdk-0.5.0/marketplace/app/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/app/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/app/v0/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/app/v0/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/app/v0/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/app/v0/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:14:07.100219 marketplace_sdk-0.5.0/marketplace/datasink_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/datasink_client/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/datasink_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/datasink_client/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18199 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/datasink_client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/datasink_client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:14:07.104219 marketplace_sdk-0.5.0/marketplace/message_broker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/message_broker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/message_broker/rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/message_broker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/marketplace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:14:07.104219 marketplace_sdk-0.5.0/marketplace_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-25 14:14:07.000000 marketplace_sdk-0.5.0/marketplace_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-25 14:14:07.000000 marketplace_sdk-0.5.0/marketplace_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:14:07.000000 marketplace_sdk-0.5.0/marketplace_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-25 14:14:07.000000 marketplace_sdk-0.5.0/marketplace_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-25 14:14:07.000000 marketplace_sdk-0.5.0/marketplace_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 14:14:07.000000 marketplace_sdk-0.5.0/marketplace_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-25 14:14:07.104219 marketplace_sdk-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-25 14:13:44.000000 marketplace_sdk-0.5.0/setup.py
```

### Comparing `marketplace_sdk-0.4.0/LICENSE` & `marketplace_sdk-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.4.0/PKG-INFO` & `marketplace_sdk-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketplace_sdk
-Version: 0.4.0
+Version: 0.5.0
 Summary: Software Development Toolkit to communicate with the Materials MarketPlace platform.
 Home-page: https://github.com/materials-marketplace/python-sdk
 Author: Carl Simon Adorf, Pablo de Andres, Pranjali Singh and the AiiDAlab team
 Author-email: simon.adorf@epfl.ch, pablo.de.andres@iwm.fraunhofer.de, pranjali.singh@iwm.fraunhofer.de
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `marketplace_sdk-0.4.0/README.md` & `marketplace_sdk-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.4.0/logos/MARVEL.png` & `marketplace_sdk-0.5.0/logos/MARVEL.png`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.4.0/logos/MarketPlace.png` & `marketplace_sdk-0.5.0/logos/MarketPlace.png`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.4.0/marketplace/app/__init__.py` & `marketplace_sdk-0.5.0/marketplace/app/__init__.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.4.0/marketplace/app/utils.py` & `marketplace_sdk-0.5.0/marketplace/app/utils.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.4.0/marketplace/app/v0/base.py` & `marketplace_sdk-0.5.0/marketplace/app/v0/base.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.4.0/marketplace/app/v0/transformation.py` & `marketplace_sdk-0.5.0/marketplace/app/v0/transformation.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.4.0/marketplace/client.py` & `marketplace_sdk-0.5.0/marketplace/client.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.4.0/marketplace/message_broker/rpc_server.py` & `marketplace_sdk-0.5.0/marketplace/message_broker/rpc_server.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.4.0/marketplace_sdk.egg-info/PKG-INFO` & `marketplace_sdk-0.5.0/marketplace_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketplace-sdk
-Version: 0.4.0
+Version: 0.5.0
 Summary: Software Development Toolkit to communicate with the Materials MarketPlace platform.
 Home-page: https://github.com/materials-marketplace/python-sdk
 Author: Carl Simon Adorf, Pablo de Andres, Pranjali Singh and the AiiDAlab team
 Author-email: simon.adorf@epfl.ch, pablo.de.andres@iwm.fraunhofer.de, pranjali.singh@iwm.fraunhofer.de
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `marketplace_sdk-0.4.0/marketplace_sdk.egg-info/SOURCES.txt` & `marketplace_sdk-0.5.0/marketplace_sdk.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.env_template
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 logos/MARVEL.png
 logos/MarketPlace.png
@@ -11,15 +12,21 @@
 marketplace/app/__init__.py
 marketplace/app/utils.py
 marketplace/app/v0/__init__.py
 marketplace/app/v0/base.py
 marketplace/app/v0/object_storage.py
 marketplace/app/v0/transformation.py
 marketplace/app/v0/utils.py
+marketplace/datasink_client/README.md
+marketplace/datasink_client/__init__.py
+marketplace/datasink_client/cli.py
+marketplace/datasink_client/session.py
+marketplace/datasink_client/utils.py
 marketplace/message_broker/__init__.py
 marketplace/message_broker/rpc_server.py
 marketplace/message_broker/utils.py
 marketplace_sdk.egg-info/PKG-INFO
 marketplace_sdk.egg-info/SOURCES.txt
 marketplace_sdk.egg-info/dependency_links.txt
+marketplace_sdk.egg-info/entry_points.txt
 marketplace_sdk.egg-info/requires.txt
 marketplace_sdk.egg-info/top_level.txt
```

