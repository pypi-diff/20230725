# Comparing `tmp/py-aws-lambda-toolkit-0.0.3.tar.gz` & `tmp/py-aws-lambda-toolkit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-aws-lambda-toolkit-0.0.3.tar", last modified: Fri Jul  7 19:16:43 2023, max compression
+gzip compressed data, was "py-aws-lambda-toolkit-0.0.4.tar", last modified: Tue Jul 25 17:34:12 2023, max compression
```

## Comparing `py-aws-lambda-toolkit-0.0.3.tar` & `py-aws-lambda-toolkit-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:43.799565 py-aws-lambda-toolkit-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-07 19:16:43.799565 py-aws-lambda-toolkit-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:43.799565 py-aws-lambda-toolkit-0.0.3/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_http_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_http_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/__tests__/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:43.799565 py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-07 19:16:43.000000 py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-07 19:16:43.000000 py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:16:43.000000 py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-07 19:16:43.000000 py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-07 19:16:43.000000 py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:43.799565 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/dynamodb_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/scan_filter_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-07 19:16:33.000000 py-aws-lambda-toolkit-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-07 19:16:43.803566 py-aws-lambda-toolkit-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:34:12.963975 py-aws-lambda-toolkit-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-25 17:34:12.963975 py-aws-lambda-toolkit-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:34:12.959975 py-aws-lambda-toolkit-0.0.4/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_http_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_http_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:34:12.963975 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/dynamodb_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/http_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/http_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/scan_filter_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:34:12.963975 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-25 17:34:12.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-25 17:34:12.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:34:12.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 17:34:12.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-25 17:34:12.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-25 17:34:12.963975 py-aws-lambda-toolkit-0.0.4/setup.cfg
```

### Comparing `py-aws-lambda-toolkit-0.0.3/LICENSE` & `py-aws-lambda-toolkit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.3/PKG-INFO` & `py-aws-lambda-toolkit-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: py-aws-lambda-toolkit
-Version: 0.0.3
+Version: 0.0.4
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
-Home-page: https://github.com/0riion/py-sls-lambda-toolkit
+Home-page: https://github.com/0riion/py-aws-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
-Keywords: aws,serverless,lambda,dynamodb,toolkit,python,sls
+Keywords: aws,serverless,lambda,dynamodb,toolkit,python,aws
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Py SLS Lambda Toolkit
+# Py aws Lambda Toolkit
 
 This is a lightweight Python toolkit for easily and quickly creating AWS Lambda functions with the Serverless Framework. It includes the following features:
 
 - DynamoDB shortcuts: Avoid boilerplate code for DynamoDB operations.
 - HTTP event processing: Get the event of the HTTP request and parse it, splitting it into the path, query string, body, headers, etc.
 - HTTP response shortcuts: Create HTTP responses with the correct format and status code.
 - JWT authentication: Create and verify JWT tokens as easily as possible.
@@ -43,18 +43,18 @@
 
 ## Usage
 
 Use the package in your code:
 
 ```python
 import logging
-from py_sls_lambda_toolkit.http_event import process_event
-from py_sls_lambda_toolkit.http_response import create_response
-from py_sls_lambda_toolkit.status_code import StatusCode
-from py_sls_lambda_toolkit.logger import logging
+from py_aws_lambda_toolkit.http_event import process_event
+from py_aws_lambda_toolkit.http_response import create_response
+from py_aws_lambda_toolkit.status_code import StatusCode
+from py_aws_lambda_toolkit.logger import logging
 
 status_code = StatusCode()
 
 def handler(event, context):
     # Process the event
     event_data = process_event(event)
     event_body = event_data.get("body", {})
```

### Comparing `py-aws-lambda-toolkit-0.0.3/README.md` & `py-aws-lambda-toolkit-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Py SLS Lambda Toolkit
+# Py aws Lambda Toolkit
 
 This is a lightweight Python toolkit for easily and quickly creating AWS Lambda functions with the Serverless Framework. It includes the following features:
 
 - DynamoDB shortcuts: Avoid boilerplate code for DynamoDB operations.
 - HTTP event processing: Get the event of the HTTP request and parse it, splitting it into the path, query string, body, headers, etc.
 - HTTP response shortcuts: Create HTTP responses with the correct format and status code.
 - JWT authentication: Create and verify JWT tokens as easily as possible.
@@ -23,18 +23,18 @@
 
 ## Usage
 
 Use the package in your code:
 
 ```python
 import logging
-from py_sls_lambda_toolkit.http_event import process_event
-from py_sls_lambda_toolkit.http_response import create_response
-from py_sls_lambda_toolkit.status_code import StatusCode
-from py_sls_lambda_toolkit.logger import logging
+from py_aws_lambda_toolkit.http_event import process_event
+from py_aws_lambda_toolkit.http_response import create_response
+from py_aws_lambda_toolkit.status_code import StatusCode
+from py_aws_lambda_toolkit.logger import logging
 
 status_code = StatusCode()
 
 def handler(event, context):
     # Process the event
     event_data = process_event(event)
     event_body = event_data.get("body", {})
```

### Comparing `py-aws-lambda-toolkit-0.0.3/__tests__/test_http_event.py` & `py-aws-lambda-toolkit-0.0.4/__tests__/test_http_event.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from py_sls_lambda_toolkit.http_event import process_event
+from py_aws_lambda_toolkit.http_event import process_event
 
 
 class TestProcessEvent(unittest.TestCase):
     def test_process_event(self):
         event = {
             'body': '{"name": "John", "age": 30}',
             'headers': {'Content-Type': 'application/json'},
```

### Comparing `py-aws-lambda-toolkit-0.0.3/__tests__/test_http_response.py` & `py-aws-lambda-toolkit-0.0.4/__tests__/test_http_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import unittest
 
-from py_sls_lambda_toolkit.http_response import create_response
-from py_sls_lambda_toolkit.settings import (
+from py_aws_lambda_toolkit.http_response import create_response
+from py_aws_lambda_toolkit.settings import (
     ACCESS_CONTROL_ALLOW_ORIGIN,
     ACCESS_CONTROL_ALLOW_CREDENTIALS,
     CONTENT_TYPE,
     ACCESS_CONTROL_ALLOWED_METHODS,
     ACCESS_CONTROL_ALLOWED_HEADERS
 )
```

### Comparing `py-aws-lambda-toolkit-0.0.3/__tests__/test_jwt.py` & `py-aws-lambda-toolkit-0.0.4/__tests__/test_jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from py_sls_lambda_toolkit.jwt import create_token, verify_token
+from py_aws_lambda_toolkit.jwt import create_token, verify_token
 import jwt
 
 class TestJWT(unittest.TestCase):
 
     def test_create_token(self,):
         user_id = 12345
         exp_time = 3600
```

### Comparing `py-aws-lambda-toolkit-0.0.3/__tests__/test_mappers.py` & `py-aws-lambda-toolkit-0.0.4/__tests__/test_mappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from py_sls_lambda_toolkit.mappers import mapper
+from py_aws_lambda_toolkit.mappers import mapper
 
 
 class TestMappers(unittest.TestCase):
 
     def test_mapper(self):
         data = {
             'name': 'John',
```

### Comparing `py-aws-lambda-toolkit-0.0.3/__tests__/test_parsers.py` & `py-aws-lambda-toolkit-0.0.4/__tests__/test_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from py_sls_lambda_toolkit.parsers import (
+from py_aws_lambda_toolkit.parsers import (
     convert_camel_to_snake,
     convert_snake_to_camel,
 )
 
 
 class TestParsers(unittest.TestCase):
```

### Comparing `py-aws-lambda-toolkit-0.0.3/__tests__/test_password.py` & `py-aws-lambda-toolkit-0.0.4/__tests__/test_password.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from py_sls_lambda_toolkit.password import (
+from py_aws_lambda_toolkit.password import (
     hash_password,
     verify_password,
 )
 
 
 class TestPassword(unittest.TestCase):
```

### Comparing `py-aws-lambda-toolkit-0.0.3/__tests__/test_validators.py` & `py-aws-lambda-toolkit-0.0.4/__tests__/test_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from py_sls_lambda_toolkit.validators import (
+from py_aws_lambda_toolkit.validators import (
     validate_path,
     validate_data,
 )
 
 
 class TestValidators(unittest.TestCase):
```

### Comparing `py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/PKG-INFO` & `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: py-aws-lambda-toolkit
-Version: 0.0.3
+Version: 0.0.4
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
-Home-page: https://github.com/0riion/py-sls-lambda-toolkit
+Home-page: https://github.com/0riion/py-aws-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
-Keywords: aws,serverless,lambda,dynamodb,toolkit,python,sls
+Keywords: aws,serverless,lambda,dynamodb,toolkit,python,aws
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Py SLS Lambda Toolkit
+# Py aws Lambda Toolkit
 
 This is a lightweight Python toolkit for easily and quickly creating AWS Lambda functions with the Serverless Framework. It includes the following features:
 
 - DynamoDB shortcuts: Avoid boilerplate code for DynamoDB operations.
 - HTTP event processing: Get the event of the HTTP request and parse it, splitting it into the path, query string, body, headers, etc.
 - HTTP response shortcuts: Create HTTP responses with the correct format and status code.
 - JWT authentication: Create and verify JWT tokens as easily as possible.
@@ -43,18 +43,18 @@
 
 ## Usage
 
 Use the package in your code:
 
 ```python
 import logging
-from py_sls_lambda_toolkit.http_event import process_event
-from py_sls_lambda_toolkit.http_response import create_response
-from py_sls_lambda_toolkit.status_code import StatusCode
-from py_sls_lambda_toolkit.logger import logging
+from py_aws_lambda_toolkit.http_event import process_event
+from py_aws_lambda_toolkit.http_response import create_response
+from py_aws_lambda_toolkit.status_code import StatusCode
+from py_aws_lambda_toolkit.logger import logging
 
 status_code = StatusCode()
 
 def handler(event, context):
     # Process the event
     event_data = process_event(event)
     event_body = event_data.get("body", {})
```

### Comparing `py-aws-lambda-toolkit-0.0.3/py_aws_lambda_toolkit.egg-info/SOURCES.txt` & `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 __tests__/test_http_response.py
 __tests__/test_jwt.py
 __tests__/test_logger.py
 __tests__/test_mappers.py
 __tests__/test_parsers.py
 __tests__/test_password.py
 __tests__/test_validators.py
+py_aws_lambda_toolkit/__init__.py
+py_aws_lambda_toolkit/dynamodb_shortcuts.py
+py_aws_lambda_toolkit/http_event.py
+py_aws_lambda_toolkit/http_response.py
+py_aws_lambda_toolkit/jwt.py
+py_aws_lambda_toolkit/logger.py
+py_aws_lambda_toolkit/mappers.py
+py_aws_lambda_toolkit/parsers.py
+py_aws_lambda_toolkit/password.py
+py_aws_lambda_toolkit/scan_filter_builder.py
+py_aws_lambda_toolkit/settings.py
+py_aws_lambda_toolkit/status_code.py
+py_aws_lambda_toolkit/validators.py
 py_aws_lambda_toolkit.egg-info/PKG-INFO
 py_aws_lambda_toolkit.egg-info/SOURCES.txt
 py_aws_lambda_toolkit.egg-info/dependency_links.txt
 py_aws_lambda_toolkit.egg-info/requires.txt
-py_aws_lambda_toolkit.egg-info/top_level.txt
-py_sls_lambda_toolkit/__init__.py
-py_sls_lambda_toolkit/dynamodb_shortcuts.py
-py_sls_lambda_toolkit/http_event.py
-py_sls_lambda_toolkit/http_response.py
-py_sls_lambda_toolkit/jwt.py
-py_sls_lambda_toolkit/logger.py
-py_sls_lambda_toolkit/mappers.py
-py_sls_lambda_toolkit/parsers.py
-py_sls_lambda_toolkit/password.py
-py_sls_lambda_toolkit/scan_filter_builder.py
-py_sls_lambda_toolkit/settings.py
-py_sls_lambda_toolkit/status_code.py
-py_sls_lambda_toolkit/validators.py
+py_aws_lambda_toolkit.egg-info/top_level.txt
```

### Comparing `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/dynamodb_shortcuts.py` & `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/dynamodb_shortcuts.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_event.py` & `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/http_event.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/http_response.py` & `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/http_response.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/jwt.py` & `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/jwt.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/mappers.py` & `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/mappers.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/parsers.py` & `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/parsers.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/password.py` & `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/password.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/scan_filter_builder.py` & `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/scan_filter_builder.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/settings.py` & `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/settings.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/status_code.py` & `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/status_code.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.3/py_sls_lambda_toolkit/validators.py` & `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         }
     },
     "required": [
         "id"
     ]
 }
 
-
+# TODO: validate custom paths
 def validate_path(path):
     try:
         if not path:
             raise ValidationError("Path is empty")
 
         validate(path, path_id_schema)
     except ValidationError as err:
```

### Comparing `py-aws-lambda-toolkit-0.0.3/setup.cfg` & `py-aws-lambda-toolkit-0.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = py-aws-lambda-toolkit
-version = 0.0.3
+version = 0.0.4
 author = Julio Flores
 author_email = juliocesarflores12@gmail.com
 author_url = juliofloresdev.com
 description = A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/0riion/py-sls-lambda-toolkit
+url = https://github.com/0riion/py-aws-lambda-toolkit
 license = MIT
 license_file = LICENSE
 classifiers = 
 	Development Status :: 1 - Planning
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.8
@@ -21,15 +21,15 @@
 keywords = 
 	aws
 	serverless
 	lambda
 	dynamodb
 	toolkit
 	python
-	sls
+	aws
 
 [options]
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	boto3==1.26.118
 	jsonschema==4.17.3
```

