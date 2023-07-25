# Comparing `tmp/pipcryptographymodV1-1.0.0.tar.gz` & `tmp/pipcryptographymodV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcryptographymodV1-1.0.0.tar", last modified: Tue Jul 25 01:03:09 2023, max compression
+gzip compressed data, was "pipcryptographymodV1-1.1.0.tar", last modified: Tue Jul 25 01:05:24 2023, max compression
```

## Comparing `pipcryptographymodV1-1.0.0.tar` & `pipcryptographymodV1-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 01:03:09.706773 pipcryptographymodV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-25 01:03:09.706773 pipcryptographymodV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 01:03:09.706773 pipcryptographymodV1-1.0.0/pipcolortoolsV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 21:14:28.000000 pipcryptographymodV1-1.0.0/pipcolortoolsV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 01:03:09.706773 pipcryptographymodV1-1.0.0/pipcryptographymodV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-25 01:03:09.000000 pipcryptographymodV1-1.0.0/pipcryptographymodV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 01:03:09.706773 pipcryptographymodV1-1.0.0/pipcryptographymodV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-25 01:03:09.000000 pipcryptographymodV1-1.0.0/pipcryptographymodV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      245 2023-07-25 01:03:09.000000 pipcryptographymodV1-1.0.0/pipcryptographymodV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 01:03:09.000000 pipcryptographymodV1-1.0.0/pipcryptographymodV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-25 01:03:09.000000 pipcryptographymodV1-1.0.0/pipcryptographymodV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 01:03:09.706773 pipcryptographymodV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      566 2023-07-25 01:03:09.000000 pipcryptographymodV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 01:05:24.640123 pipcryptographymodV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-25 01:05:24.640123 pipcryptographymodV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 01:05:24.636123 pipcryptographymodV1-1.1.0/pipcolortoolsV2/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 21:14:28.000000 pipcryptographymodV1-1.1.0/pipcolortoolsV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 01:05:24.640123 pipcryptographymodV1-1.1.0/pipcryptographymodV1/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-25 01:05:24.000000 pipcryptographymodV1-1.1.0/pipcryptographymodV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 01:05:24.640123 pipcryptographymodV1-1.1.0/pipcryptographymodV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-25 01:05:24.000000 pipcryptographymodV1-1.1.0/pipcryptographymodV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      245 2023-07-25 01:05:24.000000 pipcryptographymodV1-1.1.0/pipcryptographymodV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 01:05:24.000000 pipcryptographymodV1-1.1.0/pipcryptographymodV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-25 01:05:24.000000 pipcryptographymodV1-1.1.0/pipcryptographymodV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 01:05:24.640123 pipcryptographymodV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      566 2023-07-25 01:05:24.000000 pipcryptographymodV1-1.1.0/setup.py
```

### Comparing `pipcryptographymodV1-1.0.0/setup.py` & `pipcryptographymodV1-1.1.0/setup.py`

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
     name="pipcryptographymodV1",
     version=VERSION,
```

