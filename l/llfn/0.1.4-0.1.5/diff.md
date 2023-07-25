# Comparing `tmp/llfn-0.1.4.tar.gz` & `tmp/llfn-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llfn-0.1.4.tar", max compression
+gzip compressed data, was "llfn-0.1.5.tar", max compression
```

## Comparing `llfn-0.1.4.tar` & `llfn-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1101 2023-07-20 11:12:16.267041 llfn-0.1.4/LICENSE
--rw-r--r--   0        0        0    10940 2023-07-20 11:50:24.862974 llfn-0.1.4/README.md
--rw-r--r--   0        0        0       43 2023-07-20 10:49:19.230094 llfn-0.1.4/llfn/__init__.py
--rw-r--r--   0        0        0     2067 2023-07-21 02:24:05.180281 llfn-0.1.4/llfn/llfn.py
--rw-r--r--   0        0        0      502 2023-07-21 03:11:47.391881 llfn-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    11540 1970-01-01 00:00:00.000000 llfn-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-07-20 11:12:16.267041 llfn-0.1.5/LICENSE
+-rw-r--r--   0        0        0    11538 2023-07-24 08:27:42.806994 llfn-0.1.5/README.md
+-rw-r--r--   0        0        0       43 2023-07-20 10:49:19.230094 llfn-0.1.5/llfn/__init__.py
+-rw-r--r--   0        0        0     2810 2023-07-25 06:30:27.016609 llfn-0.1.5/llfn/llfn.py
+-rw-r--r--   0        0        0      560 2023-07-25 07:45:32.235371 llfn-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    12099 1970-01-01 00:00:00.000000 llfn-0.1.5/PKG-INFO
```

### Comparing `llfn-0.1.4/LICENSE` & `llfn-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llfn-0.1.4/README.md` & `llfn-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -84,16 +84,17 @@
 # Alternatively: bind the llm to all functions
 function_prompt.bind(llm)
 ```
 
 ### 🍺 Calling the Function
 Now you can call your function like you would for any Python function.
 
-```
+```python
 translate("Hello welcome. How are you?", "Thai")
+# สวัสดี ยินดีต้อนรับ สบายดีไหม?
 ```
 
 The beauty of this construct is that you're able to infinitely compose your applications. LLFn does not make any assumption on how you'd chain up your application logic. The only requirement for a `function_prompt` is that it returns a prompt string at the end.
 
 And ... that's it! That's just about everything you need to learn about LLFn to start building AI apps with it.
 
 <details><summary><b>👆 Click to see the full code</b></summary>
@@ -227,19 +228,29 @@
     callbacks=[StreamingStdOutCallbackHandler()],
     ...
 )
 
 function_prompt.bind(llm)
 ```
 
-### 
-
 ## Examples
 
-_Coming soon_
+### ⭐️ Single-Prompt Examples
+
+| **Task** | **Showcase** |
+|----------|--------------|
+| [Machine Translation](/examples/ex_translate_chat_model.py) | Using LangChain Chat Model |
+| [Machine Translation](/examples/ex_translate_llm.py)  | Using LangChain LLM Model |
+| [Agent Task Planner](/examples/ex_agent_tasks.py) | Defining Structured Output |
+
+### 🌈 Multi-Prompt Complex Examples
+
+| **Task** | **Showcase** |
+|----------|--------------|
+| [BabyAGI](/examples/ex_babyagi.ipynb) | Implementing BabyAGI with LLFn |
 
 ## Sponsors and Contributors
 
 We currently don't take any monetary donations! However, every issue filed and PR are extremely important to us. Here is the roster of contributors and supporters of the project.
 
 <a href="https://orge.xyz"><img height="100" alt="orge.xyz" src="https://github.com/orgexyz/LLFn/assets/891585/3502c0a6-1ab2-445d-9010-1f59f3e23cc0"></a>
```

### Comparing `llfn-0.1.4/llfn/llfn.py` & `llfn-0.1.5/llfn/llfn.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,76 @@
 from functools import update_wrapper
 from langchain.llms.base import BaseLLM
 from langchain.chat_models.base import BaseChatModel
-from langchain.schema import HumanMessage, SystemMessage
+from langchain.schema import BaseMessage, HumanMessage, SystemMessage
 from pydantic import BaseModel, Field
+from typing import List
 
 
 class LLFnFunc:
     def __init__(self, app, func):
         self.app = app
         self.func = func
         self.llm = None
+        self.examples = []
 
         class Result(BaseModel):
             result: func.__annotations__["return"] = Field(
                 ..., description="The result of the instruction"
             )
 
         self.result_type = Result
         update_wrapper(self, func)
 
     def bind(self, llm):
         self.llm = llm
 
+    def expect(self, *args, **kwargs):
+        def wrapper(inner_result):
+            prompt = self.func(*args, **kwargs)
+            expected_result = self.result_type(result=inner_result)
+            self.examples.append((prompt, expected_result.json()))
+
+        return wrapper
+
     def __call__(self, *args, **kwargs):
         if self.llm is not None:
             llm = self.llm
         elif self.app.llm is not None:
             llm = self.app.llm
         else:
             raise ValueError(
                 f'You must call "bind" before calling "{self.func.__name__}"'
             )
         user_prompt = self.func(*args, **kwargs)
         system_prompt = f"""
 - You MUST process the user's command and produce exactly one result without any other contexts or explanations
 - Your output must be a JSON dump of a Pydantic object of schema: {self.result_type.schema()}
-- Output format is EXTREMELY important. Make sure it's a valid JSON dump of the Pydantic object
+- Output format is EXTREMELY important. Make sure it's a valid JSON dump of the Pydantic object.
 """
         if isinstance(llm, BaseChatModel):
-            output = llm.predict_messages(
-                [
-                    SystemMessage(content=system_prompt),
-                    HumanMessage(content=user_prompt),
-                ]
-            ).content
+            messages: List[BaseMessage] = [SystemMessage(content=system_prompt)]
+            for prompt, expected_result in self.examples:
+                messages.append(
+                    HumanMessage(
+                        content=f"""
+Example command: {prompt}\n\n
+{expected_result}"""
+                    )
+                )
+            messages.append(HumanMessage(content=user_prompt))
+            output = llm.predict_messages(messages).content
         elif isinstance(llm, BaseLLM):
-            output = llm(
-                f"""{system_prompt}
-
-User command: {user_prompt}""
-"""
-            )
+            message = f"{system_prompt}\n\n"
+            for prompt, expected_result in self.examples:
+                message += f"""
+Example command: {prompt}\n\n
+{expected_result}\n\n"""
+            message += f"{user_prompt}"
+            output = llm(message)
         else:
             raise ValueError(f"LLM must be either a ChatModel or a BaseLLM")
         return self.result_type.parse_raw(output).result
 
 
 class LLFn:
     def __init__(self):
```

### Comparing `llfn-0.1.4/PKG-INFO` & `llfn-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: llfn
-Version: 0.1.4
+Version: 0.1.5
 Summary: Build anything from a simple text-summarizer to complex AI agents with one common primitive: function
 Author: Sorawit Suriyakarn
 Author-email: thepsint@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: langchain (>=0.0.235)
 Requires-Dist: openai (>=0.27.0)
-Requires-Dist: python-dotenv (>=1.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://github.com/othneildrew/Best-README-Template">
     <img src="https://github.com/orgexyz/LLFn/assets/891585/521df7cc-2675-41ba-ac5d-8ca57f92261b" alt="Logo" height="100">
   </a>
   <p align="center">
@@ -100,16 +99,17 @@
 # Alternatively: bind the llm to all functions
 function_prompt.bind(llm)
 ```
 
 ### 🍺 Calling the Function
 Now you can call your function like you would for any Python function.
 
-```
+```python
 translate("Hello welcome. How are you?", "Thai")
+# สวัสดี ยินดีต้อนรับ สบายดีไหม?
 ```
 
 The beauty of this construct is that you're able to infinitely compose your applications. LLFn does not make any assumption on how you'd chain up your application logic. The only requirement for a `function_prompt` is that it returns a prompt string at the end.
 
 And ... that's it! That's just about everything you need to learn about LLFn to start building AI apps with it.
 
 <details><summary><b>👆 Click to see the full code</b></summary>
@@ -243,19 +243,29 @@
     callbacks=[StreamingStdOutCallbackHandler()],
     ...
 )
 
 function_prompt.bind(llm)
 ```
 
-### 
-
 ## Examples
 
-_Coming soon_
+### ⭐️ Single-Prompt Examples
+
+| **Task** | **Showcase** |
+|----------|--------------|
+| [Machine Translation](/examples/ex_translate_chat_model.py) | Using LangChain Chat Model |
+| [Machine Translation](/examples/ex_translate_llm.py)  | Using LangChain LLM Model |
+| [Agent Task Planner](/examples/ex_agent_tasks.py) | Defining Structured Output |
+
+### 🌈 Multi-Prompt Complex Examples
+
+| **Task** | **Showcase** |
+|----------|--------------|
+| [BabyAGI](/examples/ex_babyagi.ipynb) | Implementing BabyAGI with LLFn |
 
 ## Sponsors and Contributors
 
 We currently don't take any monetary donations! However, every issue filed and PR are extremely important to us. Here is the roster of contributors and supporters of the project.
 
 <a href="https://orge.xyz"><img height="100" alt="orge.xyz" src="https://github.com/orgexyz/LLFn/assets/891585/3502c0a6-1ab2-445d-9010-1f59f3e23cc0"></a>
```

