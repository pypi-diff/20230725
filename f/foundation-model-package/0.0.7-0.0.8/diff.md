# Comparing `tmp/foundation-model-package-0.0.7.tar.gz` & `tmp/foundation-model-package-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation-model-package-0.0.7.tar", last modified: Tue Jul 25 17:11:14 2023, max compression
+gzip compressed data, was "foundation-model-package-0.0.8.tar", last modified: Tue Jul 25 19:41:55 2023, max compression
```

## Comparing `foundation-model-package-0.0.7.tar` & `foundation-model-package-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 17:11:14.679964 foundation-model-package-0.0.7/
--rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-package-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      446 2023-07-25 17:11:14.679964 foundation-model-package-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-package-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 17:11:14.649793 foundation-model-package-0.0.7/foundation_model_package.egg-info/
--rw-rw-rw-   0        0        0      446 2023-07-25 17:11:14.000000 foundation-model-package-0.0.7/foundation_model_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      509 2023-07-25 17:11:14.000000 foundation-model-package-0.0.7/foundation_model_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 17:11:14.000000 foundation-model-package-0.0.7/foundation_model_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-25 17:11:14.000000 foundation-model-package-0.0.7/foundation_model_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 17:11:14.659803 foundation-model-package-0.0.7/foundation_model_pkg/
--rw-rw-rw-   0        0        0       46 2023-07-07 21:33:54.000000 foundation-model-package-0.0.7/foundation_model_pkg/__init__.py
--rw-rw-rw-   0        0        0    16285 2023-07-25 16:55:06.000000 foundation-model-package-0.0.7/foundation_model_pkg/foundation_model.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:11:14.673452 foundation-model-package-0.0.7/foundation_model_pkg/tools/
--rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-package-0.0.7/foundation_model_pkg/tools/__init__.py
--rw-rw-rw-   0        0        0     5676 2023-07-20 19:20:36.000000 foundation-model-package-0.0.7/foundation_model_pkg/tools/foundation_model.py
--rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-package-0.0.7/foundation_model_pkg/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:11:14.673452 foundation-model-package-0.0.7/foundation_model_pkg/yamls/
--rw-rw-rw-   0        0        0      762 2023-07-25 16:57:42.000000 foundation-model-package-0.0.7/foundation_model_pkg/yamls/foundation_model.yaml
--rw-rw-rw-   0        0        0       42 2023-07-25 17:11:14.679964 foundation-model-package-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      577 2023-07-25 17:10:42.000000 foundation-model-package-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:11:14.679964 foundation-model-package-0.0.7/tests/
--rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-package-0.0.7/tests/__init__.py
--rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-package-0.0.7/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:41:55.588183 foundation-model-package-0.0.8/
+-rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-package-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      446 2023-07-25 19:41:55.588183 foundation-model-package-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-package-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 19:41:55.383670 foundation-model-package-0.0.8/foundation_model_package.egg-info/
+-rw-rw-rw-   0        0        0      446 2023-07-25 19:41:55.000000 foundation-model-package-0.0.8/foundation_model_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2023-07-25 19:41:55.000000 foundation-model-package-0.0.8/foundation_model_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 19:41:55.000000 foundation-model-package-0.0.8/foundation_model_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-25 19:41:55.000000 foundation-model-package-0.0.8/foundation_model_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 19:41:55.462906 foundation-model-package-0.0.8/foundation_model_pkg/
+-rw-rw-rw-   0        0        0       46 2023-07-07 21:33:54.000000 foundation-model-package-0.0.8/foundation_model_pkg/__init__.py
+-rw-rw-rw-   0        0        0    16381 2023-07-25 19:40:29.000000 foundation-model-package-0.0.8/foundation_model_pkg/foundation_model.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:41:55.541298 foundation-model-package-0.0.8/foundation_model_pkg/tools/
+-rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-package-0.0.8/foundation_model_pkg/tools/__init__.py
+-rw-rw-rw-   0        0        0     5676 2023-07-20 19:20:36.000000 foundation-model-package-0.0.8/foundation_model_pkg/tools/foundation_model.py
+-rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-package-0.0.8/foundation_model_pkg/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:41:55.556931 foundation-model-package-0.0.8/foundation_model_pkg/yamls/
+-rw-rw-rw-   0        0        0      762 2023-07-25 16:57:42.000000 foundation-model-package-0.0.8/foundation_model_pkg/yamls/foundation_model.yaml
+-rw-rw-rw-   0        0        0       42 2023-07-25 19:41:55.588183 foundation-model-package-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      577 2023-07-25 19:41:30.000000 foundation-model-package-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:41:55.588183 foundation-model-package-0.0.8/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-package-0.0.8/tests/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-package-0.0.8/tests/test_my_tool_1.py
```

### Comparing `foundation-model-package-0.0.7/foundation_model_pkg/foundation_model.py` & `foundation-model-package-0.0.8/foundation_model_pkg/foundation_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 import json
 import re
 import urllib.request
-
-# import uuid
+import uuid
 from abc import abstractmethod
 from enum import Enum
 from typing import Any, Dict, List, Mapping, Optional
-
-# from urllib.error import HTTPError
+from urllib.error import HTTPError
 
 from jinja2 import Template
 
 from promptflow import ToolProvider, tool
 from promptflow.connections import CustomConnection
 from promptflow.contracts.types import PromptTemplate
-from promptflow.core.tools_manager import register_builtins
+from promptflow.core.tools_manager import register_builtin_method
 
 # from ..core.contracts import StoreStage
 # from ..core.logging.utils import LoggingUtils
 # from ..core.utils.retry_utils import retry_and_handle_exceptions
 # from .contracts.telemetry import StoreToolEventCustomDimensions, StoreToolEventNames
 # from .utils.logging import ToolLoggingUtils
 # from .utils.pf_runtime_utils import PromptflowRuntimeUtils
 
 
 def validate_role(role: str) -> None:
     valid_roles = {"system", "user", "assistant"}
     if role not in valid_roles:
         valid_roles_str = ",".join([f"'{role}:\\n'" for role in valid_roles])
-        error_message = (
-            f"The Chat API requires a specific format for prompt definition, and the prompt should include separate "
-            f"lines as role delimiters: {valid_roles_str}. Current parsed role '{role}'"
-            f" does not meet the requirement. If you intend to use the Completion API, please select the appropriate"
-            f" API type and deployment name. If you do intend to use the Chat API, please refer to the guideline at "
-            f"https://aka.ms/pfdoc/chat-prompt or view the samples in our gallery that contain 'Chat' in the name."
-        )
+        error_message = f"""The Chat API requires a specific format for prompt definition, and the prompt should
+            include separate lines as role delimiters: {valid_roles_str}. Current parsed role '{role}' does not
+            meet the requirement. If you intend to use the Completion API, please select the appropriate API type
+            and deployment name. If you do intend to use the Chat API, please refer to the guideline at
+            https://aka.ms/pfdoc/chat-prompt or view the samples in our gallery that contain 'Chat' in the name."""
         raise Exception(message=error_message)
 
 
-def parse_chat(chat_str: str) -> List[str]:
+def parse_chat(chat_str: str) -> List[Dict[str, str]]:
     # openai chat api only supports below roles.
     separator = r"(?i)\n*(system|user|assistant)\s*:\s*\n"
     chunks = re.split(separator, chat_str)
     chat_list = []
     for chunk in chunks:
         last_message = chat_list[-1] if len(chat_list) > 0 else None
         if last_message and "role" in last_message and "content" not in last_message:
@@ -142,19 +138,15 @@
 
 class OSSContentFormatter(ContentFormatterBase):
     """Content handler for LLMs from the OSS catalog."""
 
     def format_request_payload(self, prompt: str, model_kwargs: Dict) -> bytes:
         input_str = json.dumps(
             {
-                "inputs": {
-                    "input_string": [
-                        ContentFormatterBase.escape_special_characters(prompt)
-                    ]
-                },
+                "inputs": {"input_string": [ContentFormatterBase.escape_special_characters(prompt)]},
                 "parameters": model_kwargs,
             }
         )
         return str.encode(input_str)
 
     def format_response_payload(self, output: bytes) -> str:
         response_json = json.loads(output)
@@ -180,19 +172,15 @@
 
 class DollyContentFormatter(ContentFormatterBase):
     """Content handler for the Dolly-v2-12b model"""
 
     def format_request_payload(self, prompt: str, model_kwargs: Dict) -> bytes:
         input_str = json.dumps(
             {
-                "input_data": {
-                    "input_string": [
-                        ContentFormatterBase.escape_special_characters(prompt)
-                    ]
-                },
+                "input_data": {"input_string": [ContentFormatterBase.escape_special_characters(prompt)]},
                 "parameters": model_kwargs,
             }
         )
         return str.encode(input_str)
 
     def format_response_payload(self, output: bytes) -> str:
         response_json = json.loads(output)
@@ -211,63 +199,51 @@
         """Formats the chat history for a multi-turn request"""
         chat_list = []
         for interaction in self.chat_history:
             if "inputs" in interaction and "question" in interaction["inputs"]:
                 chat_list.append(
                     {
                         "role": "user",
-                        "content": ContentFormatterBase.escape_special_characters(
-                            interaction["inputs"]["question"]
-                        ),
+                        "content": ContentFormatterBase.escape_special_characters(interaction["inputs"]["question"]),
                     }
                 )
             if "outputs" in interaction and "answer" in interaction["outputs"]:
                 chat_list.append(
                     {
                         "role": "assistant",
-                        "content": ContentFormatterBase.escape_special_characters(
-                            interaction["outputs"]["answer"]
-                        ),
+                        "content": ContentFormatterBase.escape_special_characters(interaction["outputs"]["answer"]),
                     }
                 )
 
         chat_list.append({"role": "user", "content": f'"{prompt}"'})
 
         return json.dumps(chat_list)
 
     def format_request_payload(self, prompt: str, model_kwargs: Dict) -> bytes:
         """Formats the request according the the chosen api"""
         request_payload = ""
 
         request_payload = (
-            Template(
-                '{"input_data": {"input_string":{{history}},"parameters": {{model_kwargs}}}}'
-            ).render(
+            Template('{"input_data": {"input_string":{{history}},"parameters": {{model_kwargs}}}}').render(
                 history=json.dumps(self.chat_history),
                 model_kwargs=json.dumps(model_kwargs),
             )
             if self.api == API.CHAT
-            else Template(
-                '{"input_data": {"input_string": ["{{prompt}}"], "parameters": {{model_kwargs}}}}'
-            ).render(
+            else Template('{"input_data": {"input_string": ["{{prompt}}"], "parameters": {{model_kwargs}}}}').render(
                 prompt=ContentFormatterBase.escape_special_characters(prompt),
                 model_kwargs=json.dumps(model_kwargs),
             )
         )
 
         return str.encode(request_payload)
 
     def format_response_payload(self, output: bytes) -> str:
         """Formats response"""
         print(json.loads(output))
-        return (
-            json.loads(output)["output"]
-            if self.api == API.CHAT
-            else json.loads(output)[0]["0"]
-        )
+        return json.loads(output)["output"] if self.api == API.CHAT else json.loads(output)[0]["0"]
 
 
 class ContentFormatterFactory:
     """Factory class for supported models"""
 
     def get_content_formatter(
         model_family: ModelFamily, api: API, chat_history: Optional[List[Dict]] = []
@@ -276,16 +252,14 @@
             return LlamaContentFormatter(chat_history=chat_history, api=api)
         elif model_family == ModelFamily.DOLLY:
             return DollyContentFormatter()
         elif model_family == ModelFamily.GPT2:
             return OSSContentFormatter()
         elif model_family == ModelFamily.FALCON:
             return HFContentFormatter()
-        else:
-            raise NotImplementedError(f"{model_family} Not Implemented Yet.")
 
 
 class AzureMLEndpointClient(object):
     """AzureML Managed Endpoint client."""
 
     def __init__(self, endpoint_url: str, endpoint_api_key: str) -> json.dumps({}):
         """Initialize the class."""
@@ -325,30 +299,30 @@
     """URL of pre-existing Endpoint. Should be passed to constructor or specified as
         env var `AZUREML_ENDPOINT_URL`."""
 
     endpoint_api_key: str = ""
     """Authentication Key for Endpoint. Should be passed to constructor or specified as
         env var `AZUREML_ENDPOINT_API_KEY`."""
 
-    http_client: Any = json.dumps({})  #: :meta private:
+    http_client: Any = None  #: :meta private:
 
-    content_formatter: Any = json.dumps({})
+    content_formatter: Any = None
     """The content formatter that provides an input and output
     transform function to handle formats between the LLM and
     the endpoint"""
 
-    model_kwargs: Optional[dict] = json.dumps({})
+    model_kwargs: Optional[Dict] = None
     """Key word arguments to pass to the model."""
 
     def __init__(
         self,
         endpoint_url: str,
         endpoint_api_key: str,
         content_formatter: ContentFormatterBase,
-        model_kwargs: Optional[dict] = json.dumps({}),
+        model_kwargs: Optional[Dict] = None,
     ):
         self.endpoint_url = endpoint_url
         self.endpoint_api_key = endpoint_api_key
         self.http_client = AzureMLEndpointClient(
             endpoint_url=self.endpoint_url,
             endpoint_api_key=self.endpoint_api_key,
         )
@@ -389,49 +363,60 @@
         body = self.content_formatter.format_request_payload(prompt, _model_kwargs)
         endpoint_response = self.http_client.call(body)
         response = self.content_formatter.format_response_payload(endpoint_response)
         return response
 
 
 class FoundationModel(ToolProvider):
+    REQUIRED_KEYS = ["endpoint_url", "endpoint_api_key", "model_family"]
+
     def __init__(self, connection: CustomConnection):
         super().__init__()
+
+        for key in self.REQUIRED_KEYS:
+            accepted_keys = ",".join([key for key in self.REQUIRED_KEYS])
+            if key not in connection:
+                raise KeyError(
+                    f"""Required key `{key}` not found in given custom connection.
+                        Required keys are: {accepted_keys}."""
+                )
+        try:
+            self.model_family = ModelFamily[connection.model_family]
+        except KeyError:
+            accepted_models = ",".join([model.name for model in ModelFamily])
+            raise KeyError(
+                f"""Given model_family '{connection.model_family}' not recognized.
+                    Supported models are: {accepted_models}."""
+            )
         self.connection = connection
 
-        # logging_config = ToolLoggingUtils.generate_config(
-        #     tool_name=self.__class__.__name__
-        # )
+        # logging_config = ToolLoggingUtils.generate_config(tool_name=self.__class__.__name__)
         # self.__logger = LoggingUtils.sdk_logger(__package__, logging_config)
-        # self.__logger.update_telemetry_context(
-        #     {StoreToolEventCustomDimensions.TOOL_INSTANCE_ID: str(uuid.uuid4())}
-        # )
+        # self.__logger.update_telemetry_context({StoreToolEventCustomDimensions.TOOL_INSTANCE_ID: str(uuid.uuid4())})
 
         # self.__logger.telemetry_event_started(
         #     event_name=StoreToolEventNames.INIT,
         #     store_stage=StoreStage.INITIALIZATION,
         # )
         # self.__logger.telemetry_event_completed(event_name=StoreToolEventNames.INIT)
         # self.__logger.flush()
 
     # @retry_and_handle_exceptions(HTTPError)
     @tool
     def foundation_model(
         self,
         prompt: PromptTemplate,
-        model_family: ModelFamily,
         api: API,
         model_kwargs: Optional[Dict] = {},
         **kwargs,
     ) -> str:
-        prompt = Template(prompt, trim_blocks=True, keep_trailing_newline=True).render(
-            **kwargs
-        )
+        prompt = Template(prompt, trim_blocks=True, keep_trailing_newline=True).render(**kwargs)
 
         content_formatter = ContentFormatterFactory.get_content_formatter(
-            model_family=model_family,
+            model_family=self.model_family,
             api=api,
             chat_history=parse_chat(prompt) if api == API.CHAT else [],
         )
 
         llm = AzureMLOnlineEndpoint(
             endpoint_url=self.connection.endpoint_url,
             endpoint_api_key=self.connection.endpoint_api_key,
@@ -449,10 +434,7 @@
         #     logger=self.__logger,
         #     flush=True,
         # )
         def _do_llm(llm: AzureMLOnlineEndpoint, prompt: str) -> str:
             return llm(prompt)
 
         return _do_llm(llm, prompt)
-
-
-register_builtins(FoundationModel)
```

### Comparing `foundation-model-package-0.0.7/foundation_model_pkg/tools/foundation_model.py` & `foundation-model-package-0.0.8/foundation_model_pkg/tools/foundation_model.py`

 * *Files identical despite different names*

### Comparing `foundation-model-package-0.0.7/foundation_model_pkg/tools/utils.py` & `foundation-model-package-0.0.8/foundation_model_pkg/tools/utils.py`

 * *Files identical despite different names*

### Comparing `foundation-model-package-0.0.7/foundation_model_pkg/yamls/foundation_model.yaml` & `foundation-model-package-0.0.8/foundation_model_pkg/yamls/foundation_model.yaml`

 * *Files identical despite different names*

### Comparing `foundation-model-package-0.0.7/setup.py` & `foundation-model-package-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="foundation-model-package",
-    version="0.0.7",
+    version="0.0.8",
     author="Matthew DeGuzman",
     author_email="t-madeguzman@microsoft.com",
     description="Package to use Foundation Models in Prompt Flow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `foundation-model-package-0.0.7/tests/test_my_tool_1.py` & `foundation-model-package-0.0.8/tests/test_my_tool_1.py`

 * *Files identical despite different names*

