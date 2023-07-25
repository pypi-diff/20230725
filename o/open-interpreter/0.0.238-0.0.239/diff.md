# Comparing `tmp/open_interpreter-0.0.238.tar.gz` & `tmp/open_interpreter-0.0.239.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.238.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.239.tar", max compression
```

## Comparing `open_interpreter-0.0.238.tar` & `open_interpreter-0.0.239.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.238/LICENSE
--rw-r--r--   0        0        0     6106 2023-07-24 03:07:00.576388 open_interpreter-0.0.238/README.md
--rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.238/interpreter/__init__.py
--rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.238/interpreter/exec.py
--rw-r--r--   0        0        0     8636 2023-07-24 05:18:21.839348 open_interpreter-0.0.238/interpreter/interpreter.py
--rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.238/interpreter/json_utils.py
--rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.238/interpreter/openai_utils.py
--rw-r--r--   0        0        0     2399 2023-07-19 15:47:18.035279 open_interpreter-0.0.238/interpreter/system_message.txt
--rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.238/interpreter/view.py
--rw-r--r--   0        0        0      564 2023-07-24 05:19:34.636882 open_interpreter-0.0.238/pyproject.toml
--rw-r--r--   0        0        0     6730 1970-01-01 00:00:00.000000 open_interpreter-0.0.238/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.239/LICENSE
+-rw-r--r--   0        0        0     6342 2023-07-25 06:11:11.305427 open_interpreter-0.0.239/README.md
+-rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.239/interpreter/__init__.py
+-rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.239/interpreter/exec.py
+-rw-r--r--   0        0        0     8999 2023-07-25 05:37:59.116112 open_interpreter-0.0.239/interpreter/interpreter.py
+-rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.239/interpreter/json_utils.py
+-rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.239/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     2399 2023-07-19 15:47:18.035279 open_interpreter-0.0.239/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.239/interpreter/view.py
+-rw-r--r--   0        0        0      556 2023-07-25 06:27:39.303393 open_interpreter-0.0.239/pyproject.toml
+-rw-r--r--   0        0        0     6966 1970-01-01 00:00:00.000000 open_interpreter-0.0.239/PKG-INFO
```

### Comparing `open_interpreter-0.0.238/LICENSE` & `open_interpreter-0.0.239/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.238/README.md` & `open_interpreter-0.0.239/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ```
 
 ### Terminal
 
 After installation, set your `OPENAI_API_KEY` environment variable, then simply run `interpreter`:
 
 ```shell
-interpreter
+interpreter // Add --safe_mode to ask for confirmation before running generated code
 ```
 
 ### Python
 
 ```python
 import interpreter
 
@@ -79,15 +79,15 @@
 ## Commands
 
 #### Interactive Chat
 
 To start an interactive chat in your terminal, either run `interpreter` from the command line:
 
 ```shell
-interpreter
+interpreter --safe_mode
 ```
 
 Or `interpreter.chat()` from a .py file:
 
 ```python
 interpreter.chat()
 ```
@@ -140,25 +140,24 @@
 
 Open Interpreter equips a [function-calling GPT-4](https://platform.openai.com/docs/guides/gpt/function-calling) with the `exec()` function.
 
 We then stream the model's messages, code, and your system's outputs to the terminal as Markdown.
 
 Only the last `model_max_tokens` of the conversation are shown to the model, so conversations can be any length, but older messages may be forgotten.
 
-Sure, here's an updated version:
-
 ## Safety Notice
 
 Since generated code is executed in your local environment, it can interact with your files and system settings, potentially leading to unexpected outcomes like data loss or security risks.
 
 - Be cautious when requesting commands that modify files or system settings.
 - Watch Open Interpreter like a self-driving car, and be prepared to end the process by closing your terminal.
 - Regularly back up your data and work in a virtual environment.
 - Open Interpreter utilizes `interpreter.forbidden_commands`, a list of potentially harmful commands that are disallowed by default. You can modify this list, but do so with caution.
 - Consider running the Open Interpreter in a restricted environment like Google Colab or Replit. These environments are more isolated, reducing the risks associated with executing arbitrary code.
+- Utilize Safe Mode by running `interpreter --safe_mode` from the terminal or setting `interpreter.safe_mode = True` in Python. This asks for user confirmation before running any code.
 
 ## Contributing
 
 As an open-source project, we are extremely open to contributions, whether it be in the form of a new feature, improved infrastructure, or better documentation.
 
 ## License
```

### Comparing `open_interpreter-0.0.238/interpreter/exec.py` & `open_interpreter-0.0.239/interpreter/exec.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.238/interpreter/interpreter.py` & `open_interpreter-0.0.239/interpreter/interpreter.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,19 @@
   system_message = f.read().strip()
 
 
 class Interpreter:
 
   def __init__(self):
     self.messages = []
-    self._logs = []
     self.system_message = system_message
     self.temperature = 0.2
     self.api_key = None
     self.max_output_chars = 2000
+    self.safe_mode = False
 
     # Commands Open Interpreter cannot run
     self.forbidden_commands = [
       "!rm -rf /",
       "!rm -rf *",
       "!find / -delete",
       "!> /dev/sda",
@@ -87,21 +87,19 @@
       "os.system('reboot')",  # Python command
       "os.system('halt')",  # Python command
       "os.system('poweroff')",  # Python command
       "os.system('passwd root')",  # Python command
       "os.system('init 0')",  # Python command
       "os.system('dd if=/dev/zero of=/dev/sda')",  # Python command
       "os.system('mkfs.ext3 /dev/sda1')",  # Python command
-      "os.system('mv directory_to_destroy /dev/null')",  # Python command
       "os.system('openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout /etc/ssl/private/apache-selfsigned.key -out /etc/ssl/certs/apache-selfsigned.crt')",  # Python command
     ]
 
   def reset(self):
     self.messages = []
-    self._logs = []
 
   def load(self, messages):
     self.messages = messages
 
   def chat(self, message=None, return_messages=False):
     self.verify_api_key()
 
@@ -126,25 +124,22 @@
         self.respond()
 
     if return_messages:
       return self.messages
 
   def display(self, delta):
 
-    old_delta = delta
-
     if delta == None:
       return
 
     if "content" in delta and delta["content"] != None:
       delta = {"type": "message", "content": delta["content"]}
     elif "function_call" in delta:
       delta = {"type": "function", "content": delta["function_call"]}
 
-    self._logs.append(["old delta:", old_delta, "new delta:", delta])
     self.view.process_delta(delta)
 
   def verify_api_key(self):
     if self.api_key == None:
       if 'OPENAI_API_KEY' in os.environ:
         self.api_key = os.environ['OPENAI_API_KEY']
       else:
@@ -216,15 +211,14 @@
 
           # For interpreter
           if func_call["name"] != "run_code":
             func_call["name"] = "run_code"
 
           function = [f for f in functions
                       if f["name"] == func_call["name"]][0]["function"]
-          self._logs.append(func_call["arguments"])
 
           # For interpreter. Sometimes it just sends the code??
           try:
             function_args = json.loads(func_call["arguments"])
           except:
             function_args = {"code": func_call["arguments"]}
 
@@ -234,25 +228,40 @@
           # For interpreter. This should always be true:
           if func_call["name"] == "run_code":
             # Pass in max_output_chars to truncate the output
             function_args["max_output_chars"] = self.max_output_chars
             # Pass in forbidden_commands
             function_args["forbidden_commands"] = self.forbidden_commands
 
-          output = function(**function_args)
+          user_declined = False
+          if self.safe_mode:
+            # Ask the user for confirmation
+            print()
+            response = input("Would you like to run the above code? (y/n) ")
+            print()
+            if response.lower().strip() != "y":
+              user_declined = True
+            else:
+              user_declined = False
+
+          if user_declined:
+            output = "The user you're chatting with declined to run this code on their machine. It may be best to ask them why, or to try another method."
+          else:
+            output = function(**function_args)
 
           event = {
             "role": "function",
             "name": func_call["name"],
             "content": output
           }
           self.messages.append(event)
 
           # Go around again
-          self.respond()
+          if not user_declined:
+            self.respond()
 
         if "content" in delta and delta.content != None:
           event["content"] += delta.content
           self.display(delta)
 
         if chunk.choices[0].finish_reason and chunk.choices[
             0].finish_reason != "function_call":
```

### Comparing `open_interpreter-0.0.238/interpreter/json_utils.py` & `open_interpreter-0.0.239/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.238/interpreter/openai_utils.py` & `open_interpreter-0.0.239/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.238/interpreter/system_message.txt` & `open_interpreter-0.0.239/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.238/interpreter/view.py` & `open_interpreter-0.0.239/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.238/pyproject.toml` & `open_interpreter-0.0.239/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"}
 ]
-version = "0.0.238"
+version = "0.0.239"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
@@ -20,8 +20,8 @@
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-interpreter = "interpreter:chat"
+interpreter = "cli:main"
```

### Comparing `open_interpreter-0.0.238/PKG-INFO` & `open_interpreter-0.0.239/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.238
+Version: 0.0.239
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -62,15 +62,15 @@
 ```
 
 ### Terminal
 
 After installation, set your `OPENAI_API_KEY` environment variable, then simply run `interpreter`:
 
 ```shell
-interpreter
+interpreter // Add --safe_mode to ask for confirmation before running generated code
 ```
 
 ### Python
 
 ```python
 import interpreter
 
@@ -97,15 +97,15 @@
 ## Commands
 
 #### Interactive Chat
 
 To start an interactive chat in your terminal, either run `interpreter` from the command line:
 
 ```shell
-interpreter
+interpreter --safe_mode
 ```
 
 Or `interpreter.chat()` from a .py file:
 
 ```python
 interpreter.chat()
 ```
@@ -158,25 +158,24 @@
 
 Open Interpreter equips a [function-calling GPT-4](https://platform.openai.com/docs/guides/gpt/function-calling) with the `exec()` function.
 
 We then stream the model's messages, code, and your system's outputs to the terminal as Markdown.
 
 Only the last `model_max_tokens` of the conversation are shown to the model, so conversations can be any length, but older messages may be forgotten.
 
-Sure, here's an updated version:
-
 ## Safety Notice
 
 Since generated code is executed in your local environment, it can interact with your files and system settings, potentially leading to unexpected outcomes like data loss or security risks.
 
 - Be cautious when requesting commands that modify files or system settings.
 - Watch Open Interpreter like a self-driving car, and be prepared to end the process by closing your terminal.
 - Regularly back up your data and work in a virtual environment.
 - Open Interpreter utilizes `interpreter.forbidden_commands`, a list of potentially harmful commands that are disallowed by default. You can modify this list, but do so with caution.
 - Consider running the Open Interpreter in a restricted environment like Google Colab or Replit. These environments are more isolated, reducing the risks associated with executing arbitrary code.
+- Utilize Safe Mode by running `interpreter --safe_mode` from the terminal or setting `interpreter.safe_mode = True` in Python. This asks for user confirmation before running any code.
 
 ## Contributing
 
 As an open-source project, we are extremely open to contributions, whether it be in the form of a new feature, improved infrastructure, or better documentation.
 
 ## License
```

