# Comparing `tmp/parea_ai-0.1.1a3.tar.gz` & `tmp/parea_ai-0.1.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parea_ai-0.1.1a3.tar", max compression
+gzip compressed data, was "parea_ai-0.1.1a4.tar", max compression
```

## Comparing `parea_ai-0.1.1a3.tar` & `parea_ai-0.1.1a4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10885 2023-07-24 02:40:37.935778 parea_ai-0.1.1a3/LICENSE
--rw-r--r--   0        0        0     3840 2023-07-24 21:35:08.489913 parea_ai-0.1.1a3/README.md
--rw-r--r--   0        0        0      595 2023-07-24 19:44:01.025559 parea_ai-0.1.1a3/parea/__init__.py
--rw-r--r--   0        0        0     2262 2023-07-25 01:36:19.918040 parea_ai-0.1.1a3/parea/api_client.py
--rw-r--r--   0        0        0     1548 2023-07-24 22:28:01.808010 parea_ai-0.1.1a3/parea/client.py
--rw-r--r--   0        0        0     1726 2023-07-25 00:59:38.687497 parea_ai-0.1.1a3/parea/example.py
--rw-r--r--   0        0        0     2099 2023-07-25 01:33:48.747173 parea_ai-0.1.1a3/parea/schemas/models.py
--rw-r--r--   0        0        0     3525 2023-07-25 01:36:39.930418 parea_ai-0.1.1a3/pyproject.toml
--rw-r--r--   0        0        0     4890 1970-01-01 00:00:00.000000 parea_ai-0.1.1a3/PKG-INFO
+-rw-r--r--   0        0        0    10885 2023-07-24 02:40:37.935778 parea_ai-0.1.1a4/LICENSE
+-rw-r--r--   0        0        0     3832 2023-07-25 03:24:03.665035 parea_ai-0.1.1a4/README.md
+-rw-r--r--   0        0        0      595 2023-07-24 19:44:01.025559 parea_ai-0.1.1a4/parea/__init__.py
+-rw-r--r--   0        0        0     2275 2023-07-25 03:22:09.962330 parea_ai-0.1.1a4/parea/api_client.py
+-rw-r--r--   0        0        0     1548 2023-07-25 01:43:54.277567 parea_ai-0.1.1a4/parea/client.py
+-rw-r--r--   0        0        0     1731 2023-07-25 03:24:03.661188 parea_ai-0.1.1a4/parea/example.py
+-rw-r--r--   0        0        0     2099 2023-07-25 01:43:54.278049 parea_ai-0.1.1a4/parea/schemas/models.py
+-rw-r--r--   0        0        0     3525 2023-07-25 03:24:09.085940 parea_ai-0.1.1a4/pyproject.toml
+-rw-r--r--   0        0        0     4882 1970-01-01 00:00:00.000000 parea_ai-0.1.1a4/PKG-INFO
```

### Comparing `parea_ai-0.1.1a3/LICENSE` & `parea_ai-0.1.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `parea_ai-0.1.1a3/README.md` & `parea_ai-0.1.1a4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -41,29 +41,29 @@
 p = Parea(api_key=os.getenv("API_KEY"))
 
 # You will find this deployment_id in the Parea dashboard
 deployment_id = '<DEPLOYMENT_ID>'
 
 # Assuming your deployed prompt's message is:
 # {"role": "user", "content": "Write a hello world program using {{x}} and the {{y}} framework."}
-inputs = {"inputs": {"x": "Golang", "y": "Fiber"}}
+inputs = {"x": "Golang", "y": "Fiber"}
 
 # You can easily unpack a dictionary into an attrs class
 test_completion = Completion(
   **{
     "deployment_id": deployment_id,
     "llm_inputs": inputs,
     "metadata": {"purpose": "testing"}
   }
 )
 
 # By passing in my inputs, in addition to the raw message with unfilled variables {{x}} and {{y}}, 
 # you we will also get the filled-in prompt:
 # {"role": "user", "content": "Write a hello world program using Golang and the Fiber framework."}
-test_get_prompt = UseDeployedPrompt(deployment_id=deployment_id, inputs=inputs)
+test_get_prompt = UseDeployedPrompt(deployment_id=deployment_id, llm_inputs=inputs)
 
 
 def main():
   completion_response: CompletionResponse = p.completion(data=test_completion)
   print(completion_response)
   deployed_prompt: UseDeployedPromptResponse = p.get_prompt(data=test_get_prompt)
   print("\n\n")
```

### Comparing `parea_ai-0.1.1a3/parea/__init__.py` & `parea_ai-0.1.1a4/parea/__init__.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.1.1a3/parea/api_client.py` & `parea_ai-0.1.1a4/parea/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Optional
 
 import httpx
 
 
 class HTTPClient:
     _instance = None
-    base_url = "https://www.optimusprompt.ai/api/parea/v1"
+    base_url = "https://optimus-prompt-backend.vercel.app/api/parea/v1"
     api_key = None
 
     def __new__(cls, *args, **kwargs):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
             cls._instance.sync_client = httpx.Client(base_url=cls.base_url, timeout=60 * 3.0)
             cls._instance.async_client = httpx.AsyncClient(base_url=cls.base_url, timeout=60 * 3.0)
```

### Comparing `parea_ai-0.1.1a3/parea/client.py` & `parea_ai-0.1.1a4/parea/client.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.1.1a3/parea/example.py` & `parea_ai-0.1.1a4/parea/example.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 # You will find this deployment_id in the Parea dashboard
 deployment_id = os.getenv("DEPLOYMENT_ID")
 # Assuming your deployed prompt's message is:
 # {"role": "user", "content": "Write a hello world program using {{x}} and the {{y}} framework."}
 llm_inputs = {"x": "Golang", "y": "Fiber"}
 
 # You can easily unpack a dictionary into an attrs class
-test_completion = Completion(**{"deployment_id": deployment_id, "llm_inputs": llm_inputs, "metadata": {"purpose": "testing"}})
+test_completion = Completion(
+    **{"deployment_id": deployment_id, "llm_inputs": llm_inputs, "metadata": {"purpose": "testing"}})
 
 # By passing in my inputs, in addition to the raw message with unfilled variables {{x}} and {{y}},
 # you we will also get the filled-in prompt:
 # {"role": "user", "content": "Write a hello world program using Golang and the Fiber framework."}
 test_get_prompt = UseDeployedPrompt(deployment_id=deployment_id, llm_inputs=llm_inputs)
```

### Comparing `parea_ai-0.1.1a3/parea/schemas/models.py` & `parea_ai-0.1.1a4/parea/schemas/models.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.1.1a3/pyproject.toml` & `parea_ai-0.1.1a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "parea-ai"
 packages = [{ include = "parea" }]
-version = "0.1.1a3"
+version = "0.1.1a4"
 description = "Parea python sdk"
 readme = "README.md"
 authors = ["joel-parea-ai <joel@parea.ai>"]
 license = "Apache Software License 2.0"
 repository = "https://github.com/parea-ai/parea-sdk"
 homepage = "https://github.com/parea-ai/parea-sdk"
```

### Comparing `parea_ai-0.1.1a3/PKG-INFO` & `parea_ai-0.1.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parea-ai
-Version: 0.1.1a3
+Version: 0.1.1a4
 Summary: Parea python sdk
 Home-page: https://github.com/parea-ai/parea-sdk
 License: Apache Software License 2.0
 Author: joel-parea-ai
 Author-email: joel@parea.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -67,29 +67,29 @@
 p = Parea(api_key=os.getenv("API_KEY"))
 
 # You will find this deployment_id in the Parea dashboard
 deployment_id = '<DEPLOYMENT_ID>'
 
 # Assuming your deployed prompt's message is:
 # {"role": "user", "content": "Write a hello world program using {{x}} and the {{y}} framework."}
-inputs = {"inputs": {"x": "Golang", "y": "Fiber"}}
+inputs = {"x": "Golang", "y": "Fiber"}
 
 # You can easily unpack a dictionary into an attrs class
 test_completion = Completion(
   **{
     "deployment_id": deployment_id,
     "llm_inputs": inputs,
     "metadata": {"purpose": "testing"}
   }
 )
 
 # By passing in my inputs, in addition to the raw message with unfilled variables {{x}} and {{y}}, 
 # you we will also get the filled-in prompt:
 # {"role": "user", "content": "Write a hello world program using Golang and the Fiber framework."}
-test_get_prompt = UseDeployedPrompt(deployment_id=deployment_id, inputs=inputs)
+test_get_prompt = UseDeployedPrompt(deployment_id=deployment_id, llm_inputs=inputs)
 
 
 def main():
   completion_response: CompletionResponse = p.completion(data=test_completion)
   print(completion_response)
   deployed_prompt: UseDeployedPromptResponse = p.get_prompt(data=test_get_prompt)
   print("\n\n")
```

