# Comparing `tmp/coder_retriever-0.1.1.tar.gz` & `tmp/coder_retriever-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coder_retriever-0.1.1.tar", max compression
+gzip compressed data, was "coder_retriever-0.1.2.tar", max compression
```

## Comparing `coder_retriever-0.1.1.tar` & `coder_retriever-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       30 2023-07-25 07:44:46.520439 coder_retriever-0.1.1/coder_retriever/__init__.py
--rw-r--r--   0        0        0       40 2023-07-25 07:44:46.520439 coder_retriever-0.1.1/coder_retriever/ai/__init__.py
--rw-r--r--   0        0        0     4056 2023-07-25 08:15:22.524423 coder_retriever-0.1.1/coder_retriever/ai/assistant.py
--rw-r--r--   0        0        0     1088 2023-07-25 07:44:46.519440 coder_retriever-0.1.1/LICENSE
--rw-r--r--   0        0        0      631 2023-07-25 08:41:50.551486 coder_retriever-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      178 2023-07-25 07:44:46.519440 coder_retriever-0.1.1/README.md
--rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 coder_retriever-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-07-25 07:44:46.520439 coder_retriever-0.1.2/coder_retriever/__init__.py
+-rw-r--r--   0        0        0       40 2023-07-25 07:44:46.520439 coder_retriever-0.1.2/coder_retriever/ai/__init__.py
+-rw-r--r--   0        0        0     4056 2023-07-25 08:15:22.524423 coder_retriever-0.1.2/coder_retriever/ai/assistant.py
+-rw-r--r--   0        0        0     1088 2023-07-25 07:44:46.519440 coder_retriever-0.1.2/LICENSE
+-rw-r--r--   0        0        0      630 2023-07-25 08:47:58.694204 coder_retriever-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      178 2023-07-25 07:44:46.519440 coder_retriever-0.1.2/README.md
+-rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 coder_retriever-0.1.2/PKG-INFO
```

### Comparing `coder_retriever-0.1.1/coder_retriever/ai/assistant.py` & `coder_retriever-0.1.2/coder_retriever/ai/assistant.py`

 * *Files identical despite different names*

### Comparing `coder_retriever-0.1.1/LICENSE` & `coder_retriever-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coder_retriever-0.1.1/pyproject.toml` & `coder_retriever-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "coder-retriever"
-version = "0.1.1"
+version = "0.1.2"
 description = "Coder Retriever: your loyal coding companion"
 authors = ["GitMarco27 <72693100+GitMarco27@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "coder_retriever"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^0.27.8"
-numpy = "<=1.24"
+numpy = "<1.24"
 pandas = "^1.5.3"
 python-dotenv = "^1.0.0"
 matplotlib = "^3.7.2"
 
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `coder_retriever-0.1.1/PKG-INFO` & `coder_retriever-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: coder-retriever
-Version: 0.1.1
+Version: 0.1.2
 Summary: Coder Retriever: your loyal coding companion
 License: MIT
 Author: GitMarco27
 Author-email: 72693100+GitMarco27@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
-Requires-Dist: numpy (<=1.24)
+Requires-Dist: numpy (<1.24)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Coder Retriever 🦮
```

