# Comparing `tmp/better_rtplot-0.1.3.tar.gz` & `tmp/better_rtplot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_rtplot-0.1.3.tar", max compression
+gzip compressed data, was "better_rtplot-0.1.4.tar", max compression
```

## Comparing `better_rtplot-0.1.3.tar` & `better_rtplot-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0    35149 2023-06-28 20:16:53.824192 better_rtplot-0.1.3/LICENSE
--rwxr-xr-x   0        0        0     7489 2023-07-19 02:18:57.469955 better_rtplot-0.1.3/README.md
--rwxr-xr-x   0        0        0      555 2023-07-19 03:46:51.071379 better_rtplot-0.1.3/pyproject.toml
--rwxr-xr-x   0        0        0     7588 2023-07-17 19:06:32.364262 better_rtplot-0.1.3/rtplot/client.py
--rwxr-xr-x   0        0        0     6240 2023-03-09 21:43:09.016987 better_rtplot-0.1.3/rtplot/example_code.py
--rwxr-xr-x   0        0        0     1062 2023-07-13 18:31:13.985659 better_rtplot-0.1.3/rtplot/plot_log.py
--rwxr-xr-x   0        0        0       71 2023-03-09 21:43:09.016987 better_rtplot-0.1.3/rtplot/saved_plots/.gitignore
--rwxr-xr-x   0        0        0    22802 2023-07-17 19:02:58.496380 better_rtplot-0.1.3/rtplot/server.py
--rw-r--r--   0        0        0     8201 1970-01-01 00:00:00.000000 better_rtplot-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2023-06-28 20:16:53.824192 better_rtplot-0.1.4/LICENSE
+-rwxr-xr-x   0        0        0     7489 2023-07-19 02:18:57.469955 better_rtplot-0.1.4/README.md
+-rwxr-xr-x   0        0        0      631 2023-07-25 16:06:34.096792 better_rtplot-0.1.4/pyproject.toml
+-rwxr-xr-x   0        0        0     7588 2023-07-17 19:06:32.364262 better_rtplot-0.1.4/rtplot/client.py
+-rwxr-xr-x   0        0        0     6240 2023-03-09 21:43:09.016987 better_rtplot-0.1.4/rtplot/example_code.py
+-rwxr-xr-x   0        0        0     1062 2023-07-13 18:31:13.985659 better_rtplot-0.1.4/rtplot/plot_log.py
+-rwxr-xr-x   0        0        0       71 2023-03-09 21:43:09.016987 better_rtplot-0.1.4/rtplot/saved_plots/.gitignore
+-rwxr-xr-x   0        0        0    22802 2023-07-17 19:02:58.496380 better_rtplot-0.1.4/rtplot/server.py
+-rw-r--r--   0        0        0     8241 1970-01-01 00:00:00.000000 better_rtplot-0.1.4/PKG-INFO
```

### Comparing `better_rtplot-0.1.3/LICENSE` & `better_rtplot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.3/README.md` & `better_rtplot-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.3/pyproject.toml` & `better_rtplot-0.1.4/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool.poetry]
 name = "better-rtplot"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["jmontp <jmontp@umich.edu>"]
 license = "GPL V3.0"
 readme = "README.md"
 packages = [{include = "rtplot"}]
 
 [tool.poetry.dependencies]
 python = ">= 3.8, <3.11"
-pandas = "1.5.3"
 numpy = "1.23.5"
-pyarrow = "11.0.0"
 pyzmq = "25.0.0"
 
+pandas = {version = "1.5.3", optional = true}
+pyarrow = {version="11.0.0", optional = true}
 pyqtgraph = {version = "0.13.0", optional = true}
 pyside6 = {version = "<= 6.4.0", optional = true}
 
-
 [tool.poetry.extras]
-server = ["pyqtgraph", "pyside6"]
+server = ["pyqtgraph", "pyside6", "pandas", "pyarrow"]
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `better_rtplot-0.1.3/rtplot/client.py` & `better_rtplot-0.1.4/rtplot/client.py`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.3/rtplot/example_code.py` & `better_rtplot-0.1.4/rtplot/example_code.py`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.3/rtplot/plot_log.py` & `better_rtplot-0.1.4/rtplot/plot_log.py`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.3/rtplot/server.py` & `better_rtplot-0.1.4/rtplot/server.py`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.3/PKG-INFO` & `better_rtplot-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: better-rtplot
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: GPL V3.0
 Author: jmontp
 Author-email: jmontp@umich.edu
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: server
 Requires-Dist: numpy (==1.23.5)
-Requires-Dist: pandas (==1.5.3)
-Requires-Dist: pyarrow (==11.0.0)
+Requires-Dist: pandas (==1.5.3) ; extra == "server"
+Requires-Dist: pyarrow (==11.0.0) ; extra == "server"
 Requires-Dist: pyqtgraph (==0.13.0) ; extra == "server"
 Requires-Dist: pyside6 (<=6.4.0) ; extra == "server"
 Requires-Dist: pyzmq (==25.0.0)
 Description-Content-Type: text/markdown
 
 ![Logo of the project](https://github.com/jmontp/rtplot/blob/master/.images/signature-stationery.png)
```

