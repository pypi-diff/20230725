# Comparing `tmp/evervault-2.2.0.tar.gz` & `tmp/evervault-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evervault-2.2.0.tar", max compression
+gzip compressed data, was "evervault-3.0.0.tar", max compression
```

## Comparing `evervault-2.2.0.tar` & `evervault-3.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1109 2023-03-14 17:26:12.028969 evervault-2.2.0/LICENSE
--rw-r--r--   0        0        0     8691 2023-03-14 17:26:12.028969 evervault-2.2.0/README.md
--rw-r--r--   0        0        0     5088 2023-03-14 17:29:21.140044 evervault-2.2.0/evervault/__init__.py
--rw-r--r--   0        0        0     3891 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/cages_v2.py
--rw-r--r--   0        0        0     3800 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/client.py
--rw-r--r--   0        0        0       55 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/crypto/__init__.py
--rw-r--r--   0        0        0     8278 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/crypto/client.py
--rw-r--r--   0        0        0       58 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/crypto/curves/__init__.py
--rw-r--r--   0        0        0     3428 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/crypto/curves/base.py
--rw-r--r--   0        0        0      779 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/crypto/curves/p256.py
--rw-r--r--   0        0        0       71 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/crypto/version.py
--rw-r--r--   0        0        0      112 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/datatypes/__init__.py
--rw-r--r--   0        0        0      376 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/datatypes/map.py
--rw-r--r--   0        0        0       43 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/errors/__init__.py
--rw-r--r--   0        0        0     1816 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/errors/error_handler.py
--rw-r--r--   0        0        0     1194 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/errors/evervault_errors.py
--rw-r--r--   0        0        0       37 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/http/__init__.py
--rw-r--r--   0        0        0     2260 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/http/outboundrelayconfig.py
--rw-r--r--   0        0        0     3087 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/http/request.py
--rw-r--r--   0        0        0     1201 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/http/requesthandler.py
--rw-r--r--   0        0        0     8546 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/http/requestintercept.py
--rw-r--r--   0        0        0       73 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/models/__init__.py
--rw-r--r--   0        0        0      315 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/models/cage.py
--rw-r--r--   0        0        0      392 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/models/cage_list.py
--rw-r--r--   0        0        0        0 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/services/__init__.py
--rw-r--r--   0        0        0      136 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/services/timeservice.py
--rw-r--r--   0        0        0     1143 2023-03-14 17:26:12.028969 evervault-2.2.0/evervault/threading/repeatedtimer.py
--rw-r--r--   0        0        0     1086 2023-03-14 17:29:21.148044 evervault-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     9622 1970-01-01 00:00:00.000000 evervault-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-05-25 15:56:34.253287 evervault-3.0.0/LICENSE
+-rw-r--r--   0        0        0     9598 2023-07-21 12:11:23.147023 evervault-3.0.0/README.md
+-rw-r--r--   0        0        0     5424 2023-07-25 11:03:54.075017 evervault-3.0.0/evervault/__init__.py
+-rw-r--r--   0        0        0     4126 2023-05-25 15:56:34.253794 evervault-3.0.0/evervault/cages_v2.py
+-rw-r--r--   0        0        0     4795 2023-07-21 12:11:23.147444 evervault-3.0.0/evervault/client.py
+-rw-r--r--   0        0        0       55 2023-05-25 15:56:34.254073 evervault-3.0.0/evervault/crypto/__init__.py
+-rw-r--r--   0        0        0     8468 2023-07-21 12:11:23.148512 evervault-3.0.0/evervault/crypto/client.py
+-rw-r--r--   0        0        0       58 2023-05-25 15:56:34.254370 evervault-3.0.0/evervault/crypto/curves/__init__.py
+-rw-r--r--   0        0        0     3428 2023-05-25 15:56:34.254522 evervault-3.0.0/evervault/crypto/curves/base.py
+-rw-r--r--   0        0        0      779 2023-05-25 15:56:34.254660 evervault-3.0.0/evervault/crypto/curves/p256.py
+-rw-r--r--   0        0        0       71 2023-05-25 15:56:34.254779 evervault-3.0.0/evervault/crypto/version.py
+-rw-r--r--   0        0        0      112 2023-05-25 15:56:34.254938 evervault-3.0.0/evervault/datatypes/__init__.py
+-rw-r--r--   0        0        0      376 2023-05-25 15:56:34.255055 evervault-3.0.0/evervault/datatypes/map.py
+-rw-r--r--   0        0        0       43 2023-05-25 15:56:34.255199 evervault-3.0.0/evervault/errors/__init__.py
+-rw-r--r--   0        0        0     1816 2023-05-25 15:56:34.255323 evervault-3.0.0/evervault/errors/error_handler.py
+-rw-r--r--   0        0        0     1194 2023-05-25 15:56:34.255426 evervault-3.0.0/evervault/errors/evervault_errors.py
+-rw-r--r--   0        0        0       37 2023-05-25 15:56:34.255561 evervault-3.0.0/evervault/http/__init__.py
+-rw-r--r--   0        0        0     2260 2023-05-25 15:56:34.255678 evervault-3.0.0/evervault/http/outboundrelayconfig.py
+-rw-r--r--   0        0        0     3926 2023-07-21 12:11:23.148904 evervault-3.0.0/evervault/http/request.py
+-rw-r--r--   0        0        0     1201 2023-05-25 15:56:34.255939 evervault-3.0.0/evervault/http/requesthandler.py
+-rw-r--r--   0        0        0     8546 2023-05-25 15:56:34.256091 evervault-3.0.0/evervault/http/requestintercept.py
+-rw-r--r--   0        0        0       73 2023-05-25 15:56:34.256292 evervault-3.0.0/evervault/models/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-25 15:56:34.256396 evervault-3.0.0/evervault/models/cage.py
+-rw-r--r--   0        0        0      392 2023-05-25 15:56:34.256485 evervault-3.0.0/evervault/models/cage_list.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:56:34.256570 evervault-3.0.0/evervault/services/__init__.py
+-rw-r--r--   0        0        0      136 2023-05-25 15:56:34.256663 evervault-3.0.0/evervault/services/timeservice.py
+-rw-r--r--   0        0        0     1143 2023-05-25 15:56:34.256806 evervault-3.0.0/evervault/threading/repeatedtimer.py
+-rw-r--r--   0        0        0     1076 2023-07-25 10:50:58.265829 evervault-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10527 1970-01-01 00:00:00.000000 evervault-3.0.0/PKG-INFO
```

### Comparing `evervault-2.2.0/LICENSE` & `evervault-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evervault-2.2.0/README.md` & `evervault-3.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -29,23 +29,26 @@
 ## Setup
 
 To make Evervault available for use in your app:
 
 ```python
 import evervault
 
-# Initialize the client with your team’s API key
-evervault.init("<YOUR_API_KEY>")
+# Initialize the client with your App's ID and App’s API key
+evervault.init("<APP_ID>", "<YOUR_API_KEY>")
 
 # Encrypt your data
 encrypted = evervault.encrypt({ "name": "Claude" })
 
 # Process the encrypted data in a Function
 result = evervault.run("<YOUR_FUNCTION_NAME>", encrypted)
 
+# Decrypt data
+result = evervault.decrypt(encrypted)
+
 # Send the decrypted data to a third-party API
 evervault.enable_outbound_relay()
 requests.post("https://example.com", json = encrypted)
 
 # Send attested requests to a Cage
 attested_session = evervault.cage_requests_session({ 'my-cage': { 'pcr_8': '...' } })
 # Attested TLS directly to the enclave
@@ -57,37 +60,52 @@
 The Evervault Python SDK exposes five functions.
 
 ### evervault.init()
 
 `evervault.init()` initializes the SDK with your API key. Configurations for the interception of outbound requests may also be passed in this function.
 
 ```python
-evervault.init(api_key = str[, decryption_domains=[], retry = bool, curve = str])
+evervault.init(app_id = str, api_key = str[, decryption_domains=[], retry = bool, curve = str])
 ```
 
 | Parameter | Type  | Description                                                                                                                                                    |
 | --------- | ----- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| api_key   | `str` | The API key of your Evervault Team                                                                                                                             |
+| app_id   | `str` | The ID of your Evervault App |
+| api_key   | `str` | The API key of your Evervault App |
 | curve     | `str` | The elliptic curve used for cryptographic operations. See [Elliptic Curve Support](https://docs.evervault.com/reference/elliptic-curve-support) to learn more. |
 
 ### evervault.encrypt()
 
 `evervault.encrypt()` encrypts data for use in your [Functions](https://docs.evervault.com/tutorial). To encrypt data at the server, simply pass a python primitive type into the `evervault.encrypt()` function. Store the encrypted data in your database as normal.
 
 ```python
 evervault.encrypt(data = dict | list | set | str | int | bool)
 ```
 
 | Parameter | Type                                        | Description          |
 | --------- | ------------------------------------------- | -------------------- |
 | data      | `dict`, `list`, `set`, `str`, `int`, `bool` | Data to be encrypted |
 
+### evervault.decrypt()
+
+`evervault.decrypt()` decrypts data previously encrypted with the `encrypt()` function or through Evervault's Relay (Evervault's encryption proxy).
+An API Key with the `decrypt` permission must be used to perform this operation.
+
+```python
+evervault.decrypt(data =  str | dict | list | bytes | bytearray)
+```
+
+| Parameter | Type                                        | Description          |
+| --------- | ------------------------------------------- |--------------------- |
+| data      | `str`, `dict`, `list`, `bytes`, `bytearray` | Data to be decrypted |
+
 ### evervault.run()
 
 `evervault.run()` invokes a Function with a given payload.
+An API Key with the `run function` permission must be used to perform this operation.
 
 ```python
 evervault.run(function_name = str, data = dict[, options = dict])
 ```
 
 | Parameter     | Type   | Description                                            |
 | ------------- | ------ | ------------------------------------------------------ |
@@ -101,14 +119,15 @@
 | ------- | --------- | ------- | ---------------------------------------------------------------------------------------- |
 | async   | `Boolean` | `False` | Run your Function in async mode. Async Function runs will be queued for processing.      |
 | version | `Integer` | `None`  | Specify the version of your Function to run. By default, the latest version will be run. |
 
 ### evervault.create_run_token()
 
 `evervault.create_run_token()` creates a single use, time bound token for invoking a function.
+An API Key with the `create Run Token` permission must be used to perform this operation.
 
 ```python
 evervault.create_run_token(function_name = str, data = dict)
 ```
 
 | Parameter     | Type   | Description                                               |
 | ------------- | ------ | --------------------------------------------------------- |
@@ -134,17 +153,17 @@
 
 `evervault.cage_requests_session()` creates a `requests` `Session` which attests all traffic between your client and the Cage. You can provide the PCRs generated at build time to have even tighter control on the attestation.
 
 ```python
 evervault.cage_requests_session([cage_attestation_data = dict])
 ```
 
-| Parameter             | Type   | Default | Description                                                                                                                                                                                          |
-| --------------------- | ------ | ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| cage_attestation_data | `dict` | `None`  | Provide attestation measures to make assertions about the code running within your enclave. The `cage_attestation_data` dict is a mapping of cage names to their corresponding attestation measures. |
+| Parameter             | Type           | Default | Description                                                                                                                                                                                          |
+| --------------------- | -------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| cage_attestation_data | `dict`, `list` | `None`  | Provide attestation measures to make assertions about the code running within your enclave. The `cage_attestation_data` dict is a mapping of cage names to their corresponding attestation measures. A list of dicts can also be used passed, if you want to allow roll-over between different sets of PCRs |
 
 ## Contributing
 
 Bug reports and pull requests are welcome on GitHub at https://github.com/evervault/evervault-python.
 
 ## Feedback
```

### Comparing `evervault-2.2.0/evervault/__init__.py` & `evervault-3.0.0/evervault/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from .client import Client
 from .errors.evervault_errors import AuthenticationError, UnsupportedCurveError
 from .cages_v2 import CageRequestsSession
 import os
 import sys
 from warnings import warn
 
-__version__ = "2.2.0"
+__version__ = "3.0.0"
 
 ev_client = None
+_app_uuid = None
 _api_key = None
 request_timeout = 30
 _retry = False
 _curve = None
 
 BASE_URL_DEFAULT = "https://api.evervault.com/"
 BASE_RUN_URL_DEFAULT = "https://run.evervault.com/"
@@ -27,27 +28,30 @@
 
 class Curves(object):
     SECP256K1 = "SECP256K1"
     SECP256R1 = "SECP256R1"
 
 
 def init(
+    app_id,
     api_key,
     decryption_domains=[],
     intercept=False,
     ignore_domains=[],
     retry=False,
     curve=Curves.SECP256K1,
     debug_requests=False,
     enable_outbound_relay=False,
 ):
+    global _app_uuid
     global _api_key
     global _retry
     global _curve
 
+    _app_uuid = app_id
     _api_key = api_key
     _retry = retry
     _curve = curve
 
     if intercept or len(ignore_domains) > 0 or len(decryption_domains) > 0:
         warn(
             """
@@ -73,14 +77,18 @@
         )
 
 
 def run(function_name, data, options={"async": False, "version": None}):
     return __client().run(function_name, data, options)
 
 
+def decrypt(data):
+    return __client().decrypt(data)
+
+
 def encrypt(data):
     return __client().encrypt(data)
 
 
 def encrypt_and_run(cage_name, data, options={"async": False, "version": None}):
     warn(
         "The `encrypt_and_run` method is deprecated and slated for removal. Please use the `encrypt` and `run` methods instead.",
@@ -131,27 +139,32 @@
     if sys.version_info.minor < 11:
         warn(
             "Using Outbound Relay with Asynchronous Python is only supported in Python >= 3.11"
         )
 
 
 def __client():
+    if not _app_uuid:
+        raise AuthenticationError(
+            "Your App's App UUID must be entered using evervault.init('<APP-ID>', '<API-KEY>')"
+        )
     if not _api_key:
         raise AuthenticationError(
-            "Your Team's API Key must be entered using evervault.init('<API-KEY>')"
+            "Your App's API Key must be entered using evervault.init('<APP-ID>', '<API-KEY>')"
         )
     if _curve not in SUPPORTED_CURVES:
         raise UnsupportedCurveError(f"The {_curve} curve is not supported.")
     global ev_client
     if not ev_client:
         max_file_size_in_mb = int(
             os.environ.get("EV_MAX_FILE_SIZE_IN_MB", MAX_FILE_SIZE_IN_MB_DEFAULT)
         )
         ev_client = Client(
             api_key=_api_key,
+            app_uuid=_app_uuid,
             request_timeout=request_timeout,
             base_url=os.environ.get("EV_API_URL", BASE_URL_DEFAULT),
             base_run_url=os.environ.get("EV_CAGE_RUN_URL", BASE_RUN_URL_DEFAULT),
             relay_url=os.environ.get("EV_TUNNEL_HOSTNAME", RELAY_URL_DEFAULT),
             ca_host=os.environ.get("EV_CERT_HOSTNAME", CA_HOST_DEFAULT),
             retry=_retry,
             curve=_curve,
```

### Comparing `evervault-2.2.0/evervault/cages_v2.py` & `evervault-3.0.0/evervault/cages_v2.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,23 +34,31 @@
         if self.cages_host in url:
             cage_name = get_cage_name_from_cage(url)
             # we patch the urllib3.connectionpool.HTTPSConnectionPool object to perform extra validation on its connection before transmitting any data
             conn = self.add_attestation_check_to_conn_validation(conn, cage_name)
         return conn
 
     def add_attestation_check_to_conn_validation(self, conn, cage_name):
-        expected_pcrs = evervault_attestation_bindings.PCRs.empty()
+        expected_pcrs = []
         if cage_name in self.attestation_data:
             given_pcrs = self.attestation_data[cage_name]
-            expected_pcrs = evervault_attestation_bindings.PCRs(
-                given_pcrs.get("pcr_0"),
-                given_pcrs.get("pcr_1"),
-                given_pcrs.get("pcr_2"),
-                given_pcrs.get("pcr_8"),
-            )
+            # if the user only supplied a single set of PCRs, convert it to a list
+            if not isinstance(given_pcrs, list):
+                given_pcrs = [given_pcrs]
+
+            for pcrs in given_pcrs:
+                expected_pcrs.append(
+                    evervault_attestation_bindings.PCRs(
+                        pcrs.get("pcr_0"),
+                        pcrs.get("pcr_1"),
+                        pcrs.get("pcr_2"),
+                        pcrs.get("pcr_8"),
+                    )
+                )
+
         original_validate_conn = (
             urllib3.connectionpool.HTTPSConnectionPool._validate_conn
         )
 
         def _validate_conn_override(self, conn):
             conn.connect()
             cert = conn.sock.getpeercert(binary_form=True)
```

### Comparing `evervault-2.2.0/evervault/client.py` & `evervault-3.0.0/evervault/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from .http.requestintercept import RequestIntercept
 from .http.requesthandler import RequestHandler
 from .http.request import Request
 from .crypto.client import Client as CryptoClient
 from .models.cage_list import CageList
 from .datatypes.map import ensure_is_integer
 from .services.timeservice import TimeService
+from .errors.evervault_errors import UndefinedDataError, DecryptionError
 
 
 class Client(object):
     def __init__(
         self,
+        app_uuid=None,
         api_key=None,
         request_timeout=30,
         base_url="https://api.evervault.com/",
         base_run_url="https://run.evervault.com/",
         relay_url="https://relay.evervault.com:443",
         ca_host="https://ca.evervault.com",
         retry=False,
         curve="SECP256K1",
         max_file_size_in_mb=25,
     ):
+        self.app_uuid = app_uuid
         self.api_key = api_key
         self.base_url = base_url
         self.base_run_url = base_run_url
         self.relay_url = relay_url
         self.ca_host = ca_host
-        request = Request(self.api_key, request_timeout, retry)
+        request = Request(self.app_uuid, self.api_key, request_timeout, retry)
         time_service = TimeService()
         self.cert = RequestIntercept(
             request, ca_host, base_run_url, base_url, api_key, relay_url, time_service
         )
         self.request_handler = RequestHandler(
             request, base_run_url, base_url, self.cert
         )
@@ -38,14 +41,30 @@
     @property
     def _auth(self):
         return (self.api_key, "")
 
     def encrypt(self, data):
         return self.crypto_client.encrypt_data(self, data)
 
+    def decrypt(self, data):
+        if data is None:
+            raise UndefinedDataError("Data is not defined")
+        elif not isinstance(data, (str, dict, list, bytes)):
+            raise DecryptionError(
+                "data must be of type `str`, `dict`, `list` or `bytes`"
+            )
+        headers = self.__build_decrypt_headers(type(data))
+
+        if type(data) == bytes:
+            return self.post("decrypt", data, headers, False)
+        else:
+            payload = {"data": data}
+            response = self.post("decrypt", payload, headers, False)
+            return response["data"]
+
     def run(self, cage_name, data, options={"async": False, "version": None}):
         optional_headers = self.__build_cage_run_headers(options)
         return self.post(cage_name, data, optional_headers, True)
 
     def encrypt_and_run(
         self, cage_name, data, options={"async": False, "version": None}
     ):
@@ -87,14 +106,21 @@
 
     def put(self, path, params):
         return self.request_handler.put(path, params).parsed_body
 
     def delete(self, path, params):
         return self.request_handler.delete(path, params).parsed_body
 
+    def __build_decrypt_headers(self, data_type):
+        headers = {}
+        headers["Content-Type"] = "application/json"
+        if data_type == bytes:
+            headers["Content-Type"] = "application/octet-stream"
+        return headers
+
     def __build_cage_run_headers(self, options):
         if options is None:
             return {}
         cage_run_headers = {}
         if "async" in options:
             if options["async"]:
                 cage_run_headers["x-async"] = "true"
```

### Comparing `evervault-2.2.0/evervault/crypto/client.py` & `evervault-3.0.0/evervault/crypto/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from cryptography.hazmat.primitives.asymmetric.ec import EllipticCurvePublicKey
 from cryptography.hazmat.primitives.serialization import Encoding, PublicFormat
 from cryptography.hazmat.primitives.ciphers.aead import AESGCM
 from cryptography.hazmat.primitives import hashes
 from secrets import token_bytes
 import base64
 import time
+import binascii
 from .version import VERSION
 from .curves.p256 import P256PublicKey
 
 BS = 32
 KEY_INTERVAL = 15
 
 SECP256R1 = "SECP256R1"
@@ -136,40 +137,45 @@
             iv,
             self.compressed_public_key,
             encrypted_bytes,
         )
 
     def __coerce_type(self, data):
         if type(data) == bool:
-            return str(int(data))
+            return "true" if data else "false"
         elif type(data) == int or type(data) == float:
             return str(data)
         else:
             return data
 
     def __format(self, header, iv, public_key, encrypted_payload):
         prefix = f":{header}" if header != "string" else ""
         return f"ev:{self.ev_version}{prefix}:{self.__base_64_remove_padding(iv)}:{self.__base_64_remove_padding(public_key)}:{self.__base_64_remove_padding(encrypted_payload)}:$"
 
     def __format_file(self, iv, public_key, encrypted_bytes):
         encrypted_file_identifier = bytes(b"\x25\x45\x56\x45\x4e\x43")
-        verion_number = bytes(b"\00") if self.curve == SECP256K1 else bytes(b"\01")
+        verion_number = bytes(b"\02") if self.curve == SECP256K1 else bytes(b"\03")
         offset_to_data = bytes([55, 00])
         flags = bytes(b"\00")
 
-        return (
+        file_bytes = (
             encrypted_file_identifier
             + verion_number
             + offset_to_data
             + bytes(public_key)
             + bytes(iv)
             + flags
             + bytes(encrypted_bytes)
         )
 
+        file_crc32 = binascii.crc32(file_bytes)
+        crc32_bytes = file_crc32.to_bytes(4, byteorder="little")
+
+        return file_bytes + crc32_bytes
+
     def __base_64_remove_padding(self, data):
         return data.rstrip("=")
 
     def __encryptable_data(self, data):
         return data is not None and (
             type(data) == str
             or type(data) == bool
```

### Comparing `evervault-2.2.0/evervault/crypto/curves/base.py` & `evervault-3.0.0/evervault/crypto/curves/base.py`

 * *Files identical despite different names*

### Comparing `evervault-2.2.0/evervault/crypto/curves/p256.py` & `evervault-3.0.0/evervault/crypto/curves/p256.py`

 * *Files identical despite different names*

### Comparing `evervault-2.2.0/evervault/errors/error_handler.py` & `evervault-3.0.0/evervault/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `evervault-2.2.0/evervault/errors/evervault_errors.py` & `evervault-3.0.0/evervault/errors/evervault_errors.py`

 * *Files identical despite different names*

### Comparing `evervault-2.2.0/evervault/http/outboundrelayconfig.py` & `evervault-3.0.0/evervault/http/outboundrelayconfig.py`

 * *Files identical despite different names*

### Comparing `evervault-2.2.0/evervault/http/request.py` & `evervault-3.0.0/evervault/http/request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,93 @@
 from ..errors import error_handler
 import json
 import requests
 import certifi
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
+import base64
 
 retry_strategy = Retry(
     total=3,
     status_forcelist=[429, 500, 502, 503, 504],
     allowed_methods=["HEAD", "GET", "OPTIONS", "POST", "PUT"],
     backoff_factor=1,
 )
 adapter = HTTPAdapter(max_retries=retry_strategy)
 
 
 class Request(object):
-    def __init__(self, api_key, timeout=30, retry=False):
+    decrypt_path = "/decrypt"
+
+    def __init__(self, app_uuid, api_key, timeout=30, retry=False):
         self.http_session = requests.Session()
         self.timeout = timeout
+        self.app_uuid = app_uuid
         self.api_key = api_key
         self.retry = retry
 
     def make_request(self, method, url, params=None, optional_headers={}, _is_ca=False):
         """
         Make a request.
 
         Keyword arguments:
         params -- The parameters of the request (default None)
         optional_headers -- Optional headers for the request (default {})
         _is_ca -- If the request is for a certificate don't parse the response body (default False)
         """
         from evervault import __version__
 
-        req_params = self.__build_headers(method, params, optional_headers, __version__)
+        req_params = self.__build_headers(
+            method, params, url, optional_headers, __version__
+        )
 
         request_object = requests if self.http_session is None else self.http_session
         if self.retry:
             request_object.mount("https://", adapter)
             request_object.mount("http://", adapter)
         resp = self.__execute_request(request_object, method, url, req_params)
         if _is_ca:
             error_handler.raise_errors_on_failure(resp, resp.content)
             return resp
         else:
-            parsed_body = self.__parse_body(resp)
+            should_parse = (
+                req_params["headers"]
+                and req_params["headers"]["Content-Type"] != "application/octet-stream"
+            )
+            parsed_body = self.__parse_body(resp, should_parse)
             error_handler.raise_errors_on_failure(resp, parsed_body)
             resp.parsed_body = parsed_body
             return resp
 
-    def __build_headers(self, method, params, optional_headers, version):
+    def __build_headers(self, method, params, url, optional_headers, version):
         req_params = {}
+
         headers = {
             "User-Agent": "evervault-python/" + version,
             "Accept-Encoding": "gzip, deflate",
             "Accept": "application/json",
             "Content-Type": "application/json",
-            "Api-Key": self.api_key,
         }
+
+        # Set correct auth header
+        if Request.decrypt_path in url:
+            auth_value = f"{self.app_uuid}:{self.api_key}"
+            encoded_auth_value_bytes = base64.b64encode(auth_value.encode("ascii"))
+            basic_auth_str = f"Basic {encoded_auth_value_bytes.decode('utf-8')}"
+            headers["Authorization"] = basic_auth_str
+        else:
+            headers["Api-Key"] = self.api_key
+
         headers.update(optional_headers)
         if method in ("POST", "PUT", "DELETE"):
-            req_params["data"] = json.dumps(params, cls=json.JSONEncoder)
+            if type(params) == bytes:
+                req_params["data"] = params
+            else:
+                req_params["data"] = json.dumps(params, cls=json.JSONEncoder)
+
         elif method == "GET":
             req_params["params"] = params
 
         req_params["headers"] = headers
         return req_params
 
     def __execute_request(self, request_object, method, url, req_params):
@@ -72,16 +96,16 @@
             url,
             timeout=self.timeout,
             verify=certifi.where(),
             allow_redirects=False,
             **req_params,
         )
 
-    def __parse_body(self, resp):
+    def __parse_body(self, resp, should_parse=True):
         if resp.content and resp.content.strip():
             try:
                 decoded_body = resp.content.decode(
                     resp.encoding or resp.apparent_encoding
                 )
-                return json.loads(decoded_body)
+                return json.loads(decoded_body) if should_parse else decoded_body
             except ValueError:
                 error_handler.raise_errors_on_failure(resp)
```

### Comparing `evervault-2.2.0/evervault/http/requesthandler.py` & `evervault-3.0.0/evervault/http/requesthandler.py`

 * *Files identical despite different names*

### Comparing `evervault-2.2.0/evervault/http/requestintercept.py` & `evervault-3.0.0/evervault/http/requestintercept.py`

 * *Files identical despite different names*

### Comparing `evervault-2.2.0/evervault/threading/repeatedtimer.py` & `evervault-3.0.0/evervault/threading/repeatedtimer.py`

 * *Files identical despite different names*

### Comparing `evervault-2.2.0/pyproject.toml` & `evervault-3.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [tool.poetry]
 name = "evervault"
-version = "2.2.0"
+version = "3.0.0"
 description = "Evervault SDK"
 authors = ["Evervault <engineering@evervault.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://evervault.com"
 repository = "https://github.com/evervault/evervault-python"
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.7.0"
 requests = "^2.24.0"
-cryptography = "^39.0.1"
+cryptography = "^41.0.0"
 certifi = "*"
 pycryptodome = "^3.10.1"
 pyasn1 = "^0.4.8"
-evervault-attestation-bindings = "0.1.0a5"
+evervault-attestation-bindings = "0.2.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-socket = "^0.4.1"
 requests-mock = "^1.9.3"
 python-semantic-release = "^7.19.2"
-flake8 = "^3.9.2"
-black = "^21.8b0"
+flake8 = "^5.0.4"
+black = "^22.3.0"
 
 [pytest]
 testpath = "tests"
 
 [tool.black]
 line-length = 88
-target-version = ['py36', 'py37', 'py38', 'py39']
+target-version = ['py37', 'py38', 'py39']
 
 [tool.semantic_release]
 version_variable = [ "evervault/__init__.py:__version__" ]
 version_toml = [ "pyproject.toml:tool.poetry.version" ]
 major_on_zero = true
 branch = "master"
 upload_to_pypi = true
```

### Comparing `evervault-2.2.0/PKG-INFO` & `evervault-3.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: evervault
-Version: 2.2.0
+Version: 3.0.0
 Summary: Evervault SDK
 Home-page: https://evervault.com
 License: MIT
 Author: Evervault
 Author-email: engineering@evervault.com
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.7.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certifi
-Requires-Dist: cryptography (>=39.0.1,<40.0.0)
-Requires-Dist: evervault-attestation-bindings (==0.1.0a5)
+Requires-Dist: cryptography (>=41.0.0,<42.0.0)
+Requires-Dist: evervault-attestation-bindings (==0.2.0)
 Requires-Dist: pyasn1 (>=0.4.8,<0.5.0)
 Requires-Dist: pycryptodome (>=3.10.1,<4.0.0)
 Requires-Dist: requests (>=2.24.0,<3.0.0)
 Project-URL: Repository, https://github.com/evervault/evervault-python
 Description-Content-Type: text/markdown
 
 [![Evervault](https://evervault.com/evervault.svg)](https://evervault.com/)
@@ -54,23 +54,26 @@
 ## Setup
 
 To make Evervault available for use in your app:
 
 ```python
 import evervault
 
-# Initialize the client with your team’s API key
-evervault.init("<YOUR_API_KEY>")
+# Initialize the client with your App's ID and App’s API key
+evervault.init("<APP_ID>", "<YOUR_API_KEY>")
 
 # Encrypt your data
 encrypted = evervault.encrypt({ "name": "Claude" })
 
 # Process the encrypted data in a Function
 result = evervault.run("<YOUR_FUNCTION_NAME>", encrypted)
 
+# Decrypt data
+result = evervault.decrypt(encrypted)
+
 # Send the decrypted data to a third-party API
 evervault.enable_outbound_relay()
 requests.post("https://example.com", json = encrypted)
 
 # Send attested requests to a Cage
 attested_session = evervault.cage_requests_session({ 'my-cage': { 'pcr_8': '...' } })
 # Attested TLS directly to the enclave
@@ -82,37 +85,52 @@
 The Evervault Python SDK exposes five functions.
 
 ### evervault.init()
 
 `evervault.init()` initializes the SDK with your API key. Configurations for the interception of outbound requests may also be passed in this function.
 
 ```python
-evervault.init(api_key = str[, decryption_domains=[], retry = bool, curve = str])
+evervault.init(app_id = str, api_key = str[, decryption_domains=[], retry = bool, curve = str])
 ```
 
 | Parameter | Type  | Description                                                                                                                                                    |
 | --------- | ----- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| api_key   | `str` | The API key of your Evervault Team                                                                                                                             |
+| app_id   | `str` | The ID of your Evervault App |
+| api_key   | `str` | The API key of your Evervault App |
 | curve     | `str` | The elliptic curve used for cryptographic operations. See [Elliptic Curve Support](https://docs.evervault.com/reference/elliptic-curve-support) to learn more. |
 
 ### evervault.encrypt()
 
 `evervault.encrypt()` encrypts data for use in your [Functions](https://docs.evervault.com/tutorial). To encrypt data at the server, simply pass a python primitive type into the `evervault.encrypt()` function. Store the encrypted data in your database as normal.
 
 ```python
 evervault.encrypt(data = dict | list | set | str | int | bool)
 ```
 
 | Parameter | Type                                        | Description          |
 | --------- | ------------------------------------------- | -------------------- |
 | data      | `dict`, `list`, `set`, `str`, `int`, `bool` | Data to be encrypted |
 
+### evervault.decrypt()
+
+`evervault.decrypt()` decrypts data previously encrypted with the `encrypt()` function or through Evervault's Relay (Evervault's encryption proxy).
+An API Key with the `decrypt` permission must be used to perform this operation.
+
+```python
+evervault.decrypt(data =  str | dict | list | bytes | bytearray)
+```
+
+| Parameter | Type                                        | Description          |
+| --------- | ------------------------------------------- |--------------------- |
+| data      | `str`, `dict`, `list`, `bytes`, `bytearray` | Data to be decrypted |
+
 ### evervault.run()
 
 `evervault.run()` invokes a Function with a given payload.
+An API Key with the `run function` permission must be used to perform this operation.
 
 ```python
 evervault.run(function_name = str, data = dict[, options = dict])
 ```
 
 | Parameter     | Type   | Description                                            |
 | ------------- | ------ | ------------------------------------------------------ |
@@ -126,14 +144,15 @@
 | ------- | --------- | ------- | ---------------------------------------------------------------------------------------- |
 | async   | `Boolean` | `False` | Run your Function in async mode. Async Function runs will be queued for processing.      |
 | version | `Integer` | `None`  | Specify the version of your Function to run. By default, the latest version will be run. |
 
 ### evervault.create_run_token()
 
 `evervault.create_run_token()` creates a single use, time bound token for invoking a function.
+An API Key with the `create Run Token` permission must be used to perform this operation.
 
 ```python
 evervault.create_run_token(function_name = str, data = dict)
 ```
 
 | Parameter     | Type   | Description                                               |
 | ------------- | ------ | --------------------------------------------------------- |
@@ -159,17 +178,17 @@
 
 `evervault.cage_requests_session()` creates a `requests` `Session` which attests all traffic between your client and the Cage. You can provide the PCRs generated at build time to have even tighter control on the attestation.
 
 ```python
 evervault.cage_requests_session([cage_attestation_data = dict])
 ```
 
-| Parameter             | Type   | Default | Description                                                                                                                                                                                          |
-| --------------------- | ------ | ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| cage_attestation_data | `dict` | `None`  | Provide attestation measures to make assertions about the code running within your enclave. The `cage_attestation_data` dict is a mapping of cage names to their corresponding attestation measures. |
+| Parameter             | Type           | Default | Description                                                                                                                                                                                          |
+| --------------------- | -------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| cage_attestation_data | `dict`, `list` | `None`  | Provide attestation measures to make assertions about the code running within your enclave. The `cage_attestation_data` dict is a mapping of cage names to their corresponding attestation measures. A list of dicts can also be used passed, if you want to allow roll-over between different sets of PCRs |
 
 ## Contributing
 
 Bug reports and pull requests are welcome on GitHub at https://github.com/evervault/evervault-python.
 
 ## Feedback
```

