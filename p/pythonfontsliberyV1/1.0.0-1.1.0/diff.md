# Comparing `tmp/pythonfontsliberyV1-1.0.0.tar.gz` & `tmp/pythonfontsliberyV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonfontsliberyV1-1.0.0.tar", last modified: Tue Jul 25 13:17:04 2023, max compression
+gzip compressed data, was "pythonfontsliberyV1-1.1.0.tar", last modified: Tue Jul 25 13:19:10 2023, max compression
```

## Comparing `pythonfontsliberyV1-1.0.0.tar` & `pythonfontsliberyV1-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:17:04.849198 pythonfontsliberyV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      352 2023-07-25 13:17:04.849198 pythonfontsliberyV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:17:04.849198 pythonfontsliberyV1-1.0.0/pipcolortoolsV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 21:14:28.000000 pythonfontsliberyV1-1.0.0/pipcolortoolsV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:17:04.849198 pythonfontsliberyV1-1.0.0/pythonfontsliberyV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-25 13:17:04.000000 pythonfontsliberyV1-1.0.0/pythonfontsliberyV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:17:04.849198 pythonfontsliberyV1-1.0.0/pythonfontsliberyV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      352 2023-07-25 13:17:04.000000 pythonfontsliberyV1-1.0.0/pythonfontsliberyV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      240 2023-07-25 13:17:04.000000 pythonfontsliberyV1-1.0.0/pythonfontsliberyV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 13:17:04.000000 pythonfontsliberyV1-1.0.0/pythonfontsliberyV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-25 13:17:04.000000 pythonfontsliberyV1-1.0.0/pythonfontsliberyV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 13:17:04.849198 pythonfontsliberyV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      565 2023-07-25 13:17:04.000000 pythonfontsliberyV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:19:10.674747 pythonfontsliberyV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-07-25 13:19:10.674747 pythonfontsliberyV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:19:10.674747 pythonfontsliberyV1-1.1.0/pipcolortoolsV2/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 21:14:28.000000 pythonfontsliberyV1-1.1.0/pipcolortoolsV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:19:10.674747 pythonfontsliberyV1-1.1.0/pythonfontsliberyV1/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-25 13:19:10.000000 pythonfontsliberyV1-1.1.0/pythonfontsliberyV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:19:10.674747 pythonfontsliberyV1-1.1.0/pythonfontsliberyV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-07-25 13:19:10.000000 pythonfontsliberyV1-1.1.0/pythonfontsliberyV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      240 2023-07-25 13:19:10.000000 pythonfontsliberyV1-1.1.0/pythonfontsliberyV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 13:19:10.000000 pythonfontsliberyV1-1.1.0/pythonfontsliberyV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-25 13:19:10.000000 pythonfontsliberyV1-1.1.0/pythonfontsliberyV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 13:19:10.674747 pythonfontsliberyV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      565 2023-07-25 13:19:10.000000 pythonfontsliberyV1-1.1.0/setup.py
```

### Comparing `pythonfontsliberyV1-1.0.0/setup.py` & `pythonfontsliberyV1-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pythonfontsliberyV1",
     version=VERSION,
```

