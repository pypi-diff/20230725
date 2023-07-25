# Comparing `tmp/transformers_js_py-0.1.5.tar.gz` & `tmp/transformers_js_py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers_js_py-0.1.5.tar", max compression
+gzip compressed data, was "transformers_js_py-0.1.6.tar", max compression
```

## Comparing `transformers_js_py-0.1.5.tar` & `transformers_js_py-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-07-23 00:23:23.289673 transformers_js_py-0.1.5/LICENSE
--rw-r--r--   0        0        0       21 2023-07-23 00:23:23.289673 transformers_js_py-0.1.5/README.md
--rw-r--r--   0        0        0      579 2023-07-23 00:23:23.289673 transformers_js_py-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2755 2023-07-23 00:23:23.289673 transformers_js_py-0.1.5/transformers_js/__init__.py
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 transformers_js_py-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 12:46:01.630470 transformers_js_py-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3879 2023-07-25 12:46:01.634470 transformers_js_py-0.1.6/README.md
+-rw-r--r--   0        0        0      579 2023-07-25 12:46:01.634470 transformers_js_py-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2755 2023-07-25 12:46:01.634470 transformers_js_py-0.1.6/transformers_js/__init__.py
+-rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 transformers_js_py-0.1.6/PKG-INFO
```

### Comparing `transformers_js_py-0.1.5/LICENSE` & `transformers_js_py-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `transformers_js_py-0.1.5/pyproject.toml` & `transformers_js_py-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transformers-js-py"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Yuichiro Tachibana (Tsuchiya) <t.yic.yt@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "transformers_js"}]
 
 [tool.poetry.dependencies]
```

### Comparing `transformers_js_py-0.1.5/transformers_js/__init__.py` & `transformers_js_py-0.1.6/transformers_js/__init__.py`

 * *Files identical despite different names*

