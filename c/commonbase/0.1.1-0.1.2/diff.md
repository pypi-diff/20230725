# Comparing `tmp/commonbase-0.1.1.tar.gz` & `tmp/commonbase-0.1.2.tar.gz`

## Comparing `commonbase-0.1.1.tar` & `commonbase-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 commonbase-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 commonbase-0.1.1/commonbase/__init__.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 commonbase-0.1.1/commonbase/completion.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 commonbase-0.1.1/commonbase/completion_response.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 commonbase-0.1.1/commonbase/exceptions.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 commonbase-0.1.1/commonbase/tests/__init__.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 commonbase-0.1.1/commonbase/tests/test_completion.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 commonbase-0.1.1/examples/completion.ipynb
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 commonbase-0.1.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 commonbase-0.1.1/LICENSE
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 commonbase-0.1.1/README.md
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 commonbase-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 commonbase-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 commonbase-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 commonbase-0.1.2/commonbase/__init__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 commonbase-0.1.2/commonbase/chat_context.py
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 commonbase-0.1.2/commonbase/completion.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 commonbase-0.1.2/commonbase/completion_response.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 commonbase-0.1.2/commonbase/exceptions.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 commonbase-0.1.2/commonbase/provider_config.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 commonbase-0.1.2/commonbase/tests/__init__.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 commonbase-0.1.2/commonbase/tests/test_completion.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 commonbase-0.1.2/commonbase/tests/test_model.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 commonbase-0.1.2/examples/completion.ipynb
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 commonbase-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 commonbase-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 commonbase-0.1.2/README.md
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 commonbase-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 commonbase-0.1.2/PKG-INFO
```

### Comparing `commonbase-0.1.1/.github/workflows/python-publish.yml` & `commonbase-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `commonbase-0.1.1/commonbase/completion_response.py` & `commonbase-0.1.2/commonbase/completion_response.py`

 * *Files identical despite different names*

### Comparing `commonbase-0.1.1/commonbase/tests/test_completion.py` & `commonbase-0.1.2/commonbase/tests/test_completion.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,48 @@
 import os
 import pytest
 import commonbase
 
 
-def test_no_project_id():
+def test_create_no_project_id():
     with pytest.raises(AssertionError):
-        commonbase.Completion.create(project_id=None, prompt="xxx")
+        commonbase.Completion.create(project_id=None, prompt="")  # type: ignore
 
 
-def test_no_prompt():
+def test_stream_no_project_id():
     with pytest.raises(AssertionError):
-        commonbase.Completion.create(project_id="xxx", prompt=None)
+        for _ in commonbase.Completion.stream(project_id=None, prompt=""):  # type: ignore
+            pass
 
 
-def test_invalid_project_id():
+def test_create_no_prompt():
+    with pytest.raises(AssertionError):
+        commonbase.Completion.create(project_id="", prompt=None)  # type: ignore
+
+
+def test_stream_no_prompt():
+    with pytest.raises(AssertionError):
+        for _ in commonbase.Completion.stream(project_id="", prompt=None):  # type: ignore
+            pass
+
+
+def test_create_invalid_project_id():
     with pytest.raises(commonbase.CommonbaseException):
         commonbase.Completion.create(project_id="", prompt="Hello")
 
 
+def test_stream_invalid_project_id():
+    with pytest.raises(commonbase.CommonbaseException):
+        for _ in commonbase.Completion.stream(project_id="", prompt="Hello"):
+            pass
+
+
 def test_completion_prompt():
     result = commonbase.Completion.create(
-        project_id=os.getenv("CB_PROJECT_ID"), prompt="Hello"
+        project_id=os.getenv("CB_PROJECT_ID") or "", prompt="Hello"
     )
 
     assert result.completed
     assert result.invocation_id is not None
     assert result.project_id is not None
     assert result.type == "text" or result.type == "chat"
     assert result.model is not None
@@ -35,25 +53,46 @@
     assert choice.text is not None
     assert choice.index >= 0
     assert choice.finish_reason is not None
 
 
 def test_completion_response():
     result = commonbase.Completion.create(
-        project_id=os.getenv("CB_PROJECT_ID"),
+        project_id=os.getenv("CB_PROJECT_ID") or "",
         prompt="Please return the string '123abc' to me without the quotes.",
     )
 
     assert result.completed and result.choices[0].text.strip() == "123abc"
 
 
 def test_completion_stream():
     response_count = 0
 
     for response in commonbase.Completion.stream(
-        project_id=os.getenv("CB_PROJECT_ID"),
+        project_id=os.getenv("CB_PROJECT_ID") or "",
         prompt="Tell me about artificial intelligence.",
     ):
         assert len(response.choices) > 0 and response.choices[0].text is not None
         response_count += 1
 
     assert response_count > 0
+
+
+def test_completion_context():
+    context = commonbase.ChatContext(
+        [
+            commonbase.ChatMessage(role="user", content="Where is Berlin located?"),
+            commonbase.ChatMessage(role="assistant", content="In the EU."),
+            commonbase.ChatMessage(role="user", content="What country?"),
+        ]
+    )
+
+    result = commonbase.Completion.create(
+        project_id=os.getenv("CB_PROJECT_ID") or "",
+        prompt="You help people with geography.",
+        chat_context=context,
+        provider_config=commonbase.ProviderConfig(
+            provider="cb-openai-eu", params=commonbase.OpenAIParams(type="chat")
+        ),
+    )
+
+    assert result.completed and "germany" in result.choices[0].text.lower()
```

### Comparing `commonbase-0.1.1/examples/completion.ipynb` & `commonbase-0.1.2/examples/completion.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333333%*

 * *Differences: {"'cells'": "{insert: [(2, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['## Usage'])])), (7, OrderedDict([('cell_type', 'markdown'), ('metadata', "*

 * *            "OrderedDict()), ('source', ['### Chat\\n', '\\n', 'To create a chat completion, use "*

 * *            "the `context` method to provide a list of chat messages.\\n', 'You must also set the "*

 * *            "OpenAI configuration to `chat`. In this mode, the `prompt` argument\\n', 'functions "*

 * *            "as […]*

```diff
@@ -22,14 +22,21 @@
                 "pip install commonbase"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "## Usage"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "A project ID is required for all Commonbase requests. You can find your project ID in the [Commonbase Dashboard](https://commonbase.com/test-50727/project/test/overview).\n",
                 "\n",
                 "To create a completion, provide your project ID and prompt to the `Completion.create` class method."
             ]
         },
         {
             "cell_type": "code",
@@ -64,14 +71,51 @@
                 "project_id=\"<YOUR PROJECT_ID>\"\n",
                 "\n",
                 "result = commonbase.Completion.stream(project_id=project_id, prompt=\"Write me a short essay about artificial intelligence.\")\n",
                 "\n",
                 "for completion in result:\n",
                 "    print(completion.choices[0].text, end=\"\")"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Chat\n",
+                "\n",
+                "To create a chat completion, use the `context` method to provide a list of chat messages.\n",
+                "You must also set the OpenAI configuration to `chat`. In this mode, the `prompt` argument\n",
+                "functions as a system message."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import commonbase\n",
+                "\n",
+                "project_id=\"XXXXXXXX-XXXXXXXX-XXXXXXXX-XXXXXXXX\"\n",
+                "\n",
+                "result = commonbase.Completion.create(\n",
+                "    project_id=project_id,\n",
+                "    prompt=\"You are an assistant who helps users with tech problems.\",\n",
+                "    chat_context=commonbase.ChatContext([\n",
+                "        commonbase.ChatMessage(role=\"user\", content=\"My internet isn't working.\"),\n",
+                "        commonbase.ChatMessage(role=\"assistant\", content=\"Have you tried restarting your router?\"),\n",
+                "        commonbase.ChatMessage(role=\"user\", content=\"Yes I've tried that.\"),\n",
+                "    ]),\n",
+                "    provider_config=commonbase.ProviderConfig(\n",
+                "        provider=\"cb-openai-eu\", params=commonbase.OpenAIParams(type=\"chat\")\n",
+                "    ),\n",
+                ")\n",
+                "\n",
+                "print(result.choices[0].text)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `commonbase-0.1.1/.gitignore` & `commonbase-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `commonbase-0.1.1/LICENSE` & `commonbase-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `commonbase-0.1.1/PKG-INFO` & `commonbase-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonbase
-Version: 0.1.1
+Version: 0.1.2
 Summary: Commonbase Python SDK
 Project-URL: Homepage, https://github.com/commonbaseapp/commonbase-python
 Project-URL: Source, https://github.com/commonbaseapp/commonbase-python
 Project-URL: Tracker, https://github.com/commonbaseapp/commonbase-python/issues
 License: MIT License
         
         Copyright (c) 2023 Commonbase
@@ -23,34 +23,39 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: requests>=2.31.0
 Requires-Dist: sseclient-py>=1.7.2
 Description-Content-Type: text/markdown
 
 # Commonbase Python SDK
 
-Commonbase allows developers to integrate with any popular LLM API provider without needing to change any code. The SDK helps with collecting data and feedback from the users and helps you fine-tune models for your specific use case.
+Commonbase allows developers to integrate with any popular LLM API provider
+without needing to change any code. The SDK helps with collecting data and
+feedback from the users and helps you fine-tune models for your specific use case.
 
 ## Installation
 
 ```
 pip install commonbase
 ```
 
 ## Usage
 
-A project ID is required for all Commonbase requests. You can find your project ID in the [Commonbase Dashboard](https://commonbase.com/test-50727/project/test/overview).
+A project ID is required for all Commonbase requests. You can find your project ID
+in the [Commonbase Dashboard](https://commonbase.com/test-50727/project/test/overview).
 
-To create a completion, provide your project ID and prompt to the `Completion.create` class method.
+## Text Completion
+
+To create a basic text completion, use the `Completion.create` class method with a `prompt` argument.
 
 ```py
 import commonbase
 
 project_id="XXXXXXXX-XXXXXXXX-XXXXXXXX-XXXXXXXX"
 
 result = commonbase.Completion.create(project_id=project_id, prompt="Hello!")
@@ -69,7 +74,34 @@
     project_id=project_id,
     prompt="Write me a short essay about artificial intelligence."
 )
 
 for completion in result:
     print(completion.choices[0].text, end="")
 ```
+
+### Chat
+
+To create a chat completion, use the `context` method to provide a list of chat messages.
+You must also set the OpenAI configuration to `chat`. In this mode, the `prompt` argument
+functions as a system message.
+
+```py
+import commonbase
+
+project_id="XXXXXXXX-XXXXXXXX-XXXXXXXX-XXXXXXXX"
+
+result = commonbase.Completion.create(
+    project_id=project_id,
+    prompt="You are an assistant who helps users with tech problems.",
+    chat_context=commonbase.ChatContext([
+        commonbase.ChatMessage(role="user", content="My internet isn't working."),
+        commonbase.ChatMessage(role="assistant", content="Have you tried restarting your router?"),
+        commonbase.ChatMessage(role="user", content="Yes I've tried that."),
+    ]),
+    provider_config=commonbase.ProviderConfig(
+        provider="cb-openai-eu", params=commonbase.OpenAIParams(type="chat")
+    ),
+)
+
+print(result.choices[0].text)
+```
```

