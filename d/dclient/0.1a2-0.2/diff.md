# Comparing `tmp/dclient-0.1a2.tar.gz` & `tmp/dclient-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dclient-0.1a2.tar", last modified: Tue Nov 22 05:40:26 2022, max compression
+gzip compressed data, was "dclient-0.2.tar", last modified: Mon Jul 24 23:27:07 2023, max compression
```

## Comparing `dclient-0.1a2.tar` & `dclient-0.2.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 05:40:26.033717 dclient-0.1a2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-22 05:39:57.000000 dclient-0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5008 2022-11-22 05:40:26.033717 dclient-0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4503 2022-11-22 05:39:57.000000 dclient-0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 05:40:26.029716 dclient-0.1a2/dclient/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-22 05:39:57.000000 dclient-0.1a2/dclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-22 05:39:57.000000 dclient-0.1a2/dclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2022-11-22 05:39:57.000000 dclient-0.1a2/dclient/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-11-22 05:39:57.000000 dclient-0.1a2/dclient/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 05:40:26.033717 dclient-0.1a2/dclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5008 2022-11-22 05:40:26.000000 dclient-0.1a2/dclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-11-22 05:40:26.000000 dclient-0.1a2/dclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 05:40:26.000000 dclient-0.1a2/dclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-22 05:40:26.000000 dclient-0.1a2/dclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-11-22 05:40:26.000000 dclient-0.1a2/dclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-22 05:40:26.000000 dclient-0.1a2/dclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-22 05:40:26.033717 dclient-0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-11-22 05:39:57.000000 dclient-0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:27:07.825789 dclient-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 23:26:51.000000 dclient-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-24 23:27:07.825789 dclient-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-24 23:26:51.000000 dclient-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:27:07.821789 dclient-0.2/dclient/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 23:26:51.000000 dclient-0.2/dclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-24 23:26:51.000000 dclient-0.2/dclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-07-24 23:26:51.000000 dclient-0.2/dclient/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 23:26:51.000000 dclient-0.2/dclient/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-24 23:26:51.000000 dclient-0.2/dclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:27:07.825789 dclient-0.2/dclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-24 23:27:07.000000 dclient-0.2/dclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-24 23:27:07.000000 dclient-0.2/dclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 23:27:07.000000 dclient-0.2/dclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 23:27:07.000000 dclient-0.2/dclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-24 23:27:07.000000 dclient-0.2/dclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 23:27:07.000000 dclient-0.2/dclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 23:27:07.825789 dclient-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-24 23:26:51.000000 dclient-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:27:07.825789 dclient-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-24 23:26:51.000000 dclient-0.2/tests/test_cli_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-24 23:26:51.000000 dclient-0.2/tests/test_datasette_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-24 23:26:51.000000 dclient-0.2/tests/test_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-24 23:26:51.000000 dclient-0.2/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-24 23:26:51.000000 dclient-0.2/tests/test_utils.py
```

### Comparing `dclient-0.1a2/LICENSE` & `dclient-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dclient-0.1a2/setup.py` & `dclient-0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.1a2"
+VERSION = "0.2"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -27,11 +27,20 @@
     license="Apache License, Version 2.0",
     version=VERSION,
     packages=["dclient"],
     entry_points={
         "datasette": ["client = dclient.plugin"],
         "console_scripts": ["dclient = dclient.cli:cli"],
     },
-    install_requires=["click", "httpx", "appdirs"],
-    extras_require={"test": ["pytest", "pytest-httpx", "cogapp", "pytest-mock"]},
+    install_requires=["click", "httpx", "sqlite-utils"],
+    extras_require={
+        "test": [
+            "pytest",
+            "pytest-asyncio",
+            "pytest-httpx",
+            "cogapp",
+            "pytest-mock",
+            "datasette>=1.0a2",
+        ]
+    },
     python_requires=">=3.7",
 )
```

