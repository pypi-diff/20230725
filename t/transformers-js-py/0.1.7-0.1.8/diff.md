# Comparing `tmp/transformers_js_py-0.1.7.tar.gz` & `tmp/transformers_js_py-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers_js_py-0.1.7.tar", max compression
+gzip compressed data, was "transformers_js_py-0.1.8.tar", max compression
```

## Comparing `transformers_js_py-0.1.7.tar` & `transformers_js_py-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-07-25 13:04:34.033870 transformers_js_py-0.1.7/LICENSE
--rw-r--r--   0        0        0     3982 2023-07-25 13:04:34.033870 transformers_js_py-0.1.7/README.md
--rw-r--r--   0        0        0      579 2023-07-25 13:04:34.033870 transformers_js_py-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2964 2023-07-25 13:04:34.033870 transformers_js_py-0.1.7/transformers_js/__init__.py
--rw-r--r--   0        0        0     4429 1970-01-01 00:00:00.000000 transformers_js_py-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 13:42:11.214656 transformers_js_py-0.1.8/LICENSE
+-rw-r--r--   0        0        0     7153 2023-07-25 13:42:11.214656 transformers_js_py-0.1.8/README.md
+-rw-r--r--   0        0        0      579 2023-07-25 13:42:11.222657 transformers_js_py-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2964 2023-07-25 13:42:11.222657 transformers_js_py-0.1.8/transformers_js/__init__.py
+-rw-r--r--   0        0        0     7600 1970-01-01 00:00:00.000000 transformers_js_py-0.1.8/PKG-INFO
```

### Comparing `transformers_js_py-0.1.7/LICENSE` & `transformers_js_py-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `transformers_js_py-0.1.7/pyproject.toml` & `transformers_js_py-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transformers-js-py"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Yuichiro Tachibana (Tsuchiya) <t.yic.yt@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "transformers_js"}]
 
 [tool.poetry.dependencies]
```

### Comparing `transformers_js_py-0.1.7/transformers_js/__init__.py` & `transformers_js_py-0.1.8/transformers_js/__init__.py`

 * *Files identical despite different names*

