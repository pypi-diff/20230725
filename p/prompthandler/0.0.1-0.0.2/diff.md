# Comparing `tmp/prompthandler-0.0.1.tar.gz` & `tmp/prompthandler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompthandler-0.0.1.tar", last modified: Tue Jul 25 13:45:41 2023, max compression
+gzip compressed data, was "prompthandler-0.0.2.tar", last modified: Tue Jul 25 15:18:32 2023, max compression
```

## Comparing `prompthandler-0.0.1.tar` & `prompthandler-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 13:45:41.335912 prompthandler-0.0.1/
--rw-rw-rw-   0        0        0     1086 2023-07-25 13:36:35.000000 prompthandler-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1075 2023-07-25 13:45:41.322909 prompthandler-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      594 2023-07-25 13:31:40.000000 prompthandler-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 13:45:41.156178 prompthandler-0.0.1/prompthandler/
--rw-rw-rw-   0        0        0       71 2023-07-25 11:06:11.000000 prompthandler-0.0.1/prompthandler/__init__.py
--rw-rw-rw-   0        0        0     2095 2023-07-25 12:48:53.000000 prompthandler-0.0.1/prompthandler/models.py
--rw-rw-rw-   0        0        0     7956 2023-07-25 12:50:34.000000 prompthandler-0.0.1/prompthandler/prompts.py
-drwxrwxrwx   0        0        0        0 2023-07-25 13:45:41.307906 prompthandler-0.0.1/prompthandler.egg-info/
--rw-rw-rw-   0        0        0     1075 2023-07-25 13:45:40.000000 prompthandler-0.0.1/prompthandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-07-25 13:45:40.000000 prompthandler-0.0.1/prompthandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 13:45:40.000000 prompthandler-0.0.1/prompthandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-25 13:45:40.000000 prompthandler-0.0.1/prompthandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-25 13:45:40.000000 prompthandler-0.0.1/prompthandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 13:45:41.337906 prompthandler-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      801 2023-07-25 13:45:30.000000 prompthandler-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:18:32.439205 prompthandler-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-25 15:18:17.000000 prompthandler-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-25 15:18:32.439205 prompthandler-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-25 15:18:17.000000 prompthandler-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:18:32.439205 prompthandler-0.0.2/prompthandler/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-25 15:18:17.000000 prompthandler-0.0.2/prompthandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-25 15:18:17.000000 prompthandler-0.0.2/prompthandler/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-25 15:18:17.000000 prompthandler-0.0.2/prompthandler/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:18:32.439205 prompthandler-0.0.2/prompthandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-25 15:18:32.000000 prompthandler-0.0.2/prompthandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 15:18:32.000000 prompthandler-0.0.2/prompthandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:18:32.000000 prompthandler-0.0.2/prompthandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 15:18:32.000000 prompthandler-0.0.2/prompthandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 15:18:32.000000 prompthandler-0.0.2/prompthandler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:18:32.439205 prompthandler-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-25 15:18:17.000000 prompthandler-0.0.2/setup.py
```

### Comparing `prompthandler-0.0.1/prompthandler/models.py` & `prompthandler-0.0.2/prompthandler/models.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import openai
-import os
-
-class openai_chat_gpt:
-    """
-    This class represents interacting with the GPT-3.5-turbo model (or other OpenAI models).
-
-    Attributes:
-        api_key (str): The OpenAI API key.
-        model (str): The name of the OpenAI model to use.
-        MAX_TOKEN (int): The maximum number of tokens allowed for the generated completion.
-        temperature (float): The temperature parameter controlling the randomness of the output.
-    """
-
-    def __init__(self, api_key=None, MAX_TOKEN=4096, temperature=0, model="gpt-3.5-turbo-0613"):
-        """
-        Initializes the OpenAI chat model with the provided settings.
-
-        Args:
-            api_key (str): The OpenAI API key.
-            MAX_TOKEN (int): The maximum number of tokens allowed for the generated completion.
-            temperature (float): The temperature parameter controlling the randomness of the output.
-            model (str): The name of the OpenAI model to use.
-        """
-        self.api_key = api_key
-        self.model = model
-        self.MAX_TOKEN = MAX_TOKEN
-        self.temperature = temperature
-        if api_key is not None:
-            openai.api_key = self.api_key
-
-    def get_completion_for_message(self, message, temperature=None):
-        """
-        Generates a completion for a given message using the specified OpenAI model.
-
-        Args:
-            message (list): List of messages representing the conversation history.
-            temperature (float): Control the randomness of the output. If not provided, it uses the default temperature.
-
-        Returns:
-            str: The completion generated by the model.
-            int: The number of tokens used by the completion.
-        """
-        if temperature is None:
-            temperature = self.temperature
-        completion = openai.ChatCompletion.create(
-            model=self.model,
-            messages=message,
-            temperature=temperature
-        )
-        return completion.choices[0].message['content'], completion['usage']['prompt_tokens']
+import openai
+import os
+
+class openai_chat_gpt:
+    """
+    This class represents interacting with the GPT-3.5-turbo model (or other OpenAI models).
+
+    Attributes:
+        api_key (str): The OpenAI API key.
+        model (str): The name of the OpenAI model to use.
+        MAX_TOKEN (int): The maximum number of tokens allowed for the generated completion.
+        temperature (float): The temperature parameter controlling the randomness of the output.
+    """
+
+    def __init__(self, api_key=None, MAX_TOKEN=4096, temperature=0, model="gpt-3.5-turbo-0613"):
+        """
+        Initializes the OpenAI chat model with the provided settings.
+
+        Args:
+            api_key (str): The OpenAI API key.
+            MAX_TOKEN (int): The maximum number of tokens allowed for the generated completion.
+            temperature (float): The temperature parameter controlling the randomness of the output.
+            model (str): The name of the OpenAI model to use.
+        """
+        self.api_key = api_key
+        self.model = model
+        self.MAX_TOKEN = MAX_TOKEN
+        self.temperature = temperature
+        if api_key is not None:
+            openai.api_key = self.api_key
+
+    def get_completion_for_message(self, message, temperature=None):
+        """
+        Generates a completion for a given message using the specified OpenAI model.
+
+        Args:
+            message (list): List of messages representing the conversation history.
+            temperature (float): Control the randomness of the output. If not provided, it uses the default temperature.
+
+        Returns:
+            str: The completion generated by the model.
+            int: The number of tokens used by the completion.
+        """
+        if temperature is None:
+            temperature = self.temperature
+        completion = openai.ChatCompletion.create(
+            model=self.model,
+            messages=message,
+            temperature=temperature
+        )
+        return completion.choices[0].message['content'], completion['usage']['prompt_tokens']
```

### Comparing `prompthandler-0.0.1/setup.py` & `prompthandler-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from setuptools import setup, find_packages
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setup(
-    name="prompthandler",
-    version="0.0.1",
-    author="prasannan-robots",
-    description="Token Management system for chatgpt and more. Keeps your prompt under token with summary support",
-    install_requires=["openai","tiktoken"],
-    packages=['prompthandler'],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    long_description=long_description,      # Long description read from the the readme file
-    long_description_content_type="text/markdown",
-    keywords='openai chatgpt prompts summarizer handler summary token gpt-4'
-)
+from setuptools import setup, find_packages
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+with open("LICENSE", "r") as fg:
+    license_val = fg.read()
+setup(
+    name="prompthandler",
+    version="0.0.2",
+    author="prasannan-robots",
+    description="Token Management system for chatgpt and more. Keeps your prompt under token with summary support",
+    install_requires=["openai","tiktoken"],
+    packages=['prompthandler'],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    license = license_val,
+    long_description=long_description,      # Long description read from the the readme file
+    long_description_content_type="text/markdown",
+    keywords='openai chatgpt prompts summarizer handler summary token gpt-4'
+)
```

