# Comparing `tmp/decorator_parser-1.0.9-py3-none-any.whl.zip` & `tmp/decorator_parser-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5763 bytes, number of entries: 9
+Zip file size: 6064 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       60 b- defN 23-Jul-08 10:47 decorator_parser/__init__.py
 -rw-r--r--  2.0 unx     1110 b- defN 23-Jul-08 10:42 decorator_parser/errors.py
--rw-r--r--  2.0 unx     4226 b- defN 23-Jul-08 10:32 decorator_parser/parse.py
--rw-r--r--  2.0 unx      240 b- defN 23-Jun-25 15:50 decorator_parser/utils.py
--rw-r--r--  2.0 unx      519 b- defN 23-Jul-08 10:48 decorator_parser-1.0.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     4165 b- defN 23-Jul-08 10:48 decorator_parser-1.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 10:48 decorator_parser-1.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jul-08 10:48 decorator_parser-1.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      759 b- defN 23-Jul-08 10:48 decorator_parser-1.0.9.dist-info/RECORD
-9 files, 11188 bytes uncompressed, 4441 bytes compressed:  60.3%
+-rw-r--r--  2.0 unx     4940 b- defN 23-Jul-25 19:10 decorator_parser/parse.py
+-rw-r--r--  2.0 unx      261 b- defN 23-Jul-23 15:49 decorator_parser/utils.py
+-rw-r--r--  2.0 unx      519 b- defN 23-Jul-25 19:15 decorator_parser-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4654 b- defN 23-Jul-25 19:15 decorator_parser-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 19:15 decorator_parser-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-25 19:15 decorator_parser-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      759 b- defN 23-Jul-25 19:15 decorator_parser-1.1.0.dist-info/RECORD
+9 files, 12412 bytes uncompressed, 4742 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: decorator_parser/parse.py
 Comment: 
 
 Filename: decorator_parser/utils.py
 Comment: 
 
-Filename: decorator_parser-1.0.9.dist-info/LICENSE
+Filename: decorator_parser-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: decorator_parser-1.0.9.dist-info/METADATA
+Filename: decorator_parser-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: decorator_parser-1.0.9.dist-info/WHEEL
+Filename: decorator_parser-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: decorator_parser-1.0.9.dist-info/top_level.txt
+Filename: decorator_parser-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: decorator_parser-1.0.9.dist-info/RECORD
+Filename: decorator_parser-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## decorator_parser/parse.py

```diff
@@ -1,26 +1,49 @@
 # Author: Michał Kostyk for Smartschool Inc.
 # Date: 2023
 # Version: 1.0.6
 
-from decorator_parser.utils import *
-from decorator_parser.errors import *
+from decorators_parser.utils import *
+from decorators_parser.errors import *
 import re
 
 
 class Parser:
-    def __init__(self, constraints={}):
+    def __init__(self, constraints={}, ignored={}):
         for key in constraints:
             if not 'regex' in constraints[key] or not 'description' in constraints[key]:
                 raise InvalidConstraintException(f"Invalid constraint for '{key}'")
 
         self.constraints = constraints
+        self.ignored = ignored
         pass
-        
+    
+
+    def parse_ignored(self, data):
+        for ignored_tag in self.ignored:
+            regex = r"(@" + re.escape(ignored_tag) + r")"
+            ignored_decorators = re.findall(regex, data)
+
+            if len(ignored_decorators) == 0:
+                continue
+            
+            decor = ignored_decorators[0]
+            decor_no_first = decor[1:]
+            data = data.replace(decor, MAGIC_CHAR + decor_no_first)
+
+        return data
 
+
+    def restore_ignored(self, result):
+        for key in result:
+            result[key] = result[key].replace(MAGIC_CHAR, "@")
+
+        return result
+    
+    
     # Parse @global decorators
     def parse_global(self, data):
         global_decorators = re.findall(r'(@global\-[^\n]*)', data)
         if len(global_decorators) == 0:
             return data, {}
         
         # Removing decorators from data
@@ -105,25 +128,28 @@
                 # Handle decorator and remove it from data
                 result = self.handle_decorator(data, result)
             except DecoratorNotFoundException:
                 # No more decorators found
                 break
             
             data = self.remove_decorator(data)
-        return result
+
+        return self.restore_ignored(result)
 
 
     # Main function for parsing file
     def parse_file(self, path):
         with open(path, 'r') as f:
             data = f.read()
 
         # Save original data for error line messages
         self.original_data = data
 
+        data = self.parse_ignored(data)
+
         # Parse global decorators
         data, global_dec = self.parse_global(data)
 
         # Split file by @new decorator
         data = self.split_by_new(data)
 
         results_list = []
```

## decorator_parser/utils.py

```diff
@@ -3,8 +3,10 @@
 # Version: 1.0.3
 # Description: Utility functions and constants used in other scripts.
 
 FAIL = '\033[91m'
 ENDC = '\033[0m'
 OKGREEN = '\033[92m'
 WARNING = '\033[93m'
-BOLD = '\033[1m'
+BOLD = '\033[1m'
+
+MAGIC_CHAR = '\007'
```

## Comparing `decorator_parser-1.0.9.dist-info/LICENSE` & `decorator_parser-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `decorator_parser-1.0.9.dist-info/METADATA` & `decorator_parser-1.1.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorator-parser
-Version: 1.0.9
+Version: 1.1.0
 Summary: Parser for text files with decorators into Python dictionaries
 Author-email: Michal Kostyk <m.kostyk22@gmail.com>
 Project-URL: Homepage, https://github.com/mkostyk/decorators-parser
 Project-URL: Bug Tracker, https://github.com/mkostyk/decorators-parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -172,7 +172,36 @@
 The output will be:
 ```python
 [
     {
         'correct': '1'
     }
 ]
+```
+
+### Ignored decorators
+
+If you need to use @ symbol for something else than decorator, you can specify
+names to exclude from the search
+
+#### Example:
+task.txt:
+```
+@question
+Some long question with @ref in it
+```
+
+run.py:
+```python
+from decorator_parser.parse import Parser
+task_parser = Parser(ignored=['ref'])
+print(task_parser.parse_file('task.txt'))
+```
+
+Will result in the following output:
+```python
+[
+    {
+        'question': 'Some long question with @ref in it'
+    }
+]
+```
```

## Comparing `decorator_parser-1.0.9.dist-info/RECORD` & `decorator_parser-1.1.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 decorator_parser/__init__.py,sha256=sx_Okl3ziNpfIbGs_KLWLPdjBV8eL9Zt75nuzErpq9g,60
 decorator_parser/errors.py,sha256=GefbMbWrJ6yVR-WK-34XbICH31wZKwLzAbwrfZW4vy8,1110
-decorator_parser/parse.py,sha256=3P_SJ-exiEmrfVZxXB5cWEDt6WZzZg0muDSSJBPb5gU,4226
-decorator_parser/utils.py,sha256=83D2giM9d645tGZDPI27sWRN-zkiJn82CYHbPDBlqbA,240
-decorator_parser-1.0.9.dist-info/LICENSE,sha256=d0IchUxRoZd6yiEkgwlRF6MEDtdQLuG3CiDQolTTkw8,519
-decorator_parser-1.0.9.dist-info/METADATA,sha256=eqI2dJ46uk4HUCJ6cQNyvrr5mS4e8gRWlRYgGO9Vkns,4165
-decorator_parser-1.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-decorator_parser-1.0.9.dist-info/top_level.txt,sha256=wp3MzzKLv5-NNCQtdxjJPnk80INShwww5TfQfiIj95M,17
-decorator_parser-1.0.9.dist-info/RECORD,,
+decorator_parser/parse.py,sha256=j5mdPTUiSo6EuqCL35zVi0SszeQh_8cGxe1WUjEJ3u8,4940
+decorator_parser/utils.py,sha256=yc1RCfV_pANGU2NofvcDPTrUzgEcInelaqEfGphgJe0,261
+decorator_parser-1.1.0.dist-info/LICENSE,sha256=d0IchUxRoZd6yiEkgwlRF6MEDtdQLuG3CiDQolTTkw8,519
+decorator_parser-1.1.0.dist-info/METADATA,sha256=uD2oJ9lIm3mEgyknENmBcRqR2NF3FwcxakfiNEqmRJg,4654
+decorator_parser-1.1.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+decorator_parser-1.1.0.dist-info/top_level.txt,sha256=wp3MzzKLv5-NNCQtdxjJPnk80INShwww5TfQfiIj95M,17
+decorator_parser-1.1.0.dist-info/RECORD,,
```

