# Comparing `tmp/pwdPackage-3.1.1.tar.gz` & `tmp/pwdPackage-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwdPackage-3.1.1.tar", last modified: Mon Jul 24 17:53:50 2023, max compression
+gzip compressed data, was "pwdPackage-4.1.1.tar", last modified: Mon Jul 24 17:54:17 2023, max compression
```

## Comparing `pwdPackage-3.1.1.tar` & `pwdPackage-4.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 17:53:50.618176 pwdPackage-3.1.1/
--rw-rw-r--   0 user      (1000) user      (1000)     1068 2023-07-14 09:35:04.000000 pwdPackage-3.1.1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)      386 2023-07-24 17:53:50.618176 pwdPackage-3.1.1/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 17:53:50.614176 pwdPackage-3.1.1/pwdPackage/
--rw-rw-r--   0 user      (1000) user      (1000)       30 2023-07-24 09:48:27.000000 pwdPackage-3.1.1/pwdPackage/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 17:53:50.618176 pwdPackage-3.1.1/pwdPackage/data/
--rw-rw-r--   0 user      (1000) user      (1000)       24 2023-07-18 11:04:17.000000 pwdPackage-3.1.1/pwdPackage/data/names.csv
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-18 11:05:29.000000 pwdPackage-3.1.1/pwdPackage/data/places.csv
--rw-rw-r--   0 user      (1000) user      (1000)     3172 2023-07-24 17:20:22.000000 pwdPackage-3.1.1/pwdPackage/passwd.py
--rw-rw-r--   0 user      (1000) user      (1000)     1896 2023-07-20 18:57:51.000000 pwdPackage-3.1.1/pwdPackage/testing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 17:53:50.618176 pwdPackage-3.1.1/pwdPackage.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      386 2023-07-24 17:53:50.000000 pwdPackage-3.1.1/pwdPackage.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      384 2023-07-24 17:53:50.000000 pwdPackage-3.1.1/pwdPackage.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:53:50.000000 pwdPackage-3.1.1/pwdPackage.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:28:39.000000 pwdPackage-3.1.1/pwdPackage.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       11 2023-07-24 17:53:50.000000 pwdPackage-3.1.1/pwdPackage.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-24 17:53:50.618176 pwdPackage-3.1.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      791 2023-07-24 17:53:16.000000 pwdPackage-3.1.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 17:54:17.203083 pwdPackage-4.1.1/
+-rw-rw-r--   0 user      (1000) user      (1000)     1068 2023-07-14 09:35:04.000000 pwdPackage-4.1.1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      386 2023-07-24 17:54:17.203083 pwdPackage-4.1.1/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 17:54:17.199083 pwdPackage-4.1.1/pwdPackage/
+-rw-rw-r--   0 user      (1000) user      (1000)       30 2023-07-24 09:48:27.000000 pwdPackage-4.1.1/pwdPackage/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 17:54:17.199083 pwdPackage-4.1.1/pwdPackage/data/
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2023-07-18 11:04:17.000000 pwdPackage-4.1.1/pwdPackage/data/names.csv
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-18 11:05:29.000000 pwdPackage-4.1.1/pwdPackage/data/places.csv
+-rw-rw-r--   0 user      (1000) user      (1000)     3172 2023-07-24 17:20:22.000000 pwdPackage-4.1.1/pwdPackage/passwd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1896 2023-07-20 18:57:51.000000 pwdPackage-4.1.1/pwdPackage/testing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 17:54:17.203083 pwdPackage-4.1.1/pwdPackage.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      386 2023-07-24 17:54:17.000000 pwdPackage-4.1.1/pwdPackage.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      384 2023-07-24 17:54:17.000000 pwdPackage-4.1.1/pwdPackage.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:54:17.000000 pwdPackage-4.1.1/pwdPackage.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:28:39.000000 pwdPackage-4.1.1/pwdPackage.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       11 2023-07-24 17:54:17.000000 pwdPackage-4.1.1/pwdPackage.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-24 17:54:17.203083 pwdPackage-4.1.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      791 2023-07-24 17:54:03.000000 pwdPackage-4.1.1/setup.py
```

### Comparing `pwdPackage-3.1.1/LICENSE.txt` & `pwdPackage-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pwdPackage-3.1.1/pwdPackage/passwd.py` & `pwdPackage-4.1.1/pwdPackage/passwd.py`

 * *Files identical despite different names*

### Comparing `pwdPackage-3.1.1/pwdPackage/testing.py` & `pwdPackage-4.1.1/pwdPackage/testing.py`

 * *Files identical despite different names*

### Comparing `pwdPackage-3.1.1/setup.py` & `pwdPackage-4.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='pwdPackage',
-    version="3.1.1",
+    version="4.1.1",
     author="Anant Chaudhary",
     zip_safe=False,
     description="password generator package",
     long_description="A package for generating passwords.",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     package_data={'pwdPackage': ['data/*.csv']},  # Correct the package_data key
```

