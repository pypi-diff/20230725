# Comparing `tmp/modelwhaleutils-0.5.2.0.tar.gz` & `tmp/modelwhaleutils-0.5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/modelwhaleutils-0.5.2.0.tar", last modified: Mon Jul 10 04:04:37 2023, max compression
+gzip compressed data, was "dist/modelwhaleutils-0.5.2.3.tar", last modified: Tue Jul 25 10:17:46 2023, max compression
```

## Comparing `modelwhaleutils-0.5.2.0.tar` & `modelwhaleutils-0.5.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/
--rw-r--r--   0 YiranTao   (502) staff       (20)      381 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/PKG-INFO
--rw-r--r--   0 YiranTao   (502) staff       (20)     3078 2021-04-16 07:51:27.000000 modelwhaleutils-0.5.2.0/README.md
-drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/modelwhaleutils.egg-info/
--rw-r--r--   0 YiranTao   (502) staff       (20)      381 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/modelwhaleutils.egg-info/PKG-INFO
--rw-r--r--   0 YiranTao   (502) staff       (20)      360 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/modelwhaleutils.egg-info/SOURCES.txt
--rw-r--r--   0 YiranTao   (502) staff       (20)        1 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/modelwhaleutils.egg-info/dependency_links.txt
--rw-r--r--   0 YiranTao   (502) staff       (20)       42 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/modelwhaleutils.egg-info/requires.txt
--rw-r--r--   0 YiranTao   (502) staff       (20)        8 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/modelwhaleutils.egg-info/top_level.txt
-drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/mwutils/
--rw-r--r--   0 YiranTao   (502) staff       (20)        0 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.2.0/mwutils/__init__.py
--rw-r--r--   0 YiranTao   (502) staff       (20)     1580 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.2.0/mwutils/keras.py
--rw-r--r--   0 YiranTao   (502) staff       (20)     4062 2023-07-10 03:51:57.000000 modelwhaleutils-0.5.2.0/mwutils/logs.py
--rw-r--r--   0 YiranTao   (502) staff       (20)    21826 2023-07-10 03:51:57.000000 modelwhaleutils-0.5.2.0/mwutils/run.py
--rw-r--r--   0 YiranTao   (502) staff       (20)     6285 2023-07-10 03:51:57.000000 modelwhaleutils-0.5.2.0/mwutils/sys_stat.py
--rw-r--r--   0 YiranTao   (502) staff       (20)     1163 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.2.0/mwutils/tf_utils.py
--rw-r--r--   0 YiranTao   (502) staff       (20)      562 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.2.0/mwutils/torch_utils.py
--rw-r--r--   0 YiranTao   (502) staff       (20)     5203 2023-07-10 03:51:57.000000 modelwhaleutils-0.5.2.0/mwutils/utils.py
--rw-r--r--   0 YiranTao   (502) staff       (20)       38 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/setup.cfg
--rw-r--r--   0 YiranTao   (502) staff       (20)      544 2023-07-10 04:04:34.000000 modelwhaleutils-0.5.2.0/setup.py
+drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-07-25 10:17:46.000000 modelwhaleutils-0.5.2.3/
+-rw-r--r--   0 YiranTao   (502) staff       (20)      381 2023-07-25 10:17:46.000000 modelwhaleutils-0.5.2.3/PKG-INFO
+-rw-r--r--   0 YiranTao   (502) staff       (20)     3078 2021-04-16 07:51:27.000000 modelwhaleutils-0.5.2.3/README.md
+drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-07-25 10:17:46.000000 modelwhaleutils-0.5.2.3/modelwhaleutils.egg-info/
+-rw-r--r--   0 YiranTao   (502) staff       (20)      381 2023-07-25 10:17:46.000000 modelwhaleutils-0.5.2.3/modelwhaleutils.egg-info/PKG-INFO
+-rw-r--r--   0 YiranTao   (502) staff       (20)      360 2023-07-25 10:17:46.000000 modelwhaleutils-0.5.2.3/modelwhaleutils.egg-info/SOURCES.txt
+-rw-r--r--   0 YiranTao   (502) staff       (20)        1 2023-07-25 10:17:46.000000 modelwhaleutils-0.5.2.3/modelwhaleutils.egg-info/dependency_links.txt
+-rw-r--r--   0 YiranTao   (502) staff       (20)       42 2023-07-25 10:17:46.000000 modelwhaleutils-0.5.2.3/modelwhaleutils.egg-info/requires.txt
+-rw-r--r--   0 YiranTao   (502) staff       (20)        8 2023-07-25 10:17:46.000000 modelwhaleutils-0.5.2.3/modelwhaleutils.egg-info/top_level.txt
+drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-07-25 10:17:46.000000 modelwhaleutils-0.5.2.3/mwutils/
+-rw-r--r--   0 YiranTao   (502) staff       (20)        0 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.2.3/mwutils/__init__.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)     1580 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.2.3/mwutils/keras.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)     4062 2023-07-10 03:51:57.000000 modelwhaleutils-0.5.2.3/mwutils/logs.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)    21826 2023-07-10 03:51:57.000000 modelwhaleutils-0.5.2.3/mwutils/run.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)     6285 2023-07-10 03:51:57.000000 modelwhaleutils-0.5.2.3/mwutils/sys_stat.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)     1163 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.2.3/mwutils/tf_utils.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)      562 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.2.3/mwutils/torch_utils.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)     5203 2023-07-10 03:51:57.000000 modelwhaleutils-0.5.2.3/mwutils/utils.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)       38 2023-07-25 10:17:46.000000 modelwhaleutils-0.5.2.3/setup.cfg
+-rw-r--r--   0 YiranTao   (502) staff       (20)      544 2023-07-25 10:17:36.000000 modelwhaleutils-0.5.2.3/setup.py
```

### Comparing `modelwhaleutils-0.5.2.0/README.md` & `modelwhaleutils-0.5.2.3/README.md`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.2.0/mwutils/keras.py` & `modelwhaleutils-0.5.2.3/mwutils/keras.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.2.0/mwutils/logs.py` & `modelwhaleutils-0.5.2.3/mwutils/logs.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.2.0/mwutils/run.py` & `modelwhaleutils-0.5.2.3/mwutils/run.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.2.0/mwutils/sys_stat.py` & `modelwhaleutils-0.5.2.3/mwutils/sys_stat.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.2.0/mwutils/tf_utils.py` & `modelwhaleutils-0.5.2.3/mwutils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.2.0/mwutils/torch_utils.py` & `modelwhaleutils-0.5.2.3/mwutils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.2.0/mwutils/utils.py` & `modelwhaleutils-0.5.2.3/mwutils/utils.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.2.0/setup.py` & `modelwhaleutils-0.5.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="modelwhaleutils",
-    version="0.5.2.0",
+    version="0.5.2.3",
     author="modalwhale team",
     description="use in mw",
     url="https://github.com/Kesci/modelwhaleutils",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

