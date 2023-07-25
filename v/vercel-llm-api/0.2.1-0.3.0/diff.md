# Comparing `tmp/vercel_llm_api-0.2.1-py3-none-any.whl.zip` & `tmp/vercel_llm_api-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 18447 bytes, number of entries: 6
--rw-r--r--  2.0 unx     5777 b- defN 23-Jul-04 02:33 vercel_ai.py
--rw-r--r--  2.0 unx    35148 b- defN 23-Jul-04 02:35 vercel_llm_api-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     7598 b- defN 23-Jul-04 02:35 vercel_llm_api-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 02:35 vercel_llm_api-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-04 02:35 vercel_llm_api-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      491 b- defN 23-Jul-04 02:35 vercel_llm_api-0.2.1.dist-info/RECORD
-6 files, 49116 bytes uncompressed, 17557 bytes compressed:  64.3%
+Zip file size: 18576 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     6042 b- defN 23-Jul-25 02:22 vercel_ai.py
+-rw-r--r--  2.0 unx    35148 b- defN 23-Jul-25 02:36 vercel_llm_api-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7729 b- defN 23-Jul-25 02:36 vercel_llm_api-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 02:36 vercel_llm_api-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-25 02:36 vercel_llm_api-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      491 b- defN 23-Jul-25 02:36 vercel_llm_api-0.3.0.dist-info/RECORD
+6 files, 49512 bytes uncompressed, 17686 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: vercel_ai.py
 Comment: 
 
-Filename: vercel_llm_api-0.2.1.dist-info/LICENSE
+Filename: vercel_llm_api-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: vercel_llm_api-0.2.1.dist-info/METADATA
+Filename: vercel_llm_api-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: vercel_llm_api-0.2.1.dist-info/WHEEL
+Filename: vercel_llm_api-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: vercel_llm_api-0.2.1.dist-info/top_level.txt
+Filename: vercel_llm_api-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: vercel_llm_api-0.2.1.dist-info/RECORD
+Filename: vercel_llm_api-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vercel_ai.py

```diff
@@ -15,32 +15,39 @@
 
 class Client:
   base_url = "https://sdk.vercel.ai"
   token_url = base_url + "/openai.jpeg" #nice try vercel
   generate_url = base_url + "/api/prompt"
   chat_url = base_url + "/api/generate"
 
-  def __init__(self):
+  def __init__(self, proxy=None):
     self.session = requests.Session(impersonate="chrome107")
     self.headers = {
-      "User-Agent": f"Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.{random.randint(0,9999)}.{random.randint(0,99)} Safari/537.36",
+      "User-Agent": "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.{rand1}.{rand2} Safari/537.36",
       "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
       "Accept-Encoding": "gzip, deflate, br",
       "Accept-Language": "en-US,en;q=0.5",
       "Te": "trailers",
       "Upgrade-Insecure-Requests": "1"
     }
     self.session.headers.update(self.headers)
 
+    self.proxy = proxy
+    if self.proxy:       
+      self.session.proxies = {
+        "http": self.proxy,
+        "https": self.proxy
+      }
+
     self.models = self.get_models()
     self.model_ids = list(self.models.keys())
     self.model_defaults = {}
     for model_id in self.models:
       self.model_defaults[model_id] = self.get_default_params(model_id)
-
+  
   def get_models(self):
     logger.info("Downloading homepage...")
     html = self.session.get(self.base_url).text
     paths_regex = r'static\/chunks.+?\.js'
     separator_regex = r'"\]\)<\/script><script>self\.__next_f\.push\(\[.,"'
 
     paths = re.findall(paths_regex, html)
@@ -138,14 +145,18 @@
       
       yield chunk
   
   def get_headers(self):
     token = self.get_token()
 
     headers = {**self.headers, **{
+      "User-Agent": self.headers["User-Agent"].format(
+        rand1=random.randint(0,9999),
+        rand2=random.randint(0,9999)
+      ),
       "Accept-Encoding": "gzip, deflate, br",
       "Custom-Encoding": token,
       "Host": "sdk.vercel.ai",
       "Origin": "https://sdk.vercel.ai",
       "Referrer": "https://sdk.vercel.ai",
       "Sec-Fetch-Dest": "empty",
       "Sec-Fetch-Mode": "cors",
```

## Comparing `vercel_llm_api-0.2.1.dist-info/LICENSE` & `vercel_llm_api-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vercel_llm_api-0.2.1.dist-info/METADATA` & `vercel_llm_api-0.3.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: vercel-llm-api
-Version: 0.2.1
+Version: 0.3.0
 Summary: A reverse engineered API for the Vercel AI playground.
 Home-page: https://github.com/ading2210/vercel-llm-api
 Author: ading2210
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: quickjs
 Requires-Dist: curl-cffi
+Requires-Dist: quickjs
 
 # Python Vercel LLM API
 
 [![PyPi Version](https://img.shields.io/pypi/v/vercel-llm-api.svg)](https://pypi.org/project/vercel-llm-api/)
 
 This is a reverse engineered API wrapper for the [Vercel AI Playground](https://play.vercel.ai/), which allows for free access to many LLMs, including OpenAI's ChatGPT, Cohere's Command Nightly, as well as some open source models.
 
@@ -42,15 +42,14 @@
  - Generate chat messages
  - Set custom parameters
  - Stream the responses
 
 ## Limitations:
  - User-agent is hardcoded
  - No auth support
- - No proxy support
  - Can't use "pro" or "hobby" models
 
 ## Installation:
 You can install this library by running the following command:
 ```
 pip3 install vercel-llm-api
 ```
@@ -58,19 +57,28 @@
 ## Documentation:
 Examples can be found in the `/examples` directory. To run these examples, simply execute the included Python files from your terminal.
 ```
 python3 examples/generate.py
 ```
 
 ### Using the Client:
-To use this library, simply import `vercel_ai` and create a `vercel_ai.Client` instance. This class does not take any arguments.
+To use this library, simply import `vercel_ai` and create a `vercel_ai.Client` instance. You can specify a proxy using the `proxy` keyword argument.
+
+Normal example:
 ```python
 import vercel_ai
 client = vercel_ai.Client()
 ```
+
+Proxied example:
+```python
+import vercel_ai
+client = vercel_ai.Client(proxy="socks5h://193.29.62.48:11003")
+```
+
 Note that the following examples assume `client` is the name of your `vercel_ai.Client` instance.
 
 #### Downloading the Available Models:
 The client downloads the available models upon initialization, and stores them in `client.models`. 
 ```python
 >>> print(json.dumps(client.models, indent=2))
```

