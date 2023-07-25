# Comparing `tmp/jinaai-0.2.1.tar.gz` & `tmp/jinaai-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinaai-0.2.1.tar", last modified: Sun Jul  2 06:39:42 2023, max compression
+gzip compressed data, was "jinaai-0.2.3.tar", last modified: Tue Jul 25 05:27:10 2023, max compression
```

## Comparing `jinaai-0.2.1.tar` & `jinaai-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-02 06:39:42.558133 jinaai-0.2.1/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.2.1/LICENSE
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    13564 2023-07-02 06:39:42.557948 jinaai-0.2.1/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    13315 2023-07-02 05:30:22.000000 jinaai-0.2.1/README.md
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-02 06:39:42.555772 jinaai-0.2.1/jinaai/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2642 2023-06-27 13:33:29.000000 jinaai-0.2.1/jinaai/__init__.py
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-02 06:39:42.557780 jinaai-0.2.1/jinaai/clients/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1082 2023-06-19 03:53:55.000000 jinaai-0.2.1/jinaai/clients/HTTPClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1856 2023-07-02 05:36:25.000000 jinaai-0.2.1/jinaai/clients/JinaChatClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2094 2023-07-02 05:51:36.000000 jinaai-0.2.1/jinaai/clients/PromptPerfectClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1934 2023-06-19 08:21:16.000000 jinaai-0.2.1/jinaai/clients/RationaleClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1686 2023-06-19 03:26:43.000000 jinaai-0.2.1/jinaai/clients/SceneXClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 04:44:46.000000 jinaai-0.2.1/jinaai/clients/__init__.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      891 2023-06-16 08:41:29.000000 jinaai-0.2.1/jinaai/utils.py
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-02 06:39:42.556528 jinaai-0.2.1/jinaai.egg-info/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    13564 2023-07-02 06:39:42.000000 jinaai-0.2.1/jinaai.egg-info/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      402 2023-07-02 06:39:42.000000 jinaai-0.2.1/jinaai.egg-info/SOURCES.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-07-02 06:39:42.000000 jinaai-0.2.1/jinaai.egg-info/dependency_links.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        9 2023-07-02 06:39:42.000000 jinaai-0.2.1/jinaai.egg-info/requires.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-07-02 06:39:42.000000 jinaai-0.2.1/jinaai.egg-info/top_level.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-07-02 06:39:42.558179 jinaai-0.2.1/setup.cfg
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      508 2023-07-02 06:38:55.000000 jinaai-0.2.1/setup.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-25 05:27:10.968061 jinaai-0.2.3/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.2.3/LICENSE
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14695 2023-07-25 05:27:10.967885 jinaai-0.2.3/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14446 2023-07-25 04:59:05.000000 jinaai-0.2.3/README.md
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-25 05:27:10.965507 jinaai-0.2.3/jinaai/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     3273 2023-07-25 04:10:03.000000 jinaai-0.2.3/jinaai/__init__.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-25 05:27:10.967712 jinaai-0.2.3/jinaai/clients/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1639 2023-07-25 03:49:04.000000 jinaai-0.2.3/jinaai/clients/BestBannerClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1082 2023-06-19 03:53:55.000000 jinaai-0.2.3/jinaai/clients/HTTPClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1856 2023-07-02 05:36:25.000000 jinaai-0.2.3/jinaai/clients/JinaChatClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2094 2023-07-02 05:51:36.000000 jinaai-0.2.3/jinaai/clients/PromptPerfectClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1934 2023-06-19 08:21:16.000000 jinaai-0.2.3/jinaai/clients/RationaleClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2020 2023-07-25 04:30:23.000000 jinaai-0.2.3/jinaai/clients/SceneXClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 04:44:46.000000 jinaai-0.2.3/jinaai/clients/__init__.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      891 2023-06-16 08:41:29.000000 jinaai-0.2.3/jinaai/utils.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-25 05:27:10.966243 jinaai-0.2.3/jinaai.egg-info/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14695 2023-07-25 05:27:10.000000 jinaai-0.2.3/jinaai.egg-info/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      437 2023-07-25 05:27:10.000000 jinaai-0.2.3/jinaai.egg-info/SOURCES.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-07-25 05:27:10.000000 jinaai-0.2.3/jinaai.egg-info/dependency_links.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        9 2023-07-25 05:27:10.000000 jinaai-0.2.3/jinaai.egg-info/requires.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-07-25 05:27:10.000000 jinaai-0.2.3/jinaai.egg-info/top_level.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-07-25 05:27:10.968104 jinaai-0.2.3/setup.cfg
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      508 2023-07-25 05:25:41.000000 jinaai-0.2.3/setup.py
```

### Comparing `jinaai-0.2.1/LICENSE` & `jinaai-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.1/PKG-INFO` & `jinaai-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: jinaai
-Version: 0.2.1
+Version: 0.2.3
 Summary: Jina AI Python SDK
 Home-page: https://github.com/jina-ai/jinaai-py.git
 Author: Jina AI
 Author-email: guillaume.roncari@jina.ai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JinaAI Python SDK
 
-The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products — [SceneXplain](https://scenex.jina.ai), [PromptPerfect](https://promptperfect.jina.ai/), [Rationale](https://rationale.jina.ai/), and [JinaChat](https://chat.jina.ai/) — into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK lets you effortlessly formulate and fine-tune prompts, thus streamlining application development.
+The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products — [SceneXplain](https://scenex.jina.ai), [PromptPerfect](https://promptperfect.jina.ai/), [Rationale](https://rationale.jina.ai/), [BestBanner](https://bestbanner.jina.ai/), and [JinaChat](https://chat.jina.ai/) — into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK lets you effortlessly formulate and fine-tune prompts, thus streamlining application development.
 
 ## Installing
 
 ### Package manager
 
 Using pip:
 ```bash
@@ -25,14 +25,15 @@
 
 To generate an API secret, you need to authenticate on each respective platform's API tab:
 
 - [SceneXplain API](https://scenex.jina.ai/api)
 - [PromptPerfect API](https://promptperfect.jina.ai/api)
 - [Rationale API](https://rationale.jina.ai/api)
 - [JinaChat API](https://chat.jina.ai/api)
+- [BestBanner API](https://bestbanner.jina.ai/api)
 
 > **Note:** Each secret is product-specific and cannot be interchanged. If you're planning to use multiple products, you'll need to generate a separate secret for each.
 
 ## Example usage
 
 
 Import the SDK and instantiate a new client with your authentication secrets:
@@ -42,14 +43,15 @@
 
 jinaai = JinaAI(
     secrets = {
         'promptperfect-secret': 'XXXXXX',
         'scenex-secret': 'XXXXXX',
         'rationale-secret': 'XXXXXX',
         'jinachat-secret': 'XXXXXX',
+        'bestbanner-secret': 'XXXXXX',
     }
 )
 ```
 
 Describe images:
 
 ```python
@@ -79,14 +81,22 @@
 
 ```python
 output = jinaai.generate(
     'Give me a recipe for a pizza with pineapple'
 )
 ```
 
+Create images from text:
+
+```python
+output = jinaai.imagine(
+    'A controversial fusion of sweet pineapple and savory pizza.'
+)
+```
+
 Use APIs together:
 
 ```python
 situations = [toBase64(img) for img in [
     'factory-1.png',
     'factory-2.png',
     'factory-3.png',
@@ -111,14 +121,18 @@
 
 recommendation = jinaai.generate('\n'.join(propmt2))
 
 swot = jinaai.decide(
     recommendation['output'],
     { 'analysis': 'swot' }
 )
+
+banners = jinaai.imagine(
+    *[desc['output'] for i, desc in enumerate(descriptions['results'])]
+)
 ```
 
 ## Raw Output
 
 You can retrieve the raw output of each APIs by passing `raw: True` in the options:
 
 ```python
@@ -142,26 +156,26 @@
 
 >| VARIABLE                              | TYPE              | VALUE 
 >|---------------------------------------|-------------------|----------
 >| input                                 | str / str array   | Image URL or Base64
 
 - Options
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| options                                | dict              | 
 >| options['algorithm']                   | None / str        | Aqua / Bolt / Comet / Dune / Ember / Flash
->| options['features']                    | None / str array  | high_quality, question_answer
+>| options['features']                    | None / str array  | high_quality, question_answer, tts, opt-out
 >| options['languages']                   | None / str array  | en, cn, de, fr, it...
 >| options['question']                    | None / str        | Question related to the picture(s)
 >| options['style']                       | None / str        | default / concise / prompt
 
 - Output
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['results']                      | dict array        | 
 >| results[0]['output']                   | str               | The picture description
 >| results[0]['i18n']                     | dict              | Contains one key for each item in languages
 >| ...i18n['cn']                          | str               | The translated picture description
 
@@ -171,21 +185,21 @@
 
 ```python
 output = JinaAI.optimize(input, options)
 ```
 
 - Input
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| input                                  | str / str array   | Image URL or Base64 / prompt to optimize
 
 - Options
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| options                                | dict              | 
 >| options['targetModel']                 | None / str        | chatgpt / gpt-4 / stablelm-tuned-alpha-7b / claude / cogenerate / text-davinci-003 / dalle / sd / midjourney / kandinsky / lexica
 >| options['features']                    | None / str array  | preview, no_spam, shorten, bypass_ethics, same_language, always_en, high_quality, redo_original_image, variable_subs, template_run
 >| options['iterations']                  | None / number     | Default: 1
 >| options['previewSettings']             | None / dict       | Contains the settings for the preview
 >| ...previewSettings['temperature']      | number            | Example: 0.9
@@ -196,15 +210,15 @@
 >| options['previewVariables']            | None / dict       | Contains one key for each variables in the prompt
 >| ...previewVariables['var1']            | str               | The value of the variable
 >| options['timeout']                     | Number            | Default: 20000
 >| options['target_language']             | None / str        | en / cn / de / fr / it...
 
 - Output
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['results']                      | dict array        | 
 >| results[0]['output']                   | str               | The optimized prompt
 
 <br/>
 
@@ -212,30 +226,30 @@
 
 ```python
 output = JinaAI.decide(input, options)
 ```
 
 - Input
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| input                                  | str / str array   | Decision to evaluate
 
 - Options
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| options                                | dict              | 
 >| options['analysis']                    | None / str        | proscons / swot / multichoice / outcomes
 >| options['style']                       | None / str        | concise / professional / humor / sarcastic / childish / genZ
 >| options['profileId']                   | None / str        | The id of the Personas you want to use
 
 - Output
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['results']                      | dict array        | 
 >| results[0]['proscons']                 | None / dict       |
 >| ...proscons['pros']                    | dict              | Contains one key for each pros
 >| ...proscons['pros']['pros1']           | str               | The explanation of the pros
 >| ...proscons['cons']                    | dict              | Contains one key for each cons
@@ -268,21 +282,21 @@
 
 ```python
 output = JinaAI.generate(input, options)
 ```
 
 - Input
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE                   | VALUE 
 >|----------------------------------------|------------------------|----------
 >| input                                  | str / str array        | Image URL or Base64 / prompt
 
 - Options
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE                   | VALUE 
 >|----------------------------------------|------------------------|----------
 >| options                                | dict                   | 
 >| options['role']                        | None / str             | user / assistant
 >| options['name']                        | None / str             | The name of the author of this message
 >| options['chatId']                      | None / str             | The id of the conversation to continue
 >| options['stream']                      | None / boolean         | Whether to stream back partial progress, Default: false
 >| options['temperature']                 | None / number          | Default: 1
@@ -292,22 +306,48 @@
 >| options['presence_penalty']            | None / number          | Number between -2.0 and 2.0, Default: 0
 >| options['frequency_penalty']           | None / number          | Number between -2.0 and 2.0, Default: 0
 >| options['logit_bias']                  | None / dict            | The likelihood for a token to appear in the completion
 >| ...logit_bias['tokenId']               | number                 | Bias value from -100 to 100
 
 - Output
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['output']                       | str               | The generated answer
 >| output['chatId']                       | str               | The chatId to continue the conversation
 
 <br/>
 
+### JinaAi.imagine
+
+```python
+output = JinaAI.imagine(input, options)
+```
+
+- Input
+
+>| VARIABLE                               | TYPE                   | VALUE 
+>|----------------------------------------|------------------------|----------
+>| input                                  | str / str array        | Prompt
+
+- Options
+
+>No options available
+
+- Output
+
+>| VARIABLE                               | TYPE              | VALUE 
+>|----------------------------------------|-------------------|----------
+>| output                                 | dict              | 
+>| output['results']                      | dict array        |
+>| results[0]['output']                   | array             | array of 4 image urls
+
+<br/>
+
 ### JinaAi.utils
 
 ```python
 outout = JinaAI.utils.image_to_base64(input)
 ```
 
 >| VARIABLE                              | TYPE              | VALUE
```

### Comparing `jinaai-0.2.1/README.md` & `jinaai-0.2.3/jinaai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,20 @@
+Metadata-Version: 2.1
+Name: jinaai
+Version: 0.2.3
+Summary: Jina AI Python SDK
+Home-page: https://github.com/jina-ai/jinaai-py.git
+Author: Jina AI
+Author-email: guillaume.roncari@jina.ai
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # JinaAI Python SDK
 
-The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products — [SceneXplain](https://scenex.jina.ai), [PromptPerfect](https://promptperfect.jina.ai/), [Rationale](https://rationale.jina.ai/), and [JinaChat](https://chat.jina.ai/) — into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK lets you effortlessly formulate and fine-tune prompts, thus streamlining application development.
+The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products — [SceneXplain](https://scenex.jina.ai), [PromptPerfect](https://promptperfect.jina.ai/), [Rationale](https://rationale.jina.ai/), [BestBanner](https://bestbanner.jina.ai/), and [JinaChat](https://chat.jina.ai/) — into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK lets you effortlessly formulate and fine-tune prompts, thus streamlining application development.
 
 ## Installing
 
 ### Package manager
 
 Using pip:
 ```bash
@@ -15,14 +25,15 @@
 
 To generate an API secret, you need to authenticate on each respective platform's API tab:
 
 - [SceneXplain API](https://scenex.jina.ai/api)
 - [PromptPerfect API](https://promptperfect.jina.ai/api)
 - [Rationale API](https://rationale.jina.ai/api)
 - [JinaChat API](https://chat.jina.ai/api)
+- [BestBanner API](https://bestbanner.jina.ai/api)
 
 > **Note:** Each secret is product-specific and cannot be interchanged. If you're planning to use multiple products, you'll need to generate a separate secret for each.
 
 ## Example usage
 
 
 Import the SDK and instantiate a new client with your authentication secrets:
@@ -32,14 +43,15 @@
 
 jinaai = JinaAI(
     secrets = {
         'promptperfect-secret': 'XXXXXX',
         'scenex-secret': 'XXXXXX',
         'rationale-secret': 'XXXXXX',
         'jinachat-secret': 'XXXXXX',
+        'bestbanner-secret': 'XXXXXX',
     }
 )
 ```
 
 Describe images:
 
 ```python
@@ -69,14 +81,22 @@
 
 ```python
 output = jinaai.generate(
     'Give me a recipe for a pizza with pineapple'
 )
 ```
 
+Create images from text:
+
+```python
+output = jinaai.imagine(
+    'A controversial fusion of sweet pineapple and savory pizza.'
+)
+```
+
 Use APIs together:
 
 ```python
 situations = [toBase64(img) for img in [
     'factory-1.png',
     'factory-2.png',
     'factory-3.png',
@@ -101,14 +121,18 @@
 
 recommendation = jinaai.generate('\n'.join(propmt2))
 
 swot = jinaai.decide(
     recommendation['output'],
     { 'analysis': 'swot' }
 )
+
+banners = jinaai.imagine(
+    *[desc['output'] for i, desc in enumerate(descriptions['results'])]
+)
 ```
 
 ## Raw Output
 
 You can retrieve the raw output of each APIs by passing `raw: True` in the options:
 
 ```python
@@ -132,26 +156,26 @@
 
 >| VARIABLE                              | TYPE              | VALUE 
 >|---------------------------------------|-------------------|----------
 >| input                                 | str / str array   | Image URL or Base64
 
 - Options
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| options                                | dict              | 
 >| options['algorithm']                   | None / str        | Aqua / Bolt / Comet / Dune / Ember / Flash
->| options['features']                    | None / str array  | high_quality, question_answer
+>| options['features']                    | None / str array  | high_quality, question_answer, tts, opt-out
 >| options['languages']                   | None / str array  | en, cn, de, fr, it...
 >| options['question']                    | None / str        | Question related to the picture(s)
 >| options['style']                       | None / str        | default / concise / prompt
 
 - Output
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['results']                      | dict array        | 
 >| results[0]['output']                   | str               | The picture description
 >| results[0]['i18n']                     | dict              | Contains one key for each item in languages
 >| ...i18n['cn']                          | str               | The translated picture description
 
@@ -161,21 +185,21 @@
 
 ```python
 output = JinaAI.optimize(input, options)
 ```
 
 - Input
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| input                                  | str / str array   | Image URL or Base64 / prompt to optimize
 
 - Options
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| options                                | dict              | 
 >| options['targetModel']                 | None / str        | chatgpt / gpt-4 / stablelm-tuned-alpha-7b / claude / cogenerate / text-davinci-003 / dalle / sd / midjourney / kandinsky / lexica
 >| options['features']                    | None / str array  | preview, no_spam, shorten, bypass_ethics, same_language, always_en, high_quality, redo_original_image, variable_subs, template_run
 >| options['iterations']                  | None / number     | Default: 1
 >| options['previewSettings']             | None / dict       | Contains the settings for the preview
 >| ...previewSettings['temperature']      | number            | Example: 0.9
@@ -186,15 +210,15 @@
 >| options['previewVariables']            | None / dict       | Contains one key for each variables in the prompt
 >| ...previewVariables['var1']            | str               | The value of the variable
 >| options['timeout']                     | Number            | Default: 20000
 >| options['target_language']             | None / str        | en / cn / de / fr / it...
 
 - Output
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['results']                      | dict array        | 
 >| results[0]['output']                   | str               | The optimized prompt
 
 <br/>
 
@@ -202,30 +226,30 @@
 
 ```python
 output = JinaAI.decide(input, options)
 ```
 
 - Input
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| input                                  | str / str array   | Decision to evaluate
 
 - Options
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| options                                | dict              | 
 >| options['analysis']                    | None / str        | proscons / swot / multichoice / outcomes
 >| options['style']                       | None / str        | concise / professional / humor / sarcastic / childish / genZ
 >| options['profileId']                   | None / str        | The id of the Personas you want to use
 
 - Output
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['results']                      | dict array        | 
 >| results[0]['proscons']                 | None / dict       |
 >| ...proscons['pros']                    | dict              | Contains one key for each pros
 >| ...proscons['pros']['pros1']           | str               | The explanation of the pros
 >| ...proscons['cons']                    | dict              | Contains one key for each cons
@@ -258,21 +282,21 @@
 
 ```python
 output = JinaAI.generate(input, options)
 ```
 
 - Input
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE                   | VALUE 
 >|----------------------------------------|------------------------|----------
 >| input                                  | str / str array        | Image URL or Base64 / prompt
 
 - Options
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE                   | VALUE 
 >|----------------------------------------|------------------------|----------
 >| options                                | dict                   | 
 >| options['role']                        | None / str             | user / assistant
 >| options['name']                        | None / str             | The name of the author of this message
 >| options['chatId']                      | None / str             | The id of the conversation to continue
 >| options['stream']                      | None / boolean         | Whether to stream back partial progress, Default: false
 >| options['temperature']                 | None / number          | Default: 1
@@ -282,22 +306,48 @@
 >| options['presence_penalty']            | None / number          | Number between -2.0 and 2.0, Default: 0
 >| options['frequency_penalty']           | None / number          | Number between -2.0 and 2.0, Default: 0
 >| options['logit_bias']                  | None / dict            | The likelihood for a token to appear in the completion
 >| ...logit_bias['tokenId']               | number                 | Bias value from -100 to 100
 
 - Output
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['output']                       | str               | The generated answer
 >| output['chatId']                       | str               | The chatId to continue the conversation
 
 <br/>
 
+### JinaAi.imagine
+
+```python
+output = JinaAI.imagine(input, options)
+```
+
+- Input
+
+>| VARIABLE                               | TYPE                   | VALUE 
+>|----------------------------------------|------------------------|----------
+>| input                                  | str / str array        | Prompt
+
+- Options
+
+>No options available
+
+- Output
+
+>| VARIABLE                               | TYPE              | VALUE 
+>|----------------------------------------|-------------------|----------
+>| output                                 | dict              | 
+>| output['results']                      | dict array        |
+>| results[0]['output']                   | array             | array of 4 image urls
+
+<br/>
+
 ### JinaAi.utils
 
 ```python
 outout = JinaAI.utils.image_to_base64(input)
 ```
 
 >| VARIABLE                              | TYPE              | VALUE
```

### Comparing `jinaai-0.2.1/jinaai/__init__.py` & `jinaai-0.2.3/jinaai/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from .clients.SceneXClient import SceneXClient
 from .clients.PromptPerfectClient import PromptPerfectClient
 from .clients.RationaleClient import RationaleClient
 from .clients.JinaChatClient import JinaChatClient
+from .clients.BestBannerClient import BestBannerClient
 from .utils import is_url, is_base64, image_to_base64
 
 class JinaAI:
     def __init__(self, secrets={}):
-        PPSecret = f"token {secrets['promptperfect-secret']}" if secrets else ''
-        SXSecret = f"token {secrets['scenex-secret']}" if secrets else ''
-        RASecret = f"token {secrets['rationale-secret']}" if secrets else ''
-        CCSecret = f"Bearer {secrets['jinachat-secret']}" if secrets else ''
+        PPSecret = f"token {secrets['promptperfect-secret']}" if secrets and 'promptperfect-secret' in secrets else ''
+        SXSecret = f"token {secrets['scenex-secret']}" if secrets and 'scenex-secret' in secrets else ''
+        RASecret = f"token {secrets['rationale-secret']}" if secrets and 'rationale-secret' in secrets else ''
+        CCSecret = f"Bearer {secrets['jinachat-secret']}" if secrets and 'jinachat-secret' in secrets else ''
+        BBSecret = f"token {secrets['bestbanner-secret']}" if secrets and 'bestbanner-secret' in secrets else ''
         self.PPClient = PromptPerfectClient(headers = { "x-api-key": PPSecret })
         self.SXClient = SceneXClient(headers = { "x-api-key": SXSecret })
         self.RAClient = RationaleClient(headers = { "x-api-key": RASecret })
         self.CCClient = JinaChatClient(headers = { "authorization": CCSecret })
+        self.BBClient = BestBannerClient(headers = { "x-api-key": BBSecret })
 
     def decide(self, input, options=None):
         if isinstance(input, list):
             data = self.RAClient.from_array(input, options)
         elif isinstance(input, str):
             data = self.RAClient.from_string(input, options)
         else:
@@ -47,16 +50,22 @@
             data = self.CCClient.from_array(input, options)
         elif isinstance(input, str):
             data = self.CCClient.from_string(input, options)
         else:
             data = input
         return self.CCClient.generate(data, options)
 
-    def generate_image(self):
-        raise Exception("banner not implemented")
+    def imagine(self, input, options=None):
+        if isinstance(input, list):
+            data = self.BBClient.from_array(input, options)
+        elif isinstance(input, str):
+            data = self.BBClient.from_string(input, options)
+        else:
+            data = input
+        return self.BBClient.imagine(data, options)
 
     class utils:
         @staticmethod
         def is_url(string):
             return is_url(string)
         @staticmethod
         def is_base64(string):
```

### Comparing `jinaai-0.2.1/jinaai/clients/HTTPClient.py` & `jinaai-0.2.3/jinaai/clients/HTTPClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.1/jinaai/clients/JinaChatClient.py` & `jinaai-0.2.3/jinaai/clients/JinaChatClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.1/jinaai/clients/PromptPerfectClient.py` & `jinaai-0.2.3/jinaai/clients/PromptPerfectClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.1/jinaai/clients/RationaleClient.py` & `jinaai-0.2.3/jinaai/clients/RationaleClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.1/jinaai/utils.py` & `jinaai-0.2.3/jinaai/utils.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.1/jinaai.egg-info/PKG-INFO` & `jinaai-0.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,10 @@
-Metadata-Version: 2.1
-Name: jinaai
-Version: 0.2.1
-Summary: Jina AI Python SDK
-Home-page: https://github.com/jina-ai/jinaai-py.git
-Author: Jina AI
-Author-email: guillaume.roncari@jina.ai
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # JinaAI Python SDK
 
-The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products — [SceneXplain](https://scenex.jina.ai), [PromptPerfect](https://promptperfect.jina.ai/), [Rationale](https://rationale.jina.ai/), and [JinaChat](https://chat.jina.ai/) — into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK lets you effortlessly formulate and fine-tune prompts, thus streamlining application development.
+The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products — [SceneXplain](https://scenex.jina.ai), [PromptPerfect](https://promptperfect.jina.ai/), [Rationale](https://rationale.jina.ai/), [BestBanner](https://bestbanner.jina.ai/), and [JinaChat](https://chat.jina.ai/) — into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK lets you effortlessly formulate and fine-tune prompts, thus streamlining application development.
 
 ## Installing
 
 ### Package manager
 
 Using pip:
 ```bash
@@ -25,14 +15,15 @@
 
 To generate an API secret, you need to authenticate on each respective platform's API tab:
 
 - [SceneXplain API](https://scenex.jina.ai/api)
 - [PromptPerfect API](https://promptperfect.jina.ai/api)
 - [Rationale API](https://rationale.jina.ai/api)
 - [JinaChat API](https://chat.jina.ai/api)
+- [BestBanner API](https://bestbanner.jina.ai/api)
 
 > **Note:** Each secret is product-specific and cannot be interchanged. If you're planning to use multiple products, you'll need to generate a separate secret for each.
 
 ## Example usage
 
 
 Import the SDK and instantiate a new client with your authentication secrets:
@@ -42,14 +33,15 @@
 
 jinaai = JinaAI(
     secrets = {
         'promptperfect-secret': 'XXXXXX',
         'scenex-secret': 'XXXXXX',
         'rationale-secret': 'XXXXXX',
         'jinachat-secret': 'XXXXXX',
+        'bestbanner-secret': 'XXXXXX',
     }
 )
 ```
 
 Describe images:
 
 ```python
@@ -79,14 +71,22 @@
 
 ```python
 output = jinaai.generate(
     'Give me a recipe for a pizza with pineapple'
 )
 ```
 
+Create images from text:
+
+```python
+output = jinaai.imagine(
+    'A controversial fusion of sweet pineapple and savory pizza.'
+)
+```
+
 Use APIs together:
 
 ```python
 situations = [toBase64(img) for img in [
     'factory-1.png',
     'factory-2.png',
     'factory-3.png',
@@ -111,14 +111,18 @@
 
 recommendation = jinaai.generate('\n'.join(propmt2))
 
 swot = jinaai.decide(
     recommendation['output'],
     { 'analysis': 'swot' }
 )
+
+banners = jinaai.imagine(
+    *[desc['output'] for i, desc in enumerate(descriptions['results'])]
+)
 ```
 
 ## Raw Output
 
 You can retrieve the raw output of each APIs by passing `raw: True` in the options:
 
 ```python
@@ -142,26 +146,26 @@
 
 >| VARIABLE                              | TYPE              | VALUE 
 >|---------------------------------------|-------------------|----------
 >| input                                 | str / str array   | Image URL or Base64
 
 - Options
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| options                                | dict              | 
 >| options['algorithm']                   | None / str        | Aqua / Bolt / Comet / Dune / Ember / Flash
->| options['features']                    | None / str array  | high_quality, question_answer
+>| options['features']                    | None / str array  | high_quality, question_answer, tts, opt-out
 >| options['languages']                   | None / str array  | en, cn, de, fr, it...
 >| options['question']                    | None / str        | Question related to the picture(s)
 >| options['style']                       | None / str        | default / concise / prompt
 
 - Output
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['results']                      | dict array        | 
 >| results[0]['output']                   | str               | The picture description
 >| results[0]['i18n']                     | dict              | Contains one key for each item in languages
 >| ...i18n['cn']                          | str               | The translated picture description
 
@@ -171,21 +175,21 @@
 
 ```python
 output = JinaAI.optimize(input, options)
 ```
 
 - Input
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| input                                  | str / str array   | Image URL or Base64 / prompt to optimize
 
 - Options
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| options                                | dict              | 
 >| options['targetModel']                 | None / str        | chatgpt / gpt-4 / stablelm-tuned-alpha-7b / claude / cogenerate / text-davinci-003 / dalle / sd / midjourney / kandinsky / lexica
 >| options['features']                    | None / str array  | preview, no_spam, shorten, bypass_ethics, same_language, always_en, high_quality, redo_original_image, variable_subs, template_run
 >| options['iterations']                  | None / number     | Default: 1
 >| options['previewSettings']             | None / dict       | Contains the settings for the preview
 >| ...previewSettings['temperature']      | number            | Example: 0.9
@@ -196,15 +200,15 @@
 >| options['previewVariables']            | None / dict       | Contains one key for each variables in the prompt
 >| ...previewVariables['var1']            | str               | The value of the variable
 >| options['timeout']                     | Number            | Default: 20000
 >| options['target_language']             | None / str        | en / cn / de / fr / it...
 
 - Output
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['results']                      | dict array        | 
 >| results[0]['output']                   | str               | The optimized prompt
 
 <br/>
 
@@ -212,30 +216,30 @@
 
 ```python
 output = JinaAI.decide(input, options)
 ```
 
 - Input
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| input                                  | str / str array   | Decision to evaluate
 
 - Options
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| options                                | dict              | 
 >| options['analysis']                    | None / str        | proscons / swot / multichoice / outcomes
 >| options['style']                       | None / str        | concise / professional / humor / sarcastic / childish / genZ
 >| options['profileId']                   | None / str        | The id of the Personas you want to use
 
 - Output
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['results']                      | dict array        | 
 >| results[0]['proscons']                 | None / dict       |
 >| ...proscons['pros']                    | dict              | Contains one key for each pros
 >| ...proscons['pros']['pros1']           | str               | The explanation of the pros
 >| ...proscons['cons']                    | dict              | Contains one key for each cons
@@ -268,21 +272,21 @@
 
 ```python
 output = JinaAI.generate(input, options)
 ```
 
 - Input
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE                   | VALUE 
 >|----------------------------------------|------------------------|----------
 >| input                                  | str / str array        | Image URL or Base64 / prompt
 
 - Options
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE                   | VALUE 
 >|----------------------------------------|------------------------|----------
 >| options                                | dict                   | 
 >| options['role']                        | None / str             | user / assistant
 >| options['name']                        | None / str             | The name of the author of this message
 >| options['chatId']                      | None / str             | The id of the conversation to continue
 >| options['stream']                      | None / boolean         | Whether to stream back partial progress, Default: false
 >| options['temperature']                 | None / number          | Default: 1
@@ -292,22 +296,48 @@
 >| options['presence_penalty']            | None / number          | Number between -2.0 and 2.0, Default: 0
 >| options['frequency_penalty']           | None / number          | Number between -2.0 and 2.0, Default: 0
 >| options['logit_bias']                  | None / dict            | The likelihood for a token to appear in the completion
 >| ...logit_bias['tokenId']               | number                 | Bias value from -100 to 100
 
 - Output
 
->| VARIABLE                              | TYPE              | VALUE 
+>| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['output']                       | str               | The generated answer
 >| output['chatId']                       | str               | The chatId to continue the conversation
 
 <br/>
 
+### JinaAi.imagine
+
+```python
+output = JinaAI.imagine(input, options)
+```
+
+- Input
+
+>| VARIABLE                               | TYPE                   | VALUE 
+>|----------------------------------------|------------------------|----------
+>| input                                  | str / str array        | Prompt
+
+- Options
+
+>No options available
+
+- Output
+
+>| VARIABLE                               | TYPE              | VALUE 
+>|----------------------------------------|-------------------|----------
+>| output                                 | dict              | 
+>| output['results']                      | dict array        |
+>| results[0]['output']                   | array             | array of 4 image urls
+
+<br/>
+
 ### JinaAi.utils
 
 ```python
 outout = JinaAI.utils.image_to_base64(input)
 ```
 
 >| VARIABLE                              | TYPE              | VALUE
```

