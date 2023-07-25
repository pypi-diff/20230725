# Comparing `tmp/chatgpt_tui-0.6.0.tar.gz` & `tmp/chatgpt_tui-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_tui-0.6.0.tar", last modified: Wed Mar 29 00:57:00 2023, max compression
+gzip compressed data, was "chatgpt_tui-0.7.0.tar", last modified: Tue Jul 25 08:46:35 2023, max compression
```

## Comparing `chatgpt_tui-0.6.0.tar` & `chatgpt_tui-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jiayipan   (501) staff       (20)        0 2023-03-29 00:57:00.895283 chatgpt_tui-0.6.0/
--rw-r--r--   0 jiayipan   (501) staff       (20)     1067 2023-03-29 00:44:13.000000 chatgpt_tui-0.6.0/LICENSE
--rw-r--r--   0 jiayipan   (501) staff       (20)     1431 2023-03-29 00:57:00.895162 chatgpt_tui-0.6.0/PKG-INFO
--rw-r--r--   0 jiayipan   (501) staff       (20)      959 2023-03-29 00:47:24.000000 chatgpt_tui-0.6.0/README.md
-drwxr-xr-x   0 jiayipan   (501) staff       (20)        0 2023-03-29 00:57:00.894020 chatgpt_tui-0.6.0/chatgpt_tui/
--rw-r--r--   0 jiayipan   (501) staff       (20)        0 2023-03-29 00:44:13.000000 chatgpt_tui-0.6.0/chatgpt_tui/__init__.py
--rw-r--r--   0 jiayipan   (501) staff       (20)     2639 2023-03-29 00:55:16.000000 chatgpt_tui-0.6.0/chatgpt_tui/app.py
--rw-r--r--   0 jiayipan   (501) staff       (20)      954 2023-03-29 00:44:13.000000 chatgpt_tui-0.6.0/chatgpt_tui/chat_api.py
--rw-r--r--   0 jiayipan   (501) staff       (20)      938 2023-03-29 00:44:13.000000 chatgpt_tui-0.6.0/chatgpt_tui/structures.py
--rw-r--r--   0 jiayipan   (501) staff       (20)     1554 2023-03-29 00:44:13.000000 chatgpt_tui-0.6.0/chatgpt_tui/style.css
--rw-r--r--   0 jiayipan   (501) staff       (20)     2260 2023-03-29 00:55:03.000000 chatgpt_tui-0.6.0/chatgpt_tui/widgets.py
-drwxr-xr-x   0 jiayipan   (501) staff       (20)        0 2023-03-29 00:57:00.895003 chatgpt_tui-0.6.0/chatgpt_tui.egg-info/
--rw-r--r--   0 jiayipan   (501) staff       (20)     1431 2023-03-29 00:57:00.000000 chatgpt_tui-0.6.0/chatgpt_tui.egg-info/PKG-INFO
--rw-r--r--   0 jiayipan   (501) staff       (20)      376 2023-03-29 00:57:00.000000 chatgpt_tui-0.6.0/chatgpt_tui.egg-info/SOURCES.txt
--rw-r--r--   0 jiayipan   (501) staff       (20)        1 2023-03-29 00:57:00.000000 chatgpt_tui-0.6.0/chatgpt_tui.egg-info/dependency_links.txt
--rw-r--r--   0 jiayipan   (501) staff       (20)       46 2023-03-29 00:57:00.000000 chatgpt_tui-0.6.0/chatgpt_tui.egg-info/entry_points.txt
--rw-r--r--   0 jiayipan   (501) staff       (20)       24 2023-03-29 00:57:00.000000 chatgpt_tui-0.6.0/chatgpt_tui.egg-info/requires.txt
--rw-r--r--   0 jiayipan   (501) staff       (20)       12 2023-03-29 00:57:00.000000 chatgpt_tui-0.6.0/chatgpt_tui.egg-info/top_level.txt
--rw-r--r--   0 jiayipan   (501) staff       (20)       38 2023-03-29 00:57:00.895318 chatgpt_tui-0.6.0/setup.cfg
--rw-r--r--   0 jiayipan   (501) staff       (20)      844 2023-03-29 00:55:26.000000 chatgpt_tui-0.6.0/setup.py
+drwxr-xr-x   0 jiayipan   (501) staff       (20)        0 2023-07-25 08:46:35.387774 chatgpt_tui-0.7.0/
+-rw-r--r--   0 jiayipan   (501) staff       (20)     1067 2023-07-25 08:30:46.000000 chatgpt_tui-0.7.0/LICENSE
+-rw-r--r--   0 jiayipan   (501) staff       (20)     1434 2023-07-25 08:46:35.387642 chatgpt_tui-0.7.0/PKG-INFO
+-rw-r--r--   0 jiayipan   (501) staff       (20)      962 2023-07-25 08:30:46.000000 chatgpt_tui-0.7.0/README.md
+drwxr-xr-x   0 jiayipan   (501) staff       (20)        0 2023-07-25 08:46:35.386710 chatgpt_tui-0.7.0/chatgpt_tui/
+-rw-r--r--   0 jiayipan   (501) staff       (20)        0 2023-07-25 08:30:46.000000 chatgpt_tui-0.7.0/chatgpt_tui/__init__.py
+-rw-r--r--   0 jiayipan   (501) staff       (20)     2639 2023-07-25 08:30:46.000000 chatgpt_tui-0.7.0/chatgpt_tui/app.py
+-rw-r--r--   0 jiayipan   (501) staff       (20)      954 2023-07-25 08:30:46.000000 chatgpt_tui-0.7.0/chatgpt_tui/chat_api.py
+-rw-r--r--   0 jiayipan   (501) staff       (20)      938 2023-07-25 08:30:46.000000 chatgpt_tui-0.7.0/chatgpt_tui/structures.py
+-rw-r--r--   0 jiayipan   (501) staff       (20)     1554 2023-07-25 08:30:46.000000 chatgpt_tui-0.7.0/chatgpt_tui/style.css
+-rw-r--r--   0 jiayipan   (501) staff       (20)     2260 2023-07-25 08:30:46.000000 chatgpt_tui-0.7.0/chatgpt_tui/widgets.py
+drwxr-xr-x   0 jiayipan   (501) staff       (20)        0 2023-07-25 08:46:35.387482 chatgpt_tui-0.7.0/chatgpt_tui.egg-info/
+-rw-r--r--   0 jiayipan   (501) staff       (20)     1434 2023-07-25 08:46:35.000000 chatgpt_tui-0.7.0/chatgpt_tui.egg-info/PKG-INFO
+-rw-r--r--   0 jiayipan   (501) staff       (20)      376 2023-07-25 08:46:35.000000 chatgpt_tui-0.7.0/chatgpt_tui.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayipan   (501) staff       (20)        1 2023-07-25 08:46:35.000000 chatgpt_tui-0.7.0/chatgpt_tui.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayipan   (501) staff       (20)       46 2023-07-25 08:46:35.000000 chatgpt_tui-0.7.0/chatgpt_tui.egg-info/entry_points.txt
+-rw-r--r--   0 jiayipan   (501) staff       (20)       30 2023-07-25 08:46:35.000000 chatgpt_tui-0.7.0/chatgpt_tui.egg-info/requires.txt
+-rw-r--r--   0 jiayipan   (501) staff       (20)       12 2023-07-25 08:46:35.000000 chatgpt_tui-0.7.0/chatgpt_tui.egg-info/top_level.txt
+-rw-r--r--   0 jiayipan   (501) staff       (20)       38 2023-07-25 08:46:35.387811 chatgpt_tui-0.7.0/setup.cfg
+-rw-r--r--   0 jiayipan   (501) staff       (20)      850 2023-07-25 08:45:29.000000 chatgpt_tui-0.7.0/setup.py
```

### Comparing `chatgpt_tui-0.6.0/LICENSE` & `chatgpt_tui-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_tui-0.6.0/PKG-INFO` & `chatgpt_tui-0.7.0/chatgpt_tui.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: chatgpt_tui
-Version: 0.6.0
+Name: chatgpt-tui
+Version: 0.7.0
 Summary: A simple TUI interface for ChatGPT.
 Home-page: https://github.com/Jiayi-Pan/ChatGPT_TUI
 Author: Jiayi Pan
 Author-email: i@jiayipan.me
 Keywords: chatbot,tui,chatgpt,chatgpt_tui
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 `catui` is a Python-based Text User Interface (TUI) for ChatGPT, powered by OpenAI's official API. It provides an easy-to-use interface that allows you to interact with ChatGPT directly from your terminal.
 
 ## Usage
 
 ### Install
 
 ```bash
-pip install chatgpt_tui
+pip install -U chatgpt_tui
 ```
 
 ### Export your OpenAI API key
 
 Before using it, you need to export your [OpenAI API key](https://platform.openai.com/account/api-keys) as an environment variable:
 
 ```bash
```

### Comparing `chatgpt_tui-0.6.0/README.md` & `chatgpt_tui-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 `catui` is a Python-based Text User Interface (TUI) for ChatGPT, powered by OpenAI's official API. It provides an easy-to-use interface that allows you to interact with ChatGPT directly from your terminal.
 
 ## Usage
 
 ### Install
 
 ```bash
-pip install chatgpt_tui
+pip install -U chatgpt_tui
 ```
 
 ### Export your OpenAI API key
 
 Before using it, you need to export your [OpenAI API key](https://platform.openai.com/account/api-keys) as an environment variable:
 
 ```bash
```

### Comparing `chatgpt_tui-0.6.0/chatgpt_tui/app.py` & `chatgpt_tui-0.7.0/chatgpt_tui/app.py`

 * *Files identical despite different names*

### Comparing `chatgpt_tui-0.6.0/chatgpt_tui/chat_api.py` & `chatgpt_tui-0.7.0/chatgpt_tui/chat_api.py`

 * *Files identical despite different names*

### Comparing `chatgpt_tui-0.6.0/chatgpt_tui/structures.py` & `chatgpt_tui-0.7.0/chatgpt_tui/structures.py`

 * *Files identical despite different names*

### Comparing `chatgpt_tui-0.6.0/chatgpt_tui/style.css` & `chatgpt_tui-0.7.0/chatgpt_tui/style.css`

 * *Files identical despite different names*

### Comparing `chatgpt_tui-0.6.0/chatgpt_tui/widgets.py` & `chatgpt_tui-0.7.0/chatgpt_tui/widgets.py`

 * *Files identical despite different names*

### Comparing `chatgpt_tui-0.6.0/chatgpt_tui.egg-info/PKG-INFO` & `chatgpt_tui-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: chatgpt-tui
-Version: 0.6.0
+Name: chatgpt_tui
+Version: 0.7.0
 Summary: A simple TUI interface for ChatGPT.
 Home-page: https://github.com/Jiayi-Pan/ChatGPT_TUI
 Author: Jiayi Pan
 Author-email: i@jiayipan.me
 Keywords: chatbot,tui,chatgpt,chatgpt_tui
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 `catui` is a Python-based Text User Interface (TUI) for ChatGPT, powered by OpenAI's official API. It provides an easy-to-use interface that allows you to interact with ChatGPT directly from your terminal.
 
 ## Usage
 
 ### Install
 
 ```bash
-pip install chatgpt_tui
+pip install -U chatgpt_tui
 ```
 
 ### Export your OpenAI API key
 
 Before using it, you need to export your [OpenAI API key](https://platform.openai.com/account/api-keys) as an environment variable:
 
 ```bash
```

### Comparing `chatgpt_tui-0.6.0/setup.py` & `chatgpt_tui-0.7.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chatgpt_tui",
-    version="0.6.0",
+    version="0.7.0",
     author="Jiayi Pan",
     author_email="i@jiayipan.me",
     description="A simple TUI interface for ChatGPT.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Jiayi-Pan/ChatGPT_TUI",
     python_requires=">=3.7",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords=["chatbot", "tui", "chatgpt", "chatgpt_tui"],
     packages=find_packages(),
-    install_requires=["textual", "httpx", "pyperclip"],
+    install_requires=["textual==0.13", "httpx", "pyperclip"],
     entry_points={
         "console_scripts": [
             "catui = chatgpt_tui.app:run"
         ]
     },
     package_data={'': ['*.css']}
 )
```

