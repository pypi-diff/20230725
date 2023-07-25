# Comparing `tmp/metaphor-python-0.1.6.tar.gz` & `tmp/metaphor-python-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaphor-python-0.1.6.tar", last modified: Tue Jul 25 07:54:06 2023, max compression
+gzip compressed data, was "metaphor-python-0.1.7.tar", last modified: Tue Jul 25 20:49:50 2023, max compression
```

## Comparing `metaphor-python-0.1.6.tar` & `metaphor-python-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 07:54:06.190925 metaphor-python-0.1.6/
--rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-25 07:54:06.190788 metaphor-python-0.1.6/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)     1505 2023-07-25 03:43:18.000000 metaphor-python-0.1.6/README.md
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 07:54:06.189954 metaphor-python-0.1.6/metaphor_python/
--rw-r--r--   0 jwang      (501) staff       (20)      180 2023-07-04 23:03:27.000000 metaphor-python-0.1.6/metaphor_python/__init__.py
--rw-r--r--   0 jwang      (501) staff       (20)     4319 2023-07-25 07:53:32.000000 metaphor-python-0.1.6/metaphor_python/api.py
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 07:54:06.190621 metaphor-python-0.1.6/metaphor_python.egg-info/
--rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-25 07:54:06.000000 metaphor-python-0.1.6/metaphor_python.egg-info/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)      263 2023-07-25 07:54:06.000000 metaphor-python-0.1.6/metaphor_python.egg-info/SOURCES.txt
--rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-25 07:54:06.000000 metaphor-python-0.1.6/metaphor_python.egg-info/dependency_links.txt
--rw-r--r--   0 jwang      (501) staff       (20)        9 2023-07-25 07:54:06.000000 metaphor-python-0.1.6/metaphor_python.egg-info/requires.txt
--rw-r--r--   0 jwang      (501) staff       (20)       16 2023-07-25 07:54:06.000000 metaphor-python-0.1.6/metaphor_python.egg-info/top_level.txt
--rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-25 07:54:06.190961 metaphor-python-0.1.6/setup.cfg
--rw-r--r--   0 jwang      (501) staff       (20)      773 2023-07-25 07:53:54.000000 metaphor-python-0.1.6/setup.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 20:49:50.103162 metaphor-python-0.1.7/
+-rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-25 20:49:50.103012 metaphor-python-0.1.7/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)     1505 2023-07-25 03:43:18.000000 metaphor-python-0.1.7/README.md
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 20:49:50.102177 metaphor-python-0.1.7/metaphor_python/
+-rw-r--r--   0 jwang      (501) staff       (20)      113 2023-07-25 20:46:42.000000 metaphor-python-0.1.7/metaphor_python/__init__.py
+-rw-r--r--   0 jwang      (501) staff       (20)     4865 2023-07-25 20:46:59.000000 metaphor-python-0.1.7/metaphor_python/api.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 20:49:50.102831 metaphor-python-0.1.7/metaphor_python.egg-info/
+-rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-25 20:49:50.000000 metaphor-python-0.1.7/metaphor_python.egg-info/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)      263 2023-07-25 20:49:50.000000 metaphor-python-0.1.7/metaphor_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-25 20:49:50.000000 metaphor-python-0.1.7/metaphor_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        9 2023-07-25 20:49:50.000000 metaphor-python-0.1.7/metaphor_python.egg-info/requires.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       16 2023-07-25 20:49:50.000000 metaphor-python-0.1.7/metaphor_python.egg-info/top_level.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-25 20:49:50.103203 metaphor-python-0.1.7/setup.cfg
+-rw-r--r--   0 jwang      (501) staff       (20)      773 2023-07-25 20:49:38.000000 metaphor-python-0.1.7/setup.py
```

### Comparing `metaphor-python-0.1.6/PKG-INFO` & `metaphor-python-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaphor-python
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package for the Metaphor API.
 Home-page: https://github.com/metaphorsystems/metaphor-python
 Author: Metaphor
 Author-email: hello@metaphor.systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metaphor-python-0.1.6/README.md` & `metaphor-python-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `metaphor-python-0.1.6/metaphor_python.egg-info/PKG-INFO` & `metaphor-python-0.1.7/metaphor_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaphor-python
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package for the Metaphor API.
 Home-page: https://github.com/metaphorsystems/metaphor-python
 Author: Metaphor
 Author-email: hello@metaphor.systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metaphor-python-0.1.6/setup.py` & `metaphor-python-0.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metaphor-python',
-    version='0.1.6',
+    version='0.1.7',
     description='A Python package for the Metaphor API.',
     author='Metaphor',
     author_email='hello@metaphor.systems',
     url='https://github.com/metaphorsystems/metaphor-python',
     packages=find_packages(),
     install_requires=[
         'requests',
```

