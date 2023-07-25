# Comparing `tmp/merkle-py-1.2.3.tar.gz` & `tmp/merkle-py-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merkle-py-1.2.3.tar", last modified: Tue May 30 08:00:57 2023, max compression
+gzip compressed data, was "merkle-py-1.2.4.tar", last modified: Tue Jul 25 08:28:42 2023, max compression
```

## Comparing `merkle-py-1.2.3.tar` & `merkle-py-1.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-05-30 08:00:57.572085 merkle-py-1.2.3/
--rw-r--r--   0 cyrildever   (501) staff       (20)       19 2022-03-21 11:01:19.000000 merkle-py-1.2.3/MANIFEST.in
--rw-r--r--   0 cyrildever   (501) staff       (20)     3323 2023-05-30 08:00:57.571821 merkle-py-1.2.3/PKG-INFO
--rw-r--r--   0 cyrildever   (501) staff       (20)     2817 2023-04-17 07:08:41.000000 merkle-py-1.2.3/README.md
--rw-r--r--   0 cyrildever   (501) staff       (20)      103 2022-03-21 11:01:19.000000 merkle-py-1.2.3/pyproject.toml
--rw-r--r--   0 cyrildever   (501) staff       (20)       38 2023-05-30 08:00:57.572154 merkle-py-1.2.3/setup.cfg
--rw-r--r--   0 cyrildever   (501) staff       (20)      902 2023-05-30 07:57:30.000000 merkle-py-1.2.3/setup.py
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-05-30 08:00:57.561236 merkle-py-1.2.3/src/
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-05-30 08:00:57.563586 merkle-py-1.2.3/src/merkle_py.egg-info/
--rw-r--r--   0 cyrildever   (501) staff       (20)     3323 2023-05-30 08:00:57.000000 merkle-py-1.2.3/src/merkle_py.egg-info/PKG-INFO
--rw-r--r--   0 cyrildever   (501) staff       (20)      452 2023-05-30 08:00:57.000000 merkle-py-1.2.3/src/merkle_py.egg-info/SOURCES.txt
--rw-r--r--   0 cyrildever   (501) staff       (20)        1 2023-05-30 08:00:57.000000 merkle-py-1.2.3/src/merkle_py.egg-info/dependency_links.txt
--rw-r--r--   0 cyrildever   (501) staff       (20)        9 2023-05-30 08:00:57.000000 merkle-py-1.2.3/src/merkle_py.egg-info/top_level.txt
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-05-30 08:00:57.568740 merkle-py-1.2.3/src/merklepy/
--rw-r--r--   0 cyrildever   (501) staff       (20)        0 2022-03-21 11:01:19.000000 merkle-py-1.2.3/src/merklepy/__init__.py
--rw-r--r--   0 cyrildever   (501) staff       (20)      657 2022-04-04 08:47:17.000000 merkle-py-1.2.3/src/merklepy/exception.py
--rw-r--r--   0 cyrildever   (501) staff       (20)      971 2022-04-04 08:47:17.000000 merkle-py-1.2.3/src/merklepy/hash.py
--rw-r--r--   0 cyrildever   (501) staff       (20)      843 2022-04-04 08:47:17.000000 merkle-py-1.2.3/src/merklepy/options.py
--rw-r--r--   0 cyrildever   (501) staff       (20)     1207 2022-04-04 08:47:17.000000 merkle-py-1.2.3/src/merklepy/path.py
--rw-r--r--   0 cyrildever   (501) staff       (20)     2287 2022-04-04 10:31:42.000000 merkle-py-1.2.3/src/merklepy/proof.py
--rw-r--r--   0 cyrildever   (501) staff       (20)     6813 2022-04-04 08:47:17.000000 merkle-py-1.2.3/src/merklepy/tree.py
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-05-30 08:00:57.571296 merkle-py-1.2.3/tests/
--rw-r--r--   0 cyrildever   (501) staff       (20)     2319 2022-04-04 08:47:17.000000 merkle-py-1.2.3/tests/test_hash.py
--rw-r--r--   0 cyrildever   (501) staff       (20)      523 2022-04-04 08:47:17.000000 merkle-py-1.2.3/tests/test_options.py
--rw-r--r--   0 cyrildever   (501) staff       (20)      875 2022-04-04 08:47:17.000000 merkle-py-1.2.3/tests/test_path.py
--rw-r--r--   0 cyrildever   (501) staff       (20)     1749 2022-04-04 08:47:17.000000 merkle-py-1.2.3/tests/test_proof.py
--rw-r--r--   0 cyrildever   (501) staff       (20)     5595 2022-04-04 08:47:17.000000 merkle-py-1.2.3/tests/test_tree.py
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-07-25 08:28:42.872265 merkle-py-1.2.4/
+-rw-r--r--   0 cyrildever   (501) staff       (20)       19 2022-03-21 11:17:45.000000 merkle-py-1.2.4/MANIFEST.in
+-rw-r--r--   0 cyrildever   (501) staff       (20)     3323 2023-07-25 08:28:42.871817 merkle-py-1.2.4/PKG-INFO
+-rw-r--r--   0 cyrildever   (501) staff       (20)     2817 2023-05-18 10:49:41.000000 merkle-py-1.2.4/README.md
+-rw-r--r--   0 cyrildever   (501) staff       (20)      103 2022-03-21 11:17:45.000000 merkle-py-1.2.4/pyproject.toml
+-rw-r--r--   0 cyrildever   (501) staff       (20)       38 2023-07-25 08:28:42.872367 merkle-py-1.2.4/setup.cfg
+-rw-r--r--   0 cyrildever   (501) staff       (20)      902 2023-07-25 08:27:13.000000 merkle-py-1.2.4/setup.py
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-07-25 08:28:42.858145 merkle-py-1.2.4/src/
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-07-25 08:28:42.861628 merkle-py-1.2.4/src/merkle_py.egg-info/
+-rw-r--r--   0 cyrildever   (501) staff       (20)     3323 2023-07-25 08:28:42.000000 merkle-py-1.2.4/src/merkle_py.egg-info/PKG-INFO
+-rw-r--r--   0 cyrildever   (501) staff       (20)      452 2023-07-25 08:28:42.000000 merkle-py-1.2.4/src/merkle_py.egg-info/SOURCES.txt
+-rw-r--r--   0 cyrildever   (501) staff       (20)        1 2023-07-25 08:28:42.000000 merkle-py-1.2.4/src/merkle_py.egg-info/dependency_links.txt
+-rw-r--r--   0 cyrildever   (501) staff       (20)        9 2023-07-25 08:28:42.000000 merkle-py-1.2.4/src/merkle_py.egg-info/top_level.txt
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-07-25 08:28:42.867109 merkle-py-1.2.4/src/merklepy/
+-rw-r--r--   0 cyrildever   (501) staff       (20)        0 2022-03-21 11:17:45.000000 merkle-py-1.2.4/src/merklepy/__init__.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)      657 2022-04-04 08:42:25.000000 merkle-py-1.2.4/src/merklepy/exception.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)      971 2022-04-04 08:42:25.000000 merkle-py-1.2.4/src/merklepy/hash.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)      843 2022-04-04 08:42:25.000000 merkle-py-1.2.4/src/merklepy/options.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)     1207 2022-04-04 08:42:25.000000 merkle-py-1.2.4/src/merklepy/path.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)     2287 2022-04-04 10:32:55.000000 merkle-py-1.2.4/src/merklepy/proof.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)     6813 2022-04-04 08:42:25.000000 merkle-py-1.2.4/src/merklepy/tree.py
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-07-25 08:28:42.871151 merkle-py-1.2.4/tests/
+-rw-r--r--   0 cyrildever   (501) staff       (20)     2319 2022-04-04 08:42:25.000000 merkle-py-1.2.4/tests/test_hash.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)      523 2022-04-04 08:42:25.000000 merkle-py-1.2.4/tests/test_options.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)      875 2022-04-04 08:42:25.000000 merkle-py-1.2.4/tests/test_path.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)     1749 2022-04-04 08:42:25.000000 merkle-py-1.2.4/tests/test_proof.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)     5595 2022-04-04 08:42:25.000000 merkle-py-1.2.4/tests/test_tree.py
```

### Comparing `merkle-py-1.2.3/PKG-INFO` & `merkle-py-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merkle-py
-Version: 1.2.3
+Version: 1.2.4
 Summary: Merkle tree for Python
 Home-page: https://github.com/cyrildever/merkle-trees/tree/master/packages/py
 Author: Cyril Dever
 Project-URL: Bug Tracker, https://github.com/cyrildever/merkle-trees/issues
 Keywords: python,merkle-tree,merkle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `merkle-py-1.2.3/README.md` & `merkle-py-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.3/setup.py` & `merkle-py-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="merkle-py",
-    version="1.2.3",
+    version="1.2.4",
     author="Cyril Dever",
     author_mail="cdever@pep-s.com",
     description="Merkle tree for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cyrildever/merkle-trees/tree/master/packages/py",
     project_urls={
```

### Comparing `merkle-py-1.2.3/src/merkle_py.egg-info/PKG-INFO` & `merkle-py-1.2.4/src/merkle_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merkle-py
-Version: 1.2.3
+Version: 1.2.4
 Summary: Merkle tree for Python
 Home-page: https://github.com/cyrildever/merkle-trees/tree/master/packages/py
 Author: Cyril Dever
 Project-URL: Bug Tracker, https://github.com/cyrildever/merkle-trees/issues
 Keywords: python,merkle-tree,merkle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `merkle-py-1.2.3/src/merklepy/exception.py` & `merkle-py-1.2.4/src/merklepy/exception.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.3/src/merklepy/hash.py` & `merkle-py-1.2.4/src/merklepy/hash.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.3/src/merklepy/options.py` & `merkle-py-1.2.4/src/merklepy/options.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.3/src/merklepy/path.py` & `merkle-py-1.2.4/src/merklepy/path.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.3/src/merklepy/proof.py` & `merkle-py-1.2.4/src/merklepy/proof.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.3/src/merklepy/tree.py` & `merkle-py-1.2.4/src/merklepy/tree.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.3/tests/test_hash.py` & `merkle-py-1.2.4/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.3/tests/test_options.py` & `merkle-py-1.2.4/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.3/tests/test_path.py` & `merkle-py-1.2.4/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.3/tests/test_proof.py` & `merkle-py-1.2.4/tests/test_proof.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.3/tests/test_tree.py` & `merkle-py-1.2.4/tests/test_tree.py`

 * *Files identical despite different names*

