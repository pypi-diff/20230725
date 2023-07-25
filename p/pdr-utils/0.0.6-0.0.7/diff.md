# Comparing `tmp/pdr-utils-0.0.6.tar.gz` & `tmp/pdr-utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdr-utils-0.0.6.tar", last modified: Tue Jul 25 06:03:24 2023, max compression
+gzip compressed data, was "pdr-utils-0.0.7.tar", last modified: Tue Jul 25 06:22:24 2023, max compression
```

## Comparing `pdr-utils-0.0.6.tar` & `pdr-utils-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:03:24.033721 pdr-utils-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 06:03:14.000000 pdr-utils-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-25 06:03:24.033721 pdr-utils-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-25 06:03:14.000000 pdr-utils-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:03:24.033721 pdr-utils-0.0.6/pdr_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:03:14.000000 pdr-utils-0.0.6/pdr_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-07-25 06:03:14.000000 pdr-utils-0.0.6/pdr_utils/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-25 06:03:14.000000 pdr-utils-0.0.6/pdr_utils/subgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:03:24.033721 pdr-utils-0.0.6/pdr_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-25 06:03:24.000000 pdr-utils-0.0.6/pdr_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-25 06:03:24.000000 pdr-utils-0.0.6/pdr_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:03:24.000000 pdr-utils-0.0.6/pdr_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:03:24.000000 pdr-utils-0.0.6/pdr_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 06:03:24.000000 pdr-utils-0.0.6/pdr_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 06:03:24.000000 pdr-utils-0.0.6/pdr_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 06:03:24.033721 pdr-utils-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-25 06:03:14.000000 pdr-utils-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:22:24.006705 pdr-utils-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 06:22:14.000000 pdr-utils-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-25 06:22:24.006705 pdr-utils-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-25 06:22:14.000000 pdr-utils-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:22:24.006705 pdr-utils-0.0.7/pdr_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:22:14.000000 pdr-utils-0.0.7/pdr_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-07-25 06:22:14.000000 pdr-utils-0.0.7/pdr_utils/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-25 06:22:14.000000 pdr-utils-0.0.7/pdr_utils/subgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:22:24.006705 pdr-utils-0.0.7/pdr_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-25 06:22:23.000000 pdr-utils-0.0.7/pdr_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-25 06:22:24.000000 pdr-utils-0.0.7/pdr_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:22:23.000000 pdr-utils-0.0.7/pdr_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:22:23.000000 pdr-utils-0.0.7/pdr_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 06:22:23.000000 pdr-utils-0.0.7/pdr_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 06:22:23.000000 pdr-utils-0.0.7/pdr_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 06:22:24.006705 pdr-utils-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-25 06:22:14.000000 pdr-utils-0.0.7/setup.py
```

### Comparing `pdr-utils-0.0.6/LICENSE` & `pdr-utils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pdr-utils-0.0.6/PKG-INFO` & `pdr-utils-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Predictoor utils lib.
 Home-page: https://github.com/oceanprotocol/pdr-utils
 Author: oceanprotocol
 Author-email: devops@oceanprotocol.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pdr-utils-0.0.6/pdr_utils/contract.py` & `pdr-utils-0.0.7/pdr_utils/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
     
     def get_price(self):
         fixed_rates=self.get_exchanges()
         if not fixed_rates:
             return
         (fixed_rate_address,exchange_id) = fixed_rates[0]
         # get datatoken price
-        exchange = FixedRate(fixed_rate_address)
+        exchange = FixedRate(self.config,fixed_rate_address)
         (baseTokenAmount, oceanFeeAmount, publishMarketFeeAmount,consumeMarketFeeAmount) = exchange.get_dt_price(exchange_id)
         return baseTokenAmount
     
     def get_current_epoch(self):
         return self.contract_instance.functions.curEpoch().call()
     
     def get_blocksPerEpoch(self):
@@ -247,18 +247,17 @@
             return None
 
     def soonest_block_to_predict(self,block):
         return self.contract_instance.functions.soonestBlockToPredict(block).call()
     
     def submit_prediction(self,predicted_value,stake_amount,prediction_block):
         """ Sumbits a prediction"""
-        stake_token = Token(self.contract_instance.functions.stakeToken().call())
         # TO DO - check allowence
         amount_wei = self.config.w3.to_wei(str(stake_amount),'ether')
-        stake_token.approve(self.contract_address,amount_wei)
+        self.token.approve(self.contract_address,amount_wei)
         gasPrice = self.config.w3.eth.gas_price
         try:
             tx = self.contract_instance.functions.submitPredval(predicted_value,amount_wei,prediction_block).transact({"from":self.config.owner,"gasPrice":gasPrice})
             print(f"Submitted prediction, txhash: {tx.hex()}")
             receipt = self.config.w3.eth.wait_for_transaction_receipt(tx)
             return receipt
         except Exception as e:
```

### Comparing `pdr-utils-0.0.6/pdr_utils/subgraph.py` & `pdr-utils-0.0.7/pdr_utils/subgraph.py`

 * *Files identical despite different names*

### Comparing `pdr-utils-0.0.6/pdr_utils.egg-info/PKG-INFO` & `pdr-utils-0.0.7/pdr_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Predictoor utils lib.
 Home-page: https://github.com/oceanprotocol/pdr-utils
 Author: oceanprotocol
 Author-email: devops@oceanprotocol.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pdr-utils-0.0.6/setup.py` & `pdr-utils-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,11 +50,11 @@
         ]
     ),
     setup_requires=setup_requirements,
     test_suite="tests",
     url="https://github.com/oceanprotocol/pdr-utils",
     # fmt: off
     # bumpversion needs single quotes
-    version='0.0.6',
+    version='0.0.7',
     # fmt: on
     zip_safe=False,
 )
```

