# Comparing `tmp/bloomfilter-py-0.2.0.tar.gz` & `tmp/bloomfilter-py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloomfilter-py-0.2.0.tar", last modified: Mon Feb 13 06:38:33 2023, max compression
+gzip compressed data, was "bloomfilter-py-0.2.1.tar", last modified: Tue Jul 25 01:08:00 2023, max compression
```

## Comparing `bloomfilter-py-0.2.0.tar` & `bloomfilter-py-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:38:33.756955 bloomfilter-py-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-13 06:38:23.000000 bloomfilter-py-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-02-13 06:38:33.756955 bloomfilter-py-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-13 06:38:23.000000 bloomfilter-py-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:38:33.756955 bloomfilter-py-0.2.0/bloomfilter/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-13 06:38:23.000000 bloomfilter-py-0.2.0/bloomfilter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-02-13 06:38:23.000000 bloomfilter-py-0.2.0/bloomfilter/bloomfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-02-13 06:38:23.000000 bloomfilter-py-0.2.0/bloomfilter/bloomfilter_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:38:33.756955 bloomfilter-py-0.2.0/bloomfilter_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-02-13 06:38:33.000000 bloomfilter-py-0.2.0/bloomfilter_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-13 06:38:33.000000 bloomfilter-py-0.2.0/bloomfilter_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 06:38:33.000000 bloomfilter-py-0.2.0/bloomfilter_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 06:38:33.000000 bloomfilter-py-0.2.0/bloomfilter_py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-13 06:38:33.000000 bloomfilter-py-0.2.0/bloomfilter_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-13 06:38:33.000000 bloomfilter-py-0.2.0/bloomfilter_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 06:38:33.756955 bloomfilter-py-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-02-13 06:38:23.000000 bloomfilter-py-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:08:00.901368 bloomfilter-py-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-25 01:07:49.000000 bloomfilter-py-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-25 01:08:00.901368 bloomfilter-py-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-25 01:07:49.000000 bloomfilter-py-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:08:00.897368 bloomfilter-py-0.2.1/bloomfilter/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 01:07:49.000000 bloomfilter-py-0.2.1/bloomfilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-07-25 01:07:49.000000 bloomfilter-py-0.2.1/bloomfilter/bloomfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-25 01:07:49.000000 bloomfilter-py-0.2.1/bloomfilter/bloomfilter_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:08:00.901368 bloomfilter-py-0.2.1/bloomfilter_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-25 01:08:00.000000 bloomfilter-py-0.2.1/bloomfilter_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-25 01:08:00.000000 bloomfilter-py-0.2.1/bloomfilter_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:08:00.000000 bloomfilter-py-0.2.1/bloomfilter_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:08:00.000000 bloomfilter-py-0.2.1/bloomfilter_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 01:08:00.000000 bloomfilter-py-0.2.1/bloomfilter_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 01:08:00.000000 bloomfilter-py-0.2.1/bloomfilter_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 01:08:00.901368 bloomfilter-py-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-25 01:07:49.000000 bloomfilter-py-0.2.1/setup.py
```

### Comparing `bloomfilter-py-0.2.0/LICENSE` & `bloomfilter-py-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bloomfilter-py-0.2.0/PKG-INFO` & `bloomfilter-py-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloomfilter-py
-Version: 0.2.0
+Version: 0.2.1
 Summary: Yet another bloomfilter implementation in Python
 Home-page: https://github.com/OldPanda/bloomfilter-py
 Author: OldPanda
 Author-email: me@old-panda.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `bloomfilter-py-0.2.0/README.md` & `bloomfilter-py-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bloomfilter-py-0.2.0/bloomfilter/bloomfilter.py` & `bloomfilter-py-0.2.1/bloomfilter/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `bloomfilter-py-0.2.0/bloomfilter/bloomfilter_strategy.py` & `bloomfilter-py-0.2.1/bloomfilter/bloomfilter_strategy.py`

 * *Files identical despite different names*

### Comparing `bloomfilter-py-0.2.0/bloomfilter_py.egg-info/PKG-INFO` & `bloomfilter-py-0.2.1/bloomfilter_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloomfilter-py
-Version: 0.2.0
+Version: 0.2.1
 Summary: Yet another bloomfilter implementation in Python
 Home-page: https://github.com/OldPanda/bloomfilter-py
 Author: OldPanda
 Author-email: me@old-panda.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `bloomfilter-py-0.2.0/setup.py` & `bloomfilter-py-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
-version = "0.2.0"
-install_requires = ["bitarray==2.6.0", "mmh3==3.0.0"]
+version = "0.2.1"
+install_requires = ["bitarray==2.7.6", "mmh3==3.1.0"]
 extras_require = {}
 
 setup(
     name="bloomfilter-py",
     version=version,
     description="Yet another bloomfilter implementation in Python",
     long_description=open("README.md").read(),
```

