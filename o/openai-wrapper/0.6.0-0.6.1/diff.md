# Comparing `tmp/openai_wrapper-0.6.0.tar.gz` & `tmp/openai_wrapper-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_wrapper-0.6.0.tar", max compression
+gzip compressed data, was "openai_wrapper-0.6.1.tar", max compression
```

## Comparing `openai_wrapper-0.6.0.tar` & `openai_wrapper-0.6.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      134 2023-07-17 09:00:29.816401 openai_wrapper-0.6.0/openai_wrapper/__init__.py
--rw-r--r--   0        0        0     5605 2023-07-17 09:00:29.816401 openai_wrapper-0.6.0/openai_wrapper/chat_completion.py
--rw-r--r--   0        0        0    18790 2023-07-17 09:00:29.816401 openai_wrapper-0.6.0/openai_wrapper/completion.py
--rw-r--r--   0        0        0     2053 2023-07-17 09:00:29.816401 openai_wrapper-0.6.0/openai_wrapper/config.py
--rw-r--r--   0        0        0     4367 2023-07-17 09:00:29.816401 openai_wrapper-0.6.0/openai_wrapper/embeddings.py
--rw-r--r--   0        0        0      729 2023-07-17 09:00:29.820401 openai_wrapper-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 openai_wrapper-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      134 2023-07-25 10:42:03.390984 openai_wrapper-0.6.1/openai_wrapper/__init__.py
+-rw-r--r--   0        0        0     5605 2023-07-25 10:42:03.390984 openai_wrapper-0.6.1/openai_wrapper/chat_completion.py
+-rw-r--r--   0        0        0    18790 2023-07-25 10:42:03.390984 openai_wrapper-0.6.1/openai_wrapper/completion.py
+-rw-r--r--   0        0        0     2053 2023-07-25 10:42:03.390984 openai_wrapper-0.6.1/openai_wrapper/config.py
+-rw-r--r--   0        0        0     4367 2023-07-25 10:42:03.390984 openai_wrapper-0.6.1/openai_wrapper/embeddings.py
+-rw-r--r--   0        0        0      729 2023-07-25 10:42:03.390984 openai_wrapper-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 openai_wrapper-0.6.1/PKG-INFO
```

### Comparing `openai_wrapper-0.6.0/openai_wrapper/chat_completion.py` & `openai_wrapper-0.6.1/openai_wrapper/chat_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             logging.info(f"Updated default params. Updated params: {self.model_params}")
 
         self.experiment_metadata = experiment_metadata
         self.project_metadata = project_metadata
         self.extra_params = extra_params
 
     def create(self,
-             messages: List[Dict[str, str]],
+             messages: List[Dict[str, Any]],
              functions: List[Dict[str, Union[str, Dict[str, Any]]]] = None,
              preprocess_messages: Callable = _preprocess_messages,
              process_response: Callable = _process_response,
              preprocess_messages_args: Dict[Any, Any] = None,
              process_response_args: Dict[Any, Any] = None) -> Dict[Any, Any]:
         """
         Create a chat completion request and store it in MongoDB
```

### Comparing `openai_wrapper-0.6.0/openai_wrapper/completion.py` & `openai_wrapper-0.6.1/openai_wrapper/completion.py`

 * *Files identical despite different names*

### Comparing `openai_wrapper-0.6.0/openai_wrapper/config.py` & `openai_wrapper-0.6.1/openai_wrapper/config.py`

 * *Files identical despite different names*

### Comparing `openai_wrapper-0.6.0/openai_wrapper/embeddings.py` & `openai_wrapper-0.6.1/openai_wrapper/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_wrapper-0.6.0/pyproject.toml` & `openai_wrapper-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-wrapper"
-version = "0.6.0"
+version = "0.6.1"
 description = "A wrapper for OpenAI's python API which wraps around the openAI functions and stores the request, response and metadata to MongoDB. The stored data can be used to fine tune GPT-3 models or HuggingFace models."
 authors = ["AI Team <datascience@prosus.com>"]
 license = "MIT License"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 openai = "^0.27.2"
```

### Comparing `openai_wrapper-0.6.0/PKG-INFO` & `openai_wrapper-0.6.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-wrapper
-Version: 0.6.0
+Version: 0.6.1
 Summary: A wrapper for OpenAI's python API which wraps around the openAI functions and stores the request, response and metadata to MongoDB. The stored data can be used to fine tune GPT-3 models or HuggingFace models.
 License: MIT
 Author: AI Team
 Author-email: datascience@prosus.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

