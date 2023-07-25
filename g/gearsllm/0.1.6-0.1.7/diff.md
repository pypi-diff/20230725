# Comparing `tmp/gearsllm-0.1.6.tar.gz` & `tmp/gearsllm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gearsllm-0.1.6.tar", max compression
+gzip compressed data, was "gearsllm-0.1.7.tar", max compression
```

## Comparing `gearsllm-0.1.6.tar` & `gearsllm-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1062 2023-07-22 21:52:20.719532 gearsllm-0.1.6/LICENSE
--rw-r--r--   0        0        0      318 2023-07-23 22:37:37.759113 gearsllm-0.1.6/README.md
--rw-r--r--   0        0        0      141 2023-07-23 22:07:23.763584 gearsllm-0.1.6/gears/__init__.py
--rw-r--r--   0        0        0     2108 2023-07-24 03:27:57.611972 gearsllm-0.1.6/gears/gear.py
--rw-r--r--   0        0        0     2592 2023-07-24 03:10:17.813919 gearsllm-0.1.6/gears/history.py
--rw-r--r--   0        0        0      105 2023-07-23 22:12:10.360968 gearsllm-0.1.6/gears/llms/__init__.py
--rw-r--r--   0        0        0      234 2023-07-23 07:06:32.890807 gearsllm-0.1.6/gears/llms/base.py
--rw-r--r--   0        0        0      930 2023-07-23 22:12:06.460243 gearsllm-0.1.6/gears/llms/echo.py
--rw-r--r--   0        0        0     3779 2023-07-24 03:02:10.728788 gearsllm-0.1.6/gears/llms/oai.py
--rw-r--r--   0        0        0     1307 2023-07-23 22:33:03.565128 gearsllm-0.1.6/gears/utils.py
--rw-r--r--   0        0        0      554 2023-07-24 03:28:25.445179 gearsllm-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 gearsllm-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-22 21:52:20.719532 gearsllm-0.1.7/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-23 22:37:37.759113 gearsllm-0.1.7/README.md
+-rw-r--r--   0        0        0      141 2023-07-23 22:07:23.763584 gearsllm-0.1.7/gears/__init__.py
+-rw-r--r--   0        0        0     2108 2023-07-25 17:57:17.857188 gearsllm-0.1.7/gears/gear.py
+-rw-r--r--   0        0        0     2592 2023-07-24 03:10:17.813919 gearsllm-0.1.7/gears/history.py
+-rw-r--r--   0        0        0      105 2023-07-23 22:12:10.360968 gearsllm-0.1.7/gears/llms/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-23 07:06:32.890807 gearsllm-0.1.7/gears/llms/base.py
+-rw-r--r--   0        0        0      930 2023-07-23 22:12:06.460243 gearsllm-0.1.7/gears/llms/echo.py
+-rw-r--r--   0        0        0     3779 2023-07-24 03:02:10.728788 gearsllm-0.1.7/gears/llms/oai.py
+-rw-r--r--   0        0        0     1307 2023-07-23 22:33:03.565128 gearsllm-0.1.7/gears/utils.py
+-rw-r--r--   0        0        0      676 2023-07-25 19:20:10.330958 gearsllm-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 gearsllm-0.1.7/PKG-INFO
```

### Comparing `gearsllm-0.1.6/LICENSE` & `gearsllm-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.6/gears/gear.py` & `gearsllm-0.1.7/gears/gear.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,29 +14,29 @@
 
 class Gear:
     def __init__(
         self,
         model: BaseLLM,
     ):
         self.model = model
-        self.template = Template(self.template())
+        self.template = self.template()
 
     async def run(
         self,
         data: BaseModel,
         history: History,
         **kwargs,
     ):
         # Construct the template with the pydantic model
         try:
             items = data.model_dump()
         except AttributeError:
             items = data.dict()
 
-        prompt = self.template.render(items)
+        prompt = Template(self.template).render(items)
 
         # Call the model
         logger.info(f"Running model with prompt: {prompt}")
         response = await self.model.run(prompt, history, **kwargs)
 
         # Transform the data from the response
         try:
```

### Comparing `gearsllm-0.1.6/gears/history.py` & `gearsllm-0.1.7/gears/history.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.6/gears/llms/echo.py` & `gearsllm-0.1.7/gears/llms/echo.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.6/gears/llms/oai.py` & `gearsllm-0.1.7/gears/llms/oai.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.6/gears/utils.py` & `gearsllm-0.1.7/gears/utils.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.6/pyproject.toml` & `gearsllm-0.1.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gearsllm"
-version = "0.1.6"
+version = "0.1.7"
 description = "Lightweight library for building LLM-based control flow."
 authors = ["Shreya Shankar <ss.shankar505@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "gears"}]
 
 [tool.poetry.dependencies]
@@ -15,11 +15,16 @@
 tenacity = "^8.2.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
 rich = "^13.4.2"
+mkdocs = "^1.4.3"
+mkdocs-material = "^9.1.19"
+mkdocstrings-python = "^1.2.1"
+pytkdocs = "^0.16.1"
+linkchecker = "^10.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gearsllm-0.1.6/PKG-INFO` & `gearsllm-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gearsllm
-Version: 0.1.6
+Version: 0.1.7
 Summary: Lightweight library for building LLM-based control flow.
 License: MIT
 Author: Shreya Shankar
 Author-email: ss.shankar505@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

