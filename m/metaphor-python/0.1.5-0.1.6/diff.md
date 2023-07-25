# Comparing `tmp/metaphor-python-0.1.5.tar.gz` & `tmp/metaphor-python-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaphor-python-0.1.5.tar", last modified: Tue Jul 25 03:48:01 2023, max compression
+gzip compressed data, was "metaphor-python-0.1.6.tar", last modified: Tue Jul 25 07:54:06 2023, max compression
```

## Comparing `metaphor-python-0.1.5.tar` & `metaphor-python-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 03:48:01.471606 metaphor-python-0.1.5/
--rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-25 03:48:01.471379 metaphor-python-0.1.5/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)     1505 2023-07-25 03:43:18.000000 metaphor-python-0.1.5/README.md
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 03:48:01.469863 metaphor-python-0.1.5/metaphor_python/
--rw-r--r--   0 jwang      (501) staff       (20)      180 2023-07-04 23:03:27.000000 metaphor-python-0.1.5/metaphor_python/__init__.py
--rw-r--r--   0 jwang      (501) staff       (20)     4279 2023-07-25 03:42:32.000000 metaphor-python-0.1.5/metaphor_python/api.py
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 03:48:01.470870 metaphor-python-0.1.5/metaphor_python.egg-info/
--rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-25 03:48:01.000000 metaphor-python-0.1.5/metaphor_python.egg-info/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)      263 2023-07-25 03:48:01.000000 metaphor-python-0.1.5/metaphor_python.egg-info/SOURCES.txt
--rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-25 03:48:01.000000 metaphor-python-0.1.5/metaphor_python.egg-info/dependency_links.txt
--rw-r--r--   0 jwang      (501) staff       (20)        9 2023-07-25 03:48:01.000000 metaphor-python-0.1.5/metaphor_python.egg-info/requires.txt
--rw-r--r--   0 jwang      (501) staff       (20)       16 2023-07-25 03:48:01.000000 metaphor-python-0.1.5/metaphor_python.egg-info/top_level.txt
--rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-25 03:48:01.471655 metaphor-python-0.1.5/setup.cfg
--rw-r--r--   0 jwang      (501) staff       (20)      773 2023-07-25 03:43:59.000000 metaphor-python-0.1.5/setup.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 07:54:06.190925 metaphor-python-0.1.6/
+-rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-25 07:54:06.190788 metaphor-python-0.1.6/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)     1505 2023-07-25 03:43:18.000000 metaphor-python-0.1.6/README.md
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 07:54:06.189954 metaphor-python-0.1.6/metaphor_python/
+-rw-r--r--   0 jwang      (501) staff       (20)      180 2023-07-04 23:03:27.000000 metaphor-python-0.1.6/metaphor_python/__init__.py
+-rw-r--r--   0 jwang      (501) staff       (20)     4319 2023-07-25 07:53:32.000000 metaphor-python-0.1.6/metaphor_python/api.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 07:54:06.190621 metaphor-python-0.1.6/metaphor_python.egg-info/
+-rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-25 07:54:06.000000 metaphor-python-0.1.6/metaphor_python.egg-info/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)      263 2023-07-25 07:54:06.000000 metaphor-python-0.1.6/metaphor_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-25 07:54:06.000000 metaphor-python-0.1.6/metaphor_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        9 2023-07-25 07:54:06.000000 metaphor-python-0.1.6/metaphor_python.egg-info/requires.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       16 2023-07-25 07:54:06.000000 metaphor-python-0.1.6/metaphor_python.egg-info/top_level.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-25 07:54:06.190961 metaphor-python-0.1.6/setup.cfg
+-rw-r--r--   0 jwang      (501) staff       (20)      773 2023-07-25 07:53:54.000000 metaphor-python-0.1.6/setup.py
```

### Comparing `metaphor-python-0.1.5/PKG-INFO` & `metaphor-python-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaphor-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python package for the Metaphor API.
 Home-page: https://github.com/metaphorsystems/metaphor-python
 Author: Metaphor
 Author-email: hello@metaphor.systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metaphor-python-0.1.5/README.md` & `metaphor-python-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `metaphor-python-0.1.5/metaphor_python/api.py` & `metaphor-python-0.1.6/metaphor_python/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     include_domains: Optional[List[str]] = None
     exclude_domains: Optional[List[str]] = None
     start_crawl_date: Optional[str] = None
     end_crawl_date: Optional[str] = None
     start_published_date: Optional[str] = None
     end_published_date: Optional[str] = None
     use_autoprompt: Optional[bool] = None
-    type: Optional[str] = None
+    type: Optional[str] = None # keyword or neural. Default is neural.
 
 @dataclass
 class Result:
     title: str
     url: str
     score: float
     id: str
```

### Comparing `metaphor-python-0.1.5/metaphor_python.egg-info/PKG-INFO` & `metaphor-python-0.1.6/metaphor_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaphor-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python package for the Metaphor API.
 Home-page: https://github.com/metaphorsystems/metaphor-python
 Author: Metaphor
 Author-email: hello@metaphor.systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metaphor-python-0.1.5/setup.py` & `metaphor-python-0.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metaphor-python',
-    version='0.1.5',
+    version='0.1.6',
     description='A Python package for the Metaphor API.',
     author='Metaphor',
     author_email='hello@metaphor.systems',
     url='https://github.com/metaphorsystems/metaphor-python',
     packages=find_packages(),
     install_requires=[
         'requests',
```

