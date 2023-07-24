# Comparing `tmp/adt-decorators-0.2.4.tar.gz` & `tmp/adt-decorators-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adt-decorators-0.2.4.tar", last modified: Mon Jul 24 23:15:52 2023, max compression
+gzip compressed data, was "adt-decorators-0.2.5.tar", last modified: Mon Jul 24 23:33:23 2023, max compression
```

## Comparing `adt-decorators-0.2.4.tar` & `adt-decorators-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:15:52.900170 adt-decorators-0.2.4/
--rw-r--r--   0 m0rphism  (1000) users      (100)     1296 2023-07-24 10:44:17.000000 adt-decorators-0.2.4/LICENSE
--rw-r--r--   0 m0rphism  (1000) users      (100)       69 2023-07-24 11:00:38.000000 adt-decorators-0.2.4/MANIFEST.in
--rw-r--r--   0 m0rphism  (1000) users      (100)     6028 2023-07-24 23:15:52.900170 adt-decorators-0.2.4/PKG-INFO
--rw-r--r--   0 m0rphism  (1000) users      (100)     5854 2023-07-24 23:12:37.000000 adt-decorators-0.2.4/README.md
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:15:52.900170 adt-decorators-0.2.4/adt/
--rw-r--r--   0 m0rphism  (1000) users      (100)     4879 2023-07-24 23:14:57.000000 adt-decorators-0.2.4/adt/__init__.py
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:15:52.900170 adt-decorators-0.2.4/adt_decorators.egg-info/
--rw-r--r--   0 m0rphism  (1000) users      (100)     6028 2023-07-24 23:15:52.000000 adt-decorators-0.2.4/adt_decorators.egg-info/PKG-INFO
--rw-r--r--   0 m0rphism  (1000) users      (100)      252 2023-07-24 23:15:52.000000 adt-decorators-0.2.4/adt_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)        1 2023-07-24 23:15:52.000000 adt-decorators-0.2.4/adt_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)        4 2023-07-24 23:15:52.000000 adt-decorators-0.2.4/adt_decorators.egg-info/top_level.txt
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:15:52.900170 adt-decorators-0.2.4/docs/
--rw-r--r--   0 m0rphism  (1000) users      (100)     5854 2023-07-24 23:12:37.000000 adt-decorators-0.2.4/docs/overview.md
--rw-r--r--   0 m0rphism  (1000) users      (100)       25 2023-07-24 08:09:40.000000 adt-decorators-0.2.4/docs/reference.md
--rw-r--r--   0 m0rphism  (1000) users      (100)      317 2023-07-24 08:51:28.000000 adt-decorators-0.2.4/mkdocs.yml
--rw-r--r--   0 m0rphism  (1000) users      (100)       38 2023-07-24 23:15:52.900170 adt-decorators-0.2.4/setup.cfg
--rw-r--r--   0 m0rphism  (1000) users      (100)      828 2023-07-24 23:15:28.000000 adt-decorators-0.2.4/setup.py
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:33:23.347318 adt-decorators-0.2.5/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     1296 2023-07-24 10:44:17.000000 adt-decorators-0.2.5/LICENSE
+-rw-r--r--   0 m0rphism  (1000) users      (100)       69 2023-07-24 11:00:38.000000 adt-decorators-0.2.5/MANIFEST.in
+-rw-r--r--   0 m0rphism  (1000) users      (100)     6016 2023-07-24 23:33:23.347318 adt-decorators-0.2.5/PKG-INFO
+-rw-r--r--   0 m0rphism  (1000) users      (100)     5842 2023-07-24 23:33:04.000000 adt-decorators-0.2.5/README.md
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:33:23.347318 adt-decorators-0.2.5/adt/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     4879 2023-07-24 23:32:14.000000 adt-decorators-0.2.5/adt/__init__.py
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:33:23.347318 adt-decorators-0.2.5/adt_decorators.egg-info/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     6016 2023-07-24 23:33:23.000000 adt-decorators-0.2.5/adt_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 m0rphism  (1000) users      (100)      252 2023-07-24 23:33:23.000000 adt-decorators-0.2.5/adt_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 m0rphism  (1000) users      (100)        1 2023-07-24 23:33:23.000000 adt-decorators-0.2.5/adt_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 m0rphism  (1000) users      (100)        4 2023-07-24 23:33:23.000000 adt-decorators-0.2.5/adt_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:33:23.347318 adt-decorators-0.2.5/docs/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     5842 2023-07-24 23:33:04.000000 adt-decorators-0.2.5/docs/overview.md
+-rw-r--r--   0 m0rphism  (1000) users      (100)       25 2023-07-24 08:09:40.000000 adt-decorators-0.2.5/docs/reference.md
+-rw-r--r--   0 m0rphism  (1000) users      (100)      317 2023-07-24 08:51:28.000000 adt-decorators-0.2.5/mkdocs.yml
+-rw-r--r--   0 m0rphism  (1000) users      (100)       38 2023-07-24 23:33:23.347318 adt-decorators-0.2.5/setup.cfg
+-rw-r--r--   0 m0rphism  (1000) users      (100)      828 2023-07-24 23:32:22.000000 adt-decorators-0.2.5/setup.py
```

### Comparing `adt-decorators-0.2.4/LICENSE` & `adt-decorators-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adt-decorators-0.2.4/PKG-INFO` & `adt-decorators-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-decorators
-Version: 0.2.4
+Version: 0.2.5
 Summary: Algebraic Data Types via Class Decorators
 Home-page: https://github.com/m0rphism/adt-decorators
 Author: Hannes Saffrich
 Author-email: saffrich@informatik.uni-freiburg.de
 License: BSD 2-clause
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -54,15 +54,15 @@
     - Constructors with no fields, are specified as the empty list.
 
 - **Getters, Setters, and Instance-Checking** methods are derived as an alternative to pattern matching, e.g.
   ```python
   if event.is_mouse_click():
       print(f"Clicked at ({event._1}, {event._2}).")
   elif event.is_key_press():
-      print(f"Pressed key {event.key}.mods}.")
+      print(f"Pressed key {event.key}.")
   ```
 
 - **Constructors are dataclasses that inherit from the decorated type.**
   The [`dataclass`](https://docs.python.org/3/library/dataclasses.html)
   decorator derives many useful method implementations,
   e.g. structural equality and string-conversion.
   Making the constructors inherit from the decorated class, allows to
@@ -73,15 +73,15 @@
   class Event:
       MouseClick: [int, int]
       KeyPress:   {'key': str, 'modifiers': list[str]}
       
       def print(self):
           match self:
               MouseClick(x, y):    print(f"Clicked at ({event._1}, {event._2}).")
-              KeyPress(key, mods): print(f"Pressed key {event.key}.mods}.")
+              KeyPress(key, mods): print(f"Pressed key {event.key}.")
 
   Event.MouseClick(5, 10).print()
   ```
 
 - **Constructors can be exported into the global namespace.**
   ```python
   @adt(export=True)  # <-- Makes `Event.` prefixes optional for constructors.
```

### Comparing `adt-decorators-0.2.4/README.md` & `adt-decorators-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     - Constructors with no fields, are specified as the empty list.
 
 - **Getters, Setters, and Instance-Checking** methods are derived as an alternative to pattern matching, e.g.
   ```python
   if event.is_mouse_click():
       print(f"Clicked at ({event._1}, {event._2}).")
   elif event.is_key_press():
-      print(f"Pressed key {event.key}.mods}.")
+      print(f"Pressed key {event.key}.")
   ```
 
 - **Constructors are dataclasses that inherit from the decorated type.**
   The [`dataclass`](https://docs.python.org/3/library/dataclasses.html)
   decorator derives many useful method implementations,
   e.g. structural equality and string-conversion.
   Making the constructors inherit from the decorated class, allows to
@@ -69,15 +69,15 @@
   class Event:
       MouseClick: [int, int]
       KeyPress:   {'key': str, 'modifiers': list[str]}
       
       def print(self):
           match self:
               MouseClick(x, y):    print(f"Clicked at ({event._1}, {event._2}).")
-              KeyPress(key, mods): print(f"Pressed key {event.key}.mods}.")
+              KeyPress(key, mods): print(f"Pressed key {event.key}.")
 
   Event.MouseClick(5, 10).print()
   ```
 
 - **Constructors can be exported into the global namespace.**
   ```python
   @adt(export=True)  # <-- Makes `Event.` prefixes optional for constructors.
```

### Comparing `adt-decorators-0.2.4/adt/__init__.py` & `adt-decorators-0.2.5/adt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Provides class decorators for Algebraic Data Types (ADTs)
 """
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 __author__ = 'Hannes Saffrich'
 
 from dataclasses import dataclass
 import inspect
 
 def adt(Class=None, export=False):
     """Class-decorator for Algebraic Data Types (ADTs).
```

### Comparing `adt-decorators-0.2.4/adt_decorators.egg-info/PKG-INFO` & `adt-decorators-0.2.5/adt_decorators.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-decorators
-Version: 0.2.4
+Version: 0.2.5
 Summary: Algebraic Data Types via Class Decorators
 Home-page: https://github.com/m0rphism/adt-decorators
 Author: Hannes Saffrich
 Author-email: saffrich@informatik.uni-freiburg.de
 License: BSD 2-clause
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -54,15 +54,15 @@
     - Constructors with no fields, are specified as the empty list.
 
 - **Getters, Setters, and Instance-Checking** methods are derived as an alternative to pattern matching, e.g.
   ```python
   if event.is_mouse_click():
       print(f"Clicked at ({event._1}, {event._2}).")
   elif event.is_key_press():
-      print(f"Pressed key {event.key}.mods}.")
+      print(f"Pressed key {event.key}.")
   ```
 
 - **Constructors are dataclasses that inherit from the decorated type.**
   The [`dataclass`](https://docs.python.org/3/library/dataclasses.html)
   decorator derives many useful method implementations,
   e.g. structural equality and string-conversion.
   Making the constructors inherit from the decorated class, allows to
@@ -73,15 +73,15 @@
   class Event:
       MouseClick: [int, int]
       KeyPress:   {'key': str, 'modifiers': list[str]}
       
       def print(self):
           match self:
               MouseClick(x, y):    print(f"Clicked at ({event._1}, {event._2}).")
-              KeyPress(key, mods): print(f"Pressed key {event.key}.mods}.")
+              KeyPress(key, mods): print(f"Pressed key {event.key}.")
 
   Event.MouseClick(5, 10).print()
   ```
 
 - **Constructors can be exported into the global namespace.**
   ```python
   @adt(export=True)  # <-- Makes `Event.` prefixes optional for constructors.
```

### Comparing `adt-decorators-0.2.4/docs/overview.md` & `adt-decorators-0.2.5/docs/overview.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     - Constructors with no fields, are specified as the empty list.
 
 - **Getters, Setters, and Instance-Checking** methods are derived as an alternative to pattern matching, e.g.
   ```python
   if event.is_mouse_click():
       print(f"Clicked at ({event._1}, {event._2}).")
   elif event.is_key_press():
-      print(f"Pressed key {event.key}.mods}.")
+      print(f"Pressed key {event.key}.")
   ```
 
 - **Constructors are dataclasses that inherit from the decorated type.**
   The [`dataclass`](https://docs.python.org/3/library/dataclasses.html)
   decorator derives many useful method implementations,
   e.g. structural equality and string-conversion.
   Making the constructors inherit from the decorated class, allows to
@@ -69,15 +69,15 @@
   class Event:
       MouseClick: [int, int]
       KeyPress:   {'key': str, 'modifiers': list[str]}
       
       def print(self):
           match self:
               MouseClick(x, y):    print(f"Clicked at ({event._1}, {event._2}).")
-              KeyPress(key, mods): print(f"Pressed key {event.key}.mods}.")
+              KeyPress(key, mods): print(f"Pressed key {event.key}.")
 
   Event.MouseClick(5, 10).print()
   ```
 
 - **Constructors can be exported into the global namespace.**
   ```python
   @adt(export=True)  # <-- Makes `Event.` prefixes optional for constructors.
```

### Comparing `adt-decorators-0.2.4/setup.py` & `adt-decorators-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     skip_end = "[//]: # (INSTALL_END)"
     begin = desc.find(skip_start)
     end = desc.find(skip_end) + len(skip_end)
     desc = desc[:begin] + desc[end:]
 
 setup(
     name='adt-decorators',
-    version='0.2.4',
+    version='0.2.5',
     description='Algebraic Data Types via Class Decorators',
     long_description=desc,
     long_description_content_type='text/markdown',
     url='https://github.com/m0rphism/adt-decorators',
     author='Hannes Saffrich',
     author_email='saffrich@informatik.uni-freiburg.de',
     license='BSD 2-clause',
```

