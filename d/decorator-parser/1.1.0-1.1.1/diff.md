# Comparing `tmp/decorator_parser-1.1.0-py3-none-any.whl.zip` & `tmp/decorator_parser-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6064 bytes, number of entries: 9
+Zip file size: 6063 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       60 b- defN 23-Jul-08 10:47 decorator_parser/__init__.py
 -rw-r--r--  2.0 unx     1110 b- defN 23-Jul-08 10:42 decorator_parser/errors.py
--rw-r--r--  2.0 unx     4940 b- defN 23-Jul-25 19:10 decorator_parser/parse.py
+-rw-r--r--  2.0 unx     4938 b- defN 23-Jul-25 19:18 decorator_parser/parse.py
 -rw-r--r--  2.0 unx      261 b- defN 23-Jul-23 15:49 decorator_parser/utils.py
--rw-r--r--  2.0 unx      519 b- defN 23-Jul-25 19:15 decorator_parser-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4654 b- defN 23-Jul-25 19:15 decorator_parser-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 19:15 decorator_parser-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jul-25 19:15 decorator_parser-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      759 b- defN 23-Jul-25 19:15 decorator_parser-1.1.0.dist-info/RECORD
-9 files, 12412 bytes uncompressed, 4742 bytes compressed:  61.8%
+-rw-r--r--  2.0 unx      519 b- defN 23-Jul-25 19:19 decorator_parser-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4654 b- defN 23-Jul-25 19:19 decorator_parser-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 19:19 decorator_parser-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-25 19:19 decorator_parser-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      759 b- defN 23-Jul-25 19:19 decorator_parser-1.1.1.dist-info/RECORD
+9 files, 12410 bytes uncompressed, 4741 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: decorator_parser/parse.py
 Comment: 
 
 Filename: decorator_parser/utils.py
 Comment: 
 
-Filename: decorator_parser-1.1.0.dist-info/LICENSE
+Filename: decorator_parser-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: decorator_parser-1.1.0.dist-info/METADATA
+Filename: decorator_parser-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: decorator_parser-1.1.0.dist-info/WHEEL
+Filename: decorator_parser-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: decorator_parser-1.1.0.dist-info/top_level.txt
+Filename: decorator_parser-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: decorator_parser-1.1.0.dist-info/RECORD
+Filename: decorator_parser-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## decorator_parser/parse.py

```diff
@@ -1,13 +1,13 @@
 # Author: Michał Kostyk for Smartschool Inc.
 # Date: 2023
 # Version: 1.0.6
 
-from decorators_parser.utils import *
-from decorators_parser.errors import *
+from decorator_parser.utils import *
+from decorator_parser.errors import *
 import re
 
 
 class Parser:
     def __init__(self, constraints={}, ignored={}):
         for key in constraints:
             if not 'regex' in constraints[key] or not 'description' in constraints[key]:
```

## Comparing `decorator_parser-1.1.0.dist-info/LICENSE` & `decorator_parser-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `decorator_parser-1.1.0.dist-info/METADATA` & `decorator_parser-1.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorator-parser
-Version: 1.1.0
+Version: 1.1.1
 Summary: Parser for text files with decorators into Python dictionaries
 Author-email: Michal Kostyk <m.kostyk22@gmail.com>
 Project-URL: Homepage, https://github.com/mkostyk/decorators-parser
 Project-URL: Bug Tracker, https://github.com/mkostyk/decorators-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

## Comparing `decorator_parser-1.1.0.dist-info/RECORD` & `decorator_parser-1.1.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 decorator_parser/__init__.py,sha256=sx_Okl3ziNpfIbGs_KLWLPdjBV8eL9Zt75nuzErpq9g,60
 decorator_parser/errors.py,sha256=GefbMbWrJ6yVR-WK-34XbICH31wZKwLzAbwrfZW4vy8,1110
-decorator_parser/parse.py,sha256=j5mdPTUiSo6EuqCL35zVi0SszeQh_8cGxe1WUjEJ3u8,4940
+decorator_parser/parse.py,sha256=ZMO3yP_H80TX5lzDA6gQ9vZTtKL6FrDOU4Ix34aGieQ,4938
 decorator_parser/utils.py,sha256=yc1RCfV_pANGU2NofvcDPTrUzgEcInelaqEfGphgJe0,261
-decorator_parser-1.1.0.dist-info/LICENSE,sha256=d0IchUxRoZd6yiEkgwlRF6MEDtdQLuG3CiDQolTTkw8,519
-decorator_parser-1.1.0.dist-info/METADATA,sha256=uD2oJ9lIm3mEgyknENmBcRqR2NF3FwcxakfiNEqmRJg,4654
-decorator_parser-1.1.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-decorator_parser-1.1.0.dist-info/top_level.txt,sha256=wp3MzzKLv5-NNCQtdxjJPnk80INShwww5TfQfiIj95M,17
-decorator_parser-1.1.0.dist-info/RECORD,,
+decorator_parser-1.1.1.dist-info/LICENSE,sha256=d0IchUxRoZd6yiEkgwlRF6MEDtdQLuG3CiDQolTTkw8,519
+decorator_parser-1.1.1.dist-info/METADATA,sha256=wZ_FJbxiRXsMww-DOLSoipDgCjHxaUzf1kWX0L8_AwM,4654
+decorator_parser-1.1.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+decorator_parser-1.1.1.dist-info/top_level.txt,sha256=wp3MzzKLv5-NNCQtdxjJPnk80INShwww5TfQfiIj95M,17
+decorator_parser-1.1.1.dist-info/RECORD,,
```

