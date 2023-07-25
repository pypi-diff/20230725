# Comparing `tmp/mutual-0.2.0.tar.gz` & `tmp/mutual-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutual-0.2.0.tar", last modified: Sat Jul 22 04:38:16 2023, max compression
+gzip compressed data, was "mutual-0.2.1.tar", last modified: Tue Jul 25 02:55:37 2023, max compression
```

## Comparing `mutual-0.2.0.tar` & `mutual-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-22 04:38:16.544933 mutual-0.2.0/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.2.0/LICENSE.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)     5949 2023-07-22 04:38:16.544755 mutual-0.2.0/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)     5523 2023-07-22 04:36:24.000000 mutual-0.2.0/README.md
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-22 04:38:16.543545 mutual-0.2.0/mutual/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1035 2023-07-22 04:22:14.000000 mutual-0.2.0/mutual/APIKey.py
--rw-r--r--   0 alexbetita   (501) staff       (20)    10382 2023-07-22 04:34:37.000000 mutual-0.2.0/mutual/Bot.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4858 2023-07-22 04:24:52.000000 mutual-0.2.0/mutual/Chat.py
--rw-r--r--   0 alexbetita   (501) staff       (20)      602 2023-07-22 04:25:05.000000 mutual-0.2.0/mutual/Dev.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3619 2023-07-22 04:25:23.000000 mutual-0.2.0/mutual/Judge.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3649 2023-07-22 04:25:41.000000 mutual-0.2.0/mutual/JudgeMessage.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3948 2023-07-22 04:26:05.000000 mutual-0.2.0/mutual/Prompt.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4174 2023-07-22 04:08:17.000000 mutual-0.2.0/mutual/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-22 04:38:16.544511 mutual-0.2.0/mutual.egg-info/
--rw-r--r--   0 alexbetita   (501) staff       (20)     5949 2023-07-22 04:38:16.000000 mutual-0.2.0/mutual.egg-info/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)      314 2023-07-22 04:38:16.000000 mutual-0.2.0/mutual.egg-info/SOURCES.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-22 04:38:16.000000 mutual-0.2.0/mutual.egg-info/dependency_links.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-22 04:38:16.000000 mutual-0.2.0/mutual.egg-info/requires.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-22 04:38:16.000000 mutual-0.2.0/mutual.egg-info/top_level.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-22 04:38:16.544986 mutual-0.2.0/setup.cfg
--rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-22 04:37:55.000000 mutual-0.2.0/setup.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-25 02:55:37.097258 mutual-0.2.1/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.2.1/LICENSE.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)     5949 2023-07-25 02:55:37.097097 mutual-0.2.1/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)     5523 2023-07-22 04:36:24.000000 mutual-0.2.1/README.md
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-25 02:55:37.095919 mutual-0.2.1/mutual/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1035 2023-07-22 04:22:14.000000 mutual-0.2.1/mutual/APIKey.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     9156 2023-07-25 02:54:54.000000 mutual-0.2.1/mutual/Bot.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4858 2023-07-22 04:24:52.000000 mutual-0.2.1/mutual/Chat.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)      602 2023-07-22 04:25:05.000000 mutual-0.2.1/mutual/Dev.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3619 2023-07-22 04:25:23.000000 mutual-0.2.1/mutual/Judge.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3649 2023-07-22 04:25:41.000000 mutual-0.2.1/mutual/JudgeMessage.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3948 2023-07-22 04:26:05.000000 mutual-0.2.1/mutual/Prompt.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4174 2023-07-22 04:08:17.000000 mutual-0.2.1/mutual/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-25 02:55:37.096850 mutual-0.2.1/mutual.egg-info/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     5949 2023-07-25 02:55:37.000000 mutual-0.2.1/mutual.egg-info/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)      314 2023-07-25 02:55:37.000000 mutual-0.2.1/mutual.egg-info/SOURCES.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-25 02:55:37.000000 mutual-0.2.1/mutual.egg-info/dependency_links.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-25 02:55:37.000000 mutual-0.2.1/mutual.egg-info/requires.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-25 02:55:37.000000 mutual-0.2.1/mutual.egg-info/top_level.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-25 02:55:37.097311 mutual-0.2.1/setup.cfg
+-rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-25 02:55:04.000000 mutual-0.2.1/setup.py
```

### Comparing `mutual-0.2.0/LICENSE.txt` & `mutual-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mutual-0.2.0/PKG-INFO` & `mutual-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mutual-0.2.0/README.md` & `mutual-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mutual-0.2.0/mutual/APIKey.py` & `mutual-0.2.1/mutual/APIKey.py`

 * *Files identical despite different names*

### Comparing `mutual-0.2.0/mutual/Bot.py` & `mutual-0.2.1/mutual/Bot.py`

 * *Files 8% similar despite different names*

```diff
@@ -173,15 +173,16 @@
 
 
         if response.status_code < 300:
             is_new_bot = False
             is_new_user = False
 
             # add the newly created bot to the bot class
-            print("\n", end="", flush=True)
+            
+
             for line in response.iter_lines():
                 if line:  # filter out keep-alive new lines
                     json_data = json.loads(line)
                     if not self.bot_id:
                         self.bot_id = json_data['data']['bot_data']['bot_id']
                     if json_data['error'] is not None and not error_logs:
                         continue
@@ -192,38 +193,17 @@
                         is_new_user = True
                         print(f"New user {json_data['data']['user_data']['username']} created interacting with bot id: {json_data['data']['bot_data']['bot_id']}")
                     if json_data['content'] =='[close]':
                         continue
                     yield json_data
 
             if flow or self.flow:
-                print("Type in clear into the input to clear the messages from the terminal...")
-            while True:
-                if flow or self.flow:
-                    print("\n\n", end="", flush=True)
-                    new_content = input("Please enter a new response or type exit to clear the screen or type clear to clear the screen: ")
-                    if new_content.strip().lower() == "exit":
-                        self.flow = False
-                        break
-                    elif new_content.strip().lower() == "clear":
-                        # Detect the OS and run the clear command accordingly
-                        if platform.system() == "Windows":
-                            os.system('cls')
-                        elif platform.system() == "Linux" or platform.system() == "Darwin":
-                            os.system('clear')
-                    else:
-                        content = new_content
-                        response = requests.post(url, data=json.dumps(data), headers=headers, stream=True)
-
-                        if response.status_code < 300:
-                            for line in response.iter_lines():
-                                if line:  # filter out keep-alive new lines
-                                    json_data = json.loads(line)
-                                    if json_data['error'] is not None and not error_logs:
-                                        continue
-                                    if json_data['content'] =='[close]':
-                                        continue
-                                    yield json_data
+                print("\n\n", end="", flush=True)
+                new_content = input("Please enter a new response or type exit to exit: ")
+                if new_content.strip().lower() == "exit":
+                    return
+                for msg in self.chat(content=new_content, username=username, prompt=prompt, multiplayer_memory=multiplayer_memory, context_window=context_window, flow=flow):
+                    yield msg
         else:
             self.default_stream_response['content'] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
             print(f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}")
             return self.default_stream_response
```

### Comparing `mutual-0.2.0/mutual/Chat.py` & `mutual-0.2.1/mutual/Chat.py`

 * *Files identical despite different names*

### Comparing `mutual-0.2.0/mutual/Dev.py` & `mutual-0.2.1/mutual/Dev.py`

 * *Files identical despite different names*

### Comparing `mutual-0.2.0/mutual/Judge.py` & `mutual-0.2.1/mutual/Judge.py`

 * *Files identical despite different names*

### Comparing `mutual-0.2.0/mutual/JudgeMessage.py` & `mutual-0.2.1/mutual/JudgeMessage.py`

 * *Files identical despite different names*

### Comparing `mutual-0.2.0/mutual/Prompt.py` & `mutual-0.2.1/mutual/Prompt.py`

 * *Files identical despite different names*

### Comparing `mutual-0.2.0/mutual/__init__.py` & `mutual-0.2.1/mutual/__init__.py`

 * *Files identical despite different names*

### Comparing `mutual-0.2.0/mutual.egg-info/PKG-INFO` & `mutual-0.2.1/mutual.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mutual-0.2.0/setup.py` & `mutual-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mutual',
-    version='0.2.0',  # beta
+    version='0.2.1',  # beta
     description='A Python client for the Mutual API.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Alex Betita', # placeholder for now
     author_email='alexbetita25@gmail.com', # placeholder for now
     url='https://github.com/Mutu-AI',  # if you have a github repo for the package
     packages=find_packages(),
```

