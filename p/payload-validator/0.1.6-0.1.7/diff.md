# Comparing `tmp/payload-validator-0.1.6.tar.gz` & `tmp/payload-validator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\payload-validator-0.1.6.tar", last modified: Sat Jul 22 17:45:13 2023, max compression
+gzip compressed data, was "dist\payload-validator-0.1.7.tar", last modified: Tue Jul 25 15:12:26 2023, max compression
```

## Comparing `payload-validator-0.1.6.tar` & `payload-validator-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 17:45:13.000000 payload-validator-0.1.6/
--rw-rw-rw-   0        0        0     1069 2023-07-22 14:40:36.000000 payload-validator-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       74 2023-07-22 08:07:09.000000 payload-validator-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0    12476 2023-07-22 17:45:13.000000 payload-validator-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    11599 2023-07-22 14:34:27.000000 payload-validator-0.1.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-22 17:45:13.000000 payload-validator-0.1.6/payload_validator/
--rw-rw-rw-   0        0        0        0 2023-07-22 17:39:10.000000 payload-validator-0.1.6/payload_validator/__init__.py
--rw-rw-rw-   0        0        0      958 2023-07-22 17:39:10.000000 payload-validator-0.1.6/payload_validator/exceptions.py
--rw-rw-rw-   0        0        0     5270 2023-07-22 17:39:10.000000 payload-validator-0.1.6/payload_validator/validators.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:45:13.000000 payload-validator-0.1.6/payload_validator.egg-info/
--rw-rw-rw-   0        0        0    12476 2023-07-22 17:45:12.000000 payload-validator-0.1.6/payload_validator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-07-22 17:45:12.000000 payload-validator-0.1.6/payload_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 17:45:12.000000 payload-validator-0.1.6/payload_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-22 17:45:12.000000 payload-validator-0.1.6/payload_validator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      893 2023-07-22 17:45:13.000000 payload-validator-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0       68 2023-07-22 07:54:29.000000 payload-validator-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:45:13.000000 payload-validator-0.1.6/tests/
--rw-rw-rw-   0        0        0        0 2023-07-22 14:07:42.000000 payload-validator-0.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0     2960 2023-07-22 17:31:36.000000 payload-validator-0.1.6/tests/test_exceptions.py
--rw-rw-rw-   0        0        0    26831 2023-07-22 17:31:47.000000 payload-validator-0.1.6/tests/test_validators.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:12:26.000000 payload-validator-0.1.7/
+-rw-rw-rw-   0        0        0     1069 2023-07-23 05:40:32.000000 payload-validator-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       74 2023-07-23 05:40:32.000000 payload-validator-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    12476 2023-07-25 15:12:26.000000 payload-validator-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11599 2023-07-23 09:56:08.000000 payload-validator-0.1.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-25 15:12:26.000000 payload-validator-0.1.7/payload_validator/
+-rw-rw-rw-   0        0        0        0 2023-07-23 05:40:32.000000 payload-validator-0.1.7/payload_validator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:12:26.000000 payload-validator-0.1.7/payload_validator/__pycache__/
+-rw-rw-rw-   0        0        0      160 2023-07-23 16:52:28.000000 payload-validator-0.1.7/payload_validator/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1622 2023-07-23 16:52:28.000000 payload-validator-0.1.7/payload_validator/__pycache__/exceptions.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6463 2023-07-25 14:47:02.000000 payload-validator-0.1.7/payload_validator/__pycache__/validators.cpython-37.pyc
+-rw-rw-rw-   0        0        0      958 2023-07-23 06:25:16.000000 payload-validator-0.1.7/payload_validator/exceptions.py
+-rw-rw-rw-   0        0        0     6080 2023-07-25 15:10:13.000000 payload-validator-0.1.7/payload_validator/validators.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:12:26.000000 payload-validator-0.1.7/payload_validator.egg-info/
+-rw-rw-rw-   0        0        0    12476 2023-07-25 15:12:26.000000 payload-validator-0.1.7/payload_validator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      541 2023-07-25 15:12:26.000000 payload-validator-0.1.7/payload_validator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 15:12:26.000000 payload-validator-0.1.7/payload_validator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-25 15:12:26.000000 payload-validator-0.1.7/payload_validator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      893 2023-07-25 15:12:26.000000 payload-validator-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0       68 2023-07-23 05:40:32.000000 payload-validator-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:12:26.000000 payload-validator-0.1.7/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-23 05:40:32.000000 payload-validator-0.1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     2960 2023-07-23 05:40:32.000000 payload-validator-0.1.7/tests/test_exceptions.py
+-rw-rw-rw-   0        0        0    38040 2023-07-25 15:10:13.000000 payload-validator-0.1.7/tests/test_validators.py
```

### Comparing `payload-validator-0.1.6/LICENSE` & `payload-validator-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `payload-validator-0.1.6/PKG-INFO` & `payload-validator-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payload-validator
-Version: 0.1.6
+Version: 0.1.7
 Summary: Validating payload datas for Python
 Home-page: https://github.com/cwadven/payload-validator
 Author: cwadven
 Author-email: cwadven4@gmail.com
 Maintainer: cwadven
 License: MIT
 Keywords: input,payload,validator,validate,validation,data,datas,python,python3,python3.6,python3.7,python3.8
```

### Comparing `payload-validator-0.1.6/README.rst` & `payload-validator-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `payload-validator-0.1.6/payload_validator/exceptions.py` & `payload-validator-0.1.7/payload_validator/exceptions.py`

 * *Files identical despite different names*

### Comparing `payload-validator-0.1.6/payload_validator/validators.py` & `payload-validator-0.1.7/payload_validator/validators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import re
+import traceback
 from abc import (
     ABC,
     abstractmethod,
 )
+from itertools import chain
 from types import FunctionType
 from typing import (
     Callable,
     Iterable,
     Optional,
     TypeVar,
     Union,
 )
 
 from payload_validator.exceptions import (
     InvalidValueError,
+    MismatchedErrorKeysException,
     ValidationException,
     ValidationNotRunException,
 )
 
 
 T = TypeVar("T")  # Use TypeVar for arbitrary object types
 
@@ -71,15 +75,15 @@
         """
         mandatory_keys example:
         {
             "displayable": "displayable is required",  # if error message is not provided, default message will be used
         }
         """
         for key, error_message in self.mandatory_keys.items():
-            if self.payload.get(key) is None:
+            if self.payload.get(key) in [None, ""]:
                 self.add_error_and_skip_validation_key(key, error_message or self.DEFAULT_MANDATORY_ERROR_MESSAGE)
 
     def _validate_payloads_type(self) -> None:
         for key, value in self.type_of_keys.items():
             type_or_funcs, error_msg = value
 
             if not isinstance(type_or_funcs, Iterable):
@@ -95,41 +99,57 @@
             if isinstance(type_or_func, FunctionType):
                 if type_or_func(payload_value):
                     return True
             elif isinstance(payload_value, type_or_func):
                 return True
         return False
 
+    def _handle_invalid_value_error_exception(self, e: InvalidValueError) -> None:
+        for key, value in e.error_value_by_key.items():
+            if key in e.add_skip_validation_keys:
+                self.add_error_and_skip_validation_key(key, value)
+            else:
+                self.add_error_context(key, value)
+
+    def _handle_skip_validation_key_payload_exception(self, e: Exception) -> None:
+        tb = traceback.extract_tb(e.__traceback__)
+        pattern = r"self\.payload(?:\.get\('([^']*)'\)|\['([^']*)'\]|(?:\[\"|\'|)([^\"\']*)(?:\"|\'|)\])"
+        for key in [match for match in chain(*re.findall(pattern, tb[-1].line)) if match]:
+            if key in self._skip_validate_keys:
+                pass
+            else:
+                raise e
+
     def _common_validate(self) -> None:
         try:
             self.common_validate()
+        except MismatchedErrorKeysException as e:
+            raise e
         except InvalidValueError as e:
-            for key, value in e.error_value_by_key.items():
-                if key in e.add_skip_validation_keys:
-                    self.add_error_and_skip_validation_key(key, value)
-                else:
-                    self.add_error_context(key, value)
+            self._handle_invalid_value_error_exception(e)
+        except Exception as e:
+            self._handle_skip_validation_key_payload_exception(e)
 
     def common_validate(self) -> None:
         """
         override this method to add custom validation
         """
         pass
 
     def _validate_methods(self) -> None:
         for x, y in self.__class__.__dict__.items():
             if type(y) == FunctionType and x.startswith("validate"):
                 try:
                     y(self)
+                except MismatchedErrorKeysException as e:
+                    raise e
                 except InvalidValueError as e:
-                    for key, value in e.error_value_by_key.items():
-                        if key in e.add_skip_validation_keys:
-                            self.add_error_and_skip_validation_key(key, value)
-                        else:
-                            self.add_error_context(key, value)
+                    self._handle_invalid_value_error_exception(e)
+                except Exception as e:
+                    self._handle_skip_validation_key_payload_exception(e)
 
     def validate(self) -> None:
         if not self._validate_called:
             self._validate_mandatory_payloads()
             self._validate_payloads_type()
             self._validate_methods()
             self._common_validate()
```

### Comparing `payload-validator-0.1.6/payload_validator.egg-info/PKG-INFO` & `payload-validator-0.1.7/payload_validator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payload-validator
-Version: 0.1.6
+Version: 0.1.7
 Summary: Validating payload datas for Python
 Home-page: https://github.com/cwadven/payload-validator
 Author: cwadven
 Author-email: cwadven4@gmail.com
 Maintainer: cwadven
 License: MIT
 Keywords: input,payload,validator,validate,validation,data,datas,python,python3,python3.6,python3.7,python3.8
```

### Comparing `payload-validator-0.1.6/setup.cfg` & `payload-validator-0.1.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6179 6c6f 6164 2d76 616c 6964   = payload-valid
 00000020: 6174 6f72 0d0a 7665 7273 696f 6e20 3d20  ator..version = 
-00000030: 302e 312e 360d 0a61 7574 686f 7220 3d20  0.1.6..author = 
+00000030: 302e 312e 370d 0a61 7574 686f 7220 3d20  0.1.7..author = 
 00000040: 6377 6164 7665 6e0d 0a61 7574 686f 725f  cwadven..author_
 00000050: 656d 6169 6c20 3d20 6377 6164 7665 6e34  email = cwadven4
 00000060: 4067 6d61 696c 2e63 6f6d 0d0a 6d61 696e  @gmail.com..main
 00000070: 7461 696e 6572 203d 2063 7761 6476 656e  tainer = cwadven
 00000080: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000090: 5661 6c69 6461 7469 6e67 2070 6179 6c6f  Validating paylo
 000000a0: 6164 2064 6174 6173 2066 6f72 2050 7974  ad datas for Pyt
```

### Comparing `payload-validator-0.1.6/tests/test_exceptions.py` & `payload-validator-0.1.7/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `payload-validator-0.1.6/tests/test_validators.py` & `payload-validator-0.1.7/tests/test_validators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+from unittest.mock import patch
 
 from payload_validator.exceptions import (
     InvalidValueError,
     MismatchedErrorKeysException,
     ValidationException,
     ValidationNotRunException,
 )
@@ -659,7 +660,252 @@
         # Given:
         payload = {"displayable": "example"}
         validator = PayloadValidator(payload)
 
         # Excepted: validate or is_valid method not called
         with self.assertRaises(ValidationNotRunException):
             _ = validator.error_context
+
+    def test_handle_invalid_value_error_exception_when_add_skip_validation_keys_not_exists(self):
+        # Given:
+        payload = {"displayable": "example"}
+        validator = PayloadValidator(payload)
+
+        # When:
+        validator._handle_invalid_value_error_exception(InvalidValueError({"displayable": "displayable error"}))
+
+        # Then:
+        self.assertEqual(len(validator._error_context), 1)
+        self.assertEqual(validator._error_context["displayable"], ["displayable error"])
+        # And: Due to add_skip_validation_keys error is not exists
+        self.assertNotIn("displayable", validator._skip_validate_keys)
+
+    def test_handle_invalid_value_error_exception_when_add_skip_validation_keys_exists(self):
+        # Given:
+        payload = {"displayable": "example"}
+        validator = PayloadValidator(payload)
+
+        # When:
+        validator._handle_invalid_value_error_exception(
+            InvalidValueError({"displayable": "displayable error"}, ["displayable"])
+        )
+
+        # Then:
+        self.assertEqual(len(validator._error_context), 1)
+        self.assertEqual(validator._error_context["displayable"], ["displayable error"])
+        # And: Due to add_skip_validation_keys error is exists
+        self.assertIn("displayable", validator._skip_validate_keys)
+
+    @patch("payload_validator.validators.PayloadValidator._handle_skip_validation_key_payload_exception")
+    def test_handle_skip_validation_key_payload_in_payload_key_not_exists_common_validate_exception(self, mock_handle_skip_validation_key_payload_exception):
+        # Given: common_validate method validation
+        class CustomValidator(PayloadValidator):
+            def common_validate(self):
+                if self.payload["start_date"] > 1:
+                    pass
+        # And: Add payload start_date key not exists
+        custom_validator = CustomValidator({})
+        custom_validator.add_error_and_skip_validation_key("start_date", "start_date is required")
+        # And: Set _validate_called to True
+        custom_validator._validate_called = True
+
+        # When:
+        custom_validator._common_validate()
+
+        # Then:
+        mock_handle_skip_validation_key_payload_exception.assert_called_once()
+        self.assertEqual(custom_validator.error_context["start_date"], ["start_date is required"])
+
+    def test_handle_skip_validation_key_payload_in_payload_key_not_exists_common_validate_exception_should_pass(self):
+        # Given: common_validate method validation
+        class CustomValidator(PayloadValidator):
+            def common_validate(self):
+                if self.payload["start_date"] > 1:
+                    pass
+
+        # And: Add payload start_date key not exists
+        custom_validator = CustomValidator({})
+        custom_validator.add_error_and_skip_validation_key("start_date", "start_date is required")
+        # And: Set _validate_called to True
+        custom_validator._validate_called = True
+
+        # When:
+        custom_validator._common_validate()
+
+        # Then:
+        self.assertEqual(custom_validator.error_context["start_date"], ["start_date is required"])
+
+    def test_handle_skip_validation_key_payload_in_payload_key_not_exists_common_validate_exception_should_not_pass(self):
+        # Given: common_validate method validation
+        class CustomValidator(PayloadValidator):
+            def common_validate(self):
+                if self.payload["start_date"] > 1:
+                    pass
+
+        # And: Add payload start_date key not exists
+        custom_validator = CustomValidator({})
+
+        # Expected:
+        with self.assertRaises(KeyError):
+            custom_validator._common_validate()
+
+    @patch("payload_validator.validators.PayloadValidator._handle_skip_validation_key_payload_exception")
+    def test_handle_skip_validation_key_payload_in_payload_key_type_invalid_common_validate_exception(self, mock_handle_skip_validation_key_payload_exception):
+        # Given: common_validate method validation
+        class CustomValidator(PayloadValidator):
+            def common_validate(self):
+                if self.payload["start_date"] > 1:
+                    pass
+
+        # And: Add payload start_date is String
+        custom_validator = CustomValidator({"start_date": "String"})
+        custom_validator.add_error_and_skip_validation_key("start_date", "type should be integer")
+        # And: Set _validate_called to True
+        custom_validator._validate_called = True
+
+        # When:
+        custom_validator._common_validate()
+
+        # Then:
+        mock_handle_skip_validation_key_payload_exception.assert_called_once()
+        self.assertEqual(custom_validator.error_context["start_date"], ["type should be integer"])
+
+    def test_handle_skip_validation_key_payload_in_payload_key_type_invalid_common_validate_exception_should_pass(self):
+        # Given: common_validate method validation
+        class CustomValidator(PayloadValidator):
+            def common_validate(self):
+                if self.payload["start_date"] > 1:
+                    pass
+
+        # And: Add payload start_date is String
+        custom_validator = CustomValidator({"start_date": "String"})
+        custom_validator.add_error_and_skip_validation_key("start_date", "type should be integer")
+        # And: Set _validate_called to True
+        custom_validator._validate_called = True
+
+        # When:
+        custom_validator._common_validate()
+
+        # Then:
+        self.assertEqual(custom_validator.error_context["start_date"], ["type should be integer"])
+
+    def test_handle_skip_validation_key_payload_in_payload_key_type_invalid_common_validate_exception_should_not_pass(self):
+        # Given: common_validate method validation
+        class CustomValidator(PayloadValidator):
+            def common_validate(self):
+                if self.payload["start_date"] > 1:
+                    pass
+
+        # And: Add payload start_date is String
+        custom_validator = CustomValidator({"start_date": "String"})
+
+        # Expected:
+        with self.assertRaises(TypeError):
+            custom_validator._common_validate()
+
+    @patch("payload_validator.validators.PayloadValidator._handle_skip_validation_key_payload_exception")
+    def test_handle_skip_validation_key_payload_in_payload_key_not_exists_validate_method_exception(self, mock_handle_skip_validation_key_payload_exception):
+        # Given: validate method validation
+        class CustomValidator(PayloadValidator):
+            def validate_start_date(self):
+                if self.payload["start_date"] > 1:
+                    pass
+
+        # And: Add payload start_date key not exists
+        custom_validator = CustomValidator({})
+        custom_validator.add_error_and_skip_validation_key("start_date", "start_date is required")
+        # And: Set _validate_called to True
+        custom_validator._validate_called = True
+
+        # When:
+        custom_validator._validate_methods()
+
+        # Then:
+        mock_handle_skip_validation_key_payload_exception.assert_called_once()
+        self.assertEqual(custom_validator.error_context["start_date"], ["start_date is required"])
+
+    def test_handle_skip_validation_key_payload_in_payload_key_not_exists_validate_method_should_pass(self):
+        # Given: validate method validation
+        class CustomValidator(PayloadValidator):
+            def validate_start_date(self):
+                if self.payload["start_date"] > 1:
+                    pass
+
+        # And: Add payload start_date key not exists
+        custom_validator = CustomValidator({})
+        custom_validator.add_error_and_skip_validation_key("start_date", "start_date is required")
+        # And: Set _validate_called to True
+        custom_validator._validate_called = True
+
+        # When:
+        custom_validator._validate_methods()
+
+        # Then:
+        self.assertEqual(custom_validator.error_context["start_date"], ["start_date is required"])
+
+    def test_handle_skip_validation_key_payload_in_payload_key_not_exists_validate_method_should_not_pass(self):
+        # Given: validate method validation
+        class CustomValidator(PayloadValidator):
+            def validate_start_date(self):
+                if self.payload["start_date"] > 1:
+                    pass
+
+        # And: Add payload start_date key not exists
+        custom_validator = CustomValidator({})
+
+        # Expected:
+        with self.assertRaises(KeyError):
+            custom_validator._validate_methods()
+
+    @patch("payload_validator.validators.PayloadValidator._handle_skip_validation_key_payload_exception")
+    def test_handle_skip_validation_key_payload_in_payload_key_type_invalid_validate_method_exception(self, mock_handle_skip_validation_key_payload_exception):
+        # Given: validate method validation
+        class CustomValidator(PayloadValidator):
+            def validate_start_date(self):
+                if self.payload["start_date"] > 1:
+                    pass
+
+        # And: Add payload start_date is String
+        custom_validator = CustomValidator({"start_date": "String"})
+        custom_validator.add_error_and_skip_validation_key("start_date", "type should be integer")
+        # And: Set _validate_called to True
+        custom_validator._validate_called = True
+
+        # When:
+        custom_validator._validate_methods()
+
+        # Then:
+        mock_handle_skip_validation_key_payload_exception.assert_called_once()
+        self.assertEqual(custom_validator.error_context["start_date"], ["type should be integer"])
+
+    def test_handle_skip_validation_key_payload_in_payload_key_type_invalid_validate_method_exception_should_pass(self):
+        # Given: validate method validation
+        class CustomValidator(PayloadValidator):
+            def validate_start_date(self):
+                if self.payload["start_date"] > 1:
+                    pass
+
+        # And: Add payload start_date is String
+        custom_validator = CustomValidator({"start_date": "String"})
+        custom_validator.add_error_and_skip_validation_key("start_date", "type should be integer")
+        # And: Set _validate_called to True
+        custom_validator._validate_called = True
+
+        # When:
+        custom_validator._validate_methods()
+
+        # Then:
+        self.assertEqual(custom_validator.error_context["start_date"], ["type should be integer"])
+
+    def test_handle_skip_validation_key_payload_in_payload_key_type_invalid_validate_method_exception_should_not_pass(self):
+        # Given: validate method validation
+        class CustomValidator(PayloadValidator):
+            def validate_start_date(self):
+                if self.payload["start_date"] > 1:
+                    pass
+
+        # And: Add payload start_date is String
+        custom_validator = CustomValidator({"start_date": "String"})
+
+        # Expected:
+        with self.assertRaises(TypeError):
+            custom_validator._validate_methods()
```

