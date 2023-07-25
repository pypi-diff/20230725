# Comparing `tmp/litechain-0.1.4.tar.gz` & `tmp/litechain-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litechain-0.1.4.tar", last modified: Thu Jul 20 20:03:42 2023, max compression
+gzip compressed data, was "litechain-0.1.5.tar", last modified: Tue Jul 25 20:29:30 2023, max compression
```

## Comparing `litechain-0.1.4.tar` & `litechain-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.057260 litechain-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 20:03:30.000000 litechain-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 20:03:30.000000 litechain-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-20 20:03:42.057260 litechain-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-20 20:03:30.000000 litechain-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.053260 litechain-0.1.4/litechain/
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.057260 litechain-0.1.4/litechain/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.057260 litechain-0.1.4/litechain/contrib/llms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/contrib/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/contrib/llms/gpt4all_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/contrib/llms/open_ai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.057260 litechain-0.1.4/litechain/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23686 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/core/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.057260 litechain-0.1.4/litechain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/utils/async_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-20 20:03:30.000000 litechain-0.1.4/litechain/utils/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.053260 litechain-0.1.4/litechain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-20 20:03:42.000000 litechain-0.1.4/litechain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-20 20:03:42.000000 litechain-0.1.4/litechain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:03:42.000000 litechain-0.1.4/litechain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-20 20:03:42.000000 litechain-0.1.4/litechain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 20:03:42.000000 litechain-0.1.4/litechain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-20 20:03:30.000000 litechain-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 20:03:42.057260 litechain-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-20 20:03:30.000000 litechain-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:42.057260 litechain-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:03:30.000000 litechain-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 20:29:19.000000 litechain-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-25 20:29:19.000000 litechain-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-25 20:29:30.534257 litechain-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-25 20:29:19.000000 litechain-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/litechain/
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/litechain/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/litechain/contrib/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/contrib/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/contrib/llms/gpt4all_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/contrib/llms/open_ai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/litechain/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23686 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/core/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/litechain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/utils/async_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/utils/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/litechain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-25 20:29:30.000000 litechain-0.1.5/litechain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-25 20:29:30.000000 litechain-0.1.5/litechain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:29:30.000000 litechain-0.1.5/litechain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-25 20:29:30.000000 litechain-0.1.5/litechain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 20:29:30.000000 litechain-0.1.5/litechain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-25 20:29:19.000000 litechain-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 20:29:30.534257 litechain-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-25 20:29:19.000000 litechain-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:19.000000 litechain-0.1.5/tests/__init__.py
```

### Comparing `litechain-0.1.4/LICENSE` & `litechain-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `litechain-0.1.4/PKG-INFO` & `litechain-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litechain
-Version: 0.1.4
+Version: 0.1.5
 Summary: Build robust LLM applications with true composability 🔗
 Home-page: https://github.com/rogeriochaves/litechain
 Author: Rogerio Chaves
 Author-email: rogeriocfj@gmail.com
 License: MIT
 Project-URL: Documentation, https://rogeriochaves.github.io/litechain/
 Project-URL: Source Code, https://github.com/rogeriochaves/litechain
```

### Comparing `litechain-0.1.4/README.md` & `litechain-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `litechain-0.1.4/litechain/__init__.py` & `litechain-0.1.5/litechain/__init__.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.4/litechain/contrib/__init__.py` & `litechain-0.1.5/litechain/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.4/litechain/contrib/llms/gpt4all_chain.py` & `litechain-0.1.5/litechain/contrib/llms/gpt4all_chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from typing import AsyncGenerator, Callable, Iterable, Optional, TypeVar
+from typing import AsyncGenerator, Callable, Iterable, Optional, TypeVar, cast
 
 from gpt4all import GPT4All
 
 from litechain.core.chain import Chain
 
 T = TypeVar("T")
 U = TypeVar("U")
@@ -61,18 +61,17 @@
         top_k=40,
         top_p=0.1,
         repeat_penalty=1.18,
         repeat_last_n=64,
         n_batch=8,
         n_threads: Optional[int] = None,
     ) -> None:
-        self.name = name
         gpt4all = GPT4All(model, n_threads=n_threads)
 
-        async def generate(prompt: str) -> AsyncGenerator[str, None]:
+        async def generate(prompt: str) -> AsyncGenerator[U, None]:
             loop = asyncio.get_event_loop()
 
             def get_outputs() -> Iterable[str]:
                 return gpt4all.generate(
                     prompt,
                     streaming=True,
                     temp=temperature,
@@ -83,10 +82,10 @@
                     repeat_last_n=repeat_last_n,
                     n_batch=n_batch,
                 )
 
             outputs = await loop.run_in_executor(None, get_outputs)
 
             for output in outputs:
-                yield output
+                yield cast(U, output)
 
-        self._call = lambda input: generate(call(input))
+        super().__init__(name, lambda input: generate(call(input)))
```

### Comparing `litechain-0.1.4/litechain/contrib/llms/open_ai.py` & `litechain-0.1.5/litechain/contrib/llms/open_ai.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     TypeVar,
     Union,
     cast,
 )
 
 import openai
 from colorama import Fore
+from retry import retry
 
 from litechain.core.chain import Chain, ChainOutput
 
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
 
@@ -60,39 +61,42 @@
         call: Callable[
             [T],
             str,
         ],
         model: str,
         temperature: Optional[float] = 0,
         max_tokens: Optional[int] = None,
+        timeout: int = 5,
+        retries: int = 3,
     ) -> None:
-        self.name = name
-
-        async def completion(prompt: str) -> AsyncGenerator[str, None]:
+        async def completion(prompt: str) -> AsyncGenerator[U, None]:
             loop = asyncio.get_event_loop()
 
+            @retry(tries=retries)
             def get_completions():
                 return openai.Completion.create(
                     model=model,
                     prompt=prompt,
                     temperature=temperature,
                     stream=True,
                     max_tokens=max_tokens,
+                    timeout=timeout,
+                    request_timeout=timeout,
                 )
 
             completions = await loop.run_in_executor(None, get_completions)
 
             for output in completions:
                 output = cast(dict, output)
                 if "choices" in output:
                     if len(output["choices"]) > 0:
                         if "text" in output["choices"][0]:
                             yield output["choices"][0]["text"]
 
-        self._call = lambda input: completion(call(input))
+        super().__init__(name, lambda input: completion(call(input)))
 
 
 @dataclass
 class OpenAIChatMessage:
     """
     OpenAIChatMessage is a data class that represents a chat message for building `OpenAIChatChain` prompt.
 
@@ -259,41 +263,44 @@
     ...
     >>> asyncio.run(example()) # doctest:+SKIP
     [{'location': 'Rio de Janeiro', 'forecast': 'sunny', 'temperature': '25 C'}]
 
     """
 
     def __init__(
-        self: "OpenAIChatChain[T, Union[OpenAIChatDelta, V]]",
+        self: "OpenAIChatChain[T, OpenAIChatDelta]",
         name: str,
         call: Callable[
             [T],
             List[OpenAIChatMessage],
         ],
         model: str,
         functions: Optional[List[Dict[str, Any]]] = None,
         function_call: Optional[Union[Literal["none", "auto"], str]] = None,
         temperature: Optional[float] = 0,
         max_tokens: Optional[int] = None,
+        timeout: int = 5,
+        retries: int = 3,
     ) -> None:
-        self.name = name
-
         async def chat_completion(
             messages: List[OpenAIChatMessage],
-        ) -> AsyncGenerator[ChainOutput[Union[OpenAIChatDelta, V]], Any]:
+        ) -> AsyncGenerator[ChainOutput[OpenAIChatDelta], None]:
             loop = asyncio.get_event_loop()
 
+            @retry(tries=retries)
             def get_completions():
                 function_kwargs = {}
                 if functions is not None:
                     function_kwargs["functions"] = functions
                 if function_call is not None:
                     function_kwargs["function_call"] = function_call
 
                 return openai.ChatCompletion.create(
+                    timeout=timeout,
+                    request_timeout=timeout,
                     model=model,
                     messages=[m.to_dict() for m in messages],
                     temperature=temperature,
                     stream=True,
                     max_tokens=max_tokens,
                     **function_kwargs,
                 )
@@ -345,8 +352,11 @@
                     if pending_function_call:
                         yield self._output_wrap(pending_function_call)
                         pending_function_call = None
             if pending_function_call:
                 yield self._output_wrap(pending_function_call)
                 pending_function_call = None
 
-        self._call = lambda input: chat_completion(call(input))
+        super().__init__(
+            name,
+            lambda input: cast(AsyncGenerator[U, None], chat_completion(call(input))),
+        )
```

### Comparing `litechain-0.1.4/litechain/core/chain.py` & `litechain-0.1.5/litechain/core/chain.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.4/litechain/utils/async_generator.py` & `litechain-0.1.5/litechain/utils/async_generator.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.4/litechain/utils/chain.py` & `litechain-0.1.5/litechain/utils/chain.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.4/litechain.egg-info/PKG-INFO` & `litechain-0.1.5/litechain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litechain
-Version: 0.1.4
+Version: 0.1.5
 Summary: Build robust LLM applications with true composability 🔗
 Home-page: https://github.com/rogeriochaves/litechain
 Author: Rogerio Chaves
 Author-email: rogeriocfj@gmail.com
 License: MIT
 Project-URL: Documentation, https://rogeriochaves.github.io/litechain/
 Project-URL: Source Code, https://github.com/rogeriochaves/litechain
```

### Comparing `litechain-0.1.4/litechain.egg-info/SOURCES.txt` & `litechain-0.1.5/litechain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litechain-0.1.4/setup.py` & `litechain-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="litechain",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=requirements,
     author="Rogerio Chaves",
     author_email="rogeriocfj@gmail.com",
     description="Build robust LLM applications with true composability 🔗",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

