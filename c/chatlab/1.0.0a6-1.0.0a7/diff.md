# Comparing `tmp/chatlab-1.0.0a6.tar.gz` & `tmp/chatlab-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatlab-1.0.0a6.tar", max compression
+gzip compressed data, was "chatlab-1.0.0a7.tar", max compression
```

## Comparing `chatlab-1.0.0a6.tar` & `chatlab-1.0.0a7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1504 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/LICENSE
--rw-r--r--   0        0        0     6009 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/README.md
--rw-r--r--   0        0        0     2324 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/chatlab/__init__.py
--rw-r--r--   0        0        0       30 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/chatlab/_version.py
--rw-r--r--   0        0        0      407 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/chatlab/builtins/__init__.py
--rw-r--r--   0        0        0     7628 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/chatlab/builtins/noteable.py
--rw-r--r--   0        0        0     8330 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/chatlab/builtins/python.py
--rw-r--r--   0        0        0    14242 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/chatlab/conversation.py
--rw-r--r--   0        0        0     2358 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/chatlab/decorators.py
--rw-r--r--   0        0        0     8006 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/chatlab/display.py
--rw-r--r--   0        0        0      114 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/chatlab/errors.py
--rw-r--r--   0        0        0     3304 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/chatlab/markdown.py
--rw-r--r--   0        0        0     3290 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/chatlab/messaging.py
--rw-r--r--   0        0        0     1869 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/chatlab/models.py
--rw-r--r--   0        0        0      174 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/chatlab/prompts.py
--rw-r--r--   0        0        0     8158 2023-07-25 13:54:18.277731 chatlab-1.0.0a6/chatlab/registry.py
--rw-r--r--   0        0        0     2858 2023-07-25 13:54:18.281731 chatlab-1.0.0a6/pyproject.toml
--rw-r--r--   0        0        0       37 2023-07-25 13:54:18.281731 chatlab-1.0.0a6/tests/__init__.py
--rw-r--r--   0        0        0      357 2023-07-25 13:54:18.281731 chatlab-1.0.0a6/tests/test_chatlab.py
--rw-r--r--   0        0        0     1103 2023-07-25 13:54:18.281731 chatlab-1.0.0a6/tests/test_decorators.py
--rw-r--r--   0        0        0     1066 2023-07-25 13:54:18.281731 chatlab-1.0.0a6/tests/test_messaging.py
--rw-r--r--   0        0        0     6052 2023-07-25 13:54:18.281731 chatlab-1.0.0a6/tests/test_registry.py
--rw-r--r--   0        0        0     7637 1970-01-01 00:00:00.000000 chatlab-1.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/LICENSE
+-rw-r--r--   0        0        0     6009 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/README.md
+-rw-r--r--   0        0        0     2324 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/_version.py
+-rw-r--r--   0        0        0      407 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/builtins/__init__.py
+-rw-r--r--   0        0        0     7628 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/builtins/noteable.py
+-rw-r--r--   0        0        0     8330 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/builtins/python.py
+-rw-r--r--   0        0        0    14242 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/conversation.py
+-rw-r--r--   0        0        0     2358 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/decorators.py
+-rw-r--r--   0        0        0     8006 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/display.py
+-rw-r--r--   0        0        0      114 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/errors.py
+-rw-r--r--   0        0        0     3304 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/markdown.py
+-rw-r--r--   0        0        0     3290 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/messaging.py
+-rw-r--r--   0        0        0     1869 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/models.py
+-rw-r--r--   0        0        0      174 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/prompts.py
+-rw-r--r--   0        0        0     8158 2023-07-25 14:05:00.805150 chatlab-1.0.0a7/chatlab/registry.py
+-rw-r--r--   0        0        0     2814 2023-07-25 14:05:00.805150 chatlab-1.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-07-25 14:05:00.805150 chatlab-1.0.0a7/tests/__init__.py
+-rw-r--r--   0        0        0      357 2023-07-25 14:05:00.805150 chatlab-1.0.0a7/tests/test_chatlab.py
+-rw-r--r--   0        0        0     1103 2023-07-25 14:05:00.805150 chatlab-1.0.0a7/tests/test_decorators.py
+-rw-r--r--   0        0        0     1066 2023-07-25 14:05:00.805150 chatlab-1.0.0a7/tests/test_messaging.py
+-rw-r--r--   0        0        0     6052 2023-07-25 14:05:00.805150 chatlab-1.0.0a7/tests/test_registry.py
+-rw-r--r--   0        0        0     7703 1970-01-01 00:00:00.000000 chatlab-1.0.0a7/PKG-INFO
```

### Comparing `chatlab-1.0.0a6/LICENSE` & `chatlab-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/README.md` & `chatlab-1.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/chatlab/__init__.py` & `chatlab-1.0.0a7/chatlab/__init__.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/chatlab/builtins/noteable.py` & `chatlab-1.0.0a7/chatlab/builtins/noteable.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/chatlab/builtins/python.py` & `chatlab-1.0.0a7/chatlab/builtins/python.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/chatlab/conversation.py` & `chatlab-1.0.0a7/chatlab/conversation.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/chatlab/decorators.py` & `chatlab-1.0.0a7/chatlab/decorators.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/chatlab/display.py` & `chatlab-1.0.0a7/chatlab/display.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/chatlab/markdown.py` & `chatlab-1.0.0a7/chatlab/markdown.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/chatlab/messaging.py` & `chatlab-1.0.0a7/chatlab/messaging.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/chatlab/models.py` & `chatlab-1.0.0a7/chatlab/models.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/chatlab/registry.py` & `chatlab-1.0.0a7/chatlab/registry.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/pyproject.toml` & `chatlab-1.0.0a7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "chatlab"
-version = "1.0.0-alpha.6"
+version = "1.0.0-alpha.7"
 homepage = "https://github.com/rgbkrk/chatlab"
 description = "Chat Plugin Experiments, Simplified. Create agents and give them superpowers in your notebooks."
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 3 - Alpha',
@@ -36,14 +36,15 @@
 python = ">=3.9.0,<3.12"
 ipython = ">=7.0.0,<9.0.0"
 openai = "^0.27.4"
 pydantic = ">=1.9.0,<2.0.0"
 vdom = "^1.0.0"
 deprecation = "^2.1.0"
 repr-llm = "^0.2.0"
+python-ulid = "^1.1.0"
 
 [tool.poetry.group.dev.dependencies]
 tox = "^4.4.11"
 black = "^23.3.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 flake8-docstrings = "^1.7.0"
@@ -57,18 +58,14 @@
 toml = "^0.10.2"
 bump2version = "^1.0.1"
 jinja2 = "^3.1.2"
 ipykernel = ">=6.0.0,<8.0.0"
 types-toml = "^0.10.8.6"
 pandas = "^2.0.2"
 
-
-[tool.poetry.group.noteable.dependencies]
-python-ulid = "^1.1.0"
-
 [tool.poetry.extras]
 noteable = ["noteable-origami", "python-ulid"]
 
 test = [
     "pytest",
     "black",
     "isort",
```

### Comparing `chatlab-1.0.0a6/tests/test_decorators.py` & `chatlab-1.0.0a7/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/tests/test_messaging.py` & `chatlab-1.0.0a7/tests/test_messaging.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/tests/test_registry.py` & `chatlab-1.0.0a7/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a6/PKG-INFO` & `chatlab-1.0.0a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatlab
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: Chat Plugin Experiments, Simplified. Create agents and give them superpowers in your notebooks.
 Home-page: https://github.com/rgbkrk/chatlab
 License: BSD-3-Clause
 Author: Kyle Kelley
 Author-email: rgbkrk@gmail.com
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -29,14 +29,15 @@
 Provides-Extra: noteable
 Provides-Extra: test
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: ipython (>=7.0.0,<9.0.0)
 Requires-Dist: noteable-origami (==1.0.0a1) ; extra == "noteable"
 Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: python-ulid (>=1.1.0,<2.0.0) ; extra == "noteable"
 Requires-Dist: repr-llm (>=0.2.0,<0.3.0)
 Requires-Dist: vdom (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # ChatLab
 
 **Chat Experiments, Simplified**
```

