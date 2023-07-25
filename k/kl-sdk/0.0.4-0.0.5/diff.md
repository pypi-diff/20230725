# Comparing `tmp/kl_sdk-0.0.4.tar.gz` & `tmp/kl_sdk-0.0.5.tar.gz`

## Comparing `kl_sdk-0.0.4.tar` & `kl_sdk-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,20 @@
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 kl_sdk-0.0.4/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kl_sdk-0.0.4/src/kl_sdk/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 kl_sdk-0.0.4/src/kl_sdk/cryptoService.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 kl_sdk-0.0.4/src/kl_sdk/sendDataWithHmac.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 kl_sdk-0.0.4/src/kl_sdk/sendReceipt.py
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 kl_sdk-0.0.4/src/kl_sdk/validatorService.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 kl_sdk-0.0.4/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 kl_sdk-0.0.4/LICENSE
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kl_sdk-0.0.4/README.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 kl_sdk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 kl_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/src/kl_sdk/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/src/kl_sdk/cryptoService.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/src/kl_sdk/getStores.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/src/kl_sdk/sendDataWithHmac.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/src/kl_sdk/sendReceipt.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/src/kl_sdk/sendTransaction.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/src/kl_sdk/trytry.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/src/kl_sdk/validatorService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/src/kl_sdk/tests/__init__.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/src/kl_sdk/tests/test_crypto_service.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/src/kl_sdk/tests/test_get_stores.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/src/kl_sdk/tests/test_send_receipt.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/src/kl_sdk/tests/test_send_transaction.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/src/kl_sdk/tests/test_validator_service.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/LICENSE
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 kl_sdk-0.0.5/PKG-INFO
```

### Comparing `kl_sdk-0.0.4/src/kl_sdk/sendDataWithHmac.py` & `kl_sdk-0.0.5/src/kl_sdk/sendDataWithHmac.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import requests
 import json
 import hashlib
 
 from cryptoService import cipher_hmac_payload
 
 def send_data_with_hmac(env, endpoint, data, hmac_signature, validator):
-    try:
-        if not data or not hmac_signature or hmac_signature == '':
-            raise ValueError(f"You have not provided Data or Hmac Signature:\nData: {data}\nhmacSignature: {hmac_signature}")
-
-        payload_validation_result = validator(data)
-
-        if payload_validation_result is not True:
-            raise ValueError(payload_validation_result)
-
-        hashed_payload = cipher_hmac_payload(data, hmac_signature)
-        headers = {
-            'Authorization': f'hmac {hashed_payload}',
-            'Content-Type': 'application/json'
-        }
-
-        url = f'https://in.{env + "." if env != "prod" else "."}killbills.{"dev" if env != "prod" else "co"}/{endpoint}'
-        response = requests.post(url, data=json.dumps(data), headers=headers)
-        response.raise_for_status()  # Raise an exception for HTTP errors (4xx, 5xx)
-
-        return response.json()
-    except (requests.exceptions.RequestException, ValueError) as error:
-        return str(error)
+
+    if not data or not hmac_signature or hmac_signature == '':
+        raise ValueError(f"You have not provided Data or Hmac Signature:\nData: {data}\nhmacSignature: {hmac_signature}")
+
+    payload_validation_result = validator(data)
+
+    if payload_validation_result is not True:
+        raise ValueError(payload_validation_result)
+
+    hashed_payload = cipher_hmac_payload(data, hmac_signature)
+    headers = {
+        'Authorization': f'hmac {hashed_payload}',
+        'Content-Type': 'application/json'
+    }
+
+    url = f'https://in.{env + "." if env != "prod" else "."}killbills.{"dev" if env != "prod" else "co"}/{endpoint}'
+    response = requests.post(url, data=json.dumps(data), headers=headers)
+    response.raise_for_status()  # Raise an exception for HTTP errors (4xx, 5xx)
+
+    return response.json()
+
```

### Comparing `kl_sdk-0.0.4/src/kl_sdk/validatorService.py` & `kl_sdk-0.0.5/src/kl_sdk/validatorService.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 from typing import List, Optional
-from pydantic import BaseModel, validator, ValidationError, conint, constr, model_validator
+from pydantic import BaseModel, validator, ValidationError, conint, constr, model_validator,PositiveFloat, PositiveInt
 import re
+from enum import Enum
 
-class TransactionPayment(BaseModel):
+class ReceiptFormat(str, Enum):
+    JSON = 'json'
+    PDF = 'pdf'
+    SVG = 'svg'
+    PNG = 'png'
+
+class Payment(BaseModel):
+    bin: str= None
+    last_four: str = None
+    auth_code: str = None
+    scheme: str = None
+    transaction_id: str = None
+
+class Transaction(BaseModel):
     reference_id: str
-    amount: float
+    amount: PositiveInt
     customer_id: str
-    transaction_date: str
-    store_name: Optional[str]
+    transaction_date: PositiveInt
+    store_name: str = None
     billing_descriptor: str
-    siret: Optional[str]
-    payment: Optional[dict]
-    currency: Optional[str]
-    pos_name: Optional[str]
-    merchant_name: Optional[str]
+    siret: str = None
+    currency: str = 'EUR'
+    pos_name: str = None
+    merchant_name: str = None
+    payment: Payment = None
+
+class TransactionPayload(BaseModel):
+    bank_id: constr(min_length=36, max_length=36)
+    callback_url: str
+    partner_name: str
+    receipt_format: ReceiptFormat
+    transaction: Transaction
 
-    @validator('amount')
-    def amount_positive(cls, value):
-        if value <= 0:
-            raise ValueError('Amount must be positive')
-        return value
 
-    @validator('transaction_date')
-    def validate_transaction_date(cls, value):
-        if not re.match(r'^\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}$', value):
-            raise ValueError('Invalid date format. Expected format: YYYY-MM-DDTHH:mm:ss')
-        return value
 
 class ReceiptPayload(BaseModel):
     reference_id: str
     amount: float
     currency: str
     date: str
     covers: Optional[int]
@@ -80,15 +91,15 @@
                 raise ValueError('Invalid tax rate. Expected 550, 1000, or 2000')
         return value
 
 
 def validate_transaction_payload(payload):
     if not payload:
         raise ValueError('No payload to validate')
-    TransactionPayment(**payload)
+    TransactionPayload(**payload)
     return True
 
 
 
 def validate_receipt_payload(payload):
     if not payload:
         raise ValueError('No payload to validate')
```

### Comparing `kl_sdk-0.0.4/.gitignore` & `kl_sdk-0.0.5/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,15 @@
 .env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
+*/.env
 
 # Spyder project settings
 .spyderproject
 .spyproject
 
 # Rope project settings
 .ropeproject
```

### Comparing `kl_sdk-0.0.4/LICENSE` & `kl_sdk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kl_sdk-0.0.4/pyproject.toml` & `kl_sdk-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kl_sdk"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "killbillsdev", email = "cto@killbills.co" }
 ]
 description = "KillBills e-receipt sdk"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "requests>=2.26.0",
-    "pydantic>=2.0.3"
+    "pydantic>=2.0.3",
+    "pytest>=7.4.0"
 ]
 
 [project.urls]
 Homepage = "https://github.com/killbillsdev/killbills-sdk-python"
 "Bug Tracker" = "https://github.com/killbillsdev/killbills-sdk-python/issues"
 
 [dependencies]
```

### Comparing `kl_sdk-0.0.4/PKG-INFO` & `kl_sdk-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: kl_sdk
-Version: 0.0.4
+Version: 0.0.5
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
+Requires-Dist: pytest>=7.4.0
 Requires-Dist: requests>=2.26.0
 Description-Content-Type: text/markdown
 
 # killbills-sdk-python
```

