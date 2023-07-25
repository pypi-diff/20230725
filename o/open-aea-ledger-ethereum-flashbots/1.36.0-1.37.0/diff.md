# Comparing `tmp/open-aea-ledger-ethereum-flashbots-1.36.0.tar.gz` & `tmp/open-aea-ledger-ethereum-flashbots-1.37.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-ledger-ethereum-flashbots-1.36.0.tar", last modified: Wed Jul 19 12:43:55 2023, max compression
+gzip compressed data, was "open-aea-ledger-ethereum-flashbots-1.37.0.tar", last modified: Tue Jul 25 13:41:16 2023, max compression
```

## Comparing `open-aea-ledger-ethereum-flashbots-1.36.0.tar` & `open-aea-ledger-ethereum-flashbots-1.37.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 12:43:55.377955 open-aea-ledger-ethereum-flashbots-1.36.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11339 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-flashbots-1.36.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-flashbots-1.36.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-07-19 12:43:55.377955 open-aea-ledger-ethereum-flashbots-1.36.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-flashbots-1.36.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 12:43:55.373955 open-aea-ledger-ethereum-flashbots-1.36.0/aea_ledger_ethereum_flashbots/
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-flashbots-1.36.0/aea_ledger_ethereum_flashbots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13945 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-flashbots-1.36.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 12:43:55.377955 open-aea-ledger-ethereum-flashbots-1.36.0/open_aea_ledger_ethereum_flashbots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-07-19 12:43:55.000000 open-aea-ledger-ethereum-flashbots-1.36.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      538 2023-07-19 12:43:55.000000 open-aea-ledger-ethereum-flashbots-1.36.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 12:43:55.000000 open-aea-ledger-ethereum-flashbots-1.36.0/open_aea_ledger_ethereum_flashbots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-19 12:43:55.000000 open-aea-ledger-ethereum-flashbots-1.36.0/open_aea_ledger_ethereum_flashbots.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-19 12:43:55.000000 open-aea-ledger-ethereum-flashbots-1.36.0/open_aea_ledger_ethereum_flashbots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-19 12:43:55.000000 open-aea-ledger-ethereum-flashbots-1.36.0/open_aea_ledger_ethereum_flashbots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-flashbots-1.36.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-19 12:43:55.377955 open-aea-ledger-ethereum-flashbots-1.36.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2686 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-flashbots-1.36.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 12:43:55.377955 open-aea-ledger-ethereum-flashbots-1.36.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-flashbots-1.36.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11057 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-flashbots-1.36.0/tests/test_ethereum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 13:41:16.660289 open-aea-ledger-ethereum-flashbots-1.37.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11339 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-flashbots-1.37.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-flashbots-1.37.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-07-25 13:41:16.660289 open-aea-ledger-ethereum-flashbots-1.37.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-flashbots-1.37.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 13:41:16.656289 open-aea-ledger-ethereum-flashbots-1.37.0/aea_ledger_ethereum_flashbots/
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-flashbots-1.37.0/aea_ledger_ethereum_flashbots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13945 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-flashbots-1.37.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 13:41:16.660289 open-aea-ledger-ethereum-flashbots-1.37.0/open_aea_ledger_ethereum_flashbots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-07-25 13:41:16.000000 open-aea-ledger-ethereum-flashbots-1.37.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      538 2023-07-25 13:41:16.000000 open-aea-ledger-ethereum-flashbots-1.37.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 13:41:16.000000 open-aea-ledger-ethereum-flashbots-1.37.0/open_aea_ledger_ethereum_flashbots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-25 13:41:16.000000 open-aea-ledger-ethereum-flashbots-1.37.0/open_aea_ledger_ethereum_flashbots.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-25 13:41:16.000000 open-aea-ledger-ethereum-flashbots-1.37.0/open_aea_ledger_ethereum_flashbots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-25 13:41:16.000000 open-aea-ledger-ethereum-flashbots-1.37.0/open_aea_ledger_ethereum_flashbots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-flashbots-1.37.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-25 13:41:16.664290 open-aea-ledger-ethereum-flashbots-1.37.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2686 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-flashbots-1.37.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 13:41:16.660289 open-aea-ledger-ethereum-flashbots-1.37.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-flashbots-1.37.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11057 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-flashbots-1.37.0/tests/test_ethereum.py
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.36.0/LICENSE` & `open-aea-ledger-ethereum-flashbots-1.37.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.36.0/PKG-INFO` & `open-aea-ledger-ethereum-flashbots-1.37.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-flashbots
-Version: 1.36.0
+Version: 1.37.0
 Summary: Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.36.0/aea_ledger_ethereum_flashbots/__init__.py` & `open-aea-ledger-ethereum-flashbots-1.37.0/aea_ledger_ethereum_flashbots/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.36.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py` & `open-aea-ledger-ethereum-flashbots-1.37.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.36.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO` & `open-aea-ledger-ethereum-flashbots-1.37.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-flashbots
-Version: 1.36.0
+Version: 1.37.0
 Summary: Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.36.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt` & `open-aea-ledger-ethereum-flashbots-1.37.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.36.0/setup.py` & `open-aea-ledger-ethereum-flashbots-1.37.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """Setup script for "aea_ledger_ethereum_flashbots" package."""
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="open-aea-ledger-ethereum-flashbots",
-    version="1.36.0",
+    version="1.37.0",
     author="Valory AG",
     license="Apache-2.0",
     description="Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.",
     long_description=(
         "Python package extending the default open-aea ethereum ledger plugin to add support for flashbots."
     ),
     long_description_content_type="text/markdown",
@@ -37,15 +37,15 @@
     package_data={
         "aea_ledger_ethereum_flashbots": [
             "py.typed",
         ]
     },
     python_requires=">=3.9,<4.0",
     install_requires=[
-        "open-aea-ledger-ethereum~=1.36.0",
+        "open-aea-ledger-ethereum~=1.37.0",
         "flashbots==1.1.1",
     ],
     tests_require=["pytest"],
     entry_points={
         "aea.cryptos": [
             "ethereum_flashbots = aea_ledger_ethereum_flashbots:EthereumFlashbotCrypto"
         ],
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.36.0/tests/__init__.py` & `open-aea-ledger-ethereum-flashbots-1.37.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.36.0/tests/test_ethereum.py` & `open-aea-ledger-ethereum-flashbots-1.37.0/tests/test_ethereum.py`

 * *Files identical despite different names*

