# Comparing `tmp/apify_shared-1.0.0b1.tar.gz` & `tmp/apify_shared-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_shared-1.0.0b1.tar", last modified: Tue Jul 25 10:55:17 2023, max compression
+gzip compressed data, was "apify_shared-1.0.0b2.tar", last modified: Tue Jul 25 11:04:23 2023, max compression
```

## Comparing `apify_shared-1.0.0b1.tar` & `apify_shared-1.0.0b2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 fn         (501) staff       (20)        0 2023-07-25 10:55:17.611444 apify_shared-1.0.0b1/
--rw-r--r--   0 fn         (501) staff       (20)    11355 2023-07-25 09:57:25.000000 apify_shared-1.0.0b1/LICENSE
--rw-r--r--   0 fn         (501) staff       (20)     1744 2023-07-25 10:55:17.611322 apify_shared-1.0.0b1/PKG-INFO
--rw-r--r--   0 fn         (501) staff       (20)      625 2023-07-24 13:23:38.000000 apify_shared-1.0.0b1/README.md
--rw-r--r--   0 fn         (501) staff       (20)     2028 2023-07-25 10:50:42.000000 apify_shared-1.0.0b1/pyproject.toml
--rw-r--r--   0 fn         (501) staff       (20)       38 2023-07-25 10:55:17.611493 apify_shared-1.0.0b1/setup.cfg
-drwxr-xr-x   0 fn         (501) staff       (20)        0 2023-07-25 10:55:17.609393 apify_shared-1.0.0b1/src/
-drwxr-xr-x   0 fn         (501) staff       (20)        0 2023-07-25 10:55:17.610417 apify_shared-1.0.0b1/src/apify_shared/
--rw-r--r--   0 fn         (501) staff       (20)       79 2023-07-21 13:03:58.000000 apify_shared-1.0.0b1/src/apify_shared/__init__.py
--rw-r--r--   0 fn         (501) staff       (20)     9324 2023-07-21 13:03:58.000000 apify_shared-1.0.0b1/src/apify_shared/consts.py
--rw-r--r--   0 fn         (501) staff       (20)        0 2023-07-21 13:03:58.000000 apify_shared-1.0.0b1/src/apify_shared/py.typed
--rw-r--r--   0 fn         (501) staff       (20)      405 2023-07-21 13:03:58.000000 apify_shared-1.0.0b1/src/apify_shared/types.py
--rw-r--r--   0 fn         (501) staff       (20)     3974 2023-07-25 07:24:44.000000 apify_shared-1.0.0b1/src/apify_shared/utils.py
-drwxr-xr-x   0 fn         (501) staff       (20)        0 2023-07-25 10:55:17.611148 apify_shared-1.0.0b1/src/apify_shared.egg-info/
--rw-r--r--   0 fn         (501) staff       (20)     1744 2023-07-25 10:55:17.000000 apify_shared-1.0.0b1/src/apify_shared.egg-info/PKG-INFO
--rw-r--r--   0 fn         (501) staff       (20)      365 2023-07-25 10:55:17.000000 apify_shared-1.0.0b1/src/apify_shared.egg-info/SOURCES.txt
--rw-r--r--   0 fn         (501) staff       (20)        1 2023-07-25 10:55:17.000000 apify_shared-1.0.0b1/src/apify_shared.egg-info/dependency_links.txt
--rw-r--r--   0 fn         (501) staff       (20)      518 2023-07-25 10:55:17.000000 apify_shared-1.0.0b1/src/apify_shared.egg-info/requires.txt
--rw-r--r--   0 fn         (501) staff       (20)       13 2023-07-25 10:55:17.000000 apify_shared-1.0.0b1/src/apify_shared.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:04:23.951278 apify_shared-1.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-25 11:03:56.000000 apify_shared-1.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-25 11:04:23.951278 apify_shared-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-25 11:03:56.000000 apify_shared-1.0.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-25 11:04:20.000000 apify_shared-1.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 11:04:23.951278 apify_shared-1.0.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:04:23.951278 apify_shared-1.0.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:04:23.951278 apify_shared-1.0.0b2/src/apify_shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 11:03:56.000000 apify_shared-1.0.0b2/src/apify_shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-07-25 11:03:56.000000 apify_shared-1.0.0b2/src/apify_shared/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:03:56.000000 apify_shared-1.0.0b2/src/apify_shared/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-25 11:03:56.000000 apify_shared-1.0.0b2/src/apify_shared/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-25 11:03:56.000000 apify_shared-1.0.0b2/src/apify_shared/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:04:23.951278 apify_shared-1.0.0b2/src/apify_shared.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-25 11:04:23.000000 apify_shared-1.0.0b2/src/apify_shared.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-25 11:04:23.000000 apify_shared-1.0.0b2/src/apify_shared.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:04:23.000000 apify_shared-1.0.0b2/src/apify_shared.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-25 11:04:23.000000 apify_shared-1.0.0b2/src/apify_shared.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 11:04:23.000000 apify_shared-1.0.0b2/src/apify_shared.egg-info/top_level.txt
```

### Comparing `apify_shared-1.0.0b1/LICENSE` & `apify_shared-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.0b1/PKG-INFO` & `apify_shared-1.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_shared
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Tools and constants shared across Apify projects.
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Apify Homepage, https://apify.com
 Project-URL: Changelog, https://github.com/apify/apify-shared-python/blob/master/CHANGELOG.md
 Project-URL: Issue tracker, https://github.com/apify/apify-shared-python/issues
 Project-URL: Source, https://github.com/apify/apify-shared-python
```

### Comparing `apify_shared-1.0.0b1/README.md` & `apify_shared-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.0b1/pyproject.toml` & `apify_shared-1.0.0b2/pyproject.toml`

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
-version = "1.0.0b1"
+version = "1.0.0b2"
 
 [project.optional-dependencies]
 dev = [
   "autopep8 ~= 2.0.2",
   "build ~= 0.10.0",
   "flake8 ~= 6.0.0",
   "flake8-bugbear ~= 23.5.9",
```

### Comparing `apify_shared-1.0.0b1/src/apify_shared/consts.py` & `apify_shared-1.0.0b2/src/apify_shared/consts.py`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.0b1/src/apify_shared/utils.py` & `apify_shared-1.0.0b2/src/apify_shared/utils.py`

 * *Files identical despite different names*

### Comparing `apify_shared-1.0.0b1/src/apify_shared.egg-info/PKG-INFO` & `apify_shared-1.0.0b2/src/apify_shared.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify-shared
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Tools and constants shared across Apify projects.
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Apify Homepage, https://apify.com
 Project-URL: Changelog, https://github.com/apify/apify-shared-python/blob/master/CHANGELOG.md
 Project-URL: Issue tracker, https://github.com/apify/apify-shared-python/issues
 Project-URL: Source, https://github.com/apify/apify-shared-python
```

### Comparing `apify_shared-1.0.0b1/src/apify_shared.egg-info/requires.txt` & `apify_shared-1.0.0b2/src/apify_shared.egg-info/requires.txt`

 * *Files identical despite different names*

