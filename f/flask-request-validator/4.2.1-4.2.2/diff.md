# Comparing `tmp/flask_request_validator-4.2.1.tar.gz` & `tmp/flask_request_validator-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_request_validator-4.2.1.tar", last modified: Thu Dec 15 23:06:44 2022, max compression
+gzip compressed data, was "flask_request_validator-4.2.2.tar", last modified: Tue Jul 25 10:35:17 2023, max compression
```

## Comparing `flask_request_validator-4.2.1.tar` & `flask_request_validator-4.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:06:44.950917 flask_request_validator-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2022-12-15 23:06:30.000000 flask_request_validator-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      927 2022-12-15 23:06:44.950917 flask_request_validator-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2022-12-15 23:06:30.000000 flask_request_validator-4.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:06:44.950917 flask_request_validator-4.2.1/flask_request_validator/
--rwxr-xr-x   0 runner    (1001) docker     (123)      455 2022-12-15 23:06:30.000000 flask_request_validator-4.2.1/flask_request_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2022-12-15 23:06:30.000000 flask_request_validator-4.2.1/flask_request_validator/after_param.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2022-12-15 23:06:30.000000 flask_request_validator-4.2.1/flask_request_validator/dt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2022-12-15 23:06:30.000000 flask_request_validator-4.2.1/flask_request_validator/error_formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4792 2022-12-15 23:06:30.000000 flask_request_validator-4.2.1/flask_request_validator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2022-12-15 23:06:30.000000 flask_request_validator-4.2.1/flask_request_validator/nested_json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5151 2022-12-15 23:06:30.000000 flask_request_validator-4.2.1/flask_request_validator/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2022-12-15 23:06:30.000000 flask_request_validator-4.2.1/flask_request_validator/valid_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7248 2022-12-15 23:06:30.000000 flask_request_validator-4.2.1/flask_request_validator/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 23:06:44.950917 flask_request_validator-4.2.1/flask_request_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2022-12-15 23:06:44.000000 flask_request_validator-4.2.1/flask_request_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2022-12-15 23:06:44.000000 flask_request_validator-4.2.1/flask_request_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 23:06:44.000000 flask_request_validator-4.2.1/flask_request_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-15 23:06:44.000000 flask_request_validator-4.2.1/flask_request_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-15 23:06:44.000000 flask_request_validator-4.2.1/flask_request_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-15 23:06:44.950917 flask_request_validator-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      961 2022-12-15 23:06:30.000000 flask_request_validator-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:35:17.656640 flask_request_validator-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 10:35:07.000000 flask_request_validator-4.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-25 10:35:17.656640 flask_request_validator-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-25 10:35:07.000000 flask_request_validator-4.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:35:17.656640 flask_request_validator-4.2.2/flask_request_validator/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      455 2023-07-25 10:35:07.000000 flask_request_validator-4.2.2/flask_request_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-25 10:35:07.000000 flask_request_validator-4.2.2/flask_request_validator/after_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-25 10:35:07.000000 flask_request_validator-4.2.2/flask_request_validator/dt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-25 10:35:07.000000 flask_request_validator-4.2.2/flask_request_validator/error_formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4961 2023-07-25 10:35:07.000000 flask_request_validator-4.2.2/flask_request_validator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-07-25 10:35:07.000000 flask_request_validator-4.2.2/flask_request_validator/nested_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5151 2023-07-25 10:35:07.000000 flask_request_validator-4.2.2/flask_request_validator/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-25 10:35:07.000000 flask_request_validator-4.2.2/flask_request_validator/valid_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7248 2023-07-25 10:35:07.000000 flask_request_validator-4.2.2/flask_request_validator/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:35:17.656640 flask_request_validator-4.2.2/flask_request_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-25 10:35:17.000000 flask_request_validator-4.2.2/flask_request_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-25 10:35:17.000000 flask_request_validator-4.2.2/flask_request_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:35:17.000000 flask_request_validator-4.2.2/flask_request_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 10:35:17.000000 flask_request_validator-4.2.2/flask_request_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-25 10:35:17.000000 flask_request_validator-4.2.2/flask_request_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 10:35:17.656640 flask_request_validator-4.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-25 10:35:07.000000 flask_request_validator-4.2.2/setup.py
```

### Comparing `flask_request_validator-4.2.1/LICENSE` & `flask_request_validator-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_request_validator-4.2.1/PKG-INFO` & `flask_request_validator-4.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: flask_request_validator
-Version: 4.2.1
+Version: 4.2.2
 Summary: Flask request data validation
 Home-page: https://github.com/d-ganchar/flask_request_validator
 Author: Danila Ganchar
 Author-email: danila.ganchar@gmail.com
 License: MIT
 Keywords: flask request validation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
```

### Comparing `flask_request_validator-4.2.1/flask_request_validator/dt_utils.py` & `flask_request_validator-4.2.2/flask_request_validator/dt_utils.py`

 * *Files identical despite different names*

### Comparing `flask_request_validator-4.2.1/flask_request_validator/error_formatter.py` & `flask_request_validator-4.2.2/flask_request_validator/error_formatter.py`

 * *Files identical despite different names*

### Comparing `flask_request_validator-4.2.1/flask_request_validator/exceptions.py` & `flask_request_validator-4.2.2/flask_request_validator/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,22 @@
 
 
 class ListRuleError(RuleError):
     def __init__(self, errors: List[Any]) -> None:
         self.errors = errors
 
 
+class MissingJsonKeyError(RuleError):
+    def __init__(self, key: str) -> None:
+        self.key = key
+
+    def __str__(self) -> str:
+        return 'key is required'
+
+
 class RulesError(RequestError):
     def __init__(self, *args: RuleError):
         self.errors = args
 
     def __str__(self) -> str:
         return '. '.join([str(e) for e in self.errors])
```

### Comparing `flask_request_validator-4.2.1/flask_request_validator/nested_json.py` & `flask_request_validator-4.2.2/flask_request_validator/nested_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import Union, Dict, List, Tuple, Any
 
 from .exceptions import (
     JsonError,
     RequiredJsonKeyError,
     JsonListItemTypeError,
-    RulesError, JsonListExpectedError, JsonDictExpectedError,
+    RulesError,
+    JsonListExpectedError,
+    JsonDictExpectedError,
+    MissingJsonKeyError,
 )
 from .rules import CompositeRule, AbstractRule
 
 
 class JsonParam:
     """
     Nested json validation
@@ -42,14 +45,25 @@
                 return
             if not isinstance(value, (str, int, float, bool,)):
                 raise JsonListItemTypeError(False)
             return
         if isinstance(nested.rules_map, dict) and not isinstance(value, dict):
             raise JsonListItemTypeError()
 
+    def _is_missing_json_key(self, key: str, value: Dict, nested: 'JsonParam'):
+        rules = nested.rules_map.get(key)
+        if isinstance(rules, JsonParam) and not rules.required:
+            return
+
+        try:
+            if key not in value:
+                raise MissingJsonKeyError(key)
+        except MissingJsonKeyError as error:
+            raise RulesError(error)
+
     def _validate_list(
         self,
         value: Union[Dict, List],
         nested: 'JsonParam',
         depth: list,
         errors: List[JsonError],
     ) -> Tuple[Union[Dict, List], List]:
@@ -97,26 +111,34 @@
         self,
         value: Union[Dict, List],
         nested: 'JsonParam',
         depth: list,
         errors: List[JsonError],
     ) -> Tuple[Any, List[JsonError], Dict[str, RulesError]]:
         err = dict()
-        for key, rules in nested.rules_map.items():
-            if key not in value:
-                continue
-            elif isinstance(rules, JsonParam):
-                new_val, errors = self.validate(value[key], rules, depth + [key], errors)
-                continue
 
+        for key, rules in nested.rules_map.items():
             try:
-                new_val = rules.validate(value[key])
-                value[key] = new_val
+                self._is_missing_json_key(key, value, nested)
             except RulesError as e:
                 err[key] = e
+                continue
+
+            key_value = value.get(key)
+            if isinstance(rules, JsonParam):
+                if key_value is None and not nested.rules_map[key].required:
+                    continue
+
+                new_val, errors = self.validate(key_value, rules, depth + [key], errors)
+            else:
+                try:
+                    new_val = rules.validate(key_value)
+                    value[key] = new_val
+                except RulesError as e:
+                    err[key] = e
 
         return value, errors, err
 
     def _check_required(self, key: str, value: dict, rule: Any):
         """
         :raises RequiredJsonKeyError
         """
```

### Comparing `flask_request_validator-4.2.1/flask_request_validator/rules.py` & `flask_request_validator-4.2.2/flask_request_validator/rules.py`

 * *Files identical despite different names*

### Comparing `flask_request_validator-4.2.1/flask_request_validator/validator.py` & `flask_request_validator-4.2.2/flask_request_validator/validator.py`

 * *Files identical despite different names*

### Comparing `flask_request_validator-4.2.1/flask_request_validator.egg-info/PKG-INFO` & `flask_request_validator-4.2.2/flask_request_validator.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: flask-request-validator
-Version: 4.2.1
+Version: 4.2.2
 Summary: Flask request data validation
 Home-page: https://github.com/d-ganchar/flask_request_validator
 Author: Danila Ganchar
 Author-email: danila.ganchar@gmail.com
 License: MIT
 Keywords: flask request validation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
```

### Comparing `flask_request_validator-4.2.1/flask_request_validator.egg-info/SOURCES.txt` & `flask_request_validator-4.2.2/flask_request_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask_request_validator-4.2.1/setup.py` & `flask_request_validator-4.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 from setuptools import setup
 
 with io.open('README.rst', 'rt', encoding='utf8') as f:
     long_description = f.read()
 
 setup(
     name='flask_request_validator',
-    version='4.2.1',
+    version='4.2.2',
     description='Flask request data validation',
     long_description=long_description,
     url='https://github.com/d-ganchar/flask_request_validator',
     author='Danila Ganchar',
     author_email='danila.ganchar@gmail.com',
     license='MIT',
     keywords='flask request validation',
     packages=['flask_request_validator'],
     install_requires=['flask'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Framework :: Flask',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
 )
```

