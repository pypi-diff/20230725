# Comparing `tmp/rlsvision-0.1.0.tar.gz` & `tmp/rlsvision-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlsvision-0.1.0.tar", last modified: Tue Jul 25 12:51:13 2023, max compression
+gzip compressed data, was "rlsvision-0.1.1.tar", last modified: Tue Jul 25 15:02:41 2023, max compression
```

## Comparing `rlsvision-0.1.0.tar` & `rlsvision-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:51:13.158074 rlsvision-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-25 12:48:23.000000 rlsvision-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-25 12:51:13.158074 rlsvision-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 12:48:23.000000 rlsvision-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-25 12:48:23.000000 rlsvision-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:51:13.158074 rlsvision-0.1.0/rlsvision/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 12:48:23.000000 rlsvision-0.1.0/rlsvision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:51:13.158074 rlsvision-0.1.0/rlsvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-25 12:51:13.000000 rlsvision-0.1.0/rlsvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-25 12:51:13.000000 rlsvision-0.1.0/rlsvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:51:13.000000 rlsvision-0.1.0/rlsvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-25 12:51:13.000000 rlsvision-0.1.0/rlsvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 12:51:13.000000 rlsvision-0.1.0/rlsvision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 12:51:13.158074 rlsvision-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:02:41.521808 rlsvision-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-25 14:59:48.000000 rlsvision-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-25 15:02:41.521808 rlsvision-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 14:59:48.000000 rlsvision-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-25 14:59:48.000000 rlsvision-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:02:41.521808 rlsvision-0.1.1/rlsvision/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 14:59:48.000000 rlsvision-0.1.1/rlsvision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:02:41.521808 rlsvision-0.1.1/rlsvision/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 14:59:48.000000 rlsvision-0.1.1/rlsvision/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-25 15:02:33.000000 rlsvision-0.1.1/rlsvision/structures/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:02:41.521808 rlsvision-0.1.1/rlsvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-25 15:02:41.000000 rlsvision-0.1.1/rlsvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-25 15:02:41.000000 rlsvision-0.1.1/rlsvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:02:41.000000 rlsvision-0.1.1/rlsvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-25 15:02:41.000000 rlsvision-0.1.1/rlsvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 15:02:41.000000 rlsvision-0.1.1/rlsvision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:02:41.521808 rlsvision-0.1.1/setup.cfg
```

### Comparing `rlsvision-0.1.0/LICENSE` & `rlsvision-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rlsvision-0.1.0/PKG-INFO` & `rlsvision-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlsvision
-Version: 0.1.0
+Version: 0.1.1
 Author-email: Mark Mayerfeld <mark.m.mayerfeld@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 RakitaLabSoftware
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,15 +20,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: repository, https://github.com/RakitaLabSoftware/rlscv
+Project-URL: repository, https://github.com/RakitaLabSoftware/rlsvision
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # RLSCV
 Reduce Boilerplate of your Computter Vision projects
```

### Comparing `rlsvision-0.1.0/pyproject.toml` & `rlsvision-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel>=0.37.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rlsvision"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 requires-python = ">=3.11"
 authors = [{ name = "Mark Mayerfeld", email = "mark.m.mayerfeld@gmail.com" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 dependencies = ["torch", "torchvision", "opencv-contrib-python", "lightning"]
 
 [project.optional-dependencies]
 dev = ["pytest", "black", "isort", "build"]
 
 [project.urls]
-repository = "https://github.com/RakitaLabSoftware/rlscv"
+repository = "https://github.com/RakitaLabSoftware/rlsvision"
 
-[tool.setuptools]
-packages = ["rlsvision"]
+[tool.setuptools.packages.find]
+include = ["rlsvision*"]
```

### Comparing `rlsvision-0.1.0/rlsvision.egg-info/PKG-INFO` & `rlsvision-0.1.1/rlsvision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlsvision
-Version: 0.1.0
+Version: 0.1.1
 Author-email: Mark Mayerfeld <mark.m.mayerfeld@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 RakitaLabSoftware
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,15 +20,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: repository, https://github.com/RakitaLabSoftware/rlscv
+Project-URL: repository, https://github.com/RakitaLabSoftware/rlsvision
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # RLSCV
 Reduce Boilerplate of your Computter Vision projects
```

