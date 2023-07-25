# Comparing `tmp/killbills_sdk-0.0.1.tar.gz` & `tmp/killbills_sdk-0.0.1b0.tar.gz`

## Comparing `killbills_sdk-0.0.1.tar` & `killbills_sdk-0.0.1b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/src/killbills_sdk/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/src/killbills_sdk/cryptoService.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/src/killbills_sdk/getStores.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/src/killbills_sdk/sendDataWithHmac.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/src/killbills_sdk/sendReceipt.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/src/killbills_sdk/sendTransaction.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/src/killbills_sdk/validatorService.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/src/killbills_sdk/tests/test_crypto_service.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/src/killbills_sdk/tests/test_get_stores.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/src/killbills_sdk/tests/test_send_receipt.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/src/killbills_sdk/tests/test_send_transaction.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/src/killbills_sdk/tests/test_validator_service.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/LICENSE
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/README.md
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/cryptoService.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/getStores.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/sendDataWithHmac.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/sendReceipt.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/sendTransaction.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/validatorService.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_crypto_service.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_get_stores.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_send_receipt.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_send_transaction.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_validator_service.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/LICENSE
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/README.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/PKG-INFO
```

### Comparing `killbills_sdk-0.0.1/src/killbills_sdk/getStores.py` & `killbills_sdk-0.0.1b0/src/killbills_sdk/getStores.py`

 * *Files identical despite different names*

### Comparing `killbills_sdk-0.0.1/src/killbills_sdk/sendDataWithHmac.py` & `killbills_sdk-0.0.1b0/src/killbills_sdk/sendDataWithHmac.py`

 * *Files identical despite different names*

### Comparing `killbills_sdk-0.0.1/src/killbills_sdk/validatorService.py` & `killbills_sdk-0.0.1b0/src/killbills_sdk/validatorService.py`

 * *Files identical despite different names*

### Comparing `killbills_sdk-0.0.1/src/killbills_sdk/tests/test_crypto_service.py` & `killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_crypto_service.py`

 * *Files identical despite different names*

### Comparing `killbills_sdk-0.0.1/src/killbills_sdk/tests/test_get_stores.py` & `killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_get_stores.py`

 * *Files identical despite different names*

### Comparing `killbills_sdk-0.0.1/src/killbills_sdk/tests/test_send_receipt.py` & `killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_send_receipt.py`

 * *Files identical despite different names*

### Comparing `killbills_sdk-0.0.1/src/killbills_sdk/tests/test_send_transaction.py` & `killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_send_transaction.py`

 * *Files identical despite different names*

### Comparing `killbills_sdk-0.0.1/src/killbills_sdk/tests/test_validator_service.py` & `killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_validator_service.py`

 * *Files identical despite different names*

### Comparing `killbills_sdk-0.0.1/.gitignore` & `killbills_sdk-0.0.1b0/.gitignore`

 * *Files identical despite different names*

### Comparing `killbills_sdk-0.0.1/LICENSE` & `killbills_sdk-0.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `killbills_sdk-0.0.1/pyproject.toml` & `killbills_sdk-0.0.1b0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "killbills_sdk"
-version = "0.0.1"
+version = "0.0.1-beta.0"
 authors = [
     { name = "killbillsdev", email = "cto@killbills.co" }
 ]
 description = "KillBills e-receipt sdk"
 logo_url = "https://a.storyblok.com/f/149852/x/797a4a2b7e/dark_logo.svg"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `killbills_sdk-0.0.1/PKG-INFO` & `killbills_sdk-0.0.1b0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: killbills_sdk
-Version: 0.0.1
+Version: 0.0.1b0
 Summary: KillBills e-receipt sdk
 Project-URL: Homepage, https://github.com/killbillsdev/killbills-sdk-python
 Project-URL: Bug Tracker, https://github.com/killbillsdev/killbills-sdk-python/issues
 Author-email: killbillsdev <cto@killbills.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: pydantic>=2.0.3
 Requires-Dist: pytest>=7.4.0
 Requires-Dist: requests>=2.26.0
 Description-Content-Type: text/markdown
 
-# killbills-sdk-python
+# killbills-sdk-python
+
+![alt text](https://a.storyblok.com/f/149852/x/797a4a2b7e/dark_logo.svg)
```

