# Comparing `tmp/apify_shared-1.0.0b2.tar.gz` & `tmp/apify_shared-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_shared-1.0.0b2.tar", last modified: Tue Jul 25 11:04:23 2023, max compression
+gzip compressed data, was "apify_shared-1.0.0b3.tar", last modified: Tue Jul 25 14:42:52 2023, max compression
```

## Comparing `apify_shared-1.0.0b2.tar` & `apify_shared-1.0.0b3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:04:23.951278 apify_shared-1.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-25 11:03:56.000000 apify_shared-1.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-25 11:04:23.951278 apify_shared-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-25 11:03:56.000000 apify_shared-1.0.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-25 11:04:20.000000 apify_shared-1.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 11:04:23.951278 apify_shared-1.0.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:04:23.951278 apify_shared-1.0.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:04:23.951278 apify_shared-1.0.0b2/src/apify_shared/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 11:03:56.000000 apify_shared-1.0.0b2/src/apify_shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-07-25 11:03:56.000000 apify_shared-1.0.0b2/src/apify_shared/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:03:56.000000 apify_shared-1.0.0b2/src/apify_shared/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-25 11:03:56.000000 apify_shared-1.0.0b2/src/apify_shared/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-25 11:03:56.000000 apify_shared-1.0.0b2/src/apify_shared/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:04:23.951278 apify_shared-1.0.0b2/src/apify_shared.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-25 11:04:23.000000 apify_shared-1.0.0b2/src/apify_shared.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-25 11:04:23.000000 apify_shared-1.0.0b2/src/apify_shared.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:04:23.000000 apify_shared-1.0.0b2/src/apify_shared.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-25 11:04:23.000000 apify_shared-1.0.0b2/src/apify_shared.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 11:04:23.000000 apify_shared-1.0.0b2/src/apify_shared.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:42:52.412179 apify_shared-1.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-25 14:42:52.412179 apify_shared-1.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-25 14:42:48.000000 apify_shared-1.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:42:52.412179 apify_shared-1.0.0b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:42:52.412179 apify_shared-1.0.0b3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:42:52.412179 apify_shared-1.0.0b3/src/apify_shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/src/apify_shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/src/apify_shared/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/src/apify_shared/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/src/apify_shared/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/src/apify_shared/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-25 14:42:12.000000 apify_shared-1.0.0b3/src/apify_shared/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:42:52.412179 apify_shared-1.0.0b3/src/apify_shared.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-25 14:42:52.000000 apify_shared-1.0.0b3/src/apify_shared.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-25 14:42:52.000000 apify_shared-1.0.0b3/src/apify_shared.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:42:52.000000 apify_shared-1.0.0b3/src/apify_shared.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-25 14:42:52.000000 apify_shared-1.0.0b3/src/apify_shared.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 14:42:52.000000 apify_shared-1.0.0b3/src/apify_shared.egg-info/top_level.txt
```

### Comparing `apify_shared-1.0.0b2/LICENSE` & `apify_shared-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.0b2/PKG-INFO` & `apify_shared-1.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_shared
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Tools and constants shared across Apify projects.
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Apify Homepage, https://apify.com
 Project-URL: Changelog, https://github.com/apify/apify-shared-python/blob/master/CHANGELOG.md
 Project-URL: Issue tracker, https://github.com/apify/apify-shared-python/issues
 Project-URL: Source, https://github.com/apify/apify-shared-python
```

### Comparing `apify_shared-1.0.0b2/README.md` & `apify_shared-1.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.0b2/pyproject.toml` & `apify_shared-1.0.0b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 dependencies = []
 description = "Tools and constants shared across Apify projects."
 keywords = ["apify", "api", "shared", "scraping", "automation"]
 license = {text = "Apache Software License"}
 name = "apify_shared"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.0.0b2"
+version = "1.0.0b3"
 
 [project.optional-dependencies]
 dev = [
   "autopep8 ~= 2.0.2",
   "build ~= 0.10.0",
   "flake8 ~= 6.0.0",
   "flake8-bugbear ~= 23.5.9",
```

### Comparing `apify_shared-1.0.0b2/src/apify_shared/consts.py` & `apify_shared-1.0.0b3/src/apify_shared/consts.py`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.0b2/src/apify_shared/utils.py` & `apify_shared-1.0.0b3/src/apify_shared/utils.py`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.0b2/src/apify_shared.egg-info/PKG-INFO` & `apify_shared-1.0.0b3/src/apify_shared.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify-shared
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Tools and constants shared across Apify projects.
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Apify Homepage, https://apify.com
 Project-URL: Changelog, https://github.com/apify/apify-shared-python/blob/master/CHANGELOG.md
 Project-URL: Issue tracker, https://github.com/apify/apify-shared-python/issues
 Project-URL: Source, https://github.com/apify/apify-shared-python
```

### Comparing `apify_shared-1.0.0b2/src/apify_shared.egg-info/requires.txt` & `apify_shared-1.0.0b3/src/apify_shared.egg-info/requires.txt`

 * *Files identical despite different names*

