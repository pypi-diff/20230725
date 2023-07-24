# Comparing `tmp/flet_pyodide-0.9.0.dev1620.tar.gz` & `tmp/flet_pyodide-0.9.0.dev1621.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_pyodide-0.9.0.dev1620.tar", max compression
+gzip compressed data, was "flet_pyodide-0.9.0.dev1621.tar", max compression
```

## Comparing `flet_pyodide-0.9.0.dev1620.tar` & `flet_pyodide-0.9.0.dev1621.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2264 2023-07-24 03:09:23.031746 flet_pyodide-0.9.0.dev1620/README.md
--rw-r--r--   0        0        0      644 2023-07-24 03:09:59.558638 flet_pyodide-0.9.0.dev1620/pyproject.toml
--rw-r--r--   0        0        0       61 2023-07-24 03:09:23.031746 flet_pyodide-0.9.0.dev1620/src/flet/__init__.py
--rw-r--r--   0        0        0       31 2023-07-24 03:09:23.031746 flet_pyodide-0.9.0.dev1620/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0     2285 2023-07-24 03:09:23.031746 flet_pyodide-0.9.0.dev1620/src/flet/flet.py
--rw-r--r--   0        0        0       55 2023-07-24 03:09:23.031746 flet_pyodide-0.9.0.dev1620/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-07-24 03:09:23.031746 flet_pyodide-0.9.0.dev1620/src/flet/plotly_chart.py
--rw-r--r--   0        0        0     3851 2023-07-24 03:09:23.031746 flet_pyodide-0.9.0.dev1620/src/flet/pyodide_connection.py
--rw-r--r--   0        0        0      103 2023-07-24 03:09:23.031746 flet_pyodide-0.9.0.dev1620/src/flet/version.py
--rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.9.0.dev1620/PKG-INFO
+-rw-r--r--   0        0        0     2264 2023-07-24 23:26:38.607216 flet_pyodide-0.9.0.dev1621/README.md
+-rw-r--r--   0        0        0      644 2023-07-24 23:27:12.949938 flet_pyodide-0.9.0.dev1621/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-07-24 23:26:38.611215 flet_pyodide-0.9.0.dev1621/src/flet/__init__.py
+-rw-r--r--   0        0        0       31 2023-07-24 23:26:38.611215 flet_pyodide-0.9.0.dev1621/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0     2285 2023-07-24 23:26:38.611215 flet_pyodide-0.9.0.dev1621/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2023-07-24 23:26:38.611215 flet_pyodide-0.9.0.dev1621/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-07-24 23:26:38.611215 flet_pyodide-0.9.0.dev1621/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0     3851 2023-07-24 23:26:38.611215 flet_pyodide-0.9.0.dev1621/src/flet/pyodide_connection.py
+-rw-r--r--   0        0        0      103 2023-07-24 23:26:38.611215 flet_pyodide-0.9.0.dev1621/src/flet/version.py
+-rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.9.0.dev1621/PKG-INFO
```

### Comparing `flet_pyodide-0.9.0.dev1620/README.md` & `flet_pyodide-0.9.0.dev1621/README.md`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.9.0.dev1620/pyproject.toml` & `flet_pyodide-0.9.0.dev1621/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-pyodide"
-version = "0.9.0.dev1620"
+version = "0.9.0.dev1621"
 description = "Flet for Pyodide - build standalone SPA in Python with Flutter UI."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.9.0.dev1620"
+flet-core = "0.9.0.dev1621"
 python = "^3.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `flet_pyodide-0.9.0.dev1620/src/flet/flet.py` & `flet_pyodide-0.9.0.dev1621/src/flet/flet.py`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.9.0.dev1620/src/flet/pyodide_connection.py` & `flet_pyodide-0.9.0.dev1621/src/flet/pyodide_connection.py`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.9.0.dev1620/PKG-INFO` & `flet_pyodide-0.9.0.dev1621/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: flet-pyodide
-Version: 0.9.0.dev1620
+Version: 0.9.0.dev1621
 Summary: Flet for Pyodide - build standalone SPA in Python with Flutter UI.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.9.0.dev1620)
+Requires-Dist: flet-core (==0.9.0.dev1621)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
 
 # Flet for Pyodide - build standalone Single-Page Applications (SPA) in Python with Flutter UI
```

