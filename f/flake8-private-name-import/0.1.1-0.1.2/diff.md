# Comparing `tmp/flake8_private_name_import-0.1.1.tar.gz` & `tmp/flake8_private_name_import-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flake8_private_name_import-0.1.1.tar", last modified: Tue Jul 25 20:54:32 2023, max compression
+gzip compressed data, was "dist/flake8_private_name_import-0.1.2.tar", last modified: Tue Jul 25 21:01:28 2023, max compression
```

## Comparing `flake8_private_name_import-0.1.1.tar` & `flake8_private_name_import-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-25 20:54:32.000000 flake8_private_name_import-0.1.1/
--rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-25 20:54:32.000000 flake8_private_name_import-0.1.1/PKG-INFO
--rw-rw-r--   0 rows      (1000) rows      (1000)       81 2023-07-25 20:19:44.000000 flake8_private_name_import-0.1.1/README.md
-drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-25 20:54:32.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/
--rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-25 20:54:31.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/PKG-INFO
--rw-rw-r--   0 rows      (1000) rows      (1000)      399 2023-07-25 20:54:32.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/SOURCES.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-25 20:54:31.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/dependency_links.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)       63 2023-07-25 20:54:31.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/entry_points.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-25 20:54:31.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/not-zip-safe
--rw-rw-r--   0 rows      (1000) rows      (1000)       29 2023-07-25 20:54:31.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/requires.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)       27 2023-07-25 20:54:31.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/top_level.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)     1395 2023-07-25 20:53:25.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.py
--rw-rw-r--   0 rows      (1000) rows      (1000)       38 2023-07-25 20:54:32.000000 flake8_private_name_import-0.1.1/setup.cfg
--rw-rw-r--   0 rows      (1000) rows      (1000)     1779 2023-07-25 20:51:33.000000 flake8_private_name_import-0.1.1/setup.py
+drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/PKG-INFO
+-rw-rw-r--   0 rows      (1000) rows      (1000)       81 2023-07-25 20:19:44.000000 flake8_private_name_import-0.1.2/README.md
+drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/PKG-INFO
+-rw-rw-r--   0 rows      (1000) rows      (1000)      399 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/SOURCES.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/dependency_links.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)       63 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/entry_points.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/not-zip-safe
+-rw-rw-r--   0 rows      (1000) rows      (1000)       29 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/requires.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)       27 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/top_level.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1383 2023-07-25 21:00:14.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.py
+-rw-rw-r--   0 rows      (1000) rows      (1000)       38 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/setup.cfg
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1779 2023-07-25 21:00:14.000000 flake8_private_name_import-0.1.2/setup.py
```

### Comparing `flake8_private_name_import-0.1.1/PKG-INFO` & `flake8_private_name_import-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8_private_name_import
-Version: 0.1.1
+Version: 0.1.2
 Summary: flake8 plugin that reports imports of private names
 Home-page: https://github.com/rows-s/flake8_private_name_import
 Author: Vladimir Marmuz
 Author-email: vladimir.rows@gmail.com
 License: MIT
 Description: flake8 plugin that reports imports of private names
 Keywords: python pep8 flake8 private import
```

### Comparing `flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/PKG-INFO` & `flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-private-name-import
-Version: 0.1.1
+Version: 0.1.2
 Summary: flake8 plugin that reports imports of private names
 Home-page: https://github.com/rows-s/flake8_private_name_import
 Author: Vladimir Marmuz
 Author-email: vladimir.rows@gmail.com
 License: MIT
 Description: flake8 plugin that reports imports of private names
 Keywords: python pep8 flake8 private import
```

### Comparing `flake8_private_name_import-0.1.1/flake8_private_name_import.py` & `flake8_private_name_import-0.1.2/flake8_private_name_import.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import _ast
 import ast
 from itertools import chain
 from typing import Any, Generator, Iterator, List, Tuple, Type
 
 
 class Visitor(ast.NodeVisitor):
     def __init__(self) -> None:
@@ -28,15 +27,15 @@
             for name in names
             if name.startswith('_')
         )
 
 
 class Plugin:
     name = __name__
-    version = '0.1.1'
+    version = '0.1.2'
 
     def __init__(self, tree: ast.AST) -> None:
         self._tree = tree
 
     def run(self) -> Generator[Tuple[int, int, str, Type[Any]], None, None]:
         visitor = Visitor()
         visitor.visit(self._tree)
```

### Comparing `flake8_private_name_import-0.1.1/setup.py` & `flake8_private_name_import-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='flake8_private_name_import',
-    version='0.1.1',
+    version='0.1.2',
     description="flake8 plugin that reports imports of private names",
     long_description="flake8 plugin that reports imports of private names",
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Framework :: Flake8',
```

