# Comparing `tmp/fastllm-0.1.2.tar.gz` & `tmp/fastllm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastllm-0.1.2.tar", max compression
+gzip compressed data, was "fastllm-0.1.3.tar", max compression
```

## Comparing `fastllm-0.1.2.tar` & `fastllm-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-07-24 18:01:27.056723 fastllm-0.1.2/LICENSE
--rw-r--r--   0        0        0     4183 2023-07-24 18:16:08.416581 fastllm-0.1.2/README.md
--rw-r--r--   0        0        0      137 2023-07-24 18:01:27.056723 fastllm-0.1.2/fastllm/__init__.py
--rw-r--r--   0        0        0    20339 2023-07-24 18:18:54.876555 fastllm-0.1.2/fastllm/base.py
--rw-r--r--   0        0        0     1449 2023-07-24 18:17:36.726567 fastllm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 fastllm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-24 18:01:27.056723 fastllm-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4374 2023-07-25 19:28:31.313986 fastllm-0.1.3/README.md
+-rw-r--r--   0        0        0      137 2023-07-24 18:01:27.056723 fastllm-0.1.3/fastllm/__init__.py
+-rw-r--r--   0        0        0    19838 2023-07-25 19:28:19.493990 fastllm-0.1.3/fastllm/base.py
+-rw-r--r--   0        0        0     1539 2023-07-25 19:28:04.093995 fastllm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5260 1970-01-01 00:00:00.000000 fastllm-0.1.3/PKG-INFO
```

### Comparing `fastllm-0.1.2/LICENSE` & `fastllm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastllm-0.1.2/README.md` & `fastllm-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # FastLLM
 
 Fast and simple wrapper around LLMs. The package aims to be simply, precise and allows for fast prototyping of agents and applications around LLMs. At the moment focus around OpenAI's chat models.
 
 **Warning - experimental package and subject to change.** For features and plans see the [roadmap](#roadmap).
 
-## Samples
+## Installation
+
+```bash
+pip install fastllm
+```
+
+## [Samples](./samples)
 
 Require an openai api key in `OPENAI_API_KEY` environment variable or `.env` file.
 
 ```bash
 export OPENAI_API_KEY=...
 ```
 
@@ -101,14 +107,16 @@
 - [x] LLM calling with backoff and retry
 - [x] Able to register functions to agents, models and prompts using decorators
 - [x] Possible to register functions on multiple levels (agent, model, prompt). The function call is only available on the level it was registered.
 - [x] Conversation history. The Model class keeps track of the conversation history.
 - [x] Function schema is inferred from python function type hints, documentation and name
 - [x] Function calling is handled by the Model class itself. Meaning if a LLM response indicate a function call, the Model class will call the function and return the result back to the LLM
 - [ ] Function calling can result in an infinite loop if LLM can not provide function name or arguments properly. This needs to be handled by the Model class.
+- [ ] Streaming with function calling
+- [ ] Option to "smartly forget" conversation history in case context length is too long.
 - [ ] Prompts with pattern using logit bias to guide LLM completion.
 - [ ] Able to switch between models (e.g. 3.5 and 4) within one agent over different prompts.
 - [ ] Handling of multiple response messages from LLMs in a single call. At the moment only the first response is kept.
 - [ ] Supporting non chat based LLMs (e.g. OpenAI's completion LLMs).
 - [ ] Supporting other LLMs over APIs except OpenAI's. (e.g. Google etc.)
 - [ ] Supporting local LLMs (e.g. llama-1, llama-2, etc.)
```

### Comparing `fastllm-0.1.2/fastllm/base.py` & `fastllm-0.1.3/fastllm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,28 +424,14 @@
             elif isinstance(arg, Message):
                 self.messages += [arg]
             elif isinstance(arg, str):
                 self.messages += [Message(arg)]
             else:
                 raise TypeError(f"Cannot add {type(arg)} to Conversation.")
 
-    def count(
-        self, value: str, recent_n: int | None = None, role: Role = Role.ASSISTANT
-    ) -> int:
-        """Counts the appearance of value in the last n messages of given role."""
-
-        messages = [message for message in self.messages if message.role == role]
-        messages = (
-            messages[-recent_n:] if recent_n and recent_n < len(messages) else messages
-        )
-
-        matches = [value in repr(m) for m in messages if m.role == role]
-
-        return sum(matches)
-
     def to_list(self) -> list[dict]:
         """Returns the messages as a list of dicts."""
 
         return [m.to_dict() for m in self.messages]
 
 
 @dataclass
```

### Comparing `fastllm-0.1.2/pyproject.toml` & `fastllm-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastllm"
-version = "0.1.2"
+version = "0.1.3"
 description = "Fast and easy wrapper around LLMs."
 authors = ["Clemens Kriechbaumer <clemens.kriechbaumer@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/clemens33/fastllm"
 repository = "https://github.com/clemens33/fastllm"
 keywords = ["agents", "chatbots", "openai", "llm", "ai"]
@@ -29,14 +29,18 @@
 ruff = "^0.0.278"
 black = "^23.7.0"
 pyright = "^1.1.317"
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 python-dotenv = "^1.0.0"
 
+[tool.poetry.group.samples.dependencies]
+requests = "^2.31.0"
+beautifulsoup4 = "^4.12.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 select = ["E", "W", "F", "D", "N"]
 ignore = ["D202"]
```

### Comparing `fastllm-0.1.2/PKG-INFO` & `fastllm-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastllm
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fast and easy wrapper around LLMs.
 Home-page: https://github.com/clemens33/fastllm
 License: Apache-2.0
 Keywords: agents,chatbots,openai,llm,ai
 Author: Clemens Kriechbaumer
 Author-email: clemens.kriechbaumer@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -23,15 +23,21 @@
 
 # FastLLM
 
 Fast and simple wrapper around LLMs. The package aims to be simply, precise and allows for fast prototyping of agents and applications around LLMs. At the moment focus around OpenAI's chat models.
 
 **Warning - experimental package and subject to change.** For features and plans see the [roadmap](#roadmap).
 
-## Samples
+## Installation
+
+```bash
+pip install fastllm
+```
+
+## [Samples](./samples)
 
 Require an openai api key in `OPENAI_API_KEY` environment variable or `.env` file.
 
 ```bash
 export OPENAI_API_KEY=...
 ```
 
@@ -124,14 +130,16 @@
 - [x] LLM calling with backoff and retry
 - [x] Able to register functions to agents, models and prompts using decorators
 - [x] Possible to register functions on multiple levels (agent, model, prompt). The function call is only available on the level it was registered.
 - [x] Conversation history. The Model class keeps track of the conversation history.
 - [x] Function schema is inferred from python function type hints, documentation and name
 - [x] Function calling is handled by the Model class itself. Meaning if a LLM response indicate a function call, the Model class will call the function and return the result back to the LLM
 - [ ] Function calling can result in an infinite loop if LLM can not provide function name or arguments properly. This needs to be handled by the Model class.
+- [ ] Streaming with function calling
+- [ ] Option to "smartly forget" conversation history in case context length is too long.
 - [ ] Prompts with pattern using logit bias to guide LLM completion.
 - [ ] Able to switch between models (e.g. 3.5 and 4) within one agent over different prompts.
 - [ ] Handling of multiple response messages from LLMs in a single call. At the moment only the first response is kept.
 - [ ] Supporting non chat based LLMs (e.g. OpenAI's completion LLMs).
 - [ ] Supporting other LLMs over APIs except OpenAI's. (e.g. Google etc.)
 - [ ] Supporting local LLMs (e.g. llama-1, llama-2, etc.)
```

