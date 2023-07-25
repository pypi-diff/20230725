# Comparing `tmp/sanic-testing-23.3.0.tar.gz` & `tmp/sanic-testing-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanic-testing-23.3.0.tar", last modified: Sun Mar 26 12:00:16 2023, max compression
+gzip compressed data, was "sanic-testing-23.6.0.tar", last modified: Tue Jul 25 09:45:05 2023, max compression
```

## Comparing `sanic-testing-23.3.0.tar` & `sanic-testing-23.6.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:00:16.919355 sanic-testing-23.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-26 12:00:04.000000 sanic-testing-23.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-03-26 12:00:16.919355 sanic-testing-23.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-26 12:00:04.000000 sanic-testing-23.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:00:16.919355 sanic-testing-23.3.0/sanic_testing/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-26 12:00:04.000000 sanic-testing-23.3.0/sanic_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-26 12:00:04.000000 sanic-testing-23.3.0/sanic_testing/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-03-26 12:00:04.000000 sanic-testing-23.3.0/sanic_testing/reusable.py
--rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-03-26 12:00:04.000000 sanic-testing-23.3.0/sanic_testing/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-26 12:00:04.000000 sanic-testing-23.3.0/sanic_testing/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:00:16.919355 sanic-testing-23.3.0/sanic_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-03-26 12:00:16.000000 sanic-testing-23.3.0/sanic_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-26 12:00:16.000000 sanic-testing-23.3.0/sanic_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 12:00:16.000000 sanic-testing-23.3.0/sanic_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-26 12:00:16.000000 sanic-testing-23.3.0/sanic_testing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-26 12:00:16.000000 sanic-testing-23.3.0/sanic_testing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 12:00:16.919355 sanic-testing-23.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-26 12:00:04.000000 sanic-testing-23.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:45:05.366941 sanic-testing-23.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-25 09:44:54.000000 sanic-testing-23.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-25 09:45:05.366941 sanic-testing-23.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-25 09:44:54.000000 sanic-testing-23.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:45:05.362941 sanic-testing-23.6.0/sanic_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-25 09:44:54.000000 sanic-testing-23.6.0/sanic_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-25 09:44:54.000000 sanic-testing-23.6.0/sanic_testing/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-07-25 09:44:54.000000 sanic-testing-23.6.0/sanic_testing/reusable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-07-25 09:44:54.000000 sanic-testing-23.6.0/sanic_testing/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-25 09:44:54.000000 sanic-testing-23.6.0/sanic_testing/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:45:05.366941 sanic-testing-23.6.0/sanic_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-25 09:45:05.000000 sanic-testing-23.6.0/sanic_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-25 09:45:05.000000 sanic-testing-23.6.0/sanic_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:45:05.000000 sanic-testing-23.6.0/sanic_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 09:45:05.000000 sanic-testing-23.6.0/sanic_testing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 09:45:05.000000 sanic-testing-23.6.0/sanic_testing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:45:05.366941 sanic-testing-23.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-25 09:44:54.000000 sanic-testing-23.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:45:05.366941 sanic-testing-23.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-25 09:44:54.000000 sanic-testing-23.6.0/tests/test_asgi_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-25 09:44:54.000000 sanic-testing-23.6.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-25 09:44:54.000000 sanic-testing-23.6.0/tests/test_test_client.py
```

### Comparing `sanic-testing-23.3.0/LICENSE` & `sanic-testing-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sanic-testing-23.3.0/PKG-INFO` & `sanic-testing-23.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: sanic-testing
-Version: 23.3.0
+Version: 23.6.0
 Summary: Core testing clients for Sanic
 Home-page: https://github.com/sanic-org/sanic-testing/
 Author: Adam Hopkins
 Author-email: admhpkns@gmail.com
 License: MIT
 Platform: any
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sanic Core Test
 
 This package is meant to be the core testing utility and clients for testing Sanic applications. It is mainly derived from `sanic.testing` which has (or will be) removed from the main Sanic repository in the future.
```

### Comparing `sanic-testing-23.3.0/README.md` & `sanic-testing-23.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sanic-testing-23.3.0/sanic_testing/reusable.py` & `sanic-testing-23.6.0/sanic_testing/reusable.py`

 * *Files identical despite different names*

### Comparing `sanic-testing-23.3.0/sanic_testing/testing.py` & `sanic-testing-23.6.0/sanic_testing/testing.py`

 * *Files identical despite different names*

### Comparing `sanic-testing-23.3.0/sanic_testing/websocket.py` & `sanic-testing-23.6.0/sanic_testing/websocket.py`

 * *Files identical despite different names*

### Comparing `sanic-testing-23.3.0/sanic_testing.egg-info/PKG-INFO` & `sanic-testing-23.6.0/sanic_testing.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: sanic-testing
-Version: 23.3.0
+Version: 23.6.0
 Summary: Core testing clients for Sanic
 Home-page: https://github.com/sanic-org/sanic-testing/
 Author: Adam Hopkins
 Author-email: admhpkns@gmail.com
 License: MIT
 Platform: any
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sanic Core Test
 
 This package is meant to be the core testing utility and clients for testing Sanic applications. It is mainly derived from `sanic.testing` which has (or will be) removed from the main Sanic repository in the future.
```

### Comparing `sanic-testing-23.3.0/setup.py` & `sanic-testing-23.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,23 +34,23 @@
     "author_email": "admhpkns@gmail.com",
     "description": ("Core testing clients for Sanic"),
     "long_description": long_description,
     "long_description_content_type": "text/markdown",
     "packages": ["sanic_testing"],
     "platforms": "any",
     "classifiers": [
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 }
-requirements = ["httpx>=0.18,<0.24"]
+requirements = ["httpx>=0.18"]
 
 tests_require = ["pytest", "sanic>=22.12", "pytest-asyncio"]
 
 setup_kwargs["install_requires"] = requirements
 setup_kwargs["tests_require"] = tests_require
 setup(**setup_kwargs)
```

