# Comparing `tmp/chatlab-1.0.0a4.tar.gz` & `tmp/chatlab-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatlab-1.0.0a4.tar", max compression
+gzip compressed data, was "chatlab-1.0.0a5.tar", max compression
```

## Comparing `chatlab-1.0.0a4.tar` & `chatlab-1.0.0a5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1504 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/LICENSE
--rw-r--r--   0        0        0     6009 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/README.md
--rw-r--r--   0        0        0     2324 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/__init__.py
--rw-r--r--   0        0        0       30 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/_version.py
--rw-r--r--   0        0        0      407 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/builtins/__init__.py
--rw-r--r--   0        0        0     4956 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/builtins/noteable.py
--rw-r--r--   0        0        0     8330 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/builtins/python.py
--rw-r--r--   0        0        0    14242 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/conversation.py
--rw-r--r--   0        0        0     2358 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/decorators.py
--rw-r--r--   0        0        0     8006 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/display.py
--rw-r--r--   0        0        0      114 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/errors.py
--rw-r--r--   0        0        0     3304 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/markdown.py
--rw-r--r--   0        0        0     3290 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/messaging.py
--rw-r--r--   0        0        0     1869 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/models.py
--rw-r--r--   0        0        0      174 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/prompts.py
--rw-r--r--   0        0        0     8158 2023-07-24 14:55:48.264188 chatlab-1.0.0a4/chatlab/registry.py
--rw-r--r--   0        0        0     2653 2023-07-24 14:55:48.268188 chatlab-1.0.0a4/pyproject.toml
--rw-r--r--   0        0        0       37 2023-07-24 14:55:48.268188 chatlab-1.0.0a4/tests/__init__.py
--rw-r--r--   0        0        0      357 2023-07-24 14:55:48.268188 chatlab-1.0.0a4/tests/test_chatlab.py
--rw-r--r--   0        0        0     1103 2023-07-24 14:55:48.268188 chatlab-1.0.0a4/tests/test_decorators.py
--rw-r--r--   0        0        0     1066 2023-07-24 14:55:48.268188 chatlab-1.0.0a4/tests/test_messaging.py
--rw-r--r--   0        0        0     6052 2023-07-24 14:55:48.268188 chatlab-1.0.0a4/tests/test_registry.py
--rw-r--r--   0        0        0     7546 1970-01-01 00:00:00.000000 chatlab-1.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/LICENSE
+-rw-r--r--   0        0        0     6009 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/README.md
+-rw-r--r--   0        0        0     2324 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/chatlab/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/chatlab/_version.py
+-rw-r--r--   0        0        0      407 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/chatlab/builtins/__init__.py
+-rw-r--r--   0        0        0     7628 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/chatlab/builtins/noteable.py
+-rw-r--r--   0        0        0     8330 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/chatlab/builtins/python.py
+-rw-r--r--   0        0        0    14242 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/chatlab/conversation.py
+-rw-r--r--   0        0        0     2358 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/chatlab/decorators.py
+-rw-r--r--   0        0        0     8006 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/chatlab/display.py
+-rw-r--r--   0        0        0      114 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/chatlab/errors.py
+-rw-r--r--   0        0        0     3304 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/chatlab/markdown.py
+-rw-r--r--   0        0        0     3290 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/chatlab/messaging.py
+-rw-r--r--   0        0        0     1869 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/chatlab/models.py
+-rw-r--r--   0        0        0      174 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/chatlab/prompts.py
+-rw-r--r--   0        0        0     8158 2023-07-25 13:43:43.822773 chatlab-1.0.0a5/chatlab/registry.py
+-rw-r--r--   0        0        0     2776 2023-07-25 13:43:43.826773 chatlab-1.0.0a5/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-07-25 13:43:43.826773 chatlab-1.0.0a5/tests/__init__.py
+-rw-r--r--   0        0        0      357 2023-07-25 13:43:43.826773 chatlab-1.0.0a5/tests/test_chatlab.py
+-rw-r--r--   0        0        0     1103 2023-07-25 13:43:43.826773 chatlab-1.0.0a5/tests/test_decorators.py
+-rw-r--r--   0        0        0     1066 2023-07-25 13:43:43.826773 chatlab-1.0.0a5/tests/test_messaging.py
+-rw-r--r--   0        0        0     6052 2023-07-25 13:43:43.826773 chatlab-1.0.0a5/tests/test_registry.py
+-rw-r--r--   0        0        0     7637 1970-01-01 00:00:00.000000 chatlab-1.0.0a5/PKG-INFO
```

### Comparing `chatlab-1.0.0a4/LICENSE` & `chatlab-1.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a4/README.md` & `chatlab-1.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a4/chatlab/__init__.py` & `chatlab-1.0.0a5/chatlab/__init__.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a4/chatlab/builtins/python.py` & `chatlab-1.0.0a5/chatlab/builtins/python.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a4/chatlab/conversation.py` & `chatlab-1.0.0a5/chatlab/conversation.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a4/chatlab/decorators.py` & `chatlab-1.0.0a5/chatlab/decorators.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a4/chatlab/display.py` & `chatlab-1.0.0a5/chatlab/display.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a4/chatlab/markdown.py` & `chatlab-1.0.0a5/chatlab/markdown.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a4/chatlab/messaging.py` & `chatlab-1.0.0a5/chatlab/messaging.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a4/chatlab/models.py` & `chatlab-1.0.0a5/chatlab/models.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a4/chatlab/registry.py` & `chatlab-1.0.0a5/chatlab/registry.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a4/pyproject.toml` & `chatlab-1.0.0a5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "chatlab"
-version = "1.0.0-alpha.4"
+version = "1.0.0-alpha.5"
 homepage = "https://github.com/rgbkrk/chatlab"
 description = "Chat Plugin Experiments, Simplified. Create agents and give them superpowers in your notebooks."
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 3 - Alpha',
@@ -58,27 +58,33 @@
 bump2version = "^1.0.1"
 jinja2 = "^3.1.2"
 ipykernel = ">=6.0.0,<8.0.0"
 types-toml = "^0.10.8.6"
 pandas = "^2.0.2"
 
 [tool.poetry.extras]
+noteable = ["noteable-origami"]
+
 test = [
     "pytest",
     "black",
     "isort",
     "mypy",
     "flake8",
     "flake8-docstrings",
     "pytest-cov"
 ]
 
 dev = ["tox", "pre-commit", "virtualenv", "pip", "twine", "toml", "bump2version"]
 
 
+[tool.poetry.dependencies.noteable-origami]
+version = "1.0.0a1"
+allow-prereleases = true
+
 [tool.black]
 line-length = 120
 skip-string-normalization = true
 target-version = ['py37', 'py38']
 include = '\.pyi?$'
 exclude = '''
 /(
```

### Comparing `chatlab-1.0.0a4/tests/test_decorators.py` & `chatlab-1.0.0a5/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a4/tests/test_messaging.py` & `chatlab-1.0.0a5/tests/test_messaging.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a4/tests/test_registry.py` & `chatlab-1.0.0a5/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a4/PKG-INFO` & `chatlab-1.0.0a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatlab
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: Chat Plugin Experiments, Simplified. Create agents and give them superpowers in your notebooks.
 Home-page: https://github.com/rgbkrk/chatlab
 License: BSD-3-Clause
 Author: Kyle Kelley
 Author-email: rgbkrk@gmail.com
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -22,17 +22,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Artificial Life
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Provides-Extra: dev
+Provides-Extra: noteable
 Provides-Extra: test
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: ipython (>=7.0.0,<9.0.0)
+Requires-Dist: noteable-origami (==1.0.0a1) ; extra == "noteable"
 Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: repr-llm (>=0.2.0,<0.3.0)
 Requires-Dist: vdom (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # ChatLab
```

