# Comparing `tmp/adt-decorators-0.2.0.tar.gz` & `tmp/adt-decorators-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adt-decorators-0.2.0.tar", last modified: Mon Jul 24 22:21:10 2023, max compression
+gzip compressed data, was "adt-decorators-0.2.1.tar", last modified: Mon Jul 24 22:28:03 2023, max compression
```

## Comparing `adt-decorators-0.2.0.tar` & `adt-decorators-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 22:21:10.651898 adt-decorators-0.2.0/
--rw-r--r--   0 m0rphism  (1000) users      (100)     1296 2023-07-24 10:44:17.000000 adt-decorators-0.2.0/LICENSE
--rw-r--r--   0 m0rphism  (1000) users      (100)       69 2023-07-24 11:00:38.000000 adt-decorators-0.2.0/MANIFEST.in
--rw-r--r--   0 m0rphism  (1000) users      (100)     5490 2023-07-24 22:21:10.651898 adt-decorators-0.2.0/PKG-INFO
--rw-r--r--   0 m0rphism  (1000) users      (100)     5066 2023-07-24 22:19:44.000000 adt-decorators-0.2.0/README.md
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 22:21:10.650898 adt-decorators-0.2.0/adt/
--rw-r--r--   0 m0rphism  (1000) users      (100)     4879 2023-07-24 22:20:39.000000 adt-decorators-0.2.0/adt/__init__.py
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 22:21:10.651898 adt-decorators-0.2.0/adt_decorators.egg-info/
--rw-r--r--   0 m0rphism  (1000) users      (100)     5490 2023-07-24 22:21:10.000000 adt-decorators-0.2.0/adt_decorators.egg-info/PKG-INFO
--rw-r--r--   0 m0rphism  (1000) users      (100)      252 2023-07-24 22:21:10.000000 adt-decorators-0.2.0/adt_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)        1 2023-07-24 22:21:10.000000 adt-decorators-0.2.0/adt_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)        4 2023-07-24 22:21:10.000000 adt-decorators-0.2.0/adt_decorators.egg-info/top_level.txt
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 22:21:10.651898 adt-decorators-0.2.0/docs/
--rw-r--r--   0 m0rphism  (1000) users      (100)     5066 2023-07-24 22:19:44.000000 adt-decorators-0.2.0/docs/overview.md
--rw-r--r--   0 m0rphism  (1000) users      (100)       25 2023-07-24 08:09:40.000000 adt-decorators-0.2.0/docs/reference.md
--rw-r--r--   0 m0rphism  (1000) users      (100)      317 2023-07-24 08:51:28.000000 adt-decorators-0.2.0/mkdocs.yml
--rw-r--r--   0 m0rphism  (1000) users      (100)       38 2023-07-24 22:21:10.651898 adt-decorators-0.2.0/setup.cfg
--rw-r--r--   0 m0rphism  (1000) users      (100)      633 2023-07-24 22:20:52.000000 adt-decorators-0.2.0/setup.py
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 22:28:03.270017 adt-decorators-0.2.1/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     1296 2023-07-24 10:44:17.000000 adt-decorators-0.2.1/LICENSE
+-rw-r--r--   0 m0rphism  (1000) users      (100)       69 2023-07-24 11:00:38.000000 adt-decorators-0.2.1/MANIFEST.in
+-rw-r--r--   0 m0rphism  (1000) users      (100)     5513 2023-07-24 22:28:03.270017 adt-decorators-0.2.1/PKG-INFO
+-rw-r--r--   0 m0rphism  (1000) users      (100)     5089 2023-07-24 22:27:02.000000 adt-decorators-0.2.1/README.md
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 22:28:03.270017 adt-decorators-0.2.1/adt/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     4879 2023-07-24 22:26:48.000000 adt-decorators-0.2.1/adt/__init__.py
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 22:28:03.270017 adt-decorators-0.2.1/adt_decorators.egg-info/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     5513 2023-07-24 22:28:03.000000 adt-decorators-0.2.1/adt_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 m0rphism  (1000) users      (100)      252 2023-07-24 22:28:03.000000 adt-decorators-0.2.1/adt_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 m0rphism  (1000) users      (100)        1 2023-07-24 22:28:03.000000 adt-decorators-0.2.1/adt_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 m0rphism  (1000) users      (100)        4 2023-07-24 22:28:03.000000 adt-decorators-0.2.1/adt_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 22:28:03.270017 adt-decorators-0.2.1/docs/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     5089 2023-07-24 22:27:02.000000 adt-decorators-0.2.1/docs/overview.md
+-rw-r--r--   0 m0rphism  (1000) users      (100)       25 2023-07-24 08:09:40.000000 adt-decorators-0.2.1/docs/reference.md
+-rw-r--r--   0 m0rphism  (1000) users      (100)      317 2023-07-24 08:51:28.000000 adt-decorators-0.2.1/mkdocs.yml
+-rw-r--r--   0 m0rphism  (1000) users      (100)       38 2023-07-24 22:28:03.270017 adt-decorators-0.2.1/setup.cfg
+-rw-r--r--   0 m0rphism  (1000) users      (100)      633 2023-07-24 22:26:44.000000 adt-decorators-0.2.1/setup.py
```

### Comparing `adt-decorators-0.2.0/LICENSE` & `adt-decorators-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adt-decorators-0.2.0/PKG-INFO` & `adt-decorators-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-decorators
-Version: 0.2.0
+Version: 0.2.1
 Summary: Algebraic Data Types via Class Decorators
 Home-page: https://github.com/m0rphism/adt-decorators
 Author: Hannes Saffrich
 Author-email: saffrich@informatik.uni-freiburg.de
 License: BSD 2-clause
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -23,14 +23,16 @@
 
 - **Simplicity.** This package exports only a single definition: the
   [`adt`](../reference/#adt.adt) class decorator.
 
 - **Concision.** Constructors are specified via class annotations,
   allowing for syntax comparable to Rust's `enum`s:
   ```python
+  from adt import adt
+
   @adt
   class Event:
       MouseClick: [int, int]
       KeyPress:   {'key': str, 'modifiers': list[str]}
   ```
 
 - **Pattern Matching.** Python's [pattern matching](https://peps.python.org/pep-0636/) via `match` is fully supported (Python >= 3.10).
```

### Comparing `adt-decorators-0.2.0/README.md` & `adt-decorators-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 - **Simplicity.** This package exports only a single definition: the
   [`adt`](../reference/#adt.adt) class decorator.
 
 - **Concision.** Constructors are specified via class annotations,
   allowing for syntax comparable to Rust's `enum`s:
   ```python
+  from adt import adt
+
   @adt
   class Event:
       MouseClick: [int, int]
       KeyPress:   {'key': str, 'modifiers': list[str]}
   ```
 
 - **Pattern Matching.** Python's [pattern matching](https://peps.python.org/pep-0636/) via `match` is fully supported (Python >= 3.10).
```

### Comparing `adt-decorators-0.2.0/adt/__init__.py` & `adt-decorators-0.2.1/adt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Provides class decorators for Algebraic Data Types (ADTs)
 """
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __author__ = 'Hannes Saffrich'
 
 from dataclasses import dataclass
 import inspect
 
 def adt(Class=None, export=False):
     """Class-decorator for Algebraic Data Types (ADTs).
```

### Comparing `adt-decorators-0.2.0/adt_decorators.egg-info/PKG-INFO` & `adt-decorators-0.2.1/adt_decorators.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-decorators
-Version: 0.2.0
+Version: 0.2.1
 Summary: Algebraic Data Types via Class Decorators
 Home-page: https://github.com/m0rphism/adt-decorators
 Author: Hannes Saffrich
 Author-email: saffrich@informatik.uni-freiburg.de
 License: BSD 2-clause
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -23,14 +23,16 @@
 
 - **Simplicity.** This package exports only a single definition: the
   [`adt`](../reference/#adt.adt) class decorator.
 
 - **Concision.** Constructors are specified via class annotations,
   allowing for syntax comparable to Rust's `enum`s:
   ```python
+  from adt import adt
+
   @adt
   class Event:
       MouseClick: [int, int]
       KeyPress:   {'key': str, 'modifiers': list[str]}
   ```
 
 - **Pattern Matching.** Python's [pattern matching](https://peps.python.org/pep-0636/) via `match` is fully supported (Python >= 3.10).
```

### Comparing `adt-decorators-0.2.0/docs/overview.md` & `adt-decorators-0.2.1/docs/overview.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 - **Simplicity.** This package exports only a single definition: the
   [`adt`](../reference/#adt.adt) class decorator.
 
 - **Concision.** Constructors are specified via class annotations,
   allowing for syntax comparable to Rust's `enum`s:
   ```python
+  from adt import adt
+
   @adt
   class Event:
       MouseClick: [int, int]
       KeyPress:   {'key': str, 'modifiers': list[str]}
   ```
 
 - **Pattern Matching.** Python's [pattern matching](https://peps.python.org/pep-0636/) via `match` is fully supported (Python >= 3.10).
```

### Comparing `adt-decorators-0.2.0/setup.py` & `adt-decorators-0.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('docs/overview.md', 'r') as f:
     desc = f.read()
 
 setup(
     name='adt-decorators',
-    version='0.2.0',    
+    version='0.2.1',    
     description='Algebraic Data Types via Class Decorators',
     long_description=desc,
     long_description_content_type='text/markdown',
     url='https://github.com/m0rphism/adt-decorators',
     author='Hannes Saffrich',
     author_email='saffrich@informatik.uni-freiburg.de',
     license='BSD 2-clause',
```

