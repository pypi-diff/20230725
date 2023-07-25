# Comparing `tmp/hugie-0.3.1.tar.gz` & `tmp/hugie-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugie-0.3.1.tar", max compression
+gzip compressed data, was "hugie-0.3.2.tar", max compression
```

## Comparing `hugie-0.3.1.tar` & `hugie-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1070 2022-11-04 11:34:23.136928 hugie-0.3.1/LICENSE
--rw-r--r--   0        0        0     2809 2023-07-20 13:53:05.306209 hugie-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-03-09 22:06:47.311232 hugie-0.3.1/hugie/__init__.py
--rw-r--r--   0        0        0      404 2023-07-20 13:53:05.306209 hugie-0.3.1/hugie/__main__.py
--rw-r--r--   0        0        0     3077 2023-07-20 13:53:05.306209 hugie-0.3.1/hugie/config.py
--rw-r--r--   0        0        0     9098 2023-07-20 13:53:05.306209 hugie-0.3.1/hugie/endpoint.py
--rw-r--r--   0        0        0     2208 2023-07-20 13:53:05.306209 hugie-0.3.1/hugie/models.py
--rw-r--r--   0        0        0      306 2023-03-09 22:06:47.311232 hugie-0.3.1/hugie/settings.py
--rw-r--r--   0        0        0      839 2023-03-09 22:06:47.311232 hugie-0.3.1/hugie/utils.py
--rw-r--r--   0        0        0      665 2023-07-20 13:59:54.593131 hugie-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3555 1970-01-01 00:00:00.000000 hugie-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-11-04 11:34:23.136928 hugie-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2887 2023-07-25 10:17:37.090001 hugie-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-09 22:06:47.311232 hugie-0.3.2/hugie/__init__.py
+-rw-r--r--   0        0        0      748 2023-07-25 10:17:37.090001 hugie-0.3.2/hugie/__main__.py
+-rw-r--r--   0        0        0     3077 2023-07-20 13:53:05.306209 hugie-0.3.2/hugie/config.py
+-rw-r--r--   0        0        0     9098 2023-07-24 15:55:34.842577 hugie-0.3.2/hugie/endpoint.py
+-rw-r--r--   0        0        0     8411 2023-07-22 23:04:08.000702 hugie-0.3.2/hugie/endpoint1.py
+-rw-r--r--   0        0        0     2208 2023-07-20 13:53:05.306209 hugie-0.3.2/hugie/models.py
+-rw-r--r--   0        0        0      306 2023-03-09 22:06:47.311232 hugie-0.3.2/hugie/settings.py
+-rw-r--r--   0        0        0      839 2023-07-22 23:13:30.452476 hugie-0.3.2/hugie/utils.py
+-rw-r--r--   0        0        0      664 2023-07-25 10:17:37.090001 hugie-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 hugie-0.3.2/PKG-INFO
```

### Comparing `hugie-0.3.1/LICENSE` & `hugie-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hugie-0.3.1/README.md` & `hugie-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,19 @@
 >>>
 Usage: hugie [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --help                          Show this message and exit.
 
 Commands:
+  Commands:
   config
   endpoint
-  version   Show version.
+  ui        Open the Hugging Face Endpoints UI in a browser
+  version   Print hugie version
 ```
 
 # Endpoint
 
 ```
 hugie endpoint --help
 >>>
```

### Comparing `hugie-0.3.1/hugie/config.py` & `hugie-0.3.2/hugie/config.py`

 * *Files identical despite different names*

### Comparing `hugie-0.3.1/hugie/endpoint.py` & `hugie-0.3.2/hugie/endpoint.py`

 * *Files identical despite different names*

### Comparing `hugie-0.3.1/hugie/models.py` & `hugie-0.3.2/hugie/models.py`

 * *Files identical despite different names*

### Comparing `hugie-0.3.1/hugie/utils.py` & `hugie-0.3.2/hugie/utils.py`

 * *Files identical despite different names*

### Comparing `hugie-0.3.1/pyproject.toml` & `hugie-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "hugie"
-version = "0.3.1"
+version = "0.3.2"
 description = "CLI for managing Hugging Face Inference Endpoints"
-authors = ["Matthew Upson <matt@mantisnlp.com>", 
+authors = ["Matthew Upson <matt@mantisnlp.com>",
             "Nick Sorros <nick@mantisnlp.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = "^0.9.0"
```

### Comparing `hugie-0.3.1/PKG-INFO` & `hugie-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugie
-Version: 0.3.1
+Version: 0.3.2
 Summary: CLI for managing Hugging Face Inference Endpoints
 License: MIT
 Author: Matthew Upson
 Author-email: matt@mantisnlp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -48,17 +48,19 @@
 >>>
 Usage: hugie [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --help                          Show this message and exit.
 
 Commands:
+  Commands:
   config
   endpoint
-  version   Show version.
+  ui        Open the Hugging Face Endpoints UI in a browser
+  version   Print hugie version
 ```
 
 # Endpoint
 
 ```
 hugie endpoint --help
 >>>
```

