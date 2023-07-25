# Comparing `tmp/kot-0.17.0.tar.gz` & `tmp/kot-0.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kot-0.17.0.tar", last modified: Tue Jul 25 18:25:41 2023, max compression
+gzip compressed data, was "kot-0.18.0.tar", last modified: Tue Jul 25 18:33:49 2023, max compression
```

## Comparing `kot-0.17.0.tar` & `kot-0.18.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:25:41.235928 kot-0.17.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 18:25:28.000000 kot-0.17.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 18:25:41.235928 kot-0.17.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-25 18:25:28.000000 kot-0.17.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:25:41.235928 kot-0.17.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-25 18:25:28.000000 kot-0.17.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:25:41.231928 kot-0.17.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:25:41.235928 kot-0.17.0/src/kot/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 18:25:28.000000 kot-0.17.0/src/kot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-07-25 18:25:28.000000 kot-0.17.0/src/kot/kot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:25:41.235928 kot-0.17.0/src/kot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 18:25:41.000000 kot-0.17.0/src/kot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-25 18:25:41.000000 kot-0.17.0/src/kot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:25:41.000000 kot-0.17.0/src/kot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:25:41.000000 kot-0.17.0/src/kot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:25:41.000000 kot-0.17.0/src/kot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 18:25:41.000000 kot-0.17.0/src/kot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 18:25:41.000000 kot-0.17.0/src/kot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:33:49.198442 kot-0.18.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 18:33:36.000000 kot-0.18.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 18:33:49.198442 kot-0.18.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-25 18:33:36.000000 kot-0.18.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:33:49.198442 kot-0.18.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-25 18:33:36.000000 kot-0.18.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:33:49.194442 kot-0.18.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:33:49.198442 kot-0.18.0/src/kot/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 18:33:36.000000 kot-0.18.0/src/kot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-07-25 18:33:36.000000 kot-0.18.0/src/kot/kot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:33:49.198442 kot-0.18.0/src/kot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 18:33:48.000000 kot-0.18.0/src/kot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-25 18:33:49.000000 kot-0.18.0/src/kot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:33:48.000000 kot-0.18.0/src/kot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:33:48.000000 kot-0.18.0/src/kot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:33:48.000000 kot-0.18.0/src/kot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 18:33:48.000000 kot-0.18.0/src/kot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 18:33:48.000000 kot-0.18.0/src/kot.egg-info/top_level.txt
```

### Comparing `kot-0.17.0/LICENSE` & `kot-0.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kot-0.17.0/PKG-INFO` & `kot-0.18.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kot
-Version: 0.17.0
+Version: 0.18.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KOT
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KOT database
```

### Comparing `kot-0.17.0/README.md` & `kot-0.18.0/README.md`

 * *Files identical despite different names*

### Comparing `kot-0.17.0/setup.py` & `kot-0.18.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='kot',
-version='0.17.0',
+version='0.18.0',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KOT',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
```

### Comparing `kot-0.17.0/src/kot/kot.py` & `kot-0.18.0/src/kot/kot.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,23 @@
                              self_datas=True,
                              folder=folder)
 
         for each_database in database_index.dict():
             KOT.database_delete(each_database, folder=folder)
 
     @staticmethod
+    def database_pop_all(folder: str = ""):
+        database_index = KOT("KOT-database-index",
+                             self_datas=True,
+                             folder=folder)
+
+        for each_database in database_index.dict():
+            KOT.database_pop(each_database, folder=folder)
+
+    @staticmethod
     def database_rename(name: str,
                         new_name: str,
                         force: bool = False,
                         folder: str = "") -> bool:
         if new_name in KOT.database_list() and not force:
             return False
         try:
```

### Comparing `kot-0.17.0/src/kot.egg-info/PKG-INFO` & `kot-0.18.0/src/kot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kot
-Version: 0.17.0
+Version: 0.18.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KOT
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KOT database
```

