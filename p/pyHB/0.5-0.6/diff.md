# Comparing `tmp/pyHB-0.5.tar.gz` & `tmp/pyHB-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyHB-0.5.tar", last modified: Tue Jul 25 14:18:17 2023, max compression
+gzip compressed data, was "pyHB-0.6.tar", last modified: Tue Jul 25 14:26:23 2023, max compression
```

## Comparing `pyHB-0.5.tar` & `pyHB-0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:18:17.673651 pyHB-0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:18:17.673651 pyHB-0.5/HB/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-25 14:17:45.000000 pyHB-0.5/HB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-25 14:17:45.000000 pyHB-0.5/HB/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    25513 2023-07-25 14:17:45.000000 pyHB-0.5/HB/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-25 14:17:45.000000 pyHB-0.5/HB/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 14:17:45.000000 pyHB-0.5/HB/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 14:17:45.000000 pyHB-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-25 14:18:17.673651 pyHB-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-25 14:17:45.000000 pyHB-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:18:17.673651 pyHB-0.5/pyHB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-25 14:18:17.000000 pyHB-0.5/pyHB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-25 14:18:17.000000 pyHB-0.5/pyHB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:18:17.000000 pyHB-0.5/pyHB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 14:18:17.000000 pyHB-0.5/pyHB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-25 14:18:17.000000 pyHB-0.5/pyHB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:18:17.673651 pyHB-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-25 14:17:45.000000 pyHB-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:26:23.832347 pyHB-0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:26:23.828347 pyHB-0.6/HB/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-25 14:26:10.000000 pyHB-0.6/HB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-25 14:26:10.000000 pyHB-0.6/HB/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25513 2023-07-25 14:26:10.000000 pyHB-0.6/HB/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-25 14:26:10.000000 pyHB-0.6/HB/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 14:26:10.000000 pyHB-0.6/HB/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 14:26:10.000000 pyHB-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-25 14:26:23.832347 pyHB-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-25 14:26:10.000000 pyHB-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:26:23.832347 pyHB-0.6/pyHB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-25 14:26:23.000000 pyHB-0.6/pyHB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-25 14:26:23.000000 pyHB-0.6/pyHB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:26:23.000000 pyHB-0.6/pyHB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 14:26:23.000000 pyHB-0.6/pyHB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-25 14:26:23.000000 pyHB-0.6/pyHB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:26:23.832347 pyHB-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-25 14:26:10.000000 pyHB-0.6/setup.py
```

### Comparing `pyHB-0.5/HB/data.py` & `pyHB-0.6/HB/data.py`

 * *Files identical despite different names*

### Comparing `pyHB-0.5/HB/functions.py` & `pyHB-0.6/HB/functions.py`

 * *Files identical despite different names*

### Comparing `pyHB-0.5/HB/startup.py` & `pyHB-0.6/HB/startup.py`

 * *Files identical despite different names*

### Comparing `pyHB-0.5/LICENSE` & `pyHB-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyHB-0.5/PKG-INFO` & `pyHB-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyHB
-Version: 0.5
+Version: 0.6
 Summary: This is a simple package which is used in HackBot Support Pyrogram + Telethon
 Home-page: https://github.com/LEGEND-AI/pyHB
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyHB,HB
 Classifier: Framework :: AsyncIO
```

### Comparing `pyHB-0.5/pyHB.egg-info/PKG-INFO` & `pyHB-0.6/pyHB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyHB
-Version: 0.5
+Version: 0.6
 Summary: This is a simple package which is used in HackBot Support Pyrogram + Telethon
 Home-page: https://github.com/LEGEND-AI/pyHB
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyHB,HB
 Classifier: Framework :: AsyncIO
```

### Comparing `pyHB-0.5/setup.py` & `pyHB-0.6/setup.py`

 * *Files identical despite different names*

