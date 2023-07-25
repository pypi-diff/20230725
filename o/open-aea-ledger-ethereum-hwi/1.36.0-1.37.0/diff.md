# Comparing `tmp/open-aea-ledger-ethereum-hwi-1.36.0.tar.gz` & `tmp/open-aea-ledger-ethereum-hwi-1.37.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-ledger-ethereum-hwi-1.36.0.tar", last modified: Wed Jul 19 12:43:54 2023, max compression
+gzip compressed data, was "open-aea-ledger-ethereum-hwi-1.37.0.tar", last modified: Tue Jul 25 13:41:15 2023, max compression
```

## Comparing `open-aea-ledger-ethereum-hwi-1.36.0.tar` & `open-aea-ledger-ethereum-hwi-1.37.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 12:43:54.421943 open-aea-ledger-ethereum-hwi-1.36.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11339 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-hwi-1.36.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-hwi-1.36.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-07-19 12:43:54.421943 open-aea-ledger-ethereum-hwi-1.36.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-hwi-1.36.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 12:43:54.417942 open-aea-ledger-ethereum-hwi-1.36.0/aea_ledger_ethereum_hwi/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-hwi-1.36.0/aea_ledger_ethereum_hwi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13912 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-hwi-1.36.0/aea_ledger_ethereum_hwi/account.py
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-hwi-1.36.0/aea_ledger_ethereum_hwi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     7390 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-hwi-1.36.0/aea_ledger_ethereum_hwi/hwi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 12:43:54.421943 open-aea-ledger-ethereum-hwi-1.36.0/open_aea_ledger_ethereum_hwi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-07-19 12:43:54.000000 open-aea-ledger-ethereum-hwi-1.36.0/open_aea_ledger_ethereum_hwi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-07-19 12:43:54.000000 open-aea-ledger-ethereum-hwi-1.36.0/open_aea_ledger_ethereum_hwi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 12:43:54.000000 open-aea-ledger-ethereum-hwi-1.36.0/open_aea_ledger_ethereum_hwi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-07-19 12:43:54.000000 open-aea-ledger-ethereum-hwi-1.36.0/open_aea_ledger_ethereum_hwi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-07-19 12:43:54.000000 open-aea-ledger-ethereum-hwi-1.36.0/open_aea_ledger_ethereum_hwi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-19 12:43:54.000000 open-aea-ledger-ethereum-hwi-1.36.0/open_aea_ledger_ethereum_hwi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-hwi-1.36.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-19 12:43:54.421943 open-aea-ledger-ethereum-hwi-1.36.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-hwi-1.36.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 12:43:54.421943 open-aea-ledger-ethereum-hwi-1.36.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-hwi-1.36.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6054 2023-07-19 12:43:04.000000 open-aea-ledger-ethereum-hwi-1.36.0/tests/test_account.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 13:41:15.548226 open-aea-ledger-ethereum-hwi-1.37.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11339 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-hwi-1.37.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-hwi-1.37.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-07-25 13:41:15.548226 open-aea-ledger-ethereum-hwi-1.37.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-hwi-1.37.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 13:41:15.544226 open-aea-ledger-ethereum-hwi-1.37.0/aea_ledger_ethereum_hwi/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-hwi-1.37.0/aea_ledger_ethereum_hwi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13912 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-hwi-1.37.0/aea_ledger_ethereum_hwi/account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-hwi-1.37.0/aea_ledger_ethereum_hwi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7390 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-hwi-1.37.0/aea_ledger_ethereum_hwi/hwi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 13:41:15.548226 open-aea-ledger-ethereum-hwi-1.37.0/open_aea_ledger_ethereum_hwi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-07-25 13:41:15.000000 open-aea-ledger-ethereum-hwi-1.37.0/open_aea_ledger_ethereum_hwi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-07-25 13:41:15.000000 open-aea-ledger-ethereum-hwi-1.37.0/open_aea_ledger_ethereum_hwi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 13:41:15.000000 open-aea-ledger-ethereum-hwi-1.37.0/open_aea_ledger_ethereum_hwi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-07-25 13:41:15.000000 open-aea-ledger-ethereum-hwi-1.37.0/open_aea_ledger_ethereum_hwi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-07-25 13:41:15.000000 open-aea-ledger-ethereum-hwi-1.37.0/open_aea_ledger_ethereum_hwi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-25 13:41:15.000000 open-aea-ledger-ethereum-hwi-1.37.0/open_aea_ledger_ethereum_hwi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-hwi-1.37.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-25 13:41:15.548226 open-aea-ledger-ethereum-hwi-1.37.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-hwi-1.37.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 13:41:15.548226 open-aea-ledger-ethereum-hwi-1.37.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-hwi-1.37.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6054 2023-07-25 13:40:20.000000 open-aea-ledger-ethereum-hwi-1.37.0/tests/test_account.py
```

### Comparing `open-aea-ledger-ethereum-hwi-1.36.0/LICENSE` & `open-aea-ledger-ethereum-hwi-1.37.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.36.0/PKG-INFO` & `open-aea-ledger-ethereum-hwi-1.37.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-hwi
-Version: 1.36.0
+Version: 1.37.0
 Summary: Python package wrapping the public and private key cryptography and support for hardware wallet interactions.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-ledger-ethereum-hwi-1.36.0/aea_ledger_ethereum_hwi/__init__.py` & `open-aea-ledger-ethereum-hwi-1.37.0/aea_ledger_ethereum_hwi/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.36.0/aea_ledger_ethereum_hwi/account.py` & `open-aea-ledger-ethereum-hwi-1.37.0/aea_ledger_ethereum_hwi/account.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.36.0/aea_ledger_ethereum_hwi/exceptions.py` & `open-aea-ledger-ethereum-hwi-1.37.0/aea_ledger_ethereum_hwi/exceptions.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.36.0/aea_ledger_ethereum_hwi/hwi.py` & `open-aea-ledger-ethereum-hwi-1.37.0/aea_ledger_ethereum_hwi/hwi.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.36.0/open_aea_ledger_ethereum_hwi.egg-info/PKG-INFO` & `open-aea-ledger-ethereum-hwi-1.37.0/open_aea_ledger_ethereum_hwi.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-hwi
-Version: 1.36.0
+Version: 1.37.0
 Summary: Python package wrapping the public and private key cryptography and support for hardware wallet interactions.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-ledger-ethereum-hwi-1.36.0/open_aea_ledger_ethereum_hwi.egg-info/SOURCES.txt` & `open-aea-ledger-ethereum-hwi-1.37.0/open_aea_ledger_ethereum_hwi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.36.0/setup.py` & `open-aea-ledger-ethereum-hwi-1.37.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """Setup script for "aea_ledger_ethereum_hwi" package."""
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="open-aea-ledger-ethereum-hwi",
-    version="1.36.0",
+    version="1.37.0",
     author="Valory AG",
     license="Apache-2.0",
     description="Python package wrapping the public and private key cryptography and support for hardware wallet interactions.",
     long_description="Python package wrapping the public and private key cryptography and support for hardware wallet interactions.",
     long_description_content_type="text/markdown",
     packages=find_packages(include=["aea_ledger_ethereum_hwi*"]),
     package_data={
@@ -38,15 +38,15 @@
         ]
     },
     install_requires=[
         "open-aea>=1.0.0, <2.0.0",
         "web3==5.31.4",
         "ipfshttpclient==0.8.0a2",
         "eth-account>=0.5.9,<0.6.0",
-        "open-aea-ledger-ethereum~=1.36.0",
+        "open-aea-ledger-ethereum~=1.37.0",
         "apduboy>=0.5.0",
         "protobuf==3.19.5",
         "construct<=2.10.61",
     ],
     tests_require=["pytest"],
     entry_points={
         "aea.cryptos": ["ethereum_hwi = aea_ledger_ethereum_hwi:EthereumHWICrypto"],
```

### Comparing `open-aea-ledger-ethereum-hwi-1.36.0/tests/__init__.py` & `open-aea-ledger-ethereum-hwi-1.37.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.36.0/tests/test_account.py` & `open-aea-ledger-ethereum-hwi-1.37.0/tests/test_account.py`

 * *Files identical despite different names*

