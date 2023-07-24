# Comparing `tmp/adt-decorators-0.2.8.tar.gz` & `tmp/adt-decorators-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adt-decorators-0.2.8.tar", last modified: Mon Jul 24 23:39:55 2023, max compression
+gzip compressed data, was "adt-decorators-0.2.9.tar", last modified: Mon Jul 24 23:53:01 2023, max compression
```

## Comparing `adt-decorators-0.2.8.tar` & `adt-decorators-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:39:55.787684 adt-decorators-0.2.8/
--rw-r--r--   0 m0rphism  (1000) users      (100)     1296 2023-07-24 10:44:17.000000 adt-decorators-0.2.8/LICENSE
--rw-r--r--   0 m0rphism  (1000) users      (100)       69 2023-07-24 11:00:38.000000 adt-decorators-0.2.8/MANIFEST.in
--rw-r--r--   0 m0rphism  (1000) users      (100)     6046 2023-07-24 23:39:55.787684 adt-decorators-0.2.8/PKG-INFO
--rw-r--r--   0 m0rphism  (1000) users      (100)     5872 2023-07-24 23:39:35.000000 adt-decorators-0.2.8/README.md
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:39:55.786684 adt-decorators-0.2.8/adt/
--rw-r--r--   0 m0rphism  (1000) users      (100)     4879 2023-07-24 23:39:38.000000 adt-decorators-0.2.8/adt/__init__.py
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:39:55.787684 adt-decorators-0.2.8/adt_decorators.egg-info/
--rw-r--r--   0 m0rphism  (1000) users      (100)     6046 2023-07-24 23:39:55.000000 adt-decorators-0.2.8/adt_decorators.egg-info/PKG-INFO
--rw-r--r--   0 m0rphism  (1000) users      (100)      252 2023-07-24 23:39:55.000000 adt-decorators-0.2.8/adt_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)        1 2023-07-24 23:39:55.000000 adt-decorators-0.2.8/adt_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)        4 2023-07-24 23:39:55.000000 adt-decorators-0.2.8/adt_decorators.egg-info/top_level.txt
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:39:55.787684 adt-decorators-0.2.8/docs/
--rw-r--r--   0 m0rphism  (1000) users      (100)     5872 2023-07-24 23:39:35.000000 adt-decorators-0.2.8/docs/overview.md
--rw-r--r--   0 m0rphism  (1000) users      (100)       25 2023-07-24 08:09:40.000000 adt-decorators-0.2.8/docs/reference.md
--rw-r--r--   0 m0rphism  (1000) users      (100)      317 2023-07-24 08:51:28.000000 adt-decorators-0.2.8/mkdocs.yml
--rw-r--r--   0 m0rphism  (1000) users      (100)       38 2023-07-24 23:39:55.787684 adt-decorators-0.2.8/setup.cfg
--rw-r--r--   0 m0rphism  (1000) users      (100)      828 2023-07-24 23:39:42.000000 adt-decorators-0.2.8/setup.py
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:53:01.623330 adt-decorators-0.2.9/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     1296 2023-07-24 10:44:17.000000 adt-decorators-0.2.9/LICENSE
+-rw-r--r--   0 m0rphism  (1000) users      (100)       69 2023-07-24 11:00:38.000000 adt-decorators-0.2.9/MANIFEST.in
+-rw-r--r--   0 m0rphism  (1000) users      (100)     6383 2023-07-24 23:53:01.623330 adt-decorators-0.2.9/PKG-INFO
+-rw-r--r--   0 m0rphism  (1000) users      (100)     6209 2023-07-24 23:51:45.000000 adt-decorators-0.2.9/README.md
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:53:01.622330 adt-decorators-0.2.9/adt/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     4960 2023-07-24 23:52:36.000000 adt-decorators-0.2.9/adt/__init__.py
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:53:01.622330 adt-decorators-0.2.9/adt_decorators.egg-info/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     6383 2023-07-24 23:53:01.000000 adt-decorators-0.2.9/adt_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 m0rphism  (1000) users      (100)      252 2023-07-24 23:53:01.000000 adt-decorators-0.2.9/adt_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 m0rphism  (1000) users      (100)        1 2023-07-24 23:53:01.000000 adt-decorators-0.2.9/adt_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 m0rphism  (1000) users      (100)        4 2023-07-24 23:53:01.000000 adt-decorators-0.2.9/adt_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:53:01.622330 adt-decorators-0.2.9/docs/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     6209 2023-07-24 23:51:45.000000 adt-decorators-0.2.9/docs/overview.md
+-rw-r--r--   0 m0rphism  (1000) users      (100)       25 2023-07-24 08:09:40.000000 adt-decorators-0.2.9/docs/reference.md
+-rw-r--r--   0 m0rphism  (1000) users      (100)      317 2023-07-24 08:51:28.000000 adt-decorators-0.2.9/mkdocs.yml
+-rw-r--r--   0 m0rphism  (1000) users      (100)       38 2023-07-24 23:53:01.623330 adt-decorators-0.2.9/setup.cfg
+-rw-r--r--   0 m0rphism  (1000) users      (100)      828 2023-07-24 23:52:41.000000 adt-decorators-0.2.9/setup.py
```

### Comparing `adt-decorators-0.2.8/LICENSE` & `adt-decorators-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adt-decorators-0.2.8/PKG-INFO` & `adt-decorators-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-decorators
-Version: 0.2.8
+Version: 0.2.9
 Summary: Algebraic Data Types via Class Decorators
 Home-page: https://github.com/m0rphism/adt-decorators
 Author: Hannes Saffrich
 Author-email: saffrich@informatik.uni-freiburg.de
 License: BSD 2-clause
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -91,14 +91,21 @@
       
       def print(self):
           match self:
               case MouseClick(x, y):    ... # <-- As promised: no `Event.MouseClick`!
               case KeyPress(key, mods): ... # <-- As promised: no `Event.KeyPress`!
   ```
 
+- **Reflection.**
+  The decorated class has a static field `constructors: dict[str, type]`
+  which maps the constructor names to their classes, e.g.
+  ```python
+  key_event = Event.constructors['KeyPress'](key='a', modifiers=['shift'])
+  ```
+
 
 ## Translation
 
 The code generated in the above example by the `adt` decorator for the
 `Event` ADT behaves equivalent to the following code, with the
 exception that the constructor classes are constructed anonymously, so
 the global namespace is not even temporarily polluted unless
@@ -129,14 +136,19 @@
   modifiers: list[str]
 
 Event.MouseClick = MouseClick
 Event.KeyPress   = KeyPress
 if not export:
     del MouseClick
     del KeyPress
+
+Event.constructors = {
+    'MouseClick': Event.MouseClick,
+    'KeyPress': Event.KeyPress,
+}
 ```
 
 ## Related packages
 
 The following compares this package to packages which aim to provide similar functionality:
 
 - [`algebraic-data-types`](https://pypi.org/project/algebraic-data-types/)
```

### Comparing `adt-decorators-0.2.8/README.md` & `adt-decorators-0.2.9/adt_decorators.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+Metadata-Version: 2.1
+Name: adt-decorators
+Version: 0.2.9
+Summary: Algebraic Data Types via Class Decorators
+Home-page: https://github.com/m0rphism/adt-decorators
+Author: Hannes Saffrich
+Author-email: saffrich@informatik.uni-freiburg.de
+License: BSD 2-clause
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Overview
 
 This package provides a class decorator for defining
 *[Algebraic Data Types (ADTs)](https://en.wikipedia.org/wiki/Algebraic_data_type)* as known from
 [Haskell](https://wiki.haskell.org/Algebraic_data_type) (`data`),
 [OCaml](https://cs3110.github.io/textbook/chapters/data/algebraic_data_types.html) (`type`), and
 [Rust](https://doc.rust-lang.org/book/ch06-01-defining-an-enum.html) (`enum`).
 
-[//]: # (INSTALL_BEGIN)
-## Installation
 
-The package is on [PyPI](https://pypi.org/project/adt-decorators/)
-and [github](https://github.com/m0rphism/adt-decorators)
-and can be installed via
-```bash
-pip install adt-decorators
-```
-[//]: # (INSTALL_END)
 
 ## Features
 
 - **Simplicity.** This package exports only a single definition: the
   [`adt`](../reference/#adt.adt) class decorator:
   ```python
   from adt import adt
@@ -87,14 +91,21 @@
       
       def print(self):
           match self:
               case MouseClick(x, y):    ... # <-- As promised: no `Event.MouseClick`!
               case KeyPress(key, mods): ... # <-- As promised: no `Event.KeyPress`!
   ```
 
+- **Reflection.**
+  The decorated class has a static field `constructors: dict[str, type]`
+  which maps the constructor names to their classes, e.g.
+  ```python
+  key_event = Event.constructors['KeyPress'](key='a', modifiers=['shift'])
+  ```
+
 
 ## Translation
 
 The code generated in the above example by the `adt` decorator for the
 `Event` ADT behaves equivalent to the following code, with the
 exception that the constructor classes are constructed anonymously, so
 the global namespace is not even temporarily polluted unless
@@ -125,14 +136,19 @@
   modifiers: list[str]
 
 Event.MouseClick = MouseClick
 Event.KeyPress   = KeyPress
 if not export:
     del MouseClick
     del KeyPress
+
+Event.constructors = {
+    'MouseClick': Event.MouseClick,
+    'KeyPress': Event.KeyPress,
+}
 ```
 
 ## Related packages
 
 The following compares this package to packages which aim to provide similar functionality:
 
 - [`algebraic-data-types`](https://pypi.org/project/algebraic-data-types/)
```

### Comparing `adt-decorators-0.2.8/adt/__init__.py` & `adt-decorators-0.2.9/adt/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Provides class decorators for Algebraic Data Types (ADTs)
 """
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 __author__ = 'Hannes Saffrich'
 
 from dataclasses import dataclass
 import inspect
 
 def adt(Class=None, export=False):
     """Class-decorator for Algebraic Data Types (ADTs).
@@ -59,27 +59,29 @@
     def decorator(Base):
         annotations = vars(Base)["__annotations__"]
         Base.__annotations__ = dict()
 
         def Base_init(self, *args, **kwargs):
             raise TypeError(f"Tryed to construct an ADT instead of one of it's constructor.")
         Base.__init__ = Base_init
+        Base.constructors = dict()
 
         for con_name, con_ty in annotations.items():
             if type(con_ty) == dict:
                 params = con_ty
             elif type(con_ty) == tuple or type(con_ty) == list:
                 params = { f"_{i+1}": t for (i, t) in enumerate(con_ty) }
             elif type(con_ty) == type:
                 params = { "_1": con_ty }
             else:
                 raise TypeError(f"ADT with invalid constructor definition {con_name}: {ty}")
 
             Con = dataclass(type(con_name, (Base, ), { "__annotations__": params }))
             setattr(Base, con_name, Con)
+            Base.constructors[con_name] = Con
 
             def is_con_gen(Con):
                 def is_con(self) -> bool:
                     return isinstance(self, Con)
                 return is_con
             is_con_name = "is_" + upper_camel_to_snake(con_name)
             setattr(Base, is_con_name, is_con_gen(Con))
```

### Comparing `adt-decorators-0.2.8/adt_decorators.egg-info/PKG-INFO` & `adt-decorators-0.2.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-Metadata-Version: 2.1
-Name: adt-decorators
-Version: 0.2.8
-Summary: Algebraic Data Types via Class Decorators
-Home-page: https://github.com/m0rphism/adt-decorators
-Author: Hannes Saffrich
-Author-email: saffrich@informatik.uni-freiburg.de
-License: BSD 2-clause
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Overview
 
 This package provides a class decorator for defining
 *[Algebraic Data Types (ADTs)](https://en.wikipedia.org/wiki/Algebraic_data_type)* as known from
 [Haskell](https://wiki.haskell.org/Algebraic_data_type) (`data`),
 [OCaml](https://cs3110.github.io/textbook/chapters/data/algebraic_data_types.html) (`type`), and
 [Rust](https://doc.rust-lang.org/book/ch06-01-defining-an-enum.html) (`enum`).
 
+[//]: # (INSTALL_BEGIN)
+## Installation
 
+The package is on [PyPI](https://pypi.org/project/adt-decorators/)
+and [github](https://github.com/m0rphism/adt-decorators)
+and can be installed via
+```bash
+pip install adt-decorators
+```
+[//]: # (INSTALL_END)
 
 ## Features
 
 - **Simplicity.** This package exports only a single definition: the
   [`adt`](../reference/#adt.adt) class decorator:
   ```python
   from adt import adt
@@ -91,14 +87,21 @@
       
       def print(self):
           match self:
               case MouseClick(x, y):    ... # <-- As promised: no `Event.MouseClick`!
               case KeyPress(key, mods): ... # <-- As promised: no `Event.KeyPress`!
   ```
 
+- **Reflection.**
+  The decorated class has a static field `constructors: dict[str, type]`
+  which maps the constructor names to their classes, e.g.
+  ```python
+  key_event = Event.constructors['KeyPress'](key='a', modifiers=['shift'])
+  ```
+
 
 ## Translation
 
 The code generated in the above example by the `adt` decorator for the
 `Event` ADT behaves equivalent to the following code, with the
 exception that the constructor classes are constructed anonymously, so
 the global namespace is not even temporarily polluted unless
@@ -129,14 +132,19 @@
   modifiers: list[str]
 
 Event.MouseClick = MouseClick
 Event.KeyPress   = KeyPress
 if not export:
     del MouseClick
     del KeyPress
+
+Event.constructors = {
+    'MouseClick': Event.MouseClick,
+    'KeyPress': Event.KeyPress,
+}
 ```
 
 ## Related packages
 
 The following compares this package to packages which aim to provide similar functionality:
 
 - [`algebraic-data-types`](https://pypi.org/project/algebraic-data-types/)
```

### Comparing `adt-decorators-0.2.8/docs/overview.md` & `adt-decorators-0.2.9/docs/overview.md`

 * *Files 8% similar despite different names*

```diff
@@ -87,14 +87,21 @@
       
       def print(self):
           match self:
               case MouseClick(x, y):    ... # <-- As promised: no `Event.MouseClick`!
               case KeyPress(key, mods): ... # <-- As promised: no `Event.KeyPress`!
   ```
 
+- **Reflection.**
+  The decorated class has a static field `constructors: dict[str, type]`
+  which maps the constructor names to their classes, e.g.
+  ```python
+  key_event = Event.constructors['KeyPress'](key='a', modifiers=['shift'])
+  ```
+
 
 ## Translation
 
 The code generated in the above example by the `adt` decorator for the
 `Event` ADT behaves equivalent to the following code, with the
 exception that the constructor classes are constructed anonymously, so
 the global namespace is not even temporarily polluted unless
@@ -125,14 +132,19 @@
   modifiers: list[str]
 
 Event.MouseClick = MouseClick
 Event.KeyPress   = KeyPress
 if not export:
     del MouseClick
     del KeyPress
+
+Event.constructors = {
+    'MouseClick': Event.MouseClick,
+    'KeyPress': Event.KeyPress,
+}
 ```
 
 ## Related packages
 
 The following compares this package to packages which aim to provide similar functionality:
 
 - [`algebraic-data-types`](https://pypi.org/project/algebraic-data-types/)
```

### Comparing `adt-decorators-0.2.8/setup.py` & `adt-decorators-0.2.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     skip_end = "[//]: # (INSTALL_END)"
     begin = desc.find(skip_start)
     end = desc.find(skip_end) + len(skip_end)
     desc = desc[:begin] + desc[end:]
 
 setup(
     name='adt-decorators',
-    version='0.2.8',
+    version='0.2.9',
     description='Algebraic Data Types via Class Decorators',
     long_description=desc,
     long_description_content_type='text/markdown',
     url='https://github.com/m0rphism/adt-decorators',
     author='Hannes Saffrich',
     author_email='saffrich@informatik.uni-freiburg.de',
     license='BSD 2-clause',
```

