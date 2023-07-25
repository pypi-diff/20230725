# Comparing `tmp/testmhdbAPI-1.1.tar.gz` & `tmp/testmhdbAPI-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/testmhdbAPI-1.1.tar", last modified: Tue Jul 25 06:18:53 2023, max compression
+gzip compressed data, was "dist/testmhdbAPI-1.2.tar", last modified: Tue Jul 25 07:40:59 2023, max compression
```

## Comparing `testmhdbAPI-1.1.tar` & `testmhdbAPI-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 06:18:53.000000 testmhdbAPI-1.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 06:18:53.000000 testmhdbAPI-1.1/machbaseAPI/
--rw-r--r--   0 root         (0) root         (0)    15368 2023-07-24 01:22:08.000000 testmhdbAPI-1.1/machbaseAPI/machbaseAPI.py
--rw-r--r--   0 root         (0) root         (0)       97 2023-07-24 01:22:08.000000 testmhdbAPI-1.1/machbaseAPI/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.1/libmachbaseAPI.so
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-24 01:22:08.000000 testmhdbAPI-1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 06:18:53.000000 testmhdbAPI-1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1264 2023-07-25 06:18:41.000000 testmhdbAPI-1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 06:18:53.000000 testmhdbAPI-1.1/testmhdbAPI.egg-info/
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-25 06:18:53.000000 testmhdbAPI-1.1/testmhdbAPI.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 06:18:53.000000 testmhdbAPI-1.1/testmhdbAPI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      236 2023-07-25 06:18:53.000000 testmhdbAPI-1.1/testmhdbAPI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      263 2023-07-25 06:18:53.000000 testmhdbAPI-1.1/testmhdbAPI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      155 2023-07-24 01:22:08.000000 testmhdbAPI-1.1/README
--rw-r--r--   0 root         (0) root         (0)      263 2023-07-25 06:18:53.000000 testmhdbAPI-1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/machbaseAPI/
+-rw-r--r--   0 root         (0) root         (0)    15368 2023-07-24 01:22:08.000000 testmhdbAPI-1.2/machbaseAPI/machbaseAPI.py
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-24 01:22:08.000000 testmhdbAPI-1.2/machbaseAPI/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.2/libmachbaseAPI.so
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-24 01:22:08.000000 testmhdbAPI-1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-07-25 07:38:34.000000 testmhdbAPI-1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/testmhdbAPI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/testmhdbAPI.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/testmhdbAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      236 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/testmhdbAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      263 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/testmhdbAPI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-24 01:22:08.000000 testmhdbAPI-1.2/README
+-rw-r--r--   0 root         (0) root         (0)      263 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/PKG-INFO
```

### Comparing `testmhdbAPI-1.1/machbaseAPI/machbaseAPI.py` & `testmhdbAPI-1.2/machbaseAPI/machbaseAPI.py`

 * *Files identical despite different names*

### Comparing `testmhdbAPI-1.1/libmachbaseAPI.so` & `testmhdbAPI-1.2/libmachbaseAPI.so`

 * *Files identical despite different names*

### Comparing `testmhdbAPI-1.1/setup.py` & `testmhdbAPI-1.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,28 +2,27 @@
  * Copyright of this product 2013-2023,
  * Machbase Corporation(or Inc.) or its subsidiaries.
  * All Rights reserved.
 """
 #coding=utf8
 
 import os, re, shutil, zipfile, platform, sys
-from setuptools import setup
+from setuptools import setup, find_packages
 from distutils.sysconfig import get_python_lib
 
 setup(
     name='testmhdbAPI',
-    version='1.1',
+    version='1.2',
     description='Test-Python3-API',
     long_description='Python3 module for Machbase',
     url='http://www.machbase.com',
     author='machbase',
     author_email='support@machbase.com',
     platforms='LINUX',
-    packages=['machbaseAPI'],
-    data_files=[(get_python_lib()+'/machbaseAPI',['libmachbaseAPI.so']),],
+    packages=find_packages(),
     python_requires='>=3.0',
 )
 
 args = sys.argv
 p = platform.system()
 
 if p == 'Windows' and args[1] == 'install':
```

