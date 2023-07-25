# Comparing `tmp/kl_sdk-0.0.6.tar.gz` & `tmp/kl_sdk-0.0.7.tar.gz`

## Comparing `kl_sdk-0.0.6.tar` & `kl_sdk-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/src/kl_sdk/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/src/kl_sdk/cryptoService.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/src/kl_sdk/getStores.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/src/kl_sdk/sendDataWithHmac.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/src/kl_sdk/sendReceipt.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/src/kl_sdk/sendTransaction.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/src/kl_sdk/trytry.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/src/kl_sdk/validatorService.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/src/kl_sdk/tests/test_crypto_service.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/src/kl_sdk/tests/test_get_stores.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/src/kl_sdk/tests/test_send_receipt.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/src/kl_sdk/tests/test_send_transaction.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/src/kl_sdk/tests/test_validator_service.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/LICENSE
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 kl_sdk-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/src/kl_sdk/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/src/kl_sdk/cryptoService.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/src/kl_sdk/getStores.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/src/kl_sdk/sendDataWithHmac.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/src/kl_sdk/sendReceipt.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/src/kl_sdk/sendTransaction.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/src/kl_sdk/trytry.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/src/kl_sdk/validatorService.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/src/kl_sdk/tests/test_crypto_service.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/src/kl_sdk/tests/test_get_stores.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/src/kl_sdk/tests/test_send_receipt.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/src/kl_sdk/tests/test_send_transaction.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/src/kl_sdk/tests/test_validator_service.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/LICENSE
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 kl_sdk-0.0.7/PKG-INFO
```

### Comparing `kl_sdk-0.0.6/src/kl_sdk/getStores.py` & `kl_sdk-0.0.7/src/kl_sdk/getStores.py`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.6/src/kl_sdk/sendDataWithHmac.py` & `kl_sdk-0.0.7/src/kl_sdk/sendDataWithHmac.py`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.6/src/kl_sdk/trytry.py` & `kl_sdk-0.0.7/src/kl_sdk/trytry.py`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.6/src/kl_sdk/validatorService.py` & `kl_sdk-0.0.7/src/kl_sdk/validatorService.py`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.6/src/kl_sdk/tests/test_crypto_service.py` & `kl_sdk-0.0.7/src/kl_sdk/tests/test_crypto_service.py`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.6/src/kl_sdk/tests/test_get_stores.py` & `kl_sdk-0.0.7/src/kl_sdk/tests/test_get_stores.py`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.6/src/kl_sdk/tests/test_send_receipt.py` & `kl_sdk-0.0.7/src/kl_sdk/tests/test_send_receipt.py`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.6/src/kl_sdk/tests/test_send_transaction.py` & `kl_sdk-0.0.7/src/kl_sdk/tests/test_send_transaction.py`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.6/src/kl_sdk/tests/test_validator_service.py` & `kl_sdk-0.0.7/src/kl_sdk/tests/test_validator_service.py`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.6/.gitignore` & `kl_sdk-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.6/LICENSE` & `kl_sdk-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.6/pyproject.toml` & `kl_sdk-0.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kl_sdk"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "killbillsdev", email = "cto@killbills.co" }
 ]
 description = "KillBills e-receipt sdk"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `kl_sdk-0.0.6/PKG-INFO` & `kl_sdk-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kl_sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: KillBills e-receipt sdk
 Project-URL: Homepage, https://github.com/killbillsdev/killbills-sdk-python
 Project-URL: Bug Tracker, https://github.com/killbillsdev/killbills-sdk-python/issues
 Author-email: killbillsdev <cto@killbills.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

