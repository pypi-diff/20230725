# Comparing `tmp/dart-tools-0.3.8.tar.gz` & `tmp/dart-tools-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dart-tools-0.3.8.tar", last modified: Fri Jun 30 05:49:36 2023, max compression
+gzip compressed data, was "dart-tools-0.3.9.tar", last modified: Tue Jul 25 19:10:09 2023, max compression
```

## Comparing `dart-tools-0.3.8.tar` & `dart-tools-0.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-30 05:49:36.599960 dart-tools-0.3.8/
--rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.8/LICENSE
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-30 05:49:36.599765 dart-tools-0.3.8/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.8/README.md
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-30 05:49:36.597704 dart-tools-0.3.8/dart/
--rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.8/dart/__init__.py
--rwxr-xr-x   0 zack       (501) staff       (20)    17371 2023-06-30 05:48:56.000000 dart-tools-0.3.8/dart/dart.py
--rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.8/dart/order_manager.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-30 05:49:36.599176 dart-tools-0.3.8/dart_tools.egg-info/
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-30 05:49:36.000000 dart-tools-0.3.8/dart_tools.egg-info/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)      339 2023-06-30 05:49:36.000000 dart-tools-0.3.8/dart_tools.egg-info/SOURCES.txt
--rw-r--r--   0 zack       (501) staff       (20)        1 2023-06-30 05:49:36.000000 dart-tools-0.3.8/dart_tools.egg-info/dependency_links.txt
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-30 05:49:36.599389 dart-tools-0.3.8/dart_tools.egg-info/dist/
--rw-r--r--   0 zack       (501) staff       (20)     8788 2023-06-03 08:11:34.000000 dart-tools-0.3.8/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz
--rw-r--r--   0 zack       (501) staff       (20)       34 2023-06-30 05:49:36.000000 dart-tools-0.3.8/dart_tools.egg-info/entry_points.txt
--rw-r--r--   0 zack       (501) staff       (20)       25 2023-06-30 05:49:36.000000 dart-tools-0.3.8/dart_tools.egg-info/requires.txt
--rw-r--r--   0 zack       (501) staff       (20)        5 2023-06-30 05:49:36.000000 dart-tools-0.3.8/dart_tools.egg-info/top_level.txt
--rw-r--r--   0 zack       (501) staff       (20)     1760 2023-06-30 05:49:12.000000 dart-tools-0.3.8/pyproject.toml
--rw-r--r--   0 zack       (501) staff       (20)       38 2023-06-30 05:49:36.600004 dart-tools-0.3.8/setup.cfg
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-07-25 19:10:09.120440 dart-tools-0.3.9/
+-rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.9/LICENSE
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-07-25 19:10:09.120190 dart-tools-0.3.9/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.9/README.md
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-07-25 19:10:09.118137 dart-tools-0.3.9/dart/
+-rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.9/dart/__init__.py
+-rwxr-xr-x   0 zack       (501) staff       (20)    17657 2023-07-25 19:08:57.000000 dart-tools-0.3.9/dart/dart.py
+-rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.9/dart/order_manager.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-07-25 19:10:09.119611 dart-tools-0.3.9/dart_tools.egg-info/
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-07-25 19:10:09.000000 dart-tools-0.3.9/dart_tools.egg-info/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)      339 2023-07-25 19:10:09.000000 dart-tools-0.3.9/dart_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 zack       (501) staff       (20)        1 2023-07-25 19:10:09.000000 dart-tools-0.3.9/dart_tools.egg-info/dependency_links.txt
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-07-25 19:10:09.119760 dart-tools-0.3.9/dart_tools.egg-info/dist/
+-rw-r--r--   0 zack       (501) staff       (20)     8788 2023-06-03 08:11:34.000000 dart-tools-0.3.9/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz
+-rw-r--r--   0 zack       (501) staff       (20)       34 2023-07-25 19:10:09.000000 dart-tools-0.3.9/dart_tools.egg-info/entry_points.txt
+-rw-r--r--   0 zack       (501) staff       (20)       25 2023-07-25 19:10:09.000000 dart-tools-0.3.9/dart_tools.egg-info/requires.txt
+-rw-r--r--   0 zack       (501) staff       (20)        5 2023-07-25 19:10:09.000000 dart-tools-0.3.9/dart_tools.egg-info/top_level.txt
+-rw-r--r--   0 zack       (501) staff       (20)     1760 2023-07-25 19:09:49.000000 dart-tools-0.3.9/pyproject.toml
+-rw-r--r--   0 zack       (501) staff       (20)       38 2023-07-25 19:10:09.120502 dart-tools-0.3.9/setup.cfg
```

### Comparing `dart-tools-0.3.8/LICENSE` & `dart-tools-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.8/PKG-INFO` & `dart-tools-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.3.8
+Version: 0.3.9
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.3.8 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.9 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.3.8/README.md` & `dart-tools-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.8/dart/dart.py` & `dart-tools-0.3.9/dart/dart.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """A CLI to interact with the Dart web app."""
 
 import argparse
+from functools import wraps
 import json
 import os
 import random
 import re
 import signal
 import string
 import subprocess
@@ -86,14 +87,25 @@
     return subprocess.check_output(cmd, shell=True).decode()
 
 
 def _get_task_url(host, duid):
     return f"{host}/search?t={duid}"
 
 
+def suppress_exception(fn):
+    @wraps(fn)
+    def wrapper(*args, **kwargs):
+        try:
+            return fn(*args, **kwargs)
+        except Exception:
+            pass
+
+    return wrapper
+
+
 def _exit_gracefully(_signal_received, _frame) -> None:
     sys.exit("Quitting.")
 
 
 class _Config:
     def __init__(self):
         self._content = {}
@@ -265,27 +277,29 @@
         sys.exit("Unknown failure, please email support@itsdart.com.")
 
 
 def print_version():
     print(f"dart-tools version {_VERSION}")
 
 
+@suppress_exception
 def print_version_update_message_maybe():
     latest = (
-        _run_cmd("pip index versions dart-tools 2>&1")
+        _run_cmd("pip --disable-pip-version-check index versions dart-tools 2>&1")
         .rsplit("LATEST:", maxsplit=1)[-1]
+        .split("\n", maxsplit=1)[0]
         .strip()
     )
     if latest == _VERSION or [int(e) for e in latest.split(".")] <= [
         int(e) for e in _VERSION.split(".")
     ]:
         return
 
     print(
-        f"A new version of dart-tools is available. To upgrade from {_VERSION} to {latest}, run\n\n\tpip install --upgrade dart-tools\n"
+        f"A new version of dart-tools is available. Upgrade from {_VERSION} to {latest} with\n\n  pip install --upgrade dart-tools\n"
     )
 
 
 def login():
     config = _Config()
     session = _Session(config)
 
@@ -323,15 +337,15 @@
     response = session.post(_COPY_BRANCH_URL_FRAG, json={"duid": task["duid"]})
     _check_response_and_maybe_exit(response)
 
     branch_name = _Git.make_task_name(user_email, task)
     _Git.checkout_branch(branch_name)
 
     print(
-        f"Started work on {task['title']} at {_get_task_url(config.host, task['duid'])} on branch {branch_name}"
+        f"Started work on\n\n  {task['title']}\n  {_get_task_url(config.host, task['duid'])}\n"
     )
 
 
 def begin_task():
     config = _Config()
     session = _Session(config)
```

### Comparing `dart-tools-0.3.8/dart/order_manager.py` & `dart-tools-0.3.9/dart/order_manager.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.8/dart_tools.egg-info/PKG-INFO` & `dart-tools-0.3.9/dart_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.3.8
+Version: 0.3.9
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.3.8 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.9 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.3.8/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz` & `dart-tools-0.3.9/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.8/pyproject.toml` & `dart-tools-0.3.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dart-tools"
-version = "0.3.8"
+version = "0.3.9"
 description = "The Dart CLI and Python Library"
 readme = "README.md"
 requires-python = ">=3.8"
 
 license = {file = "LICENSE"}
 keywords = ["dart", "cli", "projectmanagement", "taskmanagement"]
 authors = [
```

