# Comparing `tmp/scratch-getdata-1.0.6.tar.gz` & `tmp/scratch-getdata-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratch-getdata-1.0.6.tar", last modified: Tue Jul 25 19:34:25 2023, max compression
+gzip compressed data, was "scratch-getdata-1.0.7.tar", last modified: Tue Jul 25 20:56:52 2023, max compression
```

## Comparing `scratch-getdata-1.0.6.tar` & `scratch-getdata-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-25 19:34:25.406927 scratch-getdata-1.0.6/
--rw-r--r--   0 runner    (1000) runner    (1000)     2975 2023-07-25 19:34:25.406927 scratch-getdata-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     2387 2023-07-25 19:32:03.000000 scratch-getdata-1.0.6/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      686 2023-07-25 19:32:57.000000 scratch-getdata-1.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-25 19:34:25.406927 scratch-getdata-1.0.6/scratch_getdata/
--rw-r--r--   0 runner    (1000) runner    (1000)      517 2023-07-25 19:32:23.000000 scratch-getdata-1.0.6/scratch_getdata/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4214 2023-07-25 19:30:04.000000 scratch-getdata-1.0.6/scratch_getdata/api_client.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-25 19:34:25.406927 scratch-getdata-1.0.6/scratch_getdata.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2975 2023-07-25 19:34:24.000000 scratch-getdata-1.0.6/scratch_getdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      285 2023-07-25 19:34:24.000000 scratch-getdata-1.0.6/scratch_getdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-25 19:34:24.000000 scratch-getdata-1.0.6/scratch_getdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-25 19:34:24.000000 scratch-getdata-1.0.6/scratch_getdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2023-07-25 19:34:24.000000 scratch-getdata-1.0.6/scratch_getdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-25 19:34:25.406927 scratch-getdata-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-28 02:32:47.000000 scratch-getdata-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-25 20:56:52.475944 scratch-getdata-1.0.7/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2987 2023-07-25 20:56:52.475944 scratch-getdata-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2387 2023-07-25 19:32:03.000000 scratch-getdata-1.0.7/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      698 2023-07-25 20:56:17.000000 scratch-getdata-1.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-25 20:56:52.471944 scratch-getdata-1.0.7/scratch_getdata/
+-rw-r--r--   0 runner    (1000) runner    (1000)      517 2023-07-25 19:32:23.000000 scratch-getdata-1.0.7/scratch_getdata/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4214 2023-07-25 19:30:04.000000 scratch-getdata-1.0.7/scratch_getdata/api_client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-25 20:56:52.475944 scratch-getdata-1.0.7/scratch_getdata.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2987 2023-07-25 20:56:52.000000 scratch-getdata-1.0.7/scratch_getdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      285 2023-07-25 20:56:52.000000 scratch-getdata-1.0.7/scratch_getdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-25 20:56:52.000000 scratch-getdata-1.0.7/scratch_getdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-25 20:56:52.000000 scratch-getdata-1.0.7/scratch_getdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2023-07-25 20:56:52.000000 scratch-getdata-1.0.7/scratch_getdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-25 20:56:52.479945 scratch-getdata-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-28 02:32:47.000000 scratch-getdata-1.0.7/setup.py
```

### Comparing `scratch-getdata-1.0.6/PKG-INFO` & `scratch-getdata-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: scratch-getdata
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Module to fetch scratch things from ScratchGetData
 Author: kokofixcomputers
 Author-email: kokofixcomputers <kokocanfixit@kokofixcomputers.serv00.net>
-Project-URL: Github, https://github.com/kokofixcomputers/Scratch-getdata
-Project-URL: Bug Tracker, https://github.com/kokofixcomputers/Scratch-getdata/issues
+Project-URL: Github, https://github.com/scratch-getdata/scratch-getdata-python
+Project-URL: Bug Tracker, https://github.com/scratch-getdata/scratch-getdata-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ScratchAPIClient Documentation
```

### Comparing `scratch-getdata-1.0.6/README.md` & `scratch-getdata-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `scratch-getdata-1.0.6/pyproject.toml` & `scratch-getdata-1.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scratch-getdata"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="kokofixcomputers", email="kokocanfixit@kokofixcomputers.serv00.net" },
 ]
 dependencies = ['requests']
 description = "A Module to fetch scratch things from ScratchGetData"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Github" = "https://github.com/kokofixcomputers/Scratch-getdata"
-"Bug Tracker" = "https://github.com/kokofixcomputers/Scratch-getdata/issues"
+"Github" = "https://github.com/scratch-getdata/scratch-getdata-python"
+"Bug Tracker" = "https://github.com/scratch-getdata/scratch-getdata-python/issues"
```

### Comparing `scratch-getdata-1.0.6/scratch_getdata/__init__.py` & `scratch-getdata-1.0.7/scratch_getdata/__init__.py`

 * *Files identical despite different names*

### Comparing `scratch-getdata-1.0.6/scratch_getdata/api_client.py` & `scratch-getdata-1.0.7/scratch_getdata/api_client.py`

 * *Files identical despite different names*

### Comparing `scratch-getdata-1.0.6/scratch_getdata.egg-info/PKG-INFO` & `scratch-getdata-1.0.7/scratch_getdata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: scratch-getdata
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Module to fetch scratch things from ScratchGetData
 Author: kokofixcomputers
 Author-email: kokofixcomputers <kokocanfixit@kokofixcomputers.serv00.net>
-Project-URL: Github, https://github.com/kokofixcomputers/Scratch-getdata
-Project-URL: Bug Tracker, https://github.com/kokofixcomputers/Scratch-getdata/issues
+Project-URL: Github, https://github.com/scratch-getdata/scratch-getdata-python
+Project-URL: Bug Tracker, https://github.com/scratch-getdata/scratch-getdata-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ScratchAPIClient Documentation
```

