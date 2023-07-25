# Comparing `tmp/mareep-0.0.3.tar.gz` & `tmp/mareep-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mareep-0.0.3.tar", last modified: Mon Jun 26 02:14:09 2023, max compression
+gzip compressed data, was "mareep-0.0.4.tar", last modified: Tue Jul 25 04:07:01 2023, max compression
```

## Comparing `mareep-0.0.3.tar` & `mareep-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-26 02:14:09.145233 mareep-0.0.3/
--rw-r--r--   0 datnh      (501) staff       (20)      547 2023-06-26 02:14:09.145091 mareep-0.0.3/PKG-INFO
--rw-r--r--   0 datnh      (501) staff       (20)        9 2023-06-25 10:06:01.000000 mareep-0.0.3/README.md
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-26 02:14:09.142676 mareep-0.0.3/mareep/
--rw-r--r--   0 datnh      (501) staff       (20)       44 2023-06-25 09:06:35.000000 mareep-0.0.3/mareep/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)      100 2023-06-25 09:06:45.000000 mareep-0.0.3/mareep/__main__.py
--rw-r--r--   0 datnh      (501) staff       (20)     2380 2023-06-25 08:08:40.000000 mareep-0.0.3/mareep/app.py
--rw-r--r--   0 datnh      (501) staff       (20)     1557 2023-06-26 02:13:40.000000 mareep-0.0.3/mareep/function.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-26 02:14:09.143798 mareep-0.0.3/mareep/loaders/
--rw-r--r--   0 datnh      (501) staff       (20)      711 2023-06-25 08:45:35.000000 mareep-0.0.3/mareep/loaders/__init__.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-26 02:14:09.144409 mareep-0.0.3/mareep/loaders/json_loader/
--rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 08:30:33.000000 mareep-0.0.3/mareep/loaders/json_loader/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)      274 2023-06-25 08:40:30.000000 mareep-0.0.3/mareep/loaders/json_loader/loader.py
--rw-r--r--   0 datnh      (501) staff       (20)      222 2023-06-25 08:28:35.000000 mareep-0.0.3/mareep/loaders/loader.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-26 02:14:09.144777 mareep-0.0.3/mareep/loaders/yaml_loader/
--rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 09:45:41.000000 mareep-0.0.3/mareep/loaders/yaml_loader/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)      295 2023-06-25 09:46:35.000000 mareep-0.0.3/mareep/loaders/yaml_loader/loader.py
--rw-r--r--   0 datnh      (501) staff       (20)     2570 2023-06-25 13:06:37.000000 mareep-0.0.3/mareep/renderer.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-06-26 02:14:09.143539 mareep-0.0.3/mareep.egg-info/
--rw-r--r--   0 datnh      (501) staff       (20)      547 2023-06-26 02:14:09.000000 mareep-0.0.3/mareep.egg-info/PKG-INFO
--rw-r--r--   0 datnh      (501) staff       (20)      494 2023-06-26 02:14:09.000000 mareep-0.0.3/mareep.egg-info/SOURCES.txt
--rw-r--r--   0 datnh      (501) staff       (20)        1 2023-06-26 02:14:09.000000 mareep-0.0.3/mareep.egg-info/dependency_links.txt
--rw-r--r--   0 datnh      (501) staff       (20)       49 2023-06-26 02:14:09.000000 mareep-0.0.3/mareep.egg-info/entry_points.txt
--rw-r--r--   0 datnh      (501) staff       (20)       55 2023-06-26 02:14:09.000000 mareep-0.0.3/mareep.egg-info/requires.txt
--rw-r--r--   0 datnh      (501) staff       (20)        7 2023-06-26 02:14:09.000000 mareep-0.0.3/mareep.egg-info/top_level.txt
--rw-r--r--   0 datnh      (501) staff       (20)       38 2023-06-26 02:14:09.145278 mareep-0.0.3/setup.cfg
--rw-r--r--   0 datnh      (501) staff       (20)     1471 2023-06-26 02:13:46.000000 mareep-0.0.3/setup.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:07:01.233301 mareep-0.0.4/
+-rw-r--r--   0 datnh      (501) staff       (20)      547 2023-07-25 04:07:01.233126 mareep-0.0.4/PKG-INFO
+-rw-r--r--   0 datnh      (501) staff       (20)        9 2023-06-25 10:06:01.000000 mareep-0.0.4/README.md
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:07:01.229099 mareep-0.0.4/mareep/
+-rw-r--r--   0 datnh      (501) staff       (20)       44 2023-06-25 09:06:35.000000 mareep-0.0.4/mareep/__init__.py
+-rw-r--r--   0 datnh      (501) staff       (20)      100 2023-06-25 09:06:45.000000 mareep-0.0.4/mareep/__main__.py
+-rw-r--r--   0 datnh      (501) staff       (20)     2570 2023-07-25 04:05:28.000000 mareep-0.0.4/mareep/app.py
+-rw-r--r--   0 datnh      (501) staff       (20)     1524 2023-07-25 04:04:20.000000 mareep-0.0.4/mareep/function.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:07:01.231082 mareep-0.0.4/mareep/loaders/
+-rw-r--r--   0 datnh      (501) staff       (20)      711 2023-06-25 08:45:35.000000 mareep-0.0.4/mareep/loaders/__init__.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:07:01.231875 mareep-0.0.4/mareep/loaders/json_loader/
+-rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 08:30:33.000000 mareep-0.0.4/mareep/loaders/json_loader/__init__.py
+-rw-r--r--   0 datnh      (501) staff       (20)      274 2023-06-25 08:40:30.000000 mareep-0.0.4/mareep/loaders/json_loader/loader.py
+-rw-r--r--   0 datnh      (501) staff       (20)      222 2023-06-25 08:28:35.000000 mareep-0.0.4/mareep/loaders/loader.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:07:01.232644 mareep-0.0.4/mareep/loaders/yaml_loader/
+-rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 09:45:41.000000 mareep-0.0.4/mareep/loaders/yaml_loader/__init__.py
+-rw-r--r--   0 datnh      (501) staff       (20)      295 2023-06-25 09:46:35.000000 mareep-0.0.4/mareep/loaders/yaml_loader/loader.py
+-rw-r--r--   0 datnh      (501) staff       (20)     2570 2023-06-25 13:06:37.000000 mareep-0.0.4/mareep/renderer.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:07:01.230463 mareep-0.0.4/mareep.egg-info/
+-rw-r--r--   0 datnh      (501) staff       (20)      547 2023-07-25 04:07:01.000000 mareep-0.0.4/mareep.egg-info/PKG-INFO
+-rw-r--r--   0 datnh      (501) staff       (20)      494 2023-07-25 04:07:01.000000 mareep-0.0.4/mareep.egg-info/SOURCES.txt
+-rw-r--r--   0 datnh      (501) staff       (20)        1 2023-07-25 04:07:01.000000 mareep-0.0.4/mareep.egg-info/dependency_links.txt
+-rw-r--r--   0 datnh      (501) staff       (20)       49 2023-07-25 04:07:01.000000 mareep-0.0.4/mareep.egg-info/entry_points.txt
+-rw-r--r--   0 datnh      (501) staff       (20)       62 2023-07-25 04:07:01.000000 mareep-0.0.4/mareep.egg-info/requires.txt
+-rw-r--r--   0 datnh      (501) staff       (20)        7 2023-07-25 04:07:01.000000 mareep-0.0.4/mareep.egg-info/top_level.txt
+-rw-r--r--   0 datnh      (501) staff       (20)       38 2023-07-25 04:07:01.233472 mareep-0.0.4/setup.cfg
+-rw-r--r--   0 datnh      (501) staff       (20)     1471 2023-07-25 04:05:37.000000 mareep-0.0.4/setup.py
```

### Comparing `mareep-0.0.3/PKG-INFO` & `mareep-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mareep
-Version: 0.0.3
+Version: 0.0.4
 Summary: mareep
 Home-page: https://github.com/NgHoangDat/mareep.git
 Author: nghoangdat
 Author-email: 18.hoang.dat.12@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/NgHoangDat/mareep/archive/v0.0.3.tar.gz
+Download-URL: https://github.com/NgHoangDat/mareep/archive/v0.0.4.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mareep-0.0.3/mareep/app.py` & `mareep-0.0.4/mareep/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,7 +74,15 @@
     def sub_app(self, name: str):
         sub_app = App(pretty_exceptions_show_locals=False)
         self.add_typer(sub_app, name=name)
         return sub_app
 
 
 app = App(pretty_exceptions_show_locals=False)
+
+
+@app.command()
+def about():
+    import random
+    import cowsay
+    char = random.choice(cowsay.char_names)
+    print(cowsay.get_output_string(char, "This is a module for ai-evaluation"))
```

### Comparing `mareep-0.0.3/mareep/function.py` & `mareep-0.0.4/mareep/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from .app import app
 from .renderer import Renderer
 
 
 @app.command(
     context_settings={"allow_extra_args": True, "ignore_unknown_options": True},
-    invoke_without_command=True,
 )
 def render(
     ctx: Context,
     template_path: Path = Argument(..., help="Template path"),
     output_path: Path = Argument(..., help="Output path"),
 
     extensions: List[str] = Option(["j2", "jinja2", "jinja"], help="List of templete extensions"),
```

### Comparing `mareep-0.0.3/mareep/loaders/__init__.py` & `mareep-0.0.4/mareep/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `mareep-0.0.3/mareep/renderer.py` & `mareep-0.0.4/mareep/renderer.py`

 * *Files identical despite different names*

### Comparing `mareep-0.0.3/mareep.egg-info/PKG-INFO` & `mareep-0.0.4/mareep.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mareep
-Version: 0.0.3
+Version: 0.0.4
 Summary: mareep
 Home-page: https://github.com/NgHoangDat/mareep.git
 Author: nghoangdat
 Author-email: 18.hoang.dat.12@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/NgHoangDat/mareep/archive/v0.0.3.tar.gz
+Download-URL: https://github.com/NgHoangDat/mareep/archive/v0.0.4.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mareep-0.0.3/setup.py` & `mareep-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import *
 
 import setuptools
 
 __PACKAGE__ = "mareep"
-__VERSION__ = "0.0.3"
+__VERSION__ = "0.0.4"
 
 base_dir = Path(__file__).resolve().parent
 
 with open(base_dir / "README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
```

