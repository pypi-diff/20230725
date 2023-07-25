# Comparing `tmp/prompthandler-0.0.2.tar.gz` & `tmp/prompthandler-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompthandler-0.0.2.tar", last modified: Tue Jul 25 15:18:32 2023, max compression
+gzip compressed data, was "prompthandler-0.3.2.tar", last modified: Tue Jul 25 16:06:08 2023, max compression
```

## Comparing `prompthandler-0.0.2.tar` & `prompthandler-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:18:32.439205 prompthandler-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-25 15:18:17.000000 prompthandler-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-25 15:18:32.439205 prompthandler-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-25 15:18:17.000000 prompthandler-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:18:32.439205 prompthandler-0.0.2/prompthandler/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-25 15:18:17.000000 prompthandler-0.0.2/prompthandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-25 15:18:17.000000 prompthandler-0.0.2/prompthandler/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-25 15:18:17.000000 prompthandler-0.0.2/prompthandler/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:18:32.439205 prompthandler-0.0.2/prompthandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-25 15:18:32.000000 prompthandler-0.0.2/prompthandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 15:18:32.000000 prompthandler-0.0.2/prompthandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:18:32.000000 prompthandler-0.0.2/prompthandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 15:18:32.000000 prompthandler-0.0.2/prompthandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 15:18:32.000000 prompthandler-0.0.2/prompthandler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:18:32.439205 prompthandler-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-25 15:18:17.000000 prompthandler-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:06:08.507188 prompthandler-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-25 16:05:54.000000 prompthandler-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-25 16:06:08.503188 prompthandler-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-25 16:05:54.000000 prompthandler-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:06:08.503188 prompthandler-0.3.2/prompthandler/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-25 16:05:54.000000 prompthandler-0.3.2/prompthandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-25 16:05:54.000000 prompthandler-0.3.2/prompthandler/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-25 16:05:54.000000 prompthandler-0.3.2/prompthandler/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:06:08.503188 prompthandler-0.3.2/prompthandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-25 16:06:08.000000 prompthandler-0.3.2/prompthandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 16:06:08.000000 prompthandler-0.3.2/prompthandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:06:08.000000 prompthandler-0.3.2/prompthandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 16:06:08.000000 prompthandler-0.3.2/prompthandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 16:06:08.000000 prompthandler-0.3.2/prompthandler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 16:06:08.507188 prompthandler-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-25 16:05:54.000000 prompthandler-0.3.2/setup.py
```

### Comparing `prompthandler-0.0.2/LICENSE` & `prompthandler-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prompthandler-0.0.2/PKG-INFO` & `prompthandler-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompthandler
-Version: 0.0.2
+Version: 0.3.2
 Summary: Token Management system for chatgpt and more. Keeps your prompt under token with summary support
 Author: prasannan-robots
 License: MIT License
         
         Copyright (c) 2023 Prasanna
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prompthandler-0.0.2/README.md` & `prompthandler-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `prompthandler-0.0.2/prompthandler/models.py` & `prompthandler-0.3.2/prompthandler/models.py`

 * *Files identical despite different names*

### Comparing `prompthandler-0.0.2/prompthandler/prompts.py` & `prompthandler-0.3.2/prompthandler/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.update_messages()
         return {'head':self.headers,'body':self.body,'messages':self.messages}
         
     def load(self,dictionary):
         """
         Load the data from the dictionary
         """
-        self.headers - dictionary['head']
+        self.headers = dictionary['head']
         self.body = dictionary['body']
         self.messages = dictionary['messages']
         self.update()
 
     def get_completion(self, message='', update_history=True, temperature=None):
         """
         Generates a completion for the conversation history.
```

### Comparing `prompthandler-0.0.2/prompthandler.egg-info/PKG-INFO` & `prompthandler-0.3.2/prompthandler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompthandler
-Version: 0.0.2
+Version: 0.3.2
 Summary: Token Management system for chatgpt and more. Keeps your prompt under token with summary support
 Author: prasannan-robots
 License: MIT License
         
         Copyright (c) 2023 Prasanna
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prompthandler-0.0.2/setup.py` & `prompthandler-0.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 with open("README.md", "r") as fh:
     long_description = fh.read()
 with open("LICENSE", "r") as fg:
     license_val = fg.read()
 setup(
     name="prompthandler",
-    version="0.0.2",
+    version="0.3.2",
     author="prasannan-robots",
     description="Token Management system for chatgpt and more. Keeps your prompt under token with summary support",
     install_requires=["openai","tiktoken"],
     packages=['prompthandler'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

