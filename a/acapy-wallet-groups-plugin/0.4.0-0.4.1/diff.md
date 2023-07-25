# Comparing `tmp/acapy_wallet_groups_plugin-0.4.0.tar.gz` & `tmp/acapy_wallet_groups_plugin-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acapy_wallet_groups_plugin-0.4.0.tar", max compression
+gzip compressed data, was "acapy_wallet_groups_plugin-0.4.1.tar", max compression
```

## Comparing `acapy_wallet_groups_plugin-0.4.0.tar` & `acapy_wallet_groups_plugin-0.4.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11334 2023-07-25 10:16:39.541897 acapy_wallet_groups_plugin-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     1241 2023-07-25 10:16:39.541897 acapy_wallet_groups_plugin-0.4.0/acapy_wallet_groups_plugin/__init__.py
--rw-r--r--   0        0        0    10001 2023-07-25 10:16:39.541897 acapy_wallet_groups_plugin-0.4.0/acapy_wallet_groups_plugin/routes.py
--rw-r--r--   0        0        0      621 2023-07-25 10:16:39.545898 acapy_wallet_groups_plugin-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 acapy_wallet_groups_plugin-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-07-25 10:36:10.989614 acapy_wallet_groups_plugin-0.4.1/LICENSE.md
+-rw-r--r--   0        0        0     1241 2023-07-25 10:36:10.989614 acapy_wallet_groups_plugin-0.4.1/acapy_wallet_groups_plugin/__init__.py
+-rw-r--r--   0        0        0    10001 2023-07-25 10:36:10.989614 acapy_wallet_groups_plugin-0.4.1/acapy_wallet_groups_plugin/routes.py
+-rw-r--r--   0        0        0      588 2023-07-25 10:36:10.989614 acapy_wallet_groups_plugin-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      536 1970-01-01 00:00:00.000000 acapy_wallet_groups_plugin-0.4.1/PKG-INFO
```

### Comparing `acapy_wallet_groups_plugin-0.4.0/LICENSE.md` & `acapy_wallet_groups_plugin-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `acapy_wallet_groups_plugin-0.4.0/acapy_wallet_groups_plugin/__init__.py` & `acapy_wallet_groups_plugin-0.4.1/acapy_wallet_groups_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `acapy_wallet_groups_plugin-0.4.0/acapy_wallet_groups_plugin/routes.py` & `acapy_wallet_groups_plugin-0.4.1/acapy_wallet_groups_plugin/routes.py`

 * *Files identical despite different names*

### Comparing `acapy_wallet_groups_plugin-0.4.0/pyproject.toml` & `acapy_wallet_groups_plugin-0.4.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "acapy_wallet_groups_plugin"
-version = "0.4.0"
+version = "0.4.1"
 description = "Agent plugin to add a group id to a wallet"
 authors = ["Berend Sliedrecht <berend@animo.id>"]
 packages = [{ include = "acapy_wallet_groups_plugin" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9.0,<4.0.0"
-aries-cloudagent = { extras = ["indy"], version = "0.9.0" }
+aries-cloudagent = "0.9.0"
 aiohttp = "^3.8.4"
 marshmallow = "^3.5.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
 pytest-cov = "^4.1.0"
```

### Comparing `acapy_wallet_groups_plugin-0.4.0/PKG-INFO` & `acapy_wallet_groups_plugin-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: acapy-wallet-groups-plugin
-Version: 0.4.0
+Version: 0.4.1
 Summary: Agent plugin to add a group id to a wallet
 Author: Berend Sliedrecht
 Author-email: berend@animo.id
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: aries-cloudagent[indy] (==0.9.0)
+Requires-Dist: aries-cloudagent (==0.9.0)
 Requires-Dist: marshmallow (>=3.5.1,<4.0.0)
```

