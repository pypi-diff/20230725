# Comparing `tmp/pymesomb-1.0.1.tar.gz` & `tmp/pymesomb-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymesomb-1.0.1.tar", last modified: Sun Oct 23 20:38:37 2022, max compression
+gzip compressed data, was "pymesomb-1.0.2.tar", last modified: Tue Jul 25 16:51:58 2023, max compression
```

## Comparing `pymesomb-1.0.1.tar` & `pymesomb-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 hachther   (501) staff       (20)        0 2022-10-23 20:38:37.050198 pymesomb-1.0.1/
--rw-r--r--   0 hachther   (501) staff       (20)        0 2022-10-19 07:24:36.000000 pymesomb-1.0.1/LICENSE
--rw-r--r--   0 hachther   (501) staff       (20)        0 2022-10-19 07:24:48.000000 pymesomb-1.0.1/MANIFEST.in
--rw-r--r--   0 hachther   (501) staff       (20)     2936 2022-10-23 20:38:37.049934 pymesomb-1.0.1/PKG-INFO
--rw-r--r--   0 hachther   (501) staff       (20)     2552 2022-10-23 20:04:08.000000 pymesomb-1.0.1/README.md
-drwxr-xr-x   0 hachther   (501) staff       (20)        0 2022-10-23 20:38:37.044790 pymesomb-1.0.1/pymesomb/
--rw-r--r--   0 hachther   (501) staff       (20)       94 2022-10-23 20:23:21.000000 pymesomb-1.0.1/pymesomb/__init__.py
--rw-r--r--   0 hachther   (501) staff       (20)      606 2022-10-21 18:21:13.000000 pymesomb-1.0.1/pymesomb/exceptions.py
--rw-r--r--   0 hachther   (501) staff       (20)      933 2022-10-21 18:47:15.000000 pymesomb-1.0.1/pymesomb/models.py
--rw-r--r--   0 hachther   (501) staff       (20)     8261 2022-10-23 17:55:45.000000 pymesomb-1.0.1/pymesomb/operations.py
--rw-r--r--   0 hachther   (501) staff       (20)       82 2022-10-23 17:57:18.000000 pymesomb-1.0.1/pymesomb/settings.py
--rw-r--r--   0 hachther   (501) staff       (20)     2895 2022-10-21 19:07:16.000000 pymesomb-1.0.1/pymesomb/signature.py
-drwxr-xr-x   0 hachther   (501) staff       (20)        0 2022-10-23 20:38:37.049556 pymesomb-1.0.1/pymesomb.egg-info/
--rw-r--r--   0 hachther   (501) staff       (20)     2936 2022-10-23 20:38:36.000000 pymesomb-1.0.1/pymesomb.egg-info/PKG-INFO
--rw-r--r--   0 hachther   (501) staff       (20)      326 2022-10-23 20:38:37.000000 pymesomb-1.0.1/pymesomb.egg-info/SOURCES.txt
--rw-r--r--   0 hachther   (501) staff       (20)        1 2022-10-23 20:38:36.000000 pymesomb-1.0.1/pymesomb.egg-info/dependency_links.txt
--rw-r--r--   0 hachther   (501) staff       (20)        9 2022-10-23 20:38:36.000000 pymesomb-1.0.1/pymesomb.egg-info/requires.txt
--rw-r--r--   0 hachther   (501) staff       (20)        9 2022-10-23 20:38:36.000000 pymesomb-1.0.1/pymesomb.egg-info/top_level.txt
--rw-r--r--   0 hachther   (501) staff       (20)       38 2022-10-23 20:38:37.050284 pymesomb-1.0.1/setup.cfg
--rw-r--r--   0 hachther   (501) staff       (20)      825 2022-10-23 20:35:19.000000 pymesomb-1.0.1/setup.py
+drwxrwxr-x   0 hachther  (1000) hachther  (1000)        0 2023-07-25 16:51:58.924289 pymesomb-1.0.2/
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)      287 2023-07-25 12:40:15.000000 pymesomb-1.0.2/HISTORY.md
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)        0 2023-05-29 14:21:36.000000 pymesomb-1.0.2/LICENSE
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)        0 2023-05-29 14:21:36.000000 pymesomb-1.0.2/MANIFEST.in
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)     3403 2023-07-25 16:51:58.924289 pymesomb-1.0.2/PKG-INFO
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)     2731 2023-07-25 12:53:49.000000 pymesomb-1.0.2/README.md
+drwxrwxr-x   0 hachther  (1000) hachther  (1000)        0 2023-07-25 16:51:58.924289 pymesomb-1.0.2/pymesomb/
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)      133 2023-07-25 12:15:22.000000 pymesomb-1.0.2/pymesomb/__init__.py
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)      635 2023-05-29 15:36:39.000000 pymesomb-1.0.2/pymesomb/exceptions.py
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)      100 2023-07-25 10:42:01.000000 pymesomb-1.0.2/pymesomb/mesomb.py
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)     3611 2023-07-25 11:13:54.000000 pymesomb-1.0.2/pymesomb/models.py
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)     9941 2023-07-25 12:22:25.000000 pymesomb-1.0.2/pymesomb/operations.py
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)     2958 2023-07-25 12:08:05.000000 pymesomb-1.0.2/pymesomb/signature.py
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)      222 2023-07-25 11:10:39.000000 pymesomb-1.0.2/pymesomb/utils.py
+drwxrwxr-x   0 hachther  (1000) hachther  (1000)        0 2023-07-25 16:51:58.924289 pymesomb-1.0.2/pymesomb.egg-info/
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)     3403 2023-07-25 16:51:58.000000 pymesomb-1.0.2/pymesomb.egg-info/PKG-INFO
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)      353 2023-07-25 16:51:58.000000 pymesomb-1.0.2/pymesomb.egg-info/SOURCES.txt
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)        1 2023-07-25 16:51:58.000000 pymesomb-1.0.2/pymesomb.egg-info/dependency_links.txt
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)        9 2023-07-25 16:51:58.000000 pymesomb-1.0.2/pymesomb.egg-info/requires.txt
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)        9 2023-07-25 16:51:58.000000 pymesomb-1.0.2/pymesomb.egg-info/top_level.txt
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)       38 2023-07-25 16:51:58.924289 pymesomb-1.0.2/setup.cfg
+-rw-rw-r--   0 hachther  (1000) hachther  (1000)      825 2023-07-25 10:42:01.000000 pymesomb-1.0.2/setup.py
```

### Comparing `pymesomb-1.0.1/PKG-INFO` & `pymesomb-1.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pymesomb
-Version: 1.0.1
-Summary: Python client for MeSomb services.
-Home-page: https://github.com/hachther/mesomb-python-client.git
-Download-URL: https://pypi.org/project/pymesomb/
-Author: Hachther LLC
-Author-email: contact@hachther.com
-License: MIT
-Keywords: MeSomb,MobileMoney,OrangeMoney
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">Welcome to pymesomb 👋</h1>
 <p>
   <img alt="Version" src="https://img.shields.io/badge/version-1.0.0-blue.svg?cacheSeconds=2592000" />
   <a href="https://mesomb.hachther.com/en/api/v1.1/schema/" target="_blank">
     <img alt="Documentation" src="https://img.shields.io/badge/documentation-yes-brightgreen.svg" />
   </a>
   <a href="#" target="_blank">
@@ -39,32 +26,46 @@
 
 ## Usage
 
 ### Collect money from an account
 
 ```python
 from pymesomb.operations import PaymentOperation
-from pymesomb.signature import Signature
+from pymesomb.utils import RandomGenerator
 from datetime import datetime
 
 operation = PaymentOperation('<application_key>', '<access_key>', '<secret_key>')
-response = operation.make_collect(100, 'MTN', '677550203', datetime.now(), Signature.generate_nonce())
+response = operation.make_collect({
+    'amount': 100,
+    'service': 'MTN',
+    'payer': '670000000',
+    'date': datetime.now(),
+    'nonce': RandomGenerator.nonce(),
+    'trxID': '1'
+})
 print(response.is_operation_success())
 print(response.is_transaction_success())
 ```
 
 ### Depose money in an account
 
 ```python
 from pymesomb.operations import PaymentOperation
-from pymesomb.signature import Signature
+from pymesomb.utils import RandomGenerator
 from datetime import datetime
 
 operation = PaymentOperation('<application_key>', '<access_key>', '<secret_key>')
-response = operation.make_deposit(100, 'MTN', '677550203', datetime.now(), Signature.generate_nonce())
+response = operation.make_deposit({
+    'amount': 100,
+    'service': 'MTN',
+    'receiver': '670000000',
+    'date': datetime.now(),
+    'nonce': RandomGenerator.nonce(),
+    'trxID': '1'
+})
 print(response.is_operation_success())
 print(response.is_transaction_success())
 ```
 
 ### Get application status
 
 ```python
@@ -93,9 +94,7 @@
 * Twitter: [@hachther](https://twitter.com/hachther)
 * Github: [@hachther](https://github.com/hachther)
 * LinkedIn: [@hachther](https://linkedin.com/in/hachther)
 
 ## Show your support
 
 Give a ⭐️ if this project helped you!
-
-
```

#### html2text {}

```diff
@@ -1,32 +1,27 @@
-Metadata-Version: 2.1 Name: pymesomb Version: 1.0.1 Summary: Python client for
-MeSomb services. Home-page: https://github.com/hachther/mesomb-python-
-client.git Download-URL: https://pypi.org/project/pymesomb/ Author: Hachther
-LLC Author-email: contact@hachther.com License: MIT Keywords:
-MeSomb,MobileMoney,OrangeMoney Description-Content-Type: text/markdown License-
-File: LICENSE
                     ****** Welcome to pymesomb ð ******
 [Version] [Documentation] [License:_MIT] [Twitter:_hachther]
 > Python client for MeSomb Services > > You can check the full [documentation
 of the api here](https://mesomb.hachther.com/en/api/v1.1/schema/) ### ð 
 [Homepage](https://mesomb.com) ## Install ```sh pip3 install pymesomb ``` ##
 Usage ### Collect money from an account ```python from pymesomb.operations
-import PaymentOperation from pymesomb.signature import Signature from datetime
-import datetime operation = PaymentOperation('', '', '') response =
-operation.make_collect(100, 'MTN', '677550203', datetime.now(),
-Signature.generate_nonce()) print(response.is_operation_success()) print
-(response.is_transaction_success()) ``` ### Depose money in an account
-```python from pymesomb.operations import PaymentOperation from
-pymesomb.signature import Signature from datetime import datetime operation =
-PaymentOperation('', '', '') response = operation.make_deposit(100, 'MTN',
-'677550203', datetime.now(), Signature.generate_nonce()) print
+import PaymentOperation from pymesomb.utils import RandomGenerator from
+datetime import datetime operation = PaymentOperation('', '', '') response =
+operation.make_collect({ 'amount': 100, 'service': 'MTN', 'payer': '670000000',
+'date': datetime.now(), 'nonce': RandomGenerator.nonce(), 'trxID': '1' }) print
 (response.is_operation_success()) print(response.is_transaction_success()) ```
-### Get application status ```python from pymesomb.operations import
-PaymentOperation operation = PaymentOperation('', '', '') response =
-operation.get_status() print(response.name) ``` ### Get transactions by IDs
-```python from pymesomb.operations import PaymentOperation operation =
-PaymentOperation('', '', '') response = operation.get_transactions(['ID1',
-'ID2']) print(response) ``` ## Author ð¤ **Hachther LLC
+### Depose money in an account ```python from pymesomb.operations import
+PaymentOperation from pymesomb.utils import RandomGenerator from datetime
+import datetime operation = PaymentOperation('', '', '') response =
+operation.make_deposit({ 'amount': 100, 'service': 'MTN', 'receiver':
+'670000000', 'date': datetime.now(), 'nonce': RandomGenerator.nonce(), 'trxID':
+'1' }) print(response.is_operation_success()) print
+(response.is_transaction_success()) ``` ### Get application status ```python
+from pymesomb.operations import PaymentOperation operation = PaymentOperation
+('', '', '') response = operation.get_status() print(response.name) ``` ### Get
+transactions by IDs ```python from pymesomb.operations import PaymentOperation
+operation = PaymentOperation('', '', '') response = operation.get_transactions(
+['ID1', 'ID2']) print(response) ``` ## Author ð¤ **Hachther LLC
 hachther.com>** * Website: https://www.hachther.com * Twitter: [@hachther]
 (https://twitter.com/hachther) * Github: [@hachther](https://github.com/
 hachther) * LinkedIn: [@hachther](https://linkedin.com/in/hachther) ## Show
 your support Give a â­ï¸ if this project helped you!
```

### Comparing `pymesomb-1.0.1/pymesomb/exceptions.py` & `pymesomb-1.0.2/pymesomb/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 class APIException(Exception):
-  """
+    """
   Base class for REST framework exceptions.
   Subclasses should provide `.status_code` and `.default_detail` properties.
   """
-  default_detail = ''
-  default_code = 'error'
+    default_detail = ''
+    default_code = 'error'
 
-  def __init__(self, detail, code):
-    self.detail = detail or self.default_detail
-    self.code = code or self.default_code
+    def __init__(self, detail, code):
+        self.detail = detail or self.default_detail
+        self.code = code or self.default_code
 
-  def __str__(self):
-    return str(self.detail)
+    def __str__(self):
+        return str(self.detail)
 
 
 class ServiceNotFoundException(APIException):
-  pass
+    pass
 
 
 class PermissionDeniedException(APIException):
-  pass
+    pass
 
 
 class InvalidClientRequestException(APIException):
-  pass
-
+    pass
 
 
 class ServerException(APIException):
-  pass
+    pass
```

### Comparing `pymesomb-1.0.1/pymesomb/signature.py` & `pymesomb-1.0.2/pymesomb/signature.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,62 @@
-import hashlib, hmac
+import hashlib
 import hmac
 import json
-import random
-import string
 from urllib.parse import quote, urlparse
 
-from pymesomb import settings
+from pymesomb import mesomb
 
 
 class Signature:
-  @staticmethod
-  def sign_request(service, method, url, date, nonce, credentials, headers=None, body=None):
-    """
+    @staticmethod
+    def sign_request(service, method, url, date, nonce, credentials, headers=None, body=None):
+        """
     Method to use to compute signature used in MeSomb request
 
     :param service: service to use can be payment, wallet ... (the list is provide by MeSomb)
     :param method: HTTP method (GET, POST, PUT, PATCH, DELETE...)
     :param url: the full url of the request with query element https://mesomb.hachther.com/path/to/ressource?highlight=params#url-parsing
     :param date: Datetime of the request
     :param nonce: Unique string generated for each request sent to MeSomb
     :param credentials: dict containing key => value for the credential provided by MeSOmb. {'access' => access_key, 'secret' => secret_key}
     :param headers: Extra HTTP header to use in the signature
     :param body: The dict containing the body you send in your request body
     :return: Authorization to put in the header
     """
-    algorithm = settings.algorithm
-    parse = urlparse(url)
-    canonical_query = parse.query
-
-    timestamp = str(int(date.timestamp()))
+        algorithm = mesomb.algorithm
+        parse = urlparse(url)
+        canonical_query = parse.query
 
-    # CanonicalHeaders
-    if headers is None:
-      headers = {}
-    headers['host'] = '{}://{}'.format(parse.scheme, parse.netloc)
-    headers['x-mesomb-date'] = timestamp
-    headers['x-mesomb-nonce'] = nonce
-    canonical_headers = '\n'.join(['{}:{}'.format(key.lower(), headers[key].strip()) for key in sorted(headers)])
+        timestamp = str(int(date.timestamp()))
 
-    if body is None:
-      body = {}
-    request_params = json.dumps(body, separators=(',', ':'))
+        # CanonicalHeaders
+        if headers is None:
+            headers = {}
+        headers['host'] = '{}://{}'.format(parse.scheme, parse.netloc)
+        headers['x-mesomb-date'] = timestamp
+        headers['x-mesomb-nonce'] = nonce
+        canonical_headers = '\n'.join(['{}:{}'.format(key.lower(), headers[key].strip()) for key in sorted(headers)])
 
-    payload_hash = hashlib.sha1(request_params.encode('utf-8')).hexdigest()
+        if body is None:
+            body = {}
+        request_params = json.dumps(body, separators=(',', ':'))
 
-    signed_headers = ';'.join(sorted(headers))
+        payload_hash = hashlib.sha1(request_params.encode('utf-8')).hexdigest()
 
-    canonical_request = '{}\n{}\n{}\n{}\n{}\n{}'.format(method, quote(parse.path), canonical_query, canonical_headers,
-                                                        signed_headers, payload_hash)
+        signed_headers = ';'.join(sorted(headers))
 
-    scope = '{}/{}/mesomb_request'.format(date.strftime('%Y%m%d'), service)
-    string_to_sign = '{}\n{}\n{}\n{}'.format(algorithm, timestamp, scope,
-                                             hashlib.sha1(canonical_request.encode('utf-8')).hexdigest())
+        canonical_request = '{}\n{}\n{}\n{}\n{}\n{}'.format(method, quote(parse.path), canonical_query,
+                                                            canonical_headers,
+                                                            signed_headers, payload_hash)
 
-    signature = hmac.new(credentials['secret_key'].encode(), string_to_sign.encode(), hashlib.sha1).hexdigest()
+        scope = '{}/{}/mesomb_request'.format(date.strftime('%Y%m%d'), service)
+        string_to_sign = '{}\n{}\n{}\n{}'.format(algorithm, timestamp, scope,
+                                                 hashlib.sha1(canonical_request.encode('utf-8')).hexdigest())
 
-    authorization_header = '{} Credential={}/{}, SignedHeaders={}, Signature={}'.format(algorithm,
-                                                                                        credentials['access_key'], scope,
-                                                                                        signed_headers, signature)
+        signature = hmac.new(credentials['secret_key'].encode(), string_to_sign.encode(), hashlib.sha1).hexdigest()
 
-    return authorization_header
+        authorization_header = '{} Credential={}/{}, SignedHeaders={}, Signature={}'.format(algorithm,
+                                                                                            credentials['access_key'],
+                                                                                            scope,
+                                                                                            signed_headers, signature)
 
-  @staticmethod
-  def generate_nonce(length=40):
-    letters = string.ascii_letters + string.digits
-    return ''.join(random.choice(letters) for i in range(length))
+        return authorization_header
```

### Comparing `pymesomb-1.0.1/pymesomb.egg-info/PKG-INFO` & `pymesomb-1.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymesomb
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python client for MeSomb services.
 Home-page: https://github.com/hachther/mesomb-python-client.git
 Download-URL: https://pypi.org/project/pymesomb/
 Author: Hachther LLC
 Author-email: contact@hachther.com
 License: MIT
 Keywords: MeSomb,MobileMoney,OrangeMoney
@@ -39,32 +39,46 @@
 
 ## Usage
 
 ### Collect money from an account
 
 ```python
 from pymesomb.operations import PaymentOperation
-from pymesomb.signature import Signature
+from pymesomb.utils import RandomGenerator
 from datetime import datetime
 
 operation = PaymentOperation('<application_key>', '<access_key>', '<secret_key>')
-response = operation.make_collect(100, 'MTN', '677550203', datetime.now(), Signature.generate_nonce())
+response = operation.make_collect({
+    'amount': 100,
+    'service': 'MTN',
+    'payer': '670000000',
+    'date': datetime.now(),
+    'nonce': RandomGenerator.nonce(),
+    'trxID': '1'
+})
 print(response.is_operation_success())
 print(response.is_transaction_success())
 ```
 
 ### Depose money in an account
 
 ```python
 from pymesomb.operations import PaymentOperation
-from pymesomb.signature import Signature
+from pymesomb.utils import RandomGenerator
 from datetime import datetime
 
 operation = PaymentOperation('<application_key>', '<access_key>', '<secret_key>')
-response = operation.make_deposit(100, 'MTN', '677550203', datetime.now(), Signature.generate_nonce())
+response = operation.make_deposit({
+    'amount': 100,
+    'service': 'MTN',
+    'receiver': '670000000',
+    'date': datetime.now(),
+    'nonce': RandomGenerator.nonce(),
+    'trxID': '1'
+})
 print(response.is_operation_success())
 print(response.is_transaction_success())
 ```
 
 ### Get application status
 
 ```python
@@ -95,7 +109,15 @@
 * LinkedIn: [@hachther](https://linkedin.com/in/hachther)
 
 ## Show your support
 
 Give a ⭐️ if this project helped you!
 
 
+# 1.0.2 (2023-07-25)
+## === BREAKING CHANGES ===
+Only one parameter is now passed to make_deposit and make_collect. The parameter is a Map that will contain all details of your request.
+
+All method is now returning MeSomb model not dict
+
+# 1.0.0 (2022-10-20)
+First release of the module.
```

#### html2text {}

```diff
@@ -1,32 +1,37 @@
-Metadata-Version: 2.1 Name: pymesomb Version: 1.0.1 Summary: Python client for
+Metadata-Version: 2.1 Name: pymesomb Version: 1.0.2 Summary: Python client for
 MeSomb services. Home-page: https://github.com/hachther/mesomb-python-
 client.git Download-URL: https://pypi.org/project/pymesomb/ Author: Hachther
 LLC Author-email: contact@hachther.com License: MIT Keywords:
 MeSomb,MobileMoney,OrangeMoney Description-Content-Type: text/markdown License-
 File: LICENSE
                     ****** Welcome to pymesomb ð ******
 [Version] [Documentation] [License:_MIT] [Twitter:_hachther]
 > Python client for MeSomb Services > > You can check the full [documentation
 of the api here](https://mesomb.hachther.com/en/api/v1.1/schema/) ### ð 
 [Homepage](https://mesomb.com) ## Install ```sh pip3 install pymesomb ``` ##
 Usage ### Collect money from an account ```python from pymesomb.operations
-import PaymentOperation from pymesomb.signature import Signature from datetime
-import datetime operation = PaymentOperation('', '', '') response =
-operation.make_collect(100, 'MTN', '677550203', datetime.now(),
-Signature.generate_nonce()) print(response.is_operation_success()) print
-(response.is_transaction_success()) ``` ### Depose money in an account
-```python from pymesomb.operations import PaymentOperation from
-pymesomb.signature import Signature from datetime import datetime operation =
-PaymentOperation('', '', '') response = operation.make_deposit(100, 'MTN',
-'677550203', datetime.now(), Signature.generate_nonce()) print
+import PaymentOperation from pymesomb.utils import RandomGenerator from
+datetime import datetime operation = PaymentOperation('', '', '') response =
+operation.make_collect({ 'amount': 100, 'service': 'MTN', 'payer': '670000000',
+'date': datetime.now(), 'nonce': RandomGenerator.nonce(), 'trxID': '1' }) print
 (response.is_operation_success()) print(response.is_transaction_success()) ```
-### Get application status ```python from pymesomb.operations import
-PaymentOperation operation = PaymentOperation('', '', '') response =
-operation.get_status() print(response.name) ``` ### Get transactions by IDs
-```python from pymesomb.operations import PaymentOperation operation =
-PaymentOperation('', '', '') response = operation.get_transactions(['ID1',
-'ID2']) print(response) ``` ## Author ð¤ **Hachther LLC
+### Depose money in an account ```python from pymesomb.operations import
+PaymentOperation from pymesomb.utils import RandomGenerator from datetime
+import datetime operation = PaymentOperation('', '', '') response =
+operation.make_deposit({ 'amount': 100, 'service': 'MTN', 'receiver':
+'670000000', 'date': datetime.now(), 'nonce': RandomGenerator.nonce(), 'trxID':
+'1' }) print(response.is_operation_success()) print
+(response.is_transaction_success()) ``` ### Get application status ```python
+from pymesomb.operations import PaymentOperation operation = PaymentOperation
+('', '', '') response = operation.get_status() print(response.name) ``` ### Get
+transactions by IDs ```python from pymesomb.operations import PaymentOperation
+operation = PaymentOperation('', '', '') response = operation.get_transactions(
+['ID1', 'ID2']) print(response) ``` ## Author ð¤ **Hachther LLC
 hachther.com>** * Website: https://www.hachther.com * Twitter: [@hachther]
 (https://twitter.com/hachther) * Github: [@hachther](https://github.com/
 hachther) * LinkedIn: [@hachther](https://linkedin.com/in/hachther) ## Show
-your support Give a â­ï¸ if this project helped you!
+your support Give a â­ï¸ if this project helped you! # 1.0.2 (2023-07-25) ##
+=== BREAKING CHANGES === Only one parameter is now passed to make_deposit and
+make_collect. The parameter is a Map that will contain all details of your
+request. All method is now returning MeSomb model not dict # 1.0.0 (2022-10-20)
+First release of the module.
```

### Comparing `pymesomb-1.0.1/setup.py` & `pymesomb-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='pymesomb',
-    version='1.0.1',
+    version='1.0.2',
     description='Python client for MeSomb services.',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Hachther LLC',
     author_email='contact@hachther.com',
```

