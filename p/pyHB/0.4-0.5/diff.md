# Comparing `tmp/pyHB-0.4.tar.gz` & `tmp/pyHB-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyHB-0.4.tar", last modified: Tue Jul  4 05:35:17 2023, max compression
+gzip compressed data, was "pyHB-0.5.tar", last modified: Tue Jul 25 14:18:17 2023, max compression
```

## Comparing `pyHB-0.4.tar` & `pyHB-0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:17.605628 pyHB-0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:17.605628 pyHB-0.4/HB/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 05:35:06.000000 pyHB-0.4/HB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-04 05:35:06.000000 pyHB-0.4/HB/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-07-04 05:35:06.000000 pyHB-0.4/HB/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-04 05:35:06.000000 pyHB-0.4/HB/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 05:35:06.000000 pyHB-0.4/HB/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 05:35:06.000000 pyHB-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-04 05:35:17.605628 pyHB-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 05:35:06.000000 pyHB-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:35:17.605628 pyHB-0.4/pyHB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-04 05:35:17.000000 pyHB-0.4/pyHB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 05:35:17.000000 pyHB-0.4/pyHB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 05:35:17.000000 pyHB-0.4/pyHB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 05:35:17.000000 pyHB-0.4/pyHB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-04 05:35:17.000000 pyHB-0.4/pyHB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 05:35:17.609628 pyHB-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-04 05:35:06.000000 pyHB-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:18:17.673651 pyHB-0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:18:17.673651 pyHB-0.5/HB/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-25 14:17:45.000000 pyHB-0.5/HB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-25 14:17:45.000000 pyHB-0.5/HB/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25513 2023-07-25 14:17:45.000000 pyHB-0.5/HB/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-25 14:17:45.000000 pyHB-0.5/HB/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 14:17:45.000000 pyHB-0.5/HB/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 14:17:45.000000 pyHB-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-25 14:18:17.673651 pyHB-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-25 14:17:45.000000 pyHB-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:18:17.673651 pyHB-0.5/pyHB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-25 14:18:17.000000 pyHB-0.5/pyHB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-25 14:18:17.000000 pyHB-0.5/pyHB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:18:17.000000 pyHB-0.5/pyHB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 14:18:17.000000 pyHB-0.5/pyHB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-25 14:18:17.000000 pyHB-0.5/pyHB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:18:17.673651 pyHB-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-25 14:17:45.000000 pyHB-0.5/setup.py
```

### Comparing `pyHB-0.4/HB/startup.py` & `pyHB-0.5/HB/startup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
-import time
 import sys
+import time
+
+
 def bot_start():
     os.system("clear")
     ask = input("Do You Want to Start HackBot y/n: ")
     if ask.lower() == "y":
         os.system("python3 -m HackBot")
     elif ask.lower() == "n":
         print("\nOk! You Can Start It Later With by using; python3-m HackBot\n")
```

### Comparing `pyHB-0.4/LICENSE` & `pyHB-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyHB-0.4/PKG-INFO` & `pyHB-0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyHB
-Version: 0.4
+Version: 0.5
 Summary: This is a simple package which is used in HackBot Support Pyrogram + Telethon
 Home-page: https://github.com/LEGEND-AI/pyHB
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyHB,HB
 Classifier: Framework :: AsyncIO
```

### Comparing `pyHB-0.4/pyHB.egg-info/PKG-INFO` & `pyHB-0.5/pyHB.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyHB
-Version: 0.4
+Version: 0.5
 Summary: This is a simple package which is used in HackBot Support Pyrogram + Telethon
 Home-page: https://github.com/LEGEND-AI/pyHB
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyHB,HB
 Classifier: Framework :: AsyncIO
```

### Comparing `pyHB-0.4/setup.py` & `pyHB-0.5/setup.py`

 * *Files identical despite different names*

