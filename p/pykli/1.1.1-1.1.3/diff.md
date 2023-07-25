# Comparing `tmp/pykli-1.1.1.tar.gz` & `tmp/pykli-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykli-1.1.1.tar", max compression
+gzip compressed data, was "pykli-1.1.3.tar", max compression
```

## Comparing `pykli-1.1.1.tar` & `pykli-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1075 2023-07-25 07:38:07.057785 pykli-1.1.1/LICENSE
--rw-r--r--   0        0        0     1693 2023-07-25 07:38:07.057785 pykli-1.1.1/README.md
--rw-r--r--   0        0        0      549 2023-07-25 07:38:07.057785 pykli-1.1.1/pykli/__init__.py
--rw-r--r--   0        0        0     1087 2023-07-25 07:38:07.057785 pykli-1.1.1/pykli/__main__.py
--rw-r--r--   0        0        0     2402 2023-07-25 07:38:07.057785 pykli-1.1.1/pykli/completer.py
--rw-r--r--   0        0        0     1145 2023-07-25 07:38:07.057785 pykli-1.1.1/pykli/keybindgings.py
--rw-r--r--   0        0        0     1792 2023-07-25 07:38:07.057785 pykli-1.1.1/pykli/ksqldb.py
--rw-r--r--   0        0        0     2097 2023-07-25 07:38:07.057785 pykli-1.1.1/pykli/repl_eval.py
--rw-r--r--   0        0        0     9044 2023-07-25 07:38:07.057785 pykli-1.1.1/pykli/repl_print.py
--rw-r--r--   0        0        0     3291 2023-07-25 07:38:07.057785 pykli-1.1.1/pykli/repl_read.py
--rw-r--r--   0        0        0      960 2023-07-25 07:38:07.057785 pykli-1.1.1/pykli/tokens.py
--rw-r--r--   0        0        0     1063 2023-07-25 07:38:07.061786 pykli-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2649 1970-01-01 00:00:00.000000 pykli-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-25 11:59:52.163519 pykli-1.1.3/LICENSE
+-rw-r--r--   0        0        0     1693 2023-07-25 11:59:52.163519 pykli-1.1.3/README.md
+-rw-r--r--   0        0        0      549 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/__init__.py
+-rw-r--r--   0        0        0     1087 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/__main__.py
+-rw-r--r--   0        0        0     2402 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/completer.py
+-rw-r--r--   0        0        0     1145 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/keybindgings.py
+-rw-r--r--   0        0        0     1792 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/ksqldb.py
+-rw-r--r--   0        0        0     2097 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/repl_eval.py
+-rw-r--r--   0        0        0     9044 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/repl_print.py
+-rw-r--r--   0        0        0     3291 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/repl_read.py
+-rw-r--r--   0        0        0      960 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/tokens.py
+-rw-r--r--   0        0        0     1108 2023-07-25 11:59:52.163519 pykli-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2649 1970-01-01 00:00:00.000000 pykli-1.1.3/PKG-INFO
```

### Comparing `pykli-1.1.1/LICENSE` & `pykli-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pykli-1.1.1/README.md` & `pykli-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pykli-1.1.1/pykli/__init__.py` & `pykli-1.1.3/pykli/__init__.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.1/pykli/__main__.py` & `pykli-1.1.3/pykli/__main__.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.1/pykli/completer.py` & `pykli-1.1.3/pykli/completer.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.1/pykli/keybindgings.py` & `pykli-1.1.3/pykli/keybindgings.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.1/pykli/ksqldb.py` & `pykli-1.1.3/pykli/ksqldb.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.1/pykli/repl_eval.py` & `pykli-1.1.3/pykli/repl_eval.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.1/pykli/repl_print.py` & `pykli-1.1.3/pykli/repl_print.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.1/pykli/repl_read.py` & `pykli-1.1.3/pykli/repl_read.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.1/pykli/tokens.py` & `pykli-1.1.3/pykli/tokens.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.1/pyproject.toml` & `pykli-1.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyKLI"
-version = "1.1.1"
+version = "0"
 description = "Interactive ksqlDB command line client with autocompletion and syntax highlighting"
 license = "MIT"
 authors = ["Ievgenii Shepeliuk <eshepelyuk@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/eshepelyuk/pykli"
 repository = "https://github.com/eshepelyuk/pykli"
 keywords = ["cli", "kafka", "tui", "confluent", "ksql", "ksqldb"]
@@ -35,7 +35,10 @@
 [tool.ruff]
 line-length = 140
 
 [tool.pytest.ini_options]
 markers = [
     "e2e: e2e tests",
 ]
+
+[tool.poetry-version-plugin]
+source = "git-tag"
```

### Comparing `pykli-1.1.1/PKG-INFO` & `pykli-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykli
-Version: 1.1.1
+Version: 1.1.3
 Summary: Interactive ksqlDB command line client with autocompletion and syntax highlighting
 Home-page: https://github.com/eshepelyuk/pykli
 License: MIT
 Keywords: cli,kafka,tui,confluent,ksql,ksqldb
 Author: Ievgenii Shepeliuk
 Author-email: eshepelyuk@gmail.com
 Requires-Python: >=3.10,<4.0
```

