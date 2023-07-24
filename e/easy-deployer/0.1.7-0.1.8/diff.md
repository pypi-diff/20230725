# Comparing `tmp/easy_deployer-0.1.7.tar.gz` & `tmp/easy_deployer-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_deployer-0.1.7.tar", last modified: Mon Jul 24 21:47:27 2023, max compression
+gzip compressed data, was "easy_deployer-0.1.8.tar", last modified: Mon Jul 24 22:08:21 2023, max compression
```

## Comparing `easy_deployer-0.1.7.tar` & `easy_deployer-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 21:47:27.323394 easy_deployer-0.1.7/
--rw-rw-rw-   0        0        0     1086 2021-07-27 13:30:42.000000 easy_deployer-0.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0     1393 2023-07-24 21:47:27.322396 easy_deployer-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      650 2023-07-24 20:24:38.000000 easy_deployer-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 21:47:27.308434 easy_deployer-0.1.7/easy_deployer/
--rw-rw-rw-   0        0        0       90 2023-07-24 20:57:36.000000 easy_deployer-0.1.7/easy_deployer/__init__.py
--rw-rw-rw-   0        0        0    26588 2023-07-24 15:55:57.000000 easy_deployer-0.1.7/easy_deployer/github.py
--rw-rw-rw-   0        0        0    11211 2023-07-23 15:15:38.000000 easy_deployer-0.1.7/easy_deployer/heroku.py
--rw-rw-rw-   0        0        0     9304 2023-07-24 19:12:32.000000 easy_deployer-0.1.7/easy_deployer/main.py
--rw-rw-rw-   0        0        0    12360 2023-07-23 15:28:41.000000 easy_deployer-0.1.7/easy_deployer/shared_functions.py
-drwxrwxrwx   0        0        0        0 2023-07-24 21:47:27.320403 easy_deployer-0.1.7/easy_deployer.egg-info/
--rw-rw-rw-   0        0        0     1393 2023-07-24 21:47:27.000000 easy_deployer-0.1.7/easy_deployer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-07-24 21:47:27.000000 easy_deployer-0.1.7/easy_deployer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 21:47:27.000000 easy_deployer-0.1.7/easy_deployer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      156 2023-07-24 21:47:27.000000 easy_deployer-0.1.7/easy_deployer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-07-24 21:47:27.000000 easy_deployer-0.1.7/easy_deployer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 21:47:27.323394 easy_deployer-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1538 2023-07-24 20:57:32.000000 easy_deployer-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 22:08:21.300916 easy_deployer-0.1.8/
+-rw-rw-rw-   0        0        0     1086 2021-07-27 13:30:42.000000 easy_deployer-0.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     1393 2023-07-24 22:08:21.298985 easy_deployer-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      650 2023-07-24 20:24:38.000000 easy_deployer-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 22:08:21.280035 easy_deployer-0.1.8/easy_deployer/
+-rw-rw-rw-   0        0        0       90 2023-07-24 22:04:37.000000 easy_deployer-0.1.8/easy_deployer/__init__.py
+-rw-rw-rw-   0        0        0    26589 2023-07-24 22:08:07.000000 easy_deployer-0.1.8/easy_deployer/github.py
+-rw-rw-rw-   0        0        0    11212 2023-07-24 22:08:07.000000 easy_deployer-0.1.8/easy_deployer/heroku.py
+-rw-rw-rw-   0        0        0     9305 2023-07-24 22:08:08.000000 easy_deployer-0.1.8/easy_deployer/main.py
+-rw-rw-rw-   0        0        0    12360 2023-07-24 22:08:08.000000 easy_deployer-0.1.8/easy_deployer/shared_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-24 22:08:21.297989 easy_deployer-0.1.8/easy_deployer.egg-info/
+-rw-rw-rw-   0        0        0     1393 2023-07-24 22:08:21.000000 easy_deployer-0.1.8/easy_deployer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-07-24 22:08:21.000000 easy_deployer-0.1.8/easy_deployer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 22:08:21.000000 easy_deployer-0.1.8/easy_deployer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      156 2023-07-24 22:08:21.000000 easy_deployer-0.1.8/easy_deployer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-24 22:08:21.000000 easy_deployer-0.1.8/easy_deployer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 22:08:21.300916 easy_deployer-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1538 2023-07-24 22:04:42.000000 easy_deployer-0.1.8/setup.py
```

### Comparing `easy_deployer-0.1.7/LICENSE.txt` & `easy_deployer-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easy_deployer-0.1.7/PKG-INFO` & `easy_deployer-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_deployer
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package to simplify and quickly deploy your project/app/folders to the supported platforms.
 Home-page: https://github.com/medamine980/easy-deployer
 Author: Mohamed-Amine Benali
 Author-email: benali.medamine2002@gmail.com
 License: MIT
 Keywords: python,github,github-deployer,heroku,heroku-deployer,deploy,easy,easy-deployer,simple,simple-deployer
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `easy_deployer-0.1.7/README.md` & `easy_deployer-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `easy_deployer-0.1.7/easy_deployer/github.py` & `easy_deployer-0.1.8/easy_deployer/github.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding=<utf-8>
 from subprocess import Popen, PIPE, DEVNULL
 from argparse import ArgumentParser
 import os, sys, json, getpass, re, time, itertools, threading, signal, webbrowser, keyboard
 
-from shared_functions import printWarning, listPromptInquirer, promptPyInquirer, runCmd, getOS, openBash, defaultCommit
+from .shared_functions import printWarning, listPromptInquirer, promptPyInquirer, runCmd, getOS, openBash, defaultCommit
 
 def main():
     args = takeArgs() # Take the arguments
     if not os.path.exists(args["path"]):
         print("Invalid Path!")
         sys.exit(5)
     args["path"] = os.path.abspath(args["path"])
```

### Comparing `easy_deployer-0.1.7/easy_deployer/heroku.py` & `easy_deployer-0.1.8/easy_deployer/heroku.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os, sys, keyboard, json, re
 from subprocess import Popen, PIPE, run, DEVNULL
 from argparse import ArgumentParser
 
-from shared_functions import Loading, runCmd, promptPyInquirer, defaultCommit
+from .shared_functions import Loading, runCmd, promptPyInquirer, defaultCommit
 
 def main():
     args = takeArgs()
     checkSoftware("git", "git --help")
     checkSoftware("heroku", "heroku --help", "https://devcenter.heroku.com/articles/heroku-cli#download-and-install")
     args["path"] = os.path.abspath(args["path"])
     os.chdir(args["path"]) #changing to path
```

### Comparing `easy_deployer-0.1.7/easy_deployer/main.py` & `easy_deployer-0.1.8/easy_deployer/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from asyncio.subprocess import PIPE
-from shared_functions import listPromptInquirer, checkBoxPromptInquirer, runCmd, invalidAnswerExit, promptPyInquirer
+from .shared_functions import listPromptInquirer, checkBoxPromptInquirer, runCmd, invalidAnswerExit, promptPyInquirer
 from argparse import ArgumentParser
 import os, sys
 import re
 
 deploy_to_choices = ["github"]
 command_choices = ["create-update", "update", "delete"]
```

### Comparing `easy_deployer-0.1.7/easy_deployer/shared_functions.py` & `easy_deployer-0.1.8/easy_deployer/shared_functions.py`

 * *Files identical despite different names*

### Comparing `easy_deployer-0.1.7/easy_deployer.egg-info/PKG-INFO` & `easy_deployer-0.1.8/easy_deployer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-deployer
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package to simplify and quickly deploy your project/app/folders to the supported platforms.
 Home-page: https://github.com/medamine980/easy-deployer
 Author: Mohamed-Amine Benali
 Author-email: benali.medamine2002@gmail.com
 License: MIT
 Keywords: python,github,github-deployer,heroku,heroku-deployer,deploy,easy,easy-deployer,simple,simple-deployer
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `easy_deployer-0.1.7/setup.py` & `easy_deployer-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_desc = f.read()
 setup(
     name="easy_deployer",
-    version="0.1.7",
+    version="0.1.8",
     description="A package to simplify and quickly deploy your project/app/folders to the supported platforms.",
     long_description=long_desc,
     long_description_content_type='text/markdown',
     author="Mohamed-Amine Benali",
     author_email="benali.medamine2002@gmail.com",
     url="https://github.com/medamine980/easy-deployer",
     packages=find_packages(exclude=["easy_deployer.dist", "easy_deployer.ignore"]),
```

