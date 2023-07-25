# Comparing `tmp/gearsllm-0.1.7.tar.gz` & `tmp/gearsllm-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gearsllm-0.1.7.tar", max compression
+gzip compressed data, was "gearsllm-0.1.8.tar", max compression
```

## Comparing `gearsllm-0.1.7.tar` & `gearsllm-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1062 2023-07-22 21:52:20.719532 gearsllm-0.1.7/LICENSE
--rw-r--r--   0        0        0      318 2023-07-23 22:37:37.759113 gearsllm-0.1.7/README.md
--rw-r--r--   0        0        0      141 2023-07-23 22:07:23.763584 gearsllm-0.1.7/gears/__init__.py
--rw-r--r--   0        0        0     2108 2023-07-25 17:57:17.857188 gearsllm-0.1.7/gears/gear.py
--rw-r--r--   0        0        0     2592 2023-07-24 03:10:17.813919 gearsllm-0.1.7/gears/history.py
--rw-r--r--   0        0        0      105 2023-07-23 22:12:10.360968 gearsllm-0.1.7/gears/llms/__init__.py
--rw-r--r--   0        0        0      234 2023-07-23 07:06:32.890807 gearsllm-0.1.7/gears/llms/base.py
--rw-r--r--   0        0        0      930 2023-07-23 22:12:06.460243 gearsllm-0.1.7/gears/llms/echo.py
--rw-r--r--   0        0        0     3779 2023-07-24 03:02:10.728788 gearsllm-0.1.7/gears/llms/oai.py
--rw-r--r--   0        0        0     1307 2023-07-23 22:33:03.565128 gearsllm-0.1.7/gears/utils.py
--rw-r--r--   0        0        0      676 2023-07-25 19:20:10.330958 gearsllm-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 gearsllm-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-22 21:52:20.719532 gearsllm-0.1.8/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-23 22:37:37.759113 gearsllm-0.1.8/README.md
+-rw-r--r--   0        0        0      141 2023-07-23 22:07:23.763584 gearsllm-0.1.8/gears/__init__.py
+-rw-r--r--   0        0        0     2108 2023-07-25 17:57:17.857188 gearsllm-0.1.8/gears/gear.py
+-rw-r--r--   0        0        0     2592 2023-07-24 03:10:17.813919 gearsllm-0.1.8/gears/history.py
+-rw-r--r--   0        0        0      141 2023-07-25 19:38:23.801725 gearsllm-0.1.8/gears/llms/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-23 07:06:32.890807 gearsllm-0.1.8/gears/llms/base.py
+-rw-r--r--   0        0        0      930 2023-07-23 22:12:06.460243 gearsllm-0.1.8/gears/llms/echo.py
+-rw-r--r--   0        0        0     5556 2023-07-25 19:40:27.492346 gearsllm-0.1.8/gears/llms/oai.py
+-rw-r--r--   0        0        0     1307 2023-07-23 22:33:03.565128 gearsllm-0.1.8/gears/utils.py
+-rw-r--r--   0        0        0      676 2023-07-25 19:41:27.026735 gearsllm-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 gearsllm-0.1.8/PKG-INFO
```

### Comparing `gearsllm-0.1.7/LICENSE` & `gearsllm-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.7/gears/gear.py` & `gearsllm-0.1.8/gears/gear.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.7/gears/history.py` & `gearsllm-0.1.8/gears/history.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.7/gears/llms/echo.py` & `gearsllm-0.1.8/gears/llms/echo.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.7/gears/llms/oai.py` & `gearsllm-0.1.8/gears/llms/oai.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,18 +24,26 @@
 
 
 OPENAI_PRICING_MAP = {
     "gpt-3.5-turbo": {
         "prompt_tokens": float(0.0015 / 1000),
         "completion_tokens": float(0.002 / 1000),
     },
+    "gpt-35-turbo": {
+        "prompt_tokens": float(0.0015 / 1000),
+        "completion_tokens": float(0.002 / 1000),
+    },
     "gpt-3.5-turbo-16k": {
         "prompt_tokens": float(0.003 / 1000),
         "completion_tokens": float(0.004 / 1000),
     },
+    "gpt-35-turbo-16k": {
+        "prompt_tokens": float(0.003 / 1000),
+        "completion_tokens": float(0.004 / 1000),
+    },
     "gpt-4": {
         "prompt_tokens": float(0.03 / 1000),
         "completion_tokens": float(0.06 / 1000),
     },
     "gpt-4-32k": {
         "prompt_tokens": float(0.06 / 1000),
         "completion_tokens": float(0.12 / 1000),
@@ -80,15 +88,15 @@
             )
             raise
 
     async def run(
         self,
         prompt: str,
         history: History,
-        message_kwargs: dict = {},
+        **message_kwargs: Any,
     ) -> Any:
         # Construct chat history
         curr_message = Message(role="user", content=prompt, **message_kwargs)
         history.add(curr_message)
         try:
             messages = [m.model_dump() for m in history]
         except AttributeError:
@@ -98,14 +106,62 @@
             "messages": messages,
             **self.api_kwargs,
         }
         response = await self.chat_api_call(request)
         returned_message = response["choices"][0]["message"]["content"]
         history.add(
             Message(
+                role=response["choices"][0]["message"]["role"],
+                content=returned_message,
+            )
+        )
+
+        # Increment cost
+        try:
+            prompt_tokens = response["usage"]["prompt_tokens"]
+            completion_tokens = response["usage"]["completion_tokens"]
+
+            cost = (
+                OPENAI_PRICING_MAP[self.model_base]["prompt_tokens"]
+                * prompt_tokens
+                + OPENAI_PRICING_MAP[self.model_base]["completion_tokens"]
+                * completion_tokens
+            )
+            history.increment_cost(cost)
+        except KeyError:
+            logger.error(
+                f"Could not find pricing for model {self.model}. Not incrementing cost."
+            )
+
+        return response
+
+
+class AzureOpenAIChat(OpenAIChat):
+    async def run(
+        self,
+        prompt: str,
+        history: History,
+        **message_kwargs: Any,
+    ) -> Any:
+        # Construct chat history
+        curr_message = Message(role="user", content=prompt, **message_kwargs)
+        history.add(curr_message)
+        try:
+            messages = [m.model_dump() for m in history]
+        except AttributeError:
+            messages = [m.dict() for m in history]
+        request = {
+            "engine": self.model,
+            "messages": messages,
+            **self.api_kwargs,
+        }
+        response = await self.chat_api_call(request)
+        returned_message = response["choices"][0]["message"]["content"]
+        history.add(
+            Message(
                 role=response["choices"][0]["message"]["role"],
                 content=returned_message,
             )
         )
 
         # Increment cost
         try:
```

### Comparing `gearsllm-0.1.7/gears/utils.py` & `gearsllm-0.1.8/gears/utils.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.7/pyproject.toml` & `gearsllm-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gearsllm"
-version = "0.1.7"
+version = "0.1.8"
 description = "Lightweight library for building LLM-based control flow."
 authors = ["Shreya Shankar <ss.shankar505@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "gears"}]
 
 [tool.poetry.dependencies]
```

### Comparing `gearsllm-0.1.7/PKG-INFO` & `gearsllm-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gearsllm
-Version: 0.1.7
+Version: 0.1.8
 Summary: Lightweight library for building LLM-based control flow.
 License: MIT
 Author: Shreya Shankar
 Author-email: ss.shankar505@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

