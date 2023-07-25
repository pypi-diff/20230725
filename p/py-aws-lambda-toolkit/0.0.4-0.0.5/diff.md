# Comparing `tmp/py-aws-lambda-toolkit-0.0.4.tar.gz` & `tmp/py-aws-lambda-toolkit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-aws-lambda-toolkit-0.0.4.tar", last modified: Tue Jul 25 17:34:12 2023, max compression
+gzip compressed data, was "py-aws-lambda-toolkit-0.0.5.tar", last modified: Tue Jul 25 19:55:49 2023, max compression
```

## Comparing `py-aws-lambda-toolkit-0.0.4.tar` & `py-aws-lambda-toolkit-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:34:12.963975 py-aws-lambda-toolkit-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-25 17:34:12.963975 py-aws-lambda-toolkit-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:34:12.959975 py-aws-lambda-toolkit-0.0.4/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_http_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_http_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/__tests__/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:34:12.963975 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/dynamodb_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/http_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/http_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/scan_filter_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:34:12.963975 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-25 17:34:12.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-25 17:34:12.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:34:12.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 17:34:12.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-25 17:34:12.000000 py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-25 17:34:02.000000 py-aws-lambda-toolkit-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-25 17:34:12.963975 py-aws-lambda-toolkit-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:55:49.652772 py-aws-lambda-toolkit-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-25 19:55:49.652772 py-aws-lambda-toolkit-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:55:49.652772 py-aws-lambda-toolkit-0.0.5/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/__tests__/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/__tests__/test_case_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/__tests__/test_http_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/__tests__/test_http_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/__tests__/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/__tests__/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/__tests__/test_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/__tests__/test_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/__tests__/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:55:49.652772 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/case_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/dynamodb_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/http_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/http_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/scan_filter_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:55:49.652772 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-25 19:55:49.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-25 19:55:49.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:55:49.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 19:55:49.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-25 19:55:49.000000 py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-25 19:55:40.000000 py-aws-lambda-toolkit-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-25 19:55:49.652772 py-aws-lambda-toolkit-0.0.5/setup.cfg
```

### Comparing `py-aws-lambda-toolkit-0.0.4/LICENSE` & `py-aws-lambda-toolkit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.4/PKG-INFO` & `py-aws-lambda-toolkit-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-aws-lambda-toolkit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 Home-page: https://github.com/0riion/py-aws-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
 Keywords: aws,serverless,lambda,dynamodb,toolkit,python,aws
 Classifier: Development Status :: 1 - Planning
@@ -45,30 +45,30 @@
 
 Use the package in your code:
 
 ```python
 import logging
 from py_aws_lambda_toolkit.http_event import process_event
 from py_aws_lambda_toolkit.http_response import create_response
-from py_aws_lambda_toolkit.status_code import StatusCode
+from py_aws_lambda_toolkit.status import StatusCode
 from py_aws_lambda_toolkit.logger import logging
 
-status_code = StatusCode()
+status = StatusCode()
 
 def handler(event, context):
     # Process the event
     event_data = process_event(event)
     event_body = event_data.get("body", {})
 
     logging.info("Event body: %s", event_body)
 
     # Create a response
     response = create_response(
         { "ok": True, "message": "Processed event successfully" },
-        status_code=status_code.code_200_success,
+        status=status.code_200_success,
     )
 
     return response
 
 ```
 
 ## Contributing
```

### Comparing `py-aws-lambda-toolkit-0.0.4/README.md` & `py-aws-lambda-toolkit-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -25,30 +25,30 @@
 
 Use the package in your code:
 
 ```python
 import logging
 from py_aws_lambda_toolkit.http_event import process_event
 from py_aws_lambda_toolkit.http_response import create_response
-from py_aws_lambda_toolkit.status_code import StatusCode
+from py_aws_lambda_toolkit.status import StatusCode
 from py_aws_lambda_toolkit.logger import logging
 
-status_code = StatusCode()
+status = StatusCode()
 
 def handler(event, context):
     # Process the event
     event_data = process_event(event)
     event_body = event_data.get("body", {})
 
     logging.info("Event body: %s", event_body)
 
     # Create a response
     response = create_response(
         { "ok": True, "message": "Processed event successfully" },
-        status_code=status_code.code_200_success,
+        status=status.code_200_success,
     )
 
     return response
 
 ```
 
 ## Contributing
```

### Comparing `py-aws-lambda-toolkit-0.0.4/__tests__/test_mappers.py` & `py-aws-lambda-toolkit-0.0.5/__tests__/test_mappers.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.4/__tests__/test_password.py` & `py-aws-lambda-toolkit-0.0.5/__tests__/test_password.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.4/__tests__/test_validators.py` & `py-aws-lambda-toolkit-0.0.5/__tests__/test_validators.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/http_event.py` & `py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/http_event.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .logger import logging
 from typing import Dict
-from .parsers import (
-    convert_camel_to_snake,
-)
+from .case_converter import CaseConverter
+
+case_converter = CaseConverter()
 
 
 def process_event(event: Dict) -> Dict:
     try:
         body = event.get('body')
         headers = event.get('headers')
         http_method = event.get('httpMethod')
@@ -22,17 +22,18 @@
         logging.info({
             'requestContext': request_context,
             'httpMethod': http_method,
             'path': path,
             'headers': headers
         })
 
-        query_string_parameters = convert_camel_to_snake(query_string_parameters)
-        path_parameters = convert_camel_to_snake(path_parameters)
-        body = convert_camel_to_snake(body)
+        query_string_parameters = case_converter.snakeify(
+            query_string_parameters)
+        path_parameters = case_converter.snakeify(path_parameters)
+        body = case_converter.snakeify(body)
 
         return {
             'body': body,
             'headers': headers,
             'httpMethod': http_method,
             'isBase64Encoded': is_base64_encoded,
             'multiValueHeaders': multi_value_headers,
```

### Comparing `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/http_response.py` & `py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/http_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import json
-from .parsers import (
-    convert_snake_to_camel
-)
+from .case_converter import CaseConverter
 from .settings import (
     ACCESS_CONTROL_ALLOW_ORIGIN,
     ACCESS_CONTROL_ALLOW_CREDENTIALS,
     CONTENT_TYPE,
     ACCESS_CONTROL_ALLOWED_METHODS,
     ACCESS_CONTROL_ALLOWED_HEADERS
 )
 
+case_converter = CaseConverter()
+
 
 def create_response(
     response,
-    status_code=200,
+    status=200,
     custom_headers=None,
     content_type=CONTENT_TYPE
 ):
     """
         Creates an HTTP response object.
 
         Parameters:
             response (dict): The response body.
-            status_code (int): The HTTP status code to be returned.
+            status (int): The HTTP status code to be returned.
             headers (dict): The headers to be returned with the response.
             content_type (str): The content type of the response.
 
         Returns:
             dict: The HTTP response object with keys statusCode, headers, and body.
     """
     # TODO: Add support for binary data
@@ -38,14 +38,14 @@
         'Access-Control-Allow-Methods': ACCESS_CONTROL_ALLOWED_METHODS,
         'Access-Control-Allow-Headers': ACCESS_CONTROL_ALLOWED_HEADERS,
     }
 
     if custom_headers is not None:
         headers.update(custom_headers)
 
-    body = convert_snake_to_camel(response)
+    body = case_converter.camelize(response)
 
     return {
-        'statusCode': status_code,
+        'statusCode': status,
         'headers': headers,
         'body': json.dumps(body) if body is not None else None
     }
```

### Comparing `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/jwt.py` & `py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/jwt.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,38 @@
 import jwt
 import time
 
+
 def create_token(user_id, exp_time, jwt_secret):
-  payload = {'sub': user_id, 'exp': int(time.time()) + exp_time}
-  token = jwt.encode(payload, jwt_secret, algorithm='HS256')
-  return token
+    """
+    Creates a JWT token.
+    Args:
+        user_id (str): The user ID to be included in the token.
+        exp_time (int): The expiration time of the token, in seconds.
+        jwt_secret (str): The secret used to sign the token.
+    Returns:
+        str: The JWT token.
+    """
+    payload = {'sub': user_id, 'exp': int(time.time()) + exp_time}
+    token = jwt.encode(payload, jwt_secret, algorithm='HS256')
+    return token
 
 
 def verify_token(token, jwt_secret):
-  try:
-    decoded_token = jwt.decode(token, jwt_secret, algorithms=['HS256'])
-    return decoded_token['sub']
-
-  except jwt.ExpiredSignatureError:
-    raise Exception('Token has expired')
-
-  except jwt.InvalidTokenError:
-    raise Exception('Invalid token')
+    """
+    Verifies a JWT token.
+    Args:
+        token (str): The JWT token to be verified.
+        jwt_secret (str): The secret used to sign the token.
+    Returns:
+        str: The user ID from the token.
+    Raises:
+        ExpiredSignatureError: If the token has expired.
+        InvalidTokenError: If the token is invalid.
+    """
+    try:
+        decoded_token = jwt.decode(token, jwt_secret, algorithms=['HS256'])
+        return decoded_token['sub']
+    except jwt.ExpiredSignatureError:
+        raise Exception('Token has expired')
+    except jwt.InvalidTokenError:
+        raise Exception('Invalid token')
```

### Comparing `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/mappers.py` & `py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/mappers.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/scan_filter_builder.py` & `py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/scan_filter_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from boto3.dynamodb.conditions import Attr
 
+
 def equal(filter_expression, attribute, value):
     if bool(filter_expression):
         filter_expression &= Attr(attribute).eq(value)
     else:
         filter_expression = Attr(attribute).eq(value)
 
     return filter_expression
```

### Comparing `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/settings.py` & `py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/settings.py`

 * *Files identical despite different names*

### Comparing `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit/validators.py` & `py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit/validators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from jsonschema import validate
 from jsonschema.exceptions import ValidationError
 
+
 path_id_schema = {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "title": "Validate id comes in the object path",
     "type": "object",
     "properties": {
         "id": {
             "type": "string",
@@ -12,27 +13,47 @@
         }
     },
     "required": [
         "id"
     ]
 }
 
-# TODO: validate custom paths
+
 def validate_path(path):
-    try:
-        if not path:
-            raise ValidationError("Path is empty")
+    """
+    Validates the path object.
+
+    Args:
+        path (dict): The path object to be validated.
+
+    Raises:
+        ValidationError: If the path is invalid.
+    """
 
+    if not path:
+        raise ValidationError("Path is empty")
+
+    try:
         validate(path, path_id_schema)
     except ValidationError as err:
         raise ValidationError(err.message)
 
 
 def validate_data(data, schema):
-    try:
+    """
+    Validates the data object against the schema.
 
-        if not data or not schema:
-            raise ValidationError("Data or schema is empty")
+    Args:
+        data (dict): The data object to be validated.
+        schema (dict): The schema to be used for validation.
+
+    Raises:
+        ValidationError: If the data is invalid.
+    """
 
+    if not data or not schema:
+        raise ValidationError("Data or schema is empty")
+
+    try:
         validate(data, schema)
     except ValidationError as err:
         raise ValidationError(err.message)
```

### Comparing `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/PKG-INFO` & `py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-aws-lambda-toolkit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 Home-page: https://github.com/0riion/py-aws-lambda-toolkit
 Author: Julio Flores
 Author-email: juliocesarflores12@gmail.com
 License: MIT
 Keywords: aws,serverless,lambda,dynamodb,toolkit,python,aws
 Classifier: Development Status :: 1 - Planning
@@ -45,30 +45,30 @@
 
 Use the package in your code:
 
 ```python
 import logging
 from py_aws_lambda_toolkit.http_event import process_event
 from py_aws_lambda_toolkit.http_response import create_response
-from py_aws_lambda_toolkit.status_code import StatusCode
+from py_aws_lambda_toolkit.status import StatusCode
 from py_aws_lambda_toolkit.logger import logging
 
-status_code = StatusCode()
+status = StatusCode()
 
 def handler(event, context):
     # Process the event
     event_data = process_event(event)
     event_body = event_data.get("body", {})
 
     logging.info("Event body: %s", event_body)
 
     # Create a response
     response = create_response(
         { "ok": True, "message": "Processed event successfully" },
-        status_code=status_code.code_200_success,
+        status=status.code_200_success,
     )
 
     return response
 
 ```
 
 ## Contributing
```

### Comparing `py-aws-lambda-toolkit-0.0.4/py_aws_lambda_toolkit.egg-info/SOURCES.txt` & `py-aws-lambda-toolkit-0.0.5/py_aws_lambda_toolkit.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 __tests__/__init__.py
+__tests__/test_case_converter.py
 __tests__/test_http_event.py
 __tests__/test_http_response.py
 __tests__/test_jwt.py
 __tests__/test_logger.py
 __tests__/test_mappers.py
-__tests__/test_parsers.py
 __tests__/test_password.py
 __tests__/test_validators.py
 py_aws_lambda_toolkit/__init__.py
+py_aws_lambda_toolkit/case_converter.py
 py_aws_lambda_toolkit/dynamodb_shortcuts.py
 py_aws_lambda_toolkit/http_event.py
 py_aws_lambda_toolkit/http_response.py
 py_aws_lambda_toolkit/jwt.py
 py_aws_lambda_toolkit/logger.py
 py_aws_lambda_toolkit/mappers.py
-py_aws_lambda_toolkit/parsers.py
 py_aws_lambda_toolkit/password.py
 py_aws_lambda_toolkit/scan_filter_builder.py
 py_aws_lambda_toolkit/settings.py
-py_aws_lambda_toolkit/status_code.py
+py_aws_lambda_toolkit/status.py
 py_aws_lambda_toolkit/validators.py
 py_aws_lambda_toolkit.egg-info/PKG-INFO
 py_aws_lambda_toolkit.egg-info/SOURCES.txt
 py_aws_lambda_toolkit.egg-info/dependency_links.txt
 py_aws_lambda_toolkit.egg-info/requires.txt
 py_aws_lambda_toolkit.egg-info/top_level.txt
```

### Comparing `py-aws-lambda-toolkit-0.0.4/setup.cfg` & `py-aws-lambda-toolkit-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py-aws-lambda-toolkit
-version = 0.0.4
+version = 0.0.5
 author = Julio Flores
 author_email = juliocesarflores12@gmail.com
 author_url = juliofloresdev.com
 description = A toolkit for serverless and AWS, with a focus on AWS Lambda and dynamodb.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0riion/py-aws-lambda-toolkit
```

