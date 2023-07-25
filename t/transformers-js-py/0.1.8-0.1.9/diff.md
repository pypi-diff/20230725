# Comparing `tmp/transformers_js_py-0.1.8.tar.gz` & `tmp/transformers_js_py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers_js_py-0.1.8.tar", max compression
+gzip compressed data, was "transformers_js_py-0.1.9.tar", max compression
```

## Comparing `transformers_js_py-0.1.8.tar` & `transformers_js_py-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-07-25 13:42:11.214656 transformers_js_py-0.1.8/LICENSE
--rw-r--r--   0        0        0     7153 2023-07-25 13:42:11.214656 transformers_js_py-0.1.8/README.md
--rw-r--r--   0        0        0      579 2023-07-25 13:42:11.222657 transformers_js_py-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2964 2023-07-25 13:42:11.222657 transformers_js_py-0.1.8/transformers_js/__init__.py
--rw-r--r--   0        0        0     7600 1970-01-01 00:00:00.000000 transformers_js_py-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 14:24:25.882127 transformers_js_py-0.1.9/LICENSE
+-rw-r--r--   0        0        0     7801 2023-07-25 14:24:25.882127 transformers_js_py-0.1.9/README.md
+-rw-r--r--   0        0        0      579 2023-07-25 14:24:25.886127 transformers_js_py-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2964 2023-07-25 14:24:25.886127 transformers_js_py-0.1.9/transformers_js/__init__.py
+-rw-r--r--   0        0        0     8248 1970-01-01 00:00:00.000000 transformers_js_py-0.1.9/PKG-INFO
```

### Comparing `transformers_js_py-0.1.8/LICENSE` & `transformers_js_py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `transformers_js_py-0.1.8/README.md` & `transformers_js_py-0.1.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         pipe = st.session_state["pipe"]
         out = await pipe(text)
     st.write(out)
 ```
 
 ### Shinylive
 
-![Shinylive screenshot](./docs/images/Shinylive.png)
+[![Shinylive screenshot](./docs/images/Shinylive.png)](https://shinylive.io/py/editor/#code=NobwRAdghgtgpmAXGKAHVA6VBPMAaMAYwHsIAXOcpMAMwCdiYACAZwAsBLCbJjmVYnTJMAgujxM6lACZw6EgK4cAOhHqMmZOlAgsag+HRYB9AFYte-QcL4ChxrTr0G5J86tVpUxpUwC8TEpYUADmcMY0ADZK0gAUqkyJgRwYXKgKZA5wAB5k8WAUucr4TMUAKjk2EOlkxRKokVCEcGzEkbJ0fsUAouRympXFAJR4CUlBxBk1WbnGAG5yAEZQZHz5ZEVgI6pDHhCqsjSscgt0sWkZEpNkNRIscCwsHKRDiGOJAALXNe9MH1IQDoYQq1CBJJhQFjYCCEJiHTS5WKvX7gjhHCDEKo1YGVJFvMHgwmJKRkBR0MHFSn7AlExy6fR0QwWAJQADuUA4Nis9jpzkZrjMLCRKKSqA4qDgkS4cH8mm09JcRiw4sl0r2RMSYolsrZHOEWtVEDg+Xu5D4lDIAFodFBItgnixhuqNdcdezOUwDedqhkcYihrtqRrJHBSeTWFpYtdA3svLKxKhYl4fBw7ic5BJZIsFCE-GU6Ao4IGwABfPDgaDwahSACOSik8HILGBuXwRFIFCoyF5DKZlvMlpwpYAukA)
 
 [👉Online demo](https://shinylive.io/py/editor/#code=NobwRAdghgtgpmAXGKAHVA6VBPMAaMAYwHsIAXOcpMAMwCdiYACAZwAsBLCbJjmVYnTJMAgujxM6lACZw6EgK4cAOhHqMmZOlAgsag+HRYB9AFYte-QcL4ChxrTr0G5J86tVpUxpUwC8TEpYUADmcMY0ADZK0gAUqkyJgRwYXKgKZA5wAB5k8WAUucr4TMUAKjk2EOlkxRKokVCEcGzEkbJ0fsUAouRympXFAJR4CUlBxBk1WbnGAG5yAEZQZHz5ZEVgI6pDHhCqsjSscgt0sWkZEpNkNRIscCwsHKRDiGOJAALXNe9MH1IQDoYQq1CBJJhQFjYCCEJiHTS5WKvX7gjhHCDEKo1YGVJFvMHgwmJKRkBR0MHFSn7AlExy6fR0QwWAJQADuUA4Nis9jpzkZrjMLCRKKSqA4qDgkS4cH8mm09JcRiw4sl0r2RMSYolsrZHOEWtVEDg+Xu5D4lDIAFodFBItgnixhuqNdcdezOUwDedqhkcYihrtqRrJHBSeTWFpYtdA3svLKxKhYl4fBw7ic5BJZIsFCE-GU6Ao4IGwABfPDgaDwahSACOSik8HILGBuXwRFIFCoyF5DKZlvMlpwpYAukA)
 
 ```python
 from shiny import App, render, ui
 from transformers_js import import_transformers_js
```

### Comparing `transformers_js_py-0.1.8/pyproject.toml` & `transformers_js_py-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transformers-js-py"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Yuichiro Tachibana (Tsuchiya) <t.yic.yt@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "transformers_js"}]
 
 [tool.poetry.dependencies]
```

### Comparing `transformers_js_py-0.1.8/transformers_js/__init__.py` & `transformers_js_py-0.1.9/transformers_js/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers_js_py-0.1.8/PKG-INFO` & `transformers_js_py-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers-js-py
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: Apache-2.0
 Author: Yuichiro Tachibana (Tsuchiya)
 Author-email: t.yic.yt@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -112,15 +112,15 @@
         pipe = st.session_state["pipe"]
         out = await pipe(text)
     st.write(out)
 ```
 
 ### Shinylive
 
-![Shinylive screenshot](./docs/images/Shinylive.png)
+[![Shinylive screenshot](./docs/images/Shinylive.png)](https://shinylive.io/py/editor/#code=NobwRAdghgtgpmAXGKAHVA6VBPMAaMAYwHsIAXOcpMAMwCdiYACAZwAsBLCbJjmVYnTJMAgujxM6lACZw6EgK4cAOhHqMmZOlAgsag+HRYB9AFYte-QcL4ChxrTr0G5J86tVpUxpUwC8TEpYUADmcMY0ADZK0gAUqkyJgRwYXKgKZA5wAB5k8WAUucr4TMUAKjk2EOlkxRKokVCEcGzEkbJ0fsUAouRympXFAJR4CUlBxBk1WbnGAG5yAEZQZHz5ZEVgI6pDHhCqsjSscgt0sWkZEpNkNRIscCwsHKRDiGOJAALXNe9MH1IQDoYQq1CBJJhQFjYCCEJiHTS5WKvX7gjhHCDEKo1YGVJFvMHgwmJKRkBR0MHFSn7AlExy6fR0QwWAJQADuUA4Nis9jpzkZrjMLCRKKSqA4qDgkS4cH8mm09JcRiw4sl0r2RMSYolsrZHOEWtVEDg+Xu5D4lDIAFodFBItgnixhuqNdcdezOUwDedqhkcYihrtqRrJHBSeTWFpYtdA3svLKxKhYl4fBw7ic5BJZIsFCE-GU6Ao4IGwABfPDgaDwahSACOSik8HILGBuXwRFIFCoyF5DKZlvMlpwpYAukA)
 
 [👉Online demo](https://shinylive.io/py/editor/#code=NobwRAdghgtgpmAXGKAHVA6VBPMAaMAYwHsIAXOcpMAMwCdiYACAZwAsBLCbJjmVYnTJMAgujxM6lACZw6EgK4cAOhHqMmZOlAgsag+HRYB9AFYte-QcL4ChxrTr0G5J86tVpUxpUwC8TEpYUADmcMY0ADZK0gAUqkyJgRwYXKgKZA5wAB5k8WAUucr4TMUAKjk2EOlkxRKokVCEcGzEkbJ0fsUAouRympXFAJR4CUlBxBk1WbnGAG5yAEZQZHz5ZEVgI6pDHhCqsjSscgt0sWkZEpNkNRIscCwsHKRDiGOJAALXNe9MH1IQDoYQq1CBJJhQFjYCCEJiHTS5WKvX7gjhHCDEKo1YGVJFvMHgwmJKRkBR0MHFSn7AlExy6fR0QwWAJQADuUA4Nis9jpzkZrjMLCRKKSqA4qDgkS4cH8mm09JcRiw4sl0r2RMSYolsrZHOEWtVEDg+Xu5D4lDIAFodFBItgnixhuqNdcdezOUwDedqhkcYihrtqRrJHBSeTWFpYtdA3svLKxKhYl4fBw7ic5BJZIsFCE-GU6Ao4IGwABfPDgaDwahSACOSik8HILGBuXwRFIFCoyF5DKZlvMlpwpYAukA)
 
 ```python
 from shiny import App, render, ui
 from transformers_js import import_transformers_js
```

