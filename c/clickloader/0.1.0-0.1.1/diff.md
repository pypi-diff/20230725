# Comparing `tmp/clickloader-0.1.0.tar.gz` & `tmp/clickloader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickloader-0.1.0.tar", max compression
+gzip compressed data, was "clickloader-0.1.1.tar", max compression
```

## Comparing `clickloader-0.1.0.tar` & `clickloader-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-07-24 18:49:01.746366 clickloader-0.1.0/LICENSE
--rw-r--r--   0        0        0      873 2023-07-24 22:56:48.133054 clickloader-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2066 2023-07-24 22:57:29.167565 clickloader-0.1.0/README.md
--rw-r--r--   0        0        0     2145 2023-07-24 22:24:42.814177 clickloader-0.1.0/src/ccl/__init__.py
--rw-r--r--   0        0        0     2706 2023-07-24 22:06:56.467059 clickloader-0.1.0/src/ccl/finder.py
--rw-r--r--   0        0        0     2445 1970-01-01 00:00:00.000000 clickloader-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-25 01:08:11.680447 clickloader-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2066 2023-07-25 01:08:11.680447 clickloader-0.1.1/README.md
+-rw-r--r--   0        0        0     1077 2023-07-25 01:08:11.680447 clickloader-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2226 2023-07-25 01:08:11.680447 clickloader-0.1.1/src/ccl/__init__.py
+-rw-r--r--   0        0        0     2733 2023-07-25 01:08:11.680447 clickloader-0.1.1/src/ccl/finder.py
+-rw-r--r--   0        0        0     2771 1970-01-01 00:00:00.000000 clickloader-0.1.1/PKG-INFO
```

### Comparing `clickloader-0.1.0/LICENSE` & `clickloader-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clickloader-0.1.0/pyproject.toml` & `clickloader-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 [tool.poetry]
 name = "clickloader"
-version = "0.1.0"
-description = ""
+version = "0.1.1"
+description = "Click Command Loader, permit to load Click command from a given folder."
 authors = ["Julien Mauroy <pro.julien.mauroy@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ccl", from = "src"}]
+repository = "https://github.com/madebylydia/CCL"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.7"
 click = ">=8.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.280"
 black = "^23.7.0"
 isort = "^5.12.0"
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 pytest-html = "^3.2.0"
 poethepoet = "^0.21.1"
 metadeco = "^0.2.1"
+tox = "^4.6.4"
+
+
+[tool.poetry.group.actions.dependencies]
+tox-gh-actions = "^3.1.3"
 
 [tool.poe]
 poetry_command = ""
 
 [tool.poe.tasks]
 _format_black = "black ."
 _format_isort = "isort ."
```

### Comparing `clickloader-0.1.0/README.md` & `clickloader-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `clickloader-0.1.0/src/ccl/finder.py` & `clickloader-0.1.1/src/ccl/finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import ast
 import importlib.util
 import logging
 import pathlib
 from shutil import ExecError
 from typing import Literal, overload
+import typing
 
 import click
 
 _log = logging.getLogger("ccl")
 
 
 def find_cmd_func_name(path: pathlib.Path) -> str:
@@ -54,15 +55,15 @@
     path: pathlib.Path, export_function_name: str, return_type: Literal["group"]
 ) -> click.Group:
     ...
 
 
 def fetch_cmd_func(
     path: pathlib.Path, export_function_name: str, return_type: str
-) -> click.Command | click.Group:
+) -> typing.Union[click.Command, click.Group]:
     """Load a module at path and try to export a function from its name.
     Supposedly to return a click command.
 
     Parameters
     ----------
     path : pathlib.Path
         Path to the module to read.
```

### Comparing `clickloader-0.1.0/PKG-INFO` & `clickloader-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: clickloader
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: Click Command Loader, permit to load Click command from a given folder.
+Home-page: https://github.com/madebylydia/CCL
 Author: Julien Mauroy
 Author-email: pro.julien.mauroy@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0)
+Project-URL: Repository, https://github.com/madebylydia/CCL
 Description-Content-Type: text/markdown
 
 # Click Command Loader (CCL)
 
 ![Click Command Loader](.github/CCL.png)
 
 Click Command Loader (Referred as CCL) is an additional package for [Click](https://click.palletsprojects.com/) to **load Click commands from a folder.**
```

