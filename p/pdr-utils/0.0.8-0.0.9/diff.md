# Comparing `tmp/pdr-utils-0.0.8.tar.gz` & `tmp/pdr-utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdr-utils-0.0.8.tar", last modified: Tue Jul 25 06:26:53 2023, max compression
+gzip compressed data, was "pdr-utils-0.0.9.tar", last modified: Tue Jul 25 06:38:18 2023, max compression
```

## Comparing `pdr-utils-0.0.8.tar` & `pdr-utils-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:26:53.850891 pdr-utils-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 06:26:43.000000 pdr-utils-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-25 06:26:53.846891 pdr-utils-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-25 06:26:43.000000 pdr-utils-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:26:53.846891 pdr-utils-0.0.8/pdr_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:26:43.000000 pdr-utils-0.0.8/pdr_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-25 06:26:43.000000 pdr-utils-0.0.8/pdr_utils/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-25 06:26:43.000000 pdr-utils-0.0.8/pdr_utils/subgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:26:53.846891 pdr-utils-0.0.8/pdr_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-25 06:26:53.000000 pdr-utils-0.0.8/pdr_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-25 06:26:53.000000 pdr-utils-0.0.8/pdr_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:26:53.000000 pdr-utils-0.0.8/pdr_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:26:53.000000 pdr-utils-0.0.8/pdr_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 06:26:53.000000 pdr-utils-0.0.8/pdr_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 06:26:53.000000 pdr-utils-0.0.8/pdr_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 06:26:53.850891 pdr-utils-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-25 06:26:43.000000 pdr-utils-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:38:18.441758 pdr-utils-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 06:38:09.000000 pdr-utils-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-25 06:38:18.441758 pdr-utils-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-25 06:38:09.000000 pdr-utils-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:38:18.441758 pdr-utils-0.0.9/pdr_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:38:09.000000 pdr-utils-0.0.9/pdr_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14623 2023-07-25 06:38:09.000000 pdr-utils-0.0.9/pdr_utils/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-25 06:38:09.000000 pdr-utils-0.0.9/pdr_utils/subgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:38:18.441758 pdr-utils-0.0.9/pdr_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-25 06:38:18.000000 pdr-utils-0.0.9/pdr_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-25 06:38:18.000000 pdr-utils-0.0.9/pdr_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:38:18.000000 pdr-utils-0.0.9/pdr_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:38:18.000000 pdr-utils-0.0.9/pdr_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 06:38:18.000000 pdr-utils-0.0.9/pdr_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 06:38:18.000000 pdr-utils-0.0.9/pdr_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 06:38:18.441758 pdr-utils-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-25 06:38:09.000000 pdr-utils-0.0.9/setup.py
```

### Comparing `pdr-utils-0.0.8/LICENSE` & `pdr-utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pdr-utils-0.0.8/PKG-INFO` & `pdr-utils-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Predictoor utils lib.
 Home-page: https://github.com/oceanprotocol/pdr-utils
 Author: oceanprotocol
 Author-email: devops@oceanprotocol.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pdr-utils-0.0.8/pdr_utils/contract.py` & `pdr-utils-0.0.9/pdr_utils/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,19 +181,22 @@
                 self.config.w3.eth.wait_for_transaction_receipt(tx)
             return tx
         except Exception as e:
             print(e)
             return None
     
     def buy_many(self,how_many,gasLimit=None,wait_for_receipt=False):
+        """ Buys multiple accesses and returns tx hashes"""
+        txs=[]
         if how_many<1:
             return
         print(f"Buying {how_many} accesses....")
         for i in range(0,how_many):
-            self.buy_and_start_subscription(gasLimit,wait_for_receipt)
+            txs.append(self.buy_and_start_subscription(gasLimit,wait_for_receipt))
+        return txs
     
     def get_exchanges(self):
         return self.contract_instance.functions.getFixedRates().call()
     
     def get_stake_token(self):
         return self.contract_instance.functions.stakeToken().call()
```

### Comparing `pdr-utils-0.0.8/pdr_utils/subgraph.py` & `pdr-utils-0.0.9/pdr_utils/subgraph.py`

 * *Files identical despite different names*

### Comparing `pdr-utils-0.0.8/pdr_utils.egg-info/PKG-INFO` & `pdr-utils-0.0.9/pdr_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Predictoor utils lib.
 Home-page: https://github.com/oceanprotocol/pdr-utils
 Author: oceanprotocol
 Author-email: devops@oceanprotocol.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pdr-utils-0.0.8/setup.py` & `pdr-utils-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,11 +50,11 @@
         ]
     ),
     setup_requires=setup_requirements,
     test_suite="tests",
     url="https://github.com/oceanprotocol/pdr-utils",
     # fmt: off
     # bumpversion needs single quotes
-    version='0.0.8',
+    version='0.0.9',
     # fmt: on
     zip_safe=False,
 )
```

