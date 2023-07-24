# Comparing `tmp/adt-decorators-0.2.7.tar.gz` & `tmp/adt-decorators-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adt-decorators-0.2.7.tar", last modified: Mon Jul 24 23:37:43 2023, max compression
+gzip compressed data, was "adt-decorators-0.2.8.tar", last modified: Mon Jul 24 23:39:55 2023, max compression
```

## Comparing `adt-decorators-0.2.7.tar` & `adt-decorators-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:37:43.091555 adt-decorators-0.2.7/
--rw-r--r--   0 m0rphism  (1000) users      (100)     1296 2023-07-24 10:44:17.000000 adt-decorators-0.2.7/LICENSE
--rw-r--r--   0 m0rphism  (1000) users      (100)       69 2023-07-24 11:00:38.000000 adt-decorators-0.2.7/MANIFEST.in
--rw-r--r--   0 m0rphism  (1000) users      (100)     6048 2023-07-24 23:37:43.091555 adt-decorators-0.2.7/PKG-INFO
--rw-r--r--   0 m0rphism  (1000) users      (100)     5874 2023-07-24 23:37:35.000000 adt-decorators-0.2.7/README.md
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:37:43.090555 adt-decorators-0.2.7/adt/
--rw-r--r--   0 m0rphism  (1000) users      (100)     4879 2023-07-24 23:37:25.000000 adt-decorators-0.2.7/adt/__init__.py
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:37:43.090555 adt-decorators-0.2.7/adt_decorators.egg-info/
--rw-r--r--   0 m0rphism  (1000) users      (100)     6048 2023-07-24 23:37:43.000000 adt-decorators-0.2.7/adt_decorators.egg-info/PKG-INFO
--rw-r--r--   0 m0rphism  (1000) users      (100)      252 2023-07-24 23:37:43.000000 adt-decorators-0.2.7/adt_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)        1 2023-07-24 23:37:43.000000 adt-decorators-0.2.7/adt_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)        4 2023-07-24 23:37:43.000000 adt-decorators-0.2.7/adt_decorators.egg-info/top_level.txt
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:37:43.091555 adt-decorators-0.2.7/docs/
--rw-r--r--   0 m0rphism  (1000) users      (100)     5874 2023-07-24 23:37:35.000000 adt-decorators-0.2.7/docs/overview.md
--rw-r--r--   0 m0rphism  (1000) users      (100)       25 2023-07-24 08:09:40.000000 adt-decorators-0.2.7/docs/reference.md
--rw-r--r--   0 m0rphism  (1000) users      (100)      317 2023-07-24 08:51:28.000000 adt-decorators-0.2.7/mkdocs.yml
--rw-r--r--   0 m0rphism  (1000) users      (100)       38 2023-07-24 23:37:43.091555 adt-decorators-0.2.7/setup.cfg
--rw-r--r--   0 m0rphism  (1000) users      (100)      828 2023-07-24 23:37:26.000000 adt-decorators-0.2.7/setup.py
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:39:55.787684 adt-decorators-0.2.8/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     1296 2023-07-24 10:44:17.000000 adt-decorators-0.2.8/LICENSE
+-rw-r--r--   0 m0rphism  (1000) users      (100)       69 2023-07-24 11:00:38.000000 adt-decorators-0.2.8/MANIFEST.in
+-rw-r--r--   0 m0rphism  (1000) users      (100)     6046 2023-07-24 23:39:55.787684 adt-decorators-0.2.8/PKG-INFO
+-rw-r--r--   0 m0rphism  (1000) users      (100)     5872 2023-07-24 23:39:35.000000 adt-decorators-0.2.8/README.md
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:39:55.786684 adt-decorators-0.2.8/adt/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     4879 2023-07-24 23:39:38.000000 adt-decorators-0.2.8/adt/__init__.py
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:39:55.787684 adt-decorators-0.2.8/adt_decorators.egg-info/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     6046 2023-07-24 23:39:55.000000 adt-decorators-0.2.8/adt_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 m0rphism  (1000) users      (100)      252 2023-07-24 23:39:55.000000 adt-decorators-0.2.8/adt_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 m0rphism  (1000) users      (100)        1 2023-07-24 23:39:55.000000 adt-decorators-0.2.8/adt_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 m0rphism  (1000) users      (100)        4 2023-07-24 23:39:55.000000 adt-decorators-0.2.8/adt_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:39:55.787684 adt-decorators-0.2.8/docs/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     5872 2023-07-24 23:39:35.000000 adt-decorators-0.2.8/docs/overview.md
+-rw-r--r--   0 m0rphism  (1000) users      (100)       25 2023-07-24 08:09:40.000000 adt-decorators-0.2.8/docs/reference.md
+-rw-r--r--   0 m0rphism  (1000) users      (100)      317 2023-07-24 08:51:28.000000 adt-decorators-0.2.8/mkdocs.yml
+-rw-r--r--   0 m0rphism  (1000) users      (100)       38 2023-07-24 23:39:55.787684 adt-decorators-0.2.8/setup.cfg
+-rw-r--r--   0 m0rphism  (1000) users      (100)      828 2023-07-24 23:39:42.000000 adt-decorators-0.2.8/setup.py
```

### Comparing `adt-decorators-0.2.7/LICENSE` & `adt-decorators-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adt-decorators-0.2.7/PKG-INFO` & `adt-decorators-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-decorators
-Version: 0.2.7
+Version: 0.2.8
 Summary: Algebraic Data Types via Class Decorators
 Home-page: https://github.com/m0rphism/adt-decorators
 Author: Hannes Saffrich
 Author-email: saffrich@informatik.uni-freiburg.de
 License: BSD 2-clause
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -46,16 +46,16 @@
       case Event.KeyPress(key, mods): print(f"Pressed key {key}.")
   ```
 
 -   **Named and unnamed constructor fields** are supported:
 
     - Constructors with named fields, like `KeyPress`, are specified as a `dict[str, type]`;
     - Constructors with unnamed fields, like `MouseClick`,  are specified as a `list[type]`;
-    - Constructors with a single unnamed field, can also be specified as a `type`;
-    - Constructors with no fields, are specified as the empty list.
+    - Constructors with a single unnamed field can also be specified as a `type`;
+    - Constructors with no fields are specified as the empty list.
 
 - **Getters, Setters, and Instance-Checking** methods are derived as an alternative to pattern matching, e.g.
   ```python
   if event.is_mouse_click():
       print(f"Clicked at ({event._1}, {event._2}).")
   elif event.is_key_press():
       print(f"Pressed key {event.key}.")
```

### Comparing `adt-decorators-0.2.7/README.md` & `adt-decorators-0.2.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,16 @@
       case Event.KeyPress(key, mods): print(f"Pressed key {key}.")
   ```
 
 -   **Named and unnamed constructor fields** are supported:
 
     - Constructors with named fields, like `KeyPress`, are specified as a `dict[str, type]`;
     - Constructors with unnamed fields, like `MouseClick`,  are specified as a `list[type]`;
-    - Constructors with a single unnamed field, can also be specified as a `type`;
-    - Constructors with no fields, are specified as the empty list.
+    - Constructors with a single unnamed field can also be specified as a `type`;
+    - Constructors with no fields are specified as the empty list.
 
 - **Getters, Setters, and Instance-Checking** methods are derived as an alternative to pattern matching, e.g.
   ```python
   if event.is_mouse_click():
       print(f"Clicked at ({event._1}, {event._2}).")
   elif event.is_key_press():
       print(f"Pressed key {event.key}.")
```

### Comparing `adt-decorators-0.2.7/adt/__init__.py` & `adt-decorators-0.2.8/adt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Provides class decorators for Algebraic Data Types (ADTs)
 """
 
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 __author__ = 'Hannes Saffrich'
 
 from dataclasses import dataclass
 import inspect
 
 def adt(Class=None, export=False):
     """Class-decorator for Algebraic Data Types (ADTs).
```

### Comparing `adt-decorators-0.2.7/adt_decorators.egg-info/PKG-INFO` & `adt-decorators-0.2.8/adt_decorators.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-decorators
-Version: 0.2.7
+Version: 0.2.8
 Summary: Algebraic Data Types via Class Decorators
 Home-page: https://github.com/m0rphism/adt-decorators
 Author: Hannes Saffrich
 Author-email: saffrich@informatik.uni-freiburg.de
 License: BSD 2-clause
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -46,16 +46,16 @@
       case Event.KeyPress(key, mods): print(f"Pressed key {key}.")
   ```
 
 -   **Named and unnamed constructor fields** are supported:
 
     - Constructors with named fields, like `KeyPress`, are specified as a `dict[str, type]`;
     - Constructors with unnamed fields, like `MouseClick`,  are specified as a `list[type]`;
-    - Constructors with a single unnamed field, can also be specified as a `type`;
-    - Constructors with no fields, are specified as the empty list.
+    - Constructors with a single unnamed field can also be specified as a `type`;
+    - Constructors with no fields are specified as the empty list.
 
 - **Getters, Setters, and Instance-Checking** methods are derived as an alternative to pattern matching, e.g.
   ```python
   if event.is_mouse_click():
       print(f"Clicked at ({event._1}, {event._2}).")
   elif event.is_key_press():
       print(f"Pressed key {event.key}.")
```

### Comparing `adt-decorators-0.2.7/docs/overview.md` & `adt-decorators-0.2.8/docs/overview.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,16 @@
       case Event.KeyPress(key, mods): print(f"Pressed key {key}.")
   ```
 
 -   **Named and unnamed constructor fields** are supported:
 
     - Constructors with named fields, like `KeyPress`, are specified as a `dict[str, type]`;
     - Constructors with unnamed fields, like `MouseClick`,  are specified as a `list[type]`;
-    - Constructors with a single unnamed field, can also be specified as a `type`;
-    - Constructors with no fields, are specified as the empty list.
+    - Constructors with a single unnamed field can also be specified as a `type`;
+    - Constructors with no fields are specified as the empty list.
 
 - **Getters, Setters, and Instance-Checking** methods are derived as an alternative to pattern matching, e.g.
   ```python
   if event.is_mouse_click():
       print(f"Clicked at ({event._1}, {event._2}).")
   elif event.is_key_press():
       print(f"Pressed key {event.key}.")
```

### Comparing `adt-decorators-0.2.7/setup.py` & `adt-decorators-0.2.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     skip_end = "[//]: # (INSTALL_END)"
     begin = desc.find(skip_start)
     end = desc.find(skip_end) + len(skip_end)
     desc = desc[:begin] + desc[end:]
 
 setup(
     name='adt-decorators',
-    version='0.2.7',
+    version='0.2.8',
     description='Algebraic Data Types via Class Decorators',
     long_description=desc,
     long_description_content_type='text/markdown',
     url='https://github.com/m0rphism/adt-decorators',
     author='Hannes Saffrich',
     author_email='saffrich@informatik.uni-freiburg.de',
     license='BSD 2-clause',
```

