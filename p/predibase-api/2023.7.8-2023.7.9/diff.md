# Comparing `tmp/predibase-api-2023.7.8.tar.gz` & `tmp/predibase-api-2023.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predibase-api-2023.7.8.tar", last modified: Tue Jul 18 20:04:23 2023, max compression
+gzip compressed data, was "predibase-api-2023.7.9.tar", last modified: Wed Jul 19 04:40:19 2023, max compression
```

## Comparing `predibase-api-2023.7.8.tar` & `predibase-api-2023.7.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:23.867298 predibase-api-2023.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-18 20:04:23.867298 predibase-api-2023.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:23.859298 predibase-api-2023.7.8/predibase_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:23.863298 predibase-api-2023.7.8/predibase_api/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/artifacts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:23.863298 predibase-api-2023.7.8/predibase_api/artifacts/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/artifacts/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/artifacts/v1/artifacts_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:23.863298 predibase-api-2023.7.8/predibase_api/foobar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/foobar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:23.863298 predibase-api-2023.7.8/predibase_api/foobar/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/foobar/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/foobar/v1/bar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/foobar/v1/foo_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:23.863298 predibase-api-2023.7.8/predibase_api/iterml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/iterml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:23.863298 predibase-api-2023.7.8/predibase_api/iterml/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/iterml/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/iterml/v1/iterml_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:23.863298 predibase-api-2023.7.8/predibase_api/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/profiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:23.867298 predibase-api-2023.7.8/predibase_api/profiles/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/profiles/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/profiles/v1/dataset_profile_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:23.867298 predibase-api-2023.7.8/predibase_api/tenants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/tenants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:23.867298 predibase-api-2023.7.8/predibase_api/tenants/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/tenants/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/predibase_api/tenants/v1/tenants_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:23.863298 predibase-api-2023.7.8/predibase_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-18 20:04:23.000000 predibase-api-2023.7.8/predibase_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-18 20:04:23.000000 predibase-api-2023.7.8/predibase_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:04:23.000000 predibase-api-2023.7.8/predibase_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:04:00.000000 predibase-api-2023.7.8/predibase_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 20:04:23.000000 predibase-api-2023.7.8/predibase_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 20:04:23.000000 predibase-api-2023.7.8/predibase_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 20:04:23.867298 predibase-api-2023.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-18 20:03:33.000000 predibase-api-2023.7.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 20:04:18.000000 predibase-api-2023.7.8/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.623283 predibase-api-2023.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-19 04:40:19.623283 predibase-api-2023.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/artifacts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/artifacts/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/artifacts/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/artifacts/v1/artifacts_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/foobar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/foobar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/foobar/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/foobar/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/foobar/v1/bar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/foobar/v1/foo_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/iterml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/iterml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/iterml/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/iterml/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/iterml/v1/iterml_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/profiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.623283 predibase-api-2023.7.9/predibase_api/profiles/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/profiles/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/profiles/v1/dataset_profile_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.623283 predibase-api-2023.7.9/predibase_api/tenants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/tenants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.623283 predibase-api-2023.7.9/predibase_api/tenants/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/tenants/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/predibase_api/tenants/v1/tenants_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.619283 predibase-api-2023.7.9/predibase_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-19 04:40:19.000000 predibase-api-2023.7.9/predibase_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-19 04:40:19.000000 predibase-api-2023.7.9/predibase_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 04:40:19.000000 predibase-api-2023.7.9/predibase_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 04:39:48.000000 predibase-api-2023.7.9/predibase_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 04:40:19.000000 predibase-api-2023.7.9/predibase_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 04:40:19.000000 predibase-api-2023.7.9/predibase_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 04:40:19.623283 predibase-api-2023.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-19 04:39:16.000000 predibase-api-2023.7.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 04:40:06.000000 predibase-api-2023.7.9/version.txt
```

### Comparing `predibase-api-2023.7.8/predibase_api/artifacts/v1/artifacts_pb2.py` & `predibase-api-2023.7.9/predibase_api/artifacts/v1/artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.8/predibase_api/foobar/v1/bar_pb2.py` & `predibase-api-2023.7.9/predibase_api/foobar/v1/bar_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.8/predibase_api/foobar/v1/foo_pb2.py` & `predibase-api-2023.7.9/predibase_api/foobar/v1/foo_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.8/predibase_api/iterml/v1/iterml_pb2.py` & `predibase-api-2023.7.9/predibase_api/iterml/v1/iterml_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.8/predibase_api/profiles/v1/dataset_profile_pb2.py` & `predibase-api-2023.7.9/predibase_api/profiles/v1/dataset_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.8/predibase_api/tenants/v1/tenants_pb2.py` & `predibase-api-2023.7.9/predibase_api/tenants/v1/tenants_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.8/predibase_api.egg-info/SOURCES.txt` & `predibase-api-2023.7.9/predibase_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.8/setup.py` & `predibase-api-2023.7.9/setup.py`

 * *Files identical despite different names*

