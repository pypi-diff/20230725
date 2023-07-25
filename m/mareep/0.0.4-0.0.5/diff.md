# Comparing `tmp/mareep-0.0.4.tar.gz` & `tmp/mareep-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mareep-0.0.4.tar", last modified: Tue Jul 25 04:07:01 2023, max compression
+gzip compressed data, was "mareep-0.0.5.tar", last modified: Tue Jul 25 04:54:56 2023, max compression
```

## Comparing `mareep-0.0.4.tar` & `mareep-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:07:01.233301 mareep-0.0.4/
--rw-r--r--   0 datnh      (501) staff       (20)      547 2023-07-25 04:07:01.233126 mareep-0.0.4/PKG-INFO
--rw-r--r--   0 datnh      (501) staff       (20)        9 2023-06-25 10:06:01.000000 mareep-0.0.4/README.md
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:07:01.229099 mareep-0.0.4/mareep/
--rw-r--r--   0 datnh      (501) staff       (20)       44 2023-06-25 09:06:35.000000 mareep-0.0.4/mareep/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)      100 2023-06-25 09:06:45.000000 mareep-0.0.4/mareep/__main__.py
--rw-r--r--   0 datnh      (501) staff       (20)     2570 2023-07-25 04:05:28.000000 mareep-0.0.4/mareep/app.py
--rw-r--r--   0 datnh      (501) staff       (20)     1524 2023-07-25 04:04:20.000000 mareep-0.0.4/mareep/function.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:07:01.231082 mareep-0.0.4/mareep/loaders/
--rw-r--r--   0 datnh      (501) staff       (20)      711 2023-06-25 08:45:35.000000 mareep-0.0.4/mareep/loaders/__init__.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:07:01.231875 mareep-0.0.4/mareep/loaders/json_loader/
--rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 08:30:33.000000 mareep-0.0.4/mareep/loaders/json_loader/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)      274 2023-06-25 08:40:30.000000 mareep-0.0.4/mareep/loaders/json_loader/loader.py
--rw-r--r--   0 datnh      (501) staff       (20)      222 2023-06-25 08:28:35.000000 mareep-0.0.4/mareep/loaders/loader.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:07:01.232644 mareep-0.0.4/mareep/loaders/yaml_loader/
--rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 09:45:41.000000 mareep-0.0.4/mareep/loaders/yaml_loader/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)      295 2023-06-25 09:46:35.000000 mareep-0.0.4/mareep/loaders/yaml_loader/loader.py
--rw-r--r--   0 datnh      (501) staff       (20)     2570 2023-06-25 13:06:37.000000 mareep-0.0.4/mareep/renderer.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:07:01.230463 mareep-0.0.4/mareep.egg-info/
--rw-r--r--   0 datnh      (501) staff       (20)      547 2023-07-25 04:07:01.000000 mareep-0.0.4/mareep.egg-info/PKG-INFO
--rw-r--r--   0 datnh      (501) staff       (20)      494 2023-07-25 04:07:01.000000 mareep-0.0.4/mareep.egg-info/SOURCES.txt
--rw-r--r--   0 datnh      (501) staff       (20)        1 2023-07-25 04:07:01.000000 mareep-0.0.4/mareep.egg-info/dependency_links.txt
--rw-r--r--   0 datnh      (501) staff       (20)       49 2023-07-25 04:07:01.000000 mareep-0.0.4/mareep.egg-info/entry_points.txt
--rw-r--r--   0 datnh      (501) staff       (20)       62 2023-07-25 04:07:01.000000 mareep-0.0.4/mareep.egg-info/requires.txt
--rw-r--r--   0 datnh      (501) staff       (20)        7 2023-07-25 04:07:01.000000 mareep-0.0.4/mareep.egg-info/top_level.txt
--rw-r--r--   0 datnh      (501) staff       (20)       38 2023-07-25 04:07:01.233472 mareep-0.0.4/setup.cfg
--rw-r--r--   0 datnh      (501) staff       (20)     1471 2023-07-25 04:05:37.000000 mareep-0.0.4/setup.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:54:56.088733 mareep-0.0.5/
+-rw-r--r--   0 datnh      (501) staff       (20)      547 2023-07-25 04:54:56.088597 mareep-0.0.5/PKG-INFO
+-rw-r--r--   0 datnh      (501) staff       (20)        9 2023-06-25 10:06:01.000000 mareep-0.0.5/README.md
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:54:56.086111 mareep-0.0.5/mareep/
+-rw-r--r--   0 datnh      (501) staff       (20)       44 2023-06-25 09:06:35.000000 mareep-0.0.5/mareep/__init__.py
+-rw-r--r--   0 datnh      (501) staff       (20)      100 2023-06-25 09:06:45.000000 mareep-0.0.5/mareep/__main__.py
+-rw-r--r--   0 datnh      (501) staff       (20)     2570 2023-07-25 04:05:28.000000 mareep-0.0.5/mareep/app.py
+-rw-r--r--   0 datnh      (501) staff       (20)     1524 2023-07-25 04:04:20.000000 mareep-0.0.5/mareep/function.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:54:56.087372 mareep-0.0.5/mareep/loaders/
+-rw-r--r--   0 datnh      (501) staff       (20)      711 2023-07-25 04:49:37.000000 mareep-0.0.5/mareep/loaders/__init__.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:54:56.087936 mareep-0.0.5/mareep/loaders/json_loader/
+-rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 08:30:33.000000 mareep-0.0.5/mareep/loaders/json_loader/__init__.py
+-rw-r--r--   0 datnh      (501) staff       (20)      274 2023-07-25 04:25:43.000000 mareep-0.0.5/mareep/loaders/json_loader/loader.py
+-rw-r--r--   0 datnh      (501) staff       (20)      222 2023-06-25 08:28:35.000000 mareep-0.0.5/mareep/loaders/loader.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:54:56.088257 mareep-0.0.5/mareep/loaders/yaml_loader/
+-rw-r--r--   0 datnh      (501) staff       (20)       22 2023-06-25 09:45:41.000000 mareep-0.0.5/mareep/loaders/yaml_loader/__init__.py
+-rw-r--r--   0 datnh      (501) staff       (20)      295 2023-06-25 09:46:35.000000 mareep-0.0.5/mareep/loaders/yaml_loader/loader.py
+-rw-r--r--   0 datnh      (501) staff       (20)     2578 2023-07-25 04:54:31.000000 mareep-0.0.5/mareep/renderer.py
+drwxr-xr-x   0 datnh      (501) staff       (20)        0 2023-07-25 04:54:56.087060 mareep-0.0.5/mareep.egg-info/
+-rw-r--r--   0 datnh      (501) staff       (20)      547 2023-07-25 04:54:56.000000 mareep-0.0.5/mareep.egg-info/PKG-INFO
+-rw-r--r--   0 datnh      (501) staff       (20)      494 2023-07-25 04:54:56.000000 mareep-0.0.5/mareep.egg-info/SOURCES.txt
+-rw-r--r--   0 datnh      (501) staff       (20)        1 2023-07-25 04:54:56.000000 mareep-0.0.5/mareep.egg-info/dependency_links.txt
+-rw-r--r--   0 datnh      (501) staff       (20)       49 2023-07-25 04:54:56.000000 mareep-0.0.5/mareep.egg-info/entry_points.txt
+-rw-r--r--   0 datnh      (501) staff       (20)       62 2023-07-25 04:54:56.000000 mareep-0.0.5/mareep.egg-info/requires.txt
+-rw-r--r--   0 datnh      (501) staff       (20)        7 2023-07-25 04:54:56.000000 mareep-0.0.5/mareep.egg-info/top_level.txt
+-rw-r--r--   0 datnh      (501) staff       (20)       38 2023-07-25 04:54:56.088804 mareep-0.0.5/setup.cfg
+-rw-r--r--   0 datnh      (501) staff       (20)     1471 2023-07-25 04:54:39.000000 mareep-0.0.5/setup.py
```

### Comparing `mareep-0.0.4/PKG-INFO` & `mareep-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mareep
-Version: 0.0.4
+Version: 0.0.5
 Summary: mareep
 Home-page: https://github.com/NgHoangDat/mareep.git
 Author: nghoangdat
 Author-email: 18.hoang.dat.12@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/NgHoangDat/mareep/archive/v0.0.4.tar.gz
+Download-URL: https://github.com/NgHoangDat/mareep/archive/v0.0.5.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mareep-0.0.4/mareep/app.py` & `mareep-0.0.5/mareep/app.py`

 * *Files identical despite different names*

### Comparing `mareep-0.0.4/mareep/function.py` & `mareep-0.0.5/mareep/function.py`

 * *Files identical despite different names*

### Comparing `mareep-0.0.4/mareep/loaders/__init__.py` & `mareep-0.0.5/mareep/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `mareep-0.0.4/mareep/renderer.py` & `mareep-0.0.5/mareep/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,8 +76,8 @@
                     output_file: Path = self.output_path / template_file.stem
                 else:
                     output_file: Path = self.output_path / template_file.name
 
                 output_file.parent.mkdir(parents=True, exist_ok=True)
 
                 with open(output_file, "w") as fout:
-                    fout.write(template.render(env))
+                    fout.write(template.render(env).strip())
```

### Comparing `mareep-0.0.4/mareep.egg-info/PKG-INFO` & `mareep-0.0.5/mareep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mareep
-Version: 0.0.4
+Version: 0.0.5
 Summary: mareep
 Home-page: https://github.com/NgHoangDat/mareep.git
 Author: nghoangdat
 Author-email: 18.hoang.dat.12@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/NgHoangDat/mareep/archive/v0.0.4.tar.gz
+Download-URL: https://github.com/NgHoangDat/mareep/archive/v0.0.5.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mareep-0.0.4/setup.py` & `mareep-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import *
 
 import setuptools
 
 __PACKAGE__ = "mareep"
-__VERSION__ = "0.0.4"
+__VERSION__ = "0.0.5"
 
 base_dir = Path(__file__).resolve().parent
 
 with open(base_dir / "README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
```

