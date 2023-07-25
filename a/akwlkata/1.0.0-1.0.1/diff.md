# Comparing `tmp/akwlkata-1.0.0.tar.gz` & `tmp/akwlkata-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/akwlkata-1.0.0.tar", last modified: Tue Jul 25 07:42:36 2023, max compression
+gzip compressed data, was "dist/akwlkata-1.0.1.tar", last modified: Tue Jul 25 07:58:22 2023, max compression
```

## Comparing `akwlkata-1.0.0.tar` & `akwlkata-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-25 07:42:36.000000 akwlkata-1.0.0/
--rw-r--r--   0 NikkiMac   (501) staff       (20)      258 2023-07-25 07:42:36.000000 akwlkata-1.0.0/PKG-INFO
-drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-25 07:42:36.000000 akwlkata-1.0.0/akwlkata/
--rw-r--r--   0 NikkiMac   (501) staff       (20)    11100 2023-07-25 07:38:49.000000 akwlkata-1.0.0/akwlkata/AKWlkata.py
--rw-r--r--   0 NikkiMac   (501) staff       (20)      252 2023-07-25 07:13:58.000000 akwlkata-1.0.0/akwlkata/__init__.py
-drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-25 07:42:36.000000 akwlkata-1.0.0/akwlkata.egg-info/
--rw-r--r--   0 NikkiMac   (501) staff       (20)      258 2023-07-25 07:42:36.000000 akwlkata-1.0.0/akwlkata.egg-info/PKG-INFO
--rw-r--r--   0 NikkiMac   (501) staff       (20)      209 2023-07-25 07:42:36.000000 akwlkata-1.0.0/akwlkata.egg-info/SOURCES.txt
--rw-r--r--   0 NikkiMac   (501) staff       (20)        1 2023-07-25 07:42:36.000000 akwlkata-1.0.0/akwlkata.egg-info/dependency_links.txt
--rw-r--r--   0 NikkiMac   (501) staff       (20)        7 2023-07-25 07:42:36.000000 akwlkata-1.0.0/akwlkata.egg-info/requires.txt
--rw-r--r--   0 NikkiMac   (501) staff       (20)        9 2023-07-25 07:42:36.000000 akwlkata-1.0.0/akwlkata.egg-info/top_level.txt
--rw-r--r--   0 NikkiMac   (501) staff       (20)       38 2023-07-25 07:42:36.000000 akwlkata-1.0.0/setup.cfg
--rw-r--r--   0 NikkiMac   (501) staff       (20)      751 2023-07-25 07:18:31.000000 akwlkata-1.0.0/setup.py
+drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-25 07:58:22.000000 akwlkata-1.0.1/
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      282 2023-07-25 07:58:22.000000 akwlkata-1.0.1/PKG-INFO
+drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-25 07:58:22.000000 akwlkata-1.0.1/akwlkata/
+-rw-r--r--   0 NikkiMac   (501) staff       (20)    11100 2023-07-25 07:38:49.000000 akwlkata-1.0.1/akwlkata/AKWlkata.py
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      252 2023-07-25 07:13:58.000000 akwlkata-1.0.1/akwlkata/__init__.py
+drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-25 07:58:22.000000 akwlkata-1.0.1/akwlkata.egg-info/
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      282 2023-07-25 07:58:22.000000 akwlkata-1.0.1/akwlkata.egg-info/PKG-INFO
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      209 2023-07-25 07:58:22.000000 akwlkata-1.0.1/akwlkata.egg-info/SOURCES.txt
+-rw-r--r--   0 NikkiMac   (501) staff       (20)        1 2023-07-25 07:58:22.000000 akwlkata-1.0.1/akwlkata.egg-info/dependency_links.txt
+-rw-r--r--   0 NikkiMac   (501) staff       (20)        9 2023-07-25 07:58:22.000000 akwlkata-1.0.1/akwlkata.egg-info/requires.txt
+-rw-r--r--   0 NikkiMac   (501) staff       (20)        9 2023-07-25 07:58:22.000000 akwlkata-1.0.1/akwlkata.egg-info/top_level.txt
+-rw-r--r--   0 NikkiMac   (501) staff       (20)       38 2023-07-25 07:58:22.000000 akwlkata-1.0.1/setup.cfg
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      777 2023-07-25 07:58:21.000000 akwlkata-1.0.1/setup.py
```

### Comparing `akwlkata-1.0.0/akwlkata/AKWlkata.py` & `akwlkata-1.0.1/akwlkata/AKWlkata.py`

 * *Files identical despite different names*

### Comparing `akwlkata-1.0.0/setup.py` & `akwlkata-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,22 @@
     @Copyright © 2020年 Mr.Li All rights reserved
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="akwlkata",
-    version="1.0.0",
+    version="1.0.1",
     keywords=("pip", "akwlkata", "wlkata", "wlkatarobot", "kuture", "robot"),
     description="wlkata robot driver",
-    long_description="开塔机械臂驱动",
+    long_description="开塔机械臂驱动，兼容ubuntu与mac OS",
     license="MIT Licence",
 
     url="",
     author="Kuture",
     author_email="kuture@163.com",
 
     packages=find_packages(),
     include_package_data=False,
     platforms="any",
-    install_requires=['serial']
+    install_requires=['pyserial']
 )
```

