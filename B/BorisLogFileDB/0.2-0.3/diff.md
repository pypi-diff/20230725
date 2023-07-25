# Comparing `tmp/BorisLogFileDB-0.2.tar.gz` & `tmp/BorisLogFileDB-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BorisLogFileDB-0.2.tar", last modified: Tue Jul 25 08:24:22 2023, max compression
+gzip compressed data, was "dist/BorisLogFileDB-0.3.tar", last modified: Tue Jul 25 08:36:44 2023, max compression
```

## Comparing `BorisLogFileDB-0.2.tar` & `BorisLogFileDB-0.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 boris     (1000) dashu     (1000)        0 2023-07-25 08:24:22.000000 BorisLogFileDB-0.2/
-drwxr-xr-x   0 boris     (1000) dashu     (1000)        0 2023-07-25 08:24:22.000000 BorisLogFileDB-0.2/BorisLogFileDB/
--rw-r--r--   0 boris     (1000) dashu     (1000)        0 2023-07-25 03:44:21.000000 BorisLogFileDB-0.2/BorisLogFileDB/__init__.py
--rw-r--r--   0 boris     (1000) dashu     (1000)     3201 2023-07-25 03:43:13.000000 BorisLogFileDB-0.2/BorisLogFileDB/file_process.py
--rw-r--r--   0 boris     (1000) dashu     (1000)     2992 2023-07-25 03:43:13.000000 BorisLogFileDB-0.2/BorisLogFileDB/folder_file_process.py
--rw-r--r--   0 boris     (1000) dashu     (1000)      680 2023-07-25 03:43:13.000000 BorisLogFileDB-0.2/BorisLogFileDB/folder_process.py
--rw-r--r--   0 boris     (1000) dashu     (1000)     1881 2023-07-25 03:43:13.000000 BorisLogFileDB-0.2/BorisLogFileDB/log_process.py
--rw-r--r--   0 boris     (1000) dashu     (1000)     2077 2023-07-25 03:43:13.000000 BorisLogFileDB-0.2/BorisLogFileDB/logger.py
--rw-r--r--   0 boris     (1000) dashu     (1000)     2084 2023-07-25 08:23:29.000000 BorisLogFileDB-0.2/BorisLogFileDB/logger2.py
--rw-r--r--   0 boris     (1000) dashu     (1000)     7767 2023-07-25 03:43:13.000000 BorisLogFileDB-0.2/BorisLogFileDB/mysql_connect.py
-drwxr-xr-x   0 boris     (1000) dashu     (1000)        0 2023-07-25 08:24:22.000000 BorisLogFileDB-0.2/BorisLogFileDB.egg-info/
--rw-r--r--   0 boris     (1000) dashu     (1000)      428 2023-07-25 08:24:22.000000 BorisLogFileDB-0.2/BorisLogFileDB.egg-info/PKG-INFO
--rw-r--r--   0 boris     (1000) dashu     (1000)      402 2023-07-25 08:24:22.000000 BorisLogFileDB-0.2/BorisLogFileDB.egg-info/SOURCES.txt
--rw-r--r--   0 boris     (1000) dashu     (1000)        1 2023-07-25 08:24:22.000000 BorisLogFileDB-0.2/BorisLogFileDB.egg-info/dependency_links.txt
--rw-r--r--   0 boris     (1000) dashu     (1000)       15 2023-07-25 08:24:22.000000 BorisLogFileDB-0.2/BorisLogFileDB.egg-info/top_level.txt
--rw-r--r--   0 boris     (1000) dashu     (1000)      428 2023-07-25 08:24:22.000000 BorisLogFileDB-0.2/PKG-INFO
--rw-r--r--   0 boris     (1000) dashu     (1000)       38 2023-07-25 08:24:22.000000 BorisLogFileDB-0.2/setup.cfg
--rw-r--r--   0 boris     (1000) dashu     (1000)      488 2023-07-25 08:24:14.000000 BorisLogFileDB-0.2/setup.py
+drwxr-xr-x   0 boris     (1000) dashu     (1000)        0 2023-07-25 08:36:44.000000 BorisLogFileDB-0.3/
+drwxr-xr-x   0 boris     (1000) dashu     (1000)        0 2023-07-25 08:36:44.000000 BorisLogFileDB-0.3/BorisLogFileDB/
+-rw-r--r--   0 boris     (1000) dashu     (1000)        0 2023-07-25 03:44:21.000000 BorisLogFileDB-0.3/BorisLogFileDB/__init__.py
+-rw-r--r--   0 boris     (1000) dashu     (1000)     3201 2023-07-25 03:43:13.000000 BorisLogFileDB-0.3/BorisLogFileDB/file_process.py
+-rw-r--r--   0 boris     (1000) dashu     (1000)     2992 2023-07-25 03:43:13.000000 BorisLogFileDB-0.3/BorisLogFileDB/folder_file_process.py
+-rw-r--r--   0 boris     (1000) dashu     (1000)      680 2023-07-25 03:43:13.000000 BorisLogFileDB-0.3/BorisLogFileDB/folder_process.py
+-rw-r--r--   0 boris     (1000) dashu     (1000)     1888 2023-07-25 08:34:07.000000 BorisLogFileDB-0.3/BorisLogFileDB/log_process.py
+-rw-r--r--   0 boris     (1000) dashu     (1000)     2084 2023-07-25 08:23:29.000000 BorisLogFileDB-0.3/BorisLogFileDB/logger.py
+-rw-r--r--   0 boris     (1000) dashu     (1000)     7767 2023-07-25 03:43:13.000000 BorisLogFileDB-0.3/BorisLogFileDB/mysql_connect.py
+drwxr-xr-x   0 boris     (1000) dashu     (1000)        0 2023-07-25 08:36:44.000000 BorisLogFileDB-0.3/BorisLogFileDB.egg-info/
+-rw-r--r--   0 boris     (1000) dashu     (1000)      428 2023-07-25 08:36:44.000000 BorisLogFileDB-0.3/BorisLogFileDB.egg-info/PKG-INFO
+-rw-r--r--   0 boris     (1000) dashu     (1000)      376 2023-07-25 08:36:44.000000 BorisLogFileDB-0.3/BorisLogFileDB.egg-info/SOURCES.txt
+-rw-r--r--   0 boris     (1000) dashu     (1000)        1 2023-07-25 08:36:44.000000 BorisLogFileDB-0.3/BorisLogFileDB.egg-info/dependency_links.txt
+-rw-r--r--   0 boris     (1000) dashu     (1000)       15 2023-07-25 08:36:44.000000 BorisLogFileDB-0.3/BorisLogFileDB.egg-info/top_level.txt
+-rw-r--r--   0 boris     (1000) dashu     (1000)      428 2023-07-25 08:36:44.000000 BorisLogFileDB-0.3/PKG-INFO
+-rw-r--r--   0 boris     (1000) dashu     (1000)       38 2023-07-25 08:36:44.000000 BorisLogFileDB-0.3/setup.cfg
+-rw-r--r--   0 boris     (1000) dashu     (1000)      488 2023-07-25 08:36:33.000000 BorisLogFileDB-0.3/setup.py
```

### Comparing `BorisLogFileDB-0.2/BorisLogFileDB/file_process.py` & `BorisLogFileDB-0.3/BorisLogFileDB/file_process.py`

 * *Files identical despite different names*

### Comparing `BorisLogFileDB-0.2/BorisLogFileDB/folder_file_process.py` & `BorisLogFileDB-0.3/BorisLogFileDB/folder_file_process.py`

 * *Files identical despite different names*

### Comparing `BorisLogFileDB-0.2/BorisLogFileDB/folder_process.py` & `BorisLogFileDB-0.3/BorisLogFileDB/folder_process.py`

 * *Files identical despite different names*

### Comparing `BorisLogFileDB-0.2/BorisLogFileDB/log_process.py` & `BorisLogFileDB-0.3/BorisLogFileDB/log_process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding = utf-8 -*-
 __file__ = 'log_process.py'
 __date__ = '2022/11/30'
 __author__ = 'Zhiyong ZHANG'
 
 import logging
-import folder_file_process as ff
+from . import folder_file_process as ff
 
 
 class Log:
     def __init__(self, file_name, file_path):
         self.file_name = file_name
         self.file_path = file_path
```

### Comparing `BorisLogFileDB-0.2/BorisLogFileDB/logger.py` & `BorisLogFileDB-0.3/BorisLogFileDB/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 __file__ = 'logger.py'
 __date__ = '2023/1/25'
 __author__ = 'Zhiyong ZHANG'
 
 
 import logging
-import folder_file_process as ff
+from . import folder_file_process as ff
 
 
 class Log:
     def __init__(self, file_name, file_path=None):
         self.file_name = file_name
         self.file_path = file_path
```

### Comparing `BorisLogFileDB-0.2/BorisLogFileDB/mysql_connect.py` & `BorisLogFileDB-0.3/BorisLogFileDB/mysql_connect.py`

 * *Files identical despite different names*

