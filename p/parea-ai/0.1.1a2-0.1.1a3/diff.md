# Comparing `tmp/parea_ai-0.1.1a2.tar.gz` & `tmp/parea_ai-0.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parea_ai-0.1.1a2.tar", max compression
+gzip compressed data, was "parea_ai-0.1.1a3.tar", max compression
```

## Comparing `parea_ai-0.1.1a2.tar` & `parea_ai-0.1.1a3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10885 2023-07-24 02:40:37.935778 parea_ai-0.1.1a2/LICENSE
--rw-r--r--   0        0        0     3847 2023-07-24 19:52:00.224089 parea_ai-0.1.1a2/README.md
--rw-r--r--   0        0        0      595 2023-07-24 19:44:01.025559 parea_ai-0.1.1a2/parea/__init__.py
--rw-r--r--   0        0        0     2205 2023-07-24 19:44:01.025685 parea_ai-0.1.1a2/parea/api_client.py
--rw-r--r--   0        0        0     1625 2023-07-24 19:44:01.025796 parea_ai-0.1.1a2/parea/client.py
--rw-r--r--   0        0        0     1722 2023-07-24 19:44:01.025915 parea_ai-0.1.1a2/parea/example.py
--rw-r--r--   0        0        0     2082 2023-07-24 20:01:40.458007 parea_ai-0.1.1a2/parea/schemas/models.py
--rw-r--r--   0        0        0     3525 2023-07-24 20:03:08.359942 parea_ai-0.1.1a2/pyproject.toml
--rw-r--r--   0        0        0     4897 1970-01-01 00:00:00.000000 parea_ai-0.1.1a2/PKG-INFO
+-rw-r--r--   0        0        0    10885 2023-07-24 02:40:37.935778 parea_ai-0.1.1a3/LICENSE
+-rw-r--r--   0        0        0     3840 2023-07-24 21:35:08.489913 parea_ai-0.1.1a3/README.md
+-rw-r--r--   0        0        0      595 2023-07-24 19:44:01.025559 parea_ai-0.1.1a3/parea/__init__.py
+-rw-r--r--   0        0        0     2262 2023-07-25 01:36:19.918040 parea_ai-0.1.1a3/parea/api_client.py
+-rw-r--r--   0        0        0     1548 2023-07-24 22:28:01.808010 parea_ai-0.1.1a3/parea/client.py
+-rw-r--r--   0        0        0     1726 2023-07-25 00:59:38.687497 parea_ai-0.1.1a3/parea/example.py
+-rw-r--r--   0        0        0     2099 2023-07-25 01:33:48.747173 parea_ai-0.1.1a3/parea/schemas/models.py
+-rw-r--r--   0        0        0     3525 2023-07-25 01:36:39.930418 parea_ai-0.1.1a3/pyproject.toml
+-rw-r--r--   0        0        0     4890 1970-01-01 00:00:00.000000 parea_ai-0.1.1a3/PKG-INFO
```

### Comparing `parea_ai-0.1.1a2/LICENSE` & `parea_ai-0.1.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `parea_ai-0.1.1a2/README.md` & `parea_ai-0.1.1a3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ## Getting Started
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
-from parea.client import Parea
+from parea import Parea
 from parea.schemas.models import Completion, UseDeployedPrompt, CompletionResponse, UseDeployedPromptResponse
 
 load_dotenv()
 
 p = Parea(api_key=os.getenv("API_KEY"))
 
 # You will find this deployment_id in the Parea dashboard
```

### Comparing `parea_ai-0.1.1a2/parea/__init__.py` & `parea_ai-0.1.1a3/parea/__init__.py`

 * *Files identical despite different names*

### Comparing `parea_ai-0.1.1a2/parea/api_client.py` & `parea_ai-0.1.1a3/parea/api_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 from typing import Any, Optional
 
 import httpx
 
 
 class HTTPClient:
     _instance = None
-    base_url = "http://localhost:8000/api/parea/v1"
+    base_url = "https://www.optimusprompt.ai/api/parea/v1"
+    api_key = None
 
     def __new__(cls, *args, **kwargs):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
             cls._instance.sync_client = httpx.Client(base_url=cls.base_url, timeout=60 * 3.0)
             cls._instance.async_client = httpx.AsyncClient(base_url=cls.base_url, timeout=60 * 3.0)
         return cls._instance
 
+    def set_api_key(self, api_key: str):
+        self.api_key = api_key
+
     def request(
         self,
         method: str,
         endpoint: str,
         data: Optional[dict[str, Any]] = None,
         params: Optional[dict[str, Any]] = None,
-        authorization: Optional[str] = None,
+        api_key: Optional[str] = None,
     ) -> httpx.Response:
         """
         Makes an HTTP request to the specified endpoint.
         """
-        headers = {"Authorization": f"Bearer {authorization}"} if authorization else None
+        headers = {"x-api-key": self.api_key} if self.api_key else api_key
         response = self.sync_client.request(method, endpoint, json=data, headers=headers, params=params)
         response.raise_for_status()
         return response
 
     async def request_async(
         self,
         method: str,
         endpoint: str,
         data: Optional[dict[str, Any]] = None,
         params: Optional[dict[str, Any]] = None,
-        authorization: Optional[str] = None,
+        api_key: Optional[str] = None,
     ) -> httpx.Response:
         """
         Makes an asynchronous HTTP request to the specified endpoint.
         """
-        headers = {"Authorization": f"Bearer {authorization}"} if authorization else None
+        headers = {"x-api-key": self.api_key} if self.api_key else api_key
         response = await self.async_client.request(method, endpoint, json=data, headers=headers, params=params)
         response.raise_for_status()
         return response
 
     def close(self):
         """
         Closes the synchronous HTTP client.
```

### Comparing `parea_ai-0.1.1a2/parea/client.py` & `parea_ai-0.1.1a3/parea/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,42 +8,41 @@
 
 
 @define
 class Parea:
     api_key: str = field(init=True, default="")
     _client: HTTPClient = field(init=False, default=HTTPClient())
 
+    def __attrs_post_init__(self):
+        self._client.set_api_key(self.api_key)
+
     def completion(self, data: Completion) -> CompletionResponse:
         r = self._client.request(
             "POST",
             COMPLETION_ENDPOINT,
             data=asdict(data),
-            authorization=self.api_key,
         )
         return CompletionResponse(**r.json())
 
     async def acompletion(self, data: Completion) -> CompletionResponse:
         r = await self._client.request_async(
             "POST",
             COMPLETION_ENDPOINT,
             data=asdict(data),
-            authorization=self.api_key,
         )
         return CompletionResponse(**r.json())
 
     def get_prompt(self, data: UseDeployedPrompt) -> UseDeployedPromptResponse:
         r = self._client.request(
             "POST",
             DEPLOYED_PROMPT_ENDPOINT,
             data=asdict(data),
-            authorization=self.api_key,
         )
         return UseDeployedPromptResponse(**r.json())
 
     async def aget_prompt(self, data: UseDeployedPrompt) -> UseDeployedPromptResponse:
         r = await self._client.request_async(
             "POST",
             DEPLOYED_PROMPT_ENDPOINT,
             data=asdict(data),
-            authorization=self.api_key,
         )
         return UseDeployedPromptResponse(**r.json())
```

### Comparing `parea_ai-0.1.1a2/parea/example.py` & `parea_ai-0.1.1a3/parea/example.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 p = Parea(api_key=os.getenv("API_KEY"))
 
 # You will find this deployment_id in the Parea dashboard
 deployment_id = os.getenv("DEPLOYMENT_ID")
 # Assuming your deployed prompt's message is:
 # {"role": "user", "content": "Write a hello world program using {{x}} and the {{y}} framework."}
-inputs = {"inputs": {"x": "Golang", "y": "Fiber"}}
+llm_inputs = {"x": "Golang", "y": "Fiber"}
 
 # You can easily unpack a dictionary into an attrs class
-test_completion = Completion(**{"deployment_id": deployment_id, "llm_inputs": inputs, "metadata": {"purpose": "testing"}})
+test_completion = Completion(**{"deployment_id": deployment_id, "llm_inputs": llm_inputs, "metadata": {"purpose": "testing"}})
 
 # By passing in my inputs, in addition to the raw message with unfilled variables {{x}} and {{y}},
 # you we will also get the filled-in prompt:
 # {"role": "user", "content": "Write a hello world program using Golang and the Fiber framework."}
-test_get_prompt = UseDeployedPrompt(deployment_id=deployment_id, inputs=inputs)
+test_get_prompt = UseDeployedPrompt(deployment_id=deployment_id, llm_inputs=llm_inputs)
 
 
 def main():
     completion_response: CompletionResponse = p.completion(data=test_completion)
     print(completion_response)
     deployed_prompt: UseDeployedPromptResponse = p.get_prompt(data=test_get_prompt)
     print("\n\n")
```

### Comparing `parea_ai-0.1.1a2/parea/schemas/models.py` & `parea_ai-0.1.1a3/parea/schemas/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Optional, Union
 
 from enum import Enum
 
 from attrs import define
 
 
 class Role(str, Enum):
@@ -27,26 +27,26 @@
     frequency_penalty: float = 0.0
     presence_penalty: float = 0.0
     max_length: Optional[int] = None
 
 
 @define
 class LLMInputs:
-    inputs: Optional[dict[str, Any]] = None
     model: Optional[str] = None
     provider: Optional[str] = None
     model_params: Optional[ModelParams] = None
     messages: Optional[list[Message]] = None
     functions: Optional[list[Any]] = None
     function_call: Optional[Union[str, dict[str, str]]] = None
 
 
 @define
 class Completion:
-    llm_inputs: LLMInputs
+    llm_inputs: Optional[dict[str, Any]] = None
+    llm_configuration: LLMInputs = LLMInputs()
     end_user_identifier: Optional[str] = None
     deployment_id: Optional[str] = None
     name: Optional[str] = None
     metadata: Optional[dict] = None
     cache: bool = True
     log_omit_inputs: bool = False
     log_omit_outputs: bool = False
@@ -69,15 +69,15 @@
     end_timestamp: str
     error: Optional[str] = None
 
 
 @define
 class UseDeployedPrompt:
     deployment_id: str
-    inputs: Optional[dict[str, Any]] = None
+    llm_inputs: Optional[dict[str, Any]] = None
 
 
 @define
 class Prompt:
     raw_messages: list[dict[str, Any]]
     messages: list[dict[str, Any]]
     inputs: Optional[dict[str, Any]] = None
```

### Comparing `parea_ai-0.1.1a2/pyproject.toml` & `parea_ai-0.1.1a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "parea-ai"
 packages = [{ include = "parea" }]
-version = "0.1.1a2"
+version = "0.1.1a3"
 description = "Parea python sdk"
 readme = "README.md"
 authors = ["joel-parea-ai <joel@parea.ai>"]
 license = "Apache Software License 2.0"
 repository = "https://github.com/parea-ai/parea-sdk"
 homepage = "https://github.com/parea-ai/parea-sdk"
```

### Comparing `parea_ai-0.1.1a2/PKG-INFO` & `parea_ai-0.1.1a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parea-ai
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: Parea python sdk
 Home-page: https://github.com/parea-ai/parea-sdk
 License: Apache Software License 2.0
 Author: joel-parea-ai
 Author-email: joel@parea.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -55,15 +55,15 @@
 ## Getting Started
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
-from parea.client import Parea
+from parea import Parea
 from parea.schemas.models import Completion, UseDeployedPrompt, CompletionResponse, UseDeployedPromptResponse
 
 load_dotenv()
 
 p = Parea(api_key=os.getenv("API_KEY"))
 
 # You will find this deployment_id in the Parea dashboard
```

