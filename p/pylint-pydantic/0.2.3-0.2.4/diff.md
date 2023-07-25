# Comparing `tmp/pylint_pydantic-0.2.3-py3-none-any.whl.zip` & `tmp/pylint_pydantic-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 15118 bytes, number of entries: 6
--rw-r--r--  2.0 unx     2500 b- defN 23-Jul-21 02:24 pylint_pydantic/__init__.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-21 02:24 pylint_pydantic-0.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1931 b- defN 23-Jul-21 02:24 pylint_pydantic-0.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 02:24 pylint_pydantic-0.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-21 02:24 pylint_pydantic-0.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      511 b- defN 23-Jul-21 02:24 pylint_pydantic-0.2.3.dist-info/RECORD
-6 files, 40199 bytes uncompressed, 14188 bytes compressed:  64.7%
+Zip file size: 15784 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     2521 b- defN 23-Jul-25 06:20 pylint_pydantic/__init__.py
+-rw-r--r--  2.0 unx     1111 b- defN 23-Jul-25 06:20 pylint_pydantic/field.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-25 06:20 pylint_pydantic-0.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1931 b- defN 23-Jul-25 06:20 pylint_pydantic-0.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 06:20 pylint_pydantic-0.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-25 06:20 pylint_pydantic-0.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      592 b- defN 23-Jul-25 06:20 pylint_pydantic-0.2.4.dist-info/RECORD
+7 files, 41412 bytes uncompressed, 14730 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: pylint_pydantic/__init__.py
 Comment: 
 
-Filename: pylint_pydantic-0.2.3.dist-info/LICENSE
+Filename: pylint_pydantic/field.py
 Comment: 
 
-Filename: pylint_pydantic-0.2.3.dist-info/METADATA
+Filename: pylint_pydantic-0.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: pylint_pydantic-0.2.3.dist-info/WHEEL
+Filename: pylint_pydantic-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: pylint_pydantic-0.2.3.dist-info/top_level.txt
+Filename: pylint_pydantic-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: pylint_pydantic-0.2.3.dist-info/RECORD
+Filename: pylint_pydantic-0.2.4.dist-info/top_level.txt
+Comment: 
+
+Filename: pylint_pydantic-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylint_pydantic/__init__.py

```diff
@@ -1,12 +1,14 @@
 import astroid
 from astroid import MANAGER, Attribute, Call, ClassDef, FunctionDef, Name, nodes
 from pylint.checkers.design_analysis import MisdesignChecker
 from pylint_plugin_utils import suppress_message
 
+from . import field
+
 CLASSMETHOD_VALIDATOR_NAMES = {"validator", "root_validator", "field_validator"}
 MODE_VALIDATOR_NAMES = {"model_validator"}
 
 
 def _mode_validator_is_classmethod(call: Call):
     # https://docs.pydantic.dev/latest/api/functional_validators/#pydantic.functional_validators.model_validator
     for keyword in call.keywords:
```

## Comparing `pylint_pydantic-0.2.3.dist-info/LICENSE` & `pylint_pydantic-0.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pylint_pydantic-0.2.3.dist-info/METADATA` & `pylint_pydantic-0.2.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-pydantic
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Pylint plugin to help Pylint understand the Pydantic
 Home-page: https://github.com/fcfangcc/pylint-pydantic
 Author: fcfangcc
 Author-email: swjfc22@163.com
 License: GPLv3
 Keywords: pylint,pydantic
 Platform: UNKNOWN
```

