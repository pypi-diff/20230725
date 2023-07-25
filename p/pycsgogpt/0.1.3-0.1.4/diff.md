# Comparing `tmp/pycsgogpt-0.1.3.tar.gz` & `tmp/pycsgogpt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycsgogpt-0.1.3.tar", max compression
+gzip compressed data, was "pycsgogpt-0.1.4.tar", max compression
```

## Comparing `pycsgogpt-0.1.3.tar` & `pycsgogpt-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2023-07-06 19:25:41.742541 pycsgogpt-0.1.3/LICENSE
--rw-r--r--   0        0        0     1024 2023-07-06 19:25:41.742541 pycsgogpt-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-07-06 19:25:41.742541 pycsgogpt-0.1.3/pycsgogpt/__init__.py
--rw-r--r--   0        0        0      715 2023-07-06 19:25:41.742541 pycsgogpt-0.1.3/pycsgogpt/__main__.py
--rw-r--r--   0        0        0     2218 2023-07-06 19:25:41.742541 pycsgogpt-0.1.3/pycsgogpt/csgo_chatbot.py
--rw-r--r--   0        0        0      807 2023-07-06 19:25:41.742541 pycsgogpt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 pycsgogpt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-08 17:27:00.934247 pycsgogpt-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1049 2023-07-08 17:27:00.934247 pycsgogpt-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-08 17:27:00.934247 pycsgogpt-0.1.4/pycsgogpt/__init__.py
+-rw-r--r--   0        0        0      749 2023-07-08 17:27:00.934247 pycsgogpt-0.1.4/pycsgogpt/__main__.py
+-rw-r--r--   0        0        0     2218 2023-07-08 17:27:00.934247 pycsgogpt-0.1.4/pycsgogpt/csgo_chatbot.py
+-rw-r--r--   0        0        0      807 2023-07-08 17:27:00.934247 pycsgogpt-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1922 1970-01-01 00:00:00.000000 pycsgogpt-0.1.4/PKG-INFO
```

### Comparing `pycsgogpt-0.1.3/LICENSE` & `pycsgogpt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycsgogpt-0.1.3/README.md` & `pycsgogpt-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # pycsgogpt
 
 **pycsgogpt** is a CSGO chatbot powered by OpenAI GPT-3.5 Turbo. It connects to a CSGO client via Telnet and uses the GPT-3.5 Turbo model to generate responses based on incoming messages from other players. The chatbot provides an interactive and fun experience by simulating human-like conversations in the game.
 
+![Alt text](image.png)
+
+
 ## Installation
 
 ```bash
 pip install pycsgogpt
 ```
 
 ## Usage
```

### Comparing `pycsgogpt-0.1.3/pycsgogpt/__main__.py` & `pycsgogpt-0.1.4/pycsgogpt/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
     try:
         chat_bot.loop()
     except KeyboardInterrupt:
         print("Exiting...")
     except ConnectionRefusedError:
         print(f"Connection refused. Make sure you add `-netconport {telnet_port}` to the CSGO server launch options.")
+        print("Is csgo running?")
     except ConnectionAbortedError:
         print("Bye!")
 
 def main():
     app.command()(entry)
     app()
```

### Comparing `pycsgogpt-0.1.3/pycsgogpt/csgo_chatbot.py` & `pycsgogpt-0.1.4/pycsgogpt/csgo_chatbot.py`

 * *Files identical despite different names*

### Comparing `pycsgogpt-0.1.3/pyproject.toml` & `pycsgogpt-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "pycsgogpt"
-version = "0.1.3"
+version = "0.1.4"
 description = "CSGO Chatbot using OpenAI GPT-3.5 Turbo."
 authors = ["Aviv <4440524+nikeix@users.noreply.github.com>"]
 license = "MIT"
 keywords = ["csgo", "chatbot", "openai", "gpt"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `pycsgogpt-0.1.3/PKG-INFO` & `pycsgogpt-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycsgogpt
-Version: 0.1.3
+Version: 0.1.4
 Summary: CSGO Chatbot using OpenAI GPT-3.5 Turbo.
 Home-page: https://github.com/nikeix/pycsgogpt
 License: MIT
 Keywords: csgo,chatbot,openai,gpt
 Author: Aviv
 Author-email: 4440524+nikeix@users.noreply.github.com
 Requires-Python: >=3.7.1,<4.0.0
@@ -21,14 +21,17 @@
 Project-URL: Repository, https://github.com/nikeix/pycsgogpt
 Description-Content-Type: text/markdown
 
 # pycsgogpt
 
 **pycsgogpt** is a CSGO chatbot powered by OpenAI GPT-3.5 Turbo. It connects to a CSGO client via Telnet and uses the GPT-3.5 Turbo model to generate responses based on incoming messages from other players. The chatbot provides an interactive and fun experience by simulating human-like conversations in the game.
 
+![Alt text](image.png)
+
+
 ## Installation
 
 ```bash
 pip install pycsgogpt
 ```
 
 ## Usage
```

