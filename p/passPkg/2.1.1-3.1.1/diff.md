# Comparing `tmp/passPkg-2.1.1.tar.gz` & `tmp/passPkg-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passPkg-2.1.1.tar", last modified: Tue Jul 25 10:29:43 2023, max compression
+gzip compressed data, was "passPkg-3.1.1.tar", last modified: Tue Jul 25 10:35:45 2023, max compression
```

## Comparing `passPkg-2.1.1.tar` & `passPkg-3.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 10:29:43.034422 passPkg-2.1.1/
--rw-rw-r--   0 user      (1000) user      (1000)     1062 2023-07-25 10:28:57.000000 passPkg-2.1.1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)      346 2023-07-25 10:29:43.034422 passPkg-2.1.1/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 10:29:43.034422 passPkg-2.1.1/passPkg/
--rw-rw-r--   0 user      (1000) user      (1000)      654 2023-07-25 10:26:17.000000 passPkg-2.1.1/passPkg/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 10:29:43.034422 passPkg-2.1.1/passPkg.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      346 2023-07-25 10:29:42.000000 passPkg-2.1.1/passPkg.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      164 2023-07-25 10:29:42.000000 passPkg-2.1.1/passPkg.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 10:29:42.000000 passPkg-2.1.1/passPkg.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       20 2023-07-25 10:29:42.000000 passPkg-2.1.1/passPkg.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 10:29:43.034422 passPkg-2.1.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      947 2023-07-25 10:28:09.000000 passPkg-2.1.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 10:35:45.095750 passPkg-3.1.1/
+-rw-rw-r--   0 user      (1000) user      (1000)     1062 2023-07-25 10:28:57.000000 passPkg-3.1.1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      346 2023-07-25 10:35:45.095750 passPkg-3.1.1/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 10:35:45.095750 passPkg-3.1.1/passPkg/
+-rw-rw-r--   0 user      (1000) user      (1000)       34 2023-07-25 10:34:53.000000 passPkg-3.1.1/passPkg/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      654 2023-07-25 10:34:56.000000 passPkg-3.1.1/passPkg/pkgPass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 10:35:45.095750 passPkg-3.1.1/passPkg.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      346 2023-07-25 10:35:44.000000 passPkg-3.1.1/passPkg.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      183 2023-07-25 10:35:45.000000 passPkg-3.1.1/passPkg.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 10:35:44.000000 passPkg-3.1.1/passPkg.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       20 2023-07-25 10:35:44.000000 passPkg-3.1.1/passPkg.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 10:35:45.095750 passPkg-3.1.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      947 2023-07-25 10:35:04.000000 passPkg-3.1.1/setup.py
```

### Comparing `passPkg-2.1.1/LICENSE.txt` & `passPkg-3.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `passPkg-2.1.1/passPkg/__init__.py` & `passPkg-3.1.1/passPkg/pkgPass.py`

 * *Files identical despite different names*

### Comparing `passPkg-2.1.1/setup.py` & `passPkg-3.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="passPkg",                     # This is the name of the package
-    version="2.1.1",                        # The initial release version
+    version="3.1.1",                        # The initial release version
     author="Anant Chaudhary",                     # Full name of the author
     description="password generator package",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

