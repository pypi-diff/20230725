# Comparing `tmp/pykli-1.1.3.tar.gz` & `tmp/pykli-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykli-1.1.3.tar", max compression
+gzip compressed data, was "pykli-1.1.4.tar", max compression
```

## Comparing `pykli-1.1.3.tar` & `pykli-1.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1075 2023-07-25 11:59:52.163519 pykli-1.1.3/LICENSE
--rw-r--r--   0        0        0     1693 2023-07-25 11:59:52.163519 pykli-1.1.3/README.md
--rw-r--r--   0        0        0      549 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/__init__.py
--rw-r--r--   0        0        0     1087 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/__main__.py
--rw-r--r--   0        0        0     2402 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/completer.py
--rw-r--r--   0        0        0     1145 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/keybindgings.py
--rw-r--r--   0        0        0     1792 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/ksqldb.py
--rw-r--r--   0        0        0     2097 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/repl_eval.py
--rw-r--r--   0        0        0     9044 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/repl_print.py
--rw-r--r--   0        0        0     3291 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/repl_read.py
--rw-r--r--   0        0        0      960 2023-07-25 11:59:52.163519 pykli-1.1.3/pykli/tokens.py
--rw-r--r--   0        0        0     1108 2023-07-25 11:59:52.163519 pykli-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2649 1970-01-01 00:00:00.000000 pykli-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-25 17:46:38.480974 pykli-1.1.4/LICENSE
+-rw-r--r--   0        0        0     1693 2023-07-25 17:46:38.480974 pykli-1.1.4/README.md
+-rw-r--r--   0        0        0      549 2023-07-25 17:46:38.480974 pykli-1.1.4/pykli/__init__.py
+-rw-r--r--   0        0        0     1084 2023-07-25 17:46:38.480974 pykli-1.1.4/pykli/__main__.py
+-rw-r--r--   0        0        0     2402 2023-07-25 17:46:38.480974 pykli-1.1.4/pykli/completer.py
+-rw-r--r--   0        0        0     1145 2023-07-25 17:46:38.480974 pykli-1.1.4/pykli/keybindgings.py
+-rw-r--r--   0        0        0     1792 2023-07-25 17:46:38.480974 pykli-1.1.4/pykli/ksqldb.py
+-rw-r--r--   0        0        0     2097 2023-07-25 17:46:38.480974 pykli-1.1.4/pykli/repl_eval.py
+-rw-r--r--   0        0        0     9044 2023-07-25 17:46:38.480974 pykli-1.1.4/pykli/repl_print.py
+-rw-r--r--   0        0        0     3264 2023-07-25 17:46:38.480974 pykli-1.1.4/pykli/repl_read.py
+-rw-r--r--   0        0        0      960 2023-07-25 17:46:38.480974 pykli-1.1.4/pykli/tokens.py
+-rw-r--r--   0        0        0     1218 2023-07-25 17:47:24.585325 pykli-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2649 1970-01-01 00:00:00.000000 pykli-1.1.4/PKG-INFO
```

### Comparing `pykli-1.1.3/LICENSE` & `pykli-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pykli-1.1.3/README.md` & `pykli-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pykli-1.1.3/pykli/__init__.py` & `pykli-1.1.4/pykli/__init__.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.3/pykli/__main__.py` & `pykli-1.1.4/pykli/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,20 +22,21 @@
     \b SERVER The address of the ksqlDB server."""
 
     LOG.info(f"pyKLI started: server={server}, file={file}")
 
     initialize_sqlparse()
 
     eval = pykli_eval(KsqlDBClient(server))
-    prompt = pykli_prompt() if file is None else file_prompt(file)
 
     if isinstance(pykli_print(eval(Info(server))), ErrMsg):
         sys.exit(1)
 
-    evaluated = (tt for t in pykli_read(prompt) if (tt := eval(t)) is not None)
+    read = pykli_read(pykli_prompt() if file is None else file_prompt(file))
+
+    evaluated = (tt for t in read if (tt := eval(t)) is not None)
     for t in evaluated:
         pykli_print(t)
 
     sys.exit(0)
 
 
 if __name__ == "__main__":
```

### Comparing `pykli-1.1.3/pykli/completer.py` & `pykli-1.1.4/pykli/completer.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.3/pykli/keybindgings.py` & `pykli-1.1.4/pykli/keybindgings.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.3/pykli/ksqldb.py` & `pykli-1.1.4/pykli/ksqldb.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.3/pykli/repl_eval.py` & `pykli-1.1.4/pykli/repl_eval.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.3/pykli/repl_print.py` & `pykli-1.1.4/pykli/repl_print.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.3/pykli/repl_read.py` & `pykli-1.1.4/pykli/repl_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from sqlparse.sql import Comparison, Identifier
 import sqlparse
 
 from . import MONOKAI_STYLE, HISTORY_FILE, LOG
 from .completer import pykli_completer
 from .keybindgings import pykli_keys
 from .tokens import KSQL, Stmt, ErrMsg, PullQuery, SessionVar
-from .repl_print import pok
+
 
 class file_prompt:
     def __init__(self, path):
         self._path = path
 
     def __call__(self):
         if  self._path:
```

### Comparing `pykli-1.1.3/pykli/tokens.py` & `pykli-1.1.4/pykli/tokens.py`

 * *Files identical despite different names*

### Comparing `pykli-1.1.3/pyproject.toml` & `pykli-1.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyKLI"
-version = "0"
+version = "1.1.4"
 description = "Interactive ksqlDB command line client with autocompletion and syntax highlighting"
 license = "MIT"
 authors = ["Ievgenii Shepeliuk <eshepelyuk@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/eshepelyuk/pykli"
 repository = "https://github.com/eshepelyuk/pykli"
 keywords = ["cli", "kafka", "tui", "confluent", "ksql", "ksqldb"]
@@ -25,20 +25,23 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-mock = "^3.11.1"
 exceptiongroup = {version = "^1", python = "<3.11"}
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.ruff]
 line-length = 140
 
 [tool.pytest.ini_options]
 markers = [
     "e2e: e2e tests",
 ]
 
-[tool.poetry-version-plugin]
-source = "git-tag"
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+pattern = "default-unprefixed"
+metadata = false
```

### Comparing `pykli-1.1.3/PKG-INFO` & `pykli-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykli
-Version: 1.1.3
+Version: 1.1.4
 Summary: Interactive ksqlDB command line client with autocompletion and syntax highlighting
 Home-page: https://github.com/eshepelyuk/pykli
 License: MIT
 Keywords: cli,kafka,tui,confluent,ksql,ksqldb
 Author: Ievgenii Shepeliuk
 Author-email: eshepelyuk@gmail.com
 Requires-Python: >=3.10,<4.0
```

