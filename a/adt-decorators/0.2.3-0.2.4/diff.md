# Comparing `tmp/adt-decorators-0.2.3.tar.gz` & `tmp/adt-decorators-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adt-decorators-0.2.3.tar", last modified: Mon Jul 24 23:14:26 2023, max compression
+gzip compressed data, was "adt-decorators-0.2.4.tar", last modified: Mon Jul 24 23:15:52 2023, max compression
```

## Comparing `adt-decorators-0.2.3.tar` & `adt-decorators-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:14:26.087144 adt-decorators-0.2.3/
--rw-r--r--   0 m0rphism  (1000) users      (100)     1296 2023-07-24 10:44:17.000000 adt-decorators-0.2.3/LICENSE
--rw-r--r--   0 m0rphism  (1000) users      (100)       69 2023-07-24 11:00:38.000000 adt-decorators-0.2.3/MANIFEST.in
--rw-r--r--   0 m0rphism  (1000) users      (100)      675 2023-07-24 23:14:26.087144 adt-decorators-0.2.3/PKG-INFO
--rw-r--r--   0 m0rphism  (1000) users      (100)     5854 2023-07-24 23:12:37.000000 adt-decorators-0.2.3/README.md
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:14:26.086144 adt-decorators-0.2.3/adt/
--rw-r--r--   0 m0rphism  (1000) users      (100)     4879 2023-07-24 23:14:06.000000 adt-decorators-0.2.3/adt/__init__.py
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:14:26.086144 adt-decorators-0.2.3/adt_decorators.egg-info/
--rw-r--r--   0 m0rphism  (1000) users      (100)      675 2023-07-24 23:14:26.000000 adt-decorators-0.2.3/adt_decorators.egg-info/PKG-INFO
--rw-r--r--   0 m0rphism  (1000) users      (100)      252 2023-07-24 23:14:26.000000 adt-decorators-0.2.3/adt_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)        1 2023-07-24 23:14:26.000000 adt-decorators-0.2.3/adt_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 m0rphism  (1000) users      (100)        4 2023-07-24 23:14:26.000000 adt-decorators-0.2.3/adt_decorators.egg-info/top_level.txt
-drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:14:26.087144 adt-decorators-0.2.3/docs/
--rw-r--r--   0 m0rphism  (1000) users      (100)     5854 2023-07-24 23:12:37.000000 adt-decorators-0.2.3/docs/overview.md
--rw-r--r--   0 m0rphism  (1000) users      (100)       25 2023-07-24 08:09:40.000000 adt-decorators-0.2.3/docs/reference.md
--rw-r--r--   0 m0rphism  (1000) users      (100)      317 2023-07-24 08:51:28.000000 adt-decorators-0.2.3/mkdocs.yml
--rw-r--r--   0 m0rphism  (1000) users      (100)       38 2023-07-24 23:14:26.087144 adt-decorators-0.2.3/setup.cfg
--rw-r--r--   0 m0rphism  (1000) users      (100)      818 2023-07-24 23:14:03.000000 adt-decorators-0.2.3/setup.py
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:15:52.900170 adt-decorators-0.2.4/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     1296 2023-07-24 10:44:17.000000 adt-decorators-0.2.4/LICENSE
+-rw-r--r--   0 m0rphism  (1000) users      (100)       69 2023-07-24 11:00:38.000000 adt-decorators-0.2.4/MANIFEST.in
+-rw-r--r--   0 m0rphism  (1000) users      (100)     6028 2023-07-24 23:15:52.900170 adt-decorators-0.2.4/PKG-INFO
+-rw-r--r--   0 m0rphism  (1000) users      (100)     5854 2023-07-24 23:12:37.000000 adt-decorators-0.2.4/README.md
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:15:52.900170 adt-decorators-0.2.4/adt/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     4879 2023-07-24 23:14:57.000000 adt-decorators-0.2.4/adt/__init__.py
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:15:52.900170 adt-decorators-0.2.4/adt_decorators.egg-info/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     6028 2023-07-24 23:15:52.000000 adt-decorators-0.2.4/adt_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 m0rphism  (1000) users      (100)      252 2023-07-24 23:15:52.000000 adt-decorators-0.2.4/adt_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 m0rphism  (1000) users      (100)        1 2023-07-24 23:15:52.000000 adt-decorators-0.2.4/adt_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 m0rphism  (1000) users      (100)        4 2023-07-24 23:15:52.000000 adt-decorators-0.2.4/adt_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 m0rphism  (1000) users      (100)        0 2023-07-24 23:15:52.900170 adt-decorators-0.2.4/docs/
+-rw-r--r--   0 m0rphism  (1000) users      (100)     5854 2023-07-24 23:12:37.000000 adt-decorators-0.2.4/docs/overview.md
+-rw-r--r--   0 m0rphism  (1000) users      (100)       25 2023-07-24 08:09:40.000000 adt-decorators-0.2.4/docs/reference.md
+-rw-r--r--   0 m0rphism  (1000) users      (100)      317 2023-07-24 08:51:28.000000 adt-decorators-0.2.4/mkdocs.yml
+-rw-r--r--   0 m0rphism  (1000) users      (100)       38 2023-07-24 23:15:52.900170 adt-decorators-0.2.4/setup.cfg
+-rw-r--r--   0 m0rphism  (1000) users      (100)      828 2023-07-24 23:15:28.000000 adt-decorators-0.2.4/setup.py
```

### Comparing `adt-decorators-0.2.3/LICENSE` & `adt-decorators-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adt-decorators-0.2.3/README.md` & `adt-decorators-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `adt-decorators-0.2.3/adt/__init__.py` & `adt-decorators-0.2.4/adt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Provides class decorators for Algebraic Data Types (ADTs)
 """
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 __author__ = 'Hannes Saffrich'
 
 from dataclasses import dataclass
 import inspect
 
 def adt(Class=None, export=False):
     """Class-decorator for Algebraic Data Types (ADTs).
```

### Comparing `adt-decorators-0.2.3/docs/overview.md` & `adt-decorators-0.2.4/docs/overview.md`

 * *Files identical despite different names*

### Comparing `adt-decorators-0.2.3/setup.py` & `adt-decorators-0.2.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 with open('docs/overview.md', 'r') as f:
     desc = f.read()
     skip_start = "[//]: # (INSTALL_BEGIN)"
     skip_end = "[//]: # (INSTALL_END)"
     begin = desc.find(skip_start)
     end = desc.find(skip_end) + len(skip_end)
-    desc = desc[begin:end]
+    desc = desc[:begin] + desc[end:]
 
 setup(
     name='adt-decorators',
-    version='0.2.3',
+    version='0.2.4',
     description='Algebraic Data Types via Class Decorators',
     long_description=desc,
     long_description_content_type='text/markdown',
     url='https://github.com/m0rphism/adt-decorators',
     author='Hannes Saffrich',
     author_email='saffrich@informatik.uni-freiburg.de',
     license='BSD 2-clause',
```

