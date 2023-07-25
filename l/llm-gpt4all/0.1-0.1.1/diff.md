# Comparing `tmp/llm-gpt4all-0.1.tar.gz` & `tmp/llm-gpt4all-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-gpt4all-0.1.tar", last modified: Wed Jul 12 14:38:50 2023, max compression
+gzip compressed data, was "llm-gpt4all-0.1.1.tar", last modified: Tue Jul 25 21:29:45 2023, max compression
```

## Comparing `llm-gpt4all-0.1.tar` & `llm-gpt4all-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:38:50.552926 llm-gpt4all-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 14:38:36.000000 llm-gpt4all-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-12 14:38:50.552926 llm-gpt4all-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-12 14:38:36.000000 llm-gpt4all-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:38:50.552926 llm-gpt4all-0.1/llm_gpt4all.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-12 14:38:50.000000 llm-gpt4all-0.1/llm_gpt4all.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-12 14:38:50.000000 llm-gpt4all-0.1/llm_gpt4all.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:38:50.000000 llm-gpt4all-0.1/llm_gpt4all.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 14:38:50.000000 llm-gpt4all-0.1/llm_gpt4all.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:38:50.000000 llm-gpt4all-0.1/llm_gpt4all.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 14:38:50.000000 llm-gpt4all-0.1/llm_gpt4all.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-07-12 14:38:36.000000 llm-gpt4all-0.1/llm_gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:38:50.552926 llm-gpt4all-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-12 14:38:36.000000 llm-gpt4all-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:38:50.552926 llm-gpt4all-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-12 14:38:36.000000 llm-gpt4all-0.1/tests/test_llm_gpt4all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:29:45.026077 llm-gpt4all-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 21:29:26.000000 llm-gpt4all-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-25 21:29:45.026077 llm-gpt4all-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-25 21:29:26.000000 llm-gpt4all-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:29:45.026077 llm-gpt4all-0.1.1/llm_gpt4all.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-25 21:29:45.000000 llm-gpt4all-0.1.1/llm_gpt4all.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-25 21:29:45.000000 llm-gpt4all-0.1.1/llm_gpt4all.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:29:45.000000 llm-gpt4all-0.1.1/llm_gpt4all.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 21:29:45.000000 llm-gpt4all-0.1.1/llm_gpt4all.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:29:45.000000 llm-gpt4all-0.1.1/llm_gpt4all.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 21:29:45.000000 llm-gpt4all-0.1.1/llm_gpt4all.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-25 21:29:26.000000 llm-gpt4all-0.1.1/llm_gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:29:45.026077 llm-gpt4all-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-25 21:29:26.000000 llm-gpt4all-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:29:45.026077 llm-gpt4all-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-25 21:29:26.000000 llm-gpt4all-0.1.1/tests/test_llm_gpt4all.py
```

### Comparing `llm-gpt4all-0.1/LICENSE` & `llm-gpt4all-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-gpt4all-0.1/PKG-INFO` & `llm-gpt4all-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-gpt4all
-Version: 0.1
+Version: 0.1.1
 Summary: Plugin for LLM adding support for GPT4ALL models
 Home-page: https://github.com/simonw/llm-gpt4all
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/llm-gpt4all/issues
 Project-URL: CI, https://github.com/simonw/llm-gpt4all/actions
 Project-URL: Changelog, https://github.com/simonw/llm-gpt4all/releases
```

### Comparing `llm-gpt4all-0.1/README.md` & `llm-gpt4all-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `llm-gpt4all-0.1/llm_gpt4all.egg-info/PKG-INFO` & `llm-gpt4all-0.1.1/llm_gpt4all.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-gpt4all
-Version: 0.1
+Version: 0.1.1
 Summary: Plugin for LLM adding support for GPT4ALL models
 Home-page: https://github.com/simonw/llm-gpt4all
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/llm-gpt4all/issues
 Project-URL: CI, https://github.com/simonw/llm-gpt4all/actions
 Project-URL: Changelog, https://github.com/simonw/llm-gpt4all/releases
```

### Comparing `llm-gpt4all-0.1/llm_gpt4all.py` & `llm-gpt4all-0.1.1/llm_gpt4all.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from gpt4all import GPT4All as _GPT4All
 from pathlib import Path
 from typing import Optional
 import httpx
+import urllib3
 import json
 import llm
 import os
 import sys
 import time
 from typing import List, Optional, Tuple
 
@@ -162,15 +163,15 @@
         response.raise_for_status()  # This will raise an HTTPError if the request fails
 
         # If successful, write to the file
         with open(path, "w") as file:
             json.dump(response.json(), file)
 
         return response.json()
-    except httpx.HTTPError:
+    except (httpx.HTTPError, urllib3.exceptions.NameResolutionError):
         # If there's an existing file, load it
         if path.is_file():
             with open(path, "r") as file:
                 return json.load(file)
         else:
             # If not, raise an error
             raise DownloadError(
```

### Comparing `llm-gpt4all-0.1/setup.py` & `llm-gpt4all-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.1"
+VERSION = "0.1.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `llm-gpt4all-0.1/tests/test_llm_gpt4all.py` & `llm-gpt4all-0.1.1/tests/test_llm_gpt4all.py`

 * *Files identical despite different names*

