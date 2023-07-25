# Comparing `tmp/invenio-moodle-0.2.1.tar.gz` & `tmp/invenio-moodle-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-moodle-0.2.1.tar", last modified: Tue Jul 25 12:37:37 2023, max compression
+gzip compressed data, was "invenio-moodle-0.2.2.tar", last modified: Tue Jul 25 13:02:51 2023, max compression
```

## Comparing `invenio-moodle-0.2.1.tar` & `invenio-moodle-0.2.2.tar`

### file list

```diff
@@ -1,45 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:37:37.644982 invenio-moodle-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-25 12:37:37.644982 invenio-moodle-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:37:37.640982 invenio-moodle-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10163 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:37:37.640982 invenio-moodle-0.2.1/invenio_moodle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-25 12:37:37.000000 invenio-moodle-0.2.1/invenio_moodle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-25 12:37:37.000000 invenio-moodle-0.2.1/invenio_moodle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:37:37.000000 invenio-moodle-0.2.1/invenio_moodle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 12:37:37.000000 invenio-moodle-0.2.1/invenio_moodle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:37:37.000000 invenio-moodle-0.2.1/invenio_moodle.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-25 12:37:37.000000 invenio-moodle-0.2.1/invenio_moodle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:37:37.000000 invenio-moodle-0.2.1/invenio_moodle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-25 12:37:37.644982 invenio-moodle-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:37:37.640982 invenio-moodle-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:37:37.640982 invenio-moodle-0.2.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/tests/data/lom_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/tests/data/minimal_record.json
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/tests/test_invenio_moodle.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:02:51.335488 invenio-moodle-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-25 13:02:51.335488 invenio-moodle-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:02:51.331488 invenio-moodle-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10163 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:02:51.331488 invenio-moodle-0.2.2/invenio_moodle/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/invenio_moodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/invenio_moodle/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/invenio_moodle/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/invenio_moodle/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/invenio_moodle/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/invenio_moodle/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/invenio_moodle/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/invenio_moodle/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/invenio_moodle/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/invenio_moodle/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/invenio_moodle/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:02:51.331488 invenio-moodle-0.2.2/invenio_moodle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-25 13:02:51.000000 invenio-moodle-0.2.2/invenio_moodle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-25 13:02:51.000000 invenio-moodle-0.2.2/invenio_moodle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:02:51.000000 invenio-moodle-0.2.2/invenio_moodle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 13:02:51.000000 invenio-moodle-0.2.2/invenio_moodle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:02:51.000000 invenio-moodle-0.2.2/invenio_moodle.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-25 13:02:51.000000 invenio-moodle-0.2.2/invenio_moodle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 13:02:51.000000 invenio-moodle-0.2.2/invenio_moodle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-25 13:02:51.335488 invenio-moodle-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:02:51.335488 invenio-moodle-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:02:51.335488 invenio-moodle-0.2.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/tests/data/lom_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/tests/data/minimal_record.json
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/tests/test_invenio_moodle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-25 13:02:45.000000 invenio-moodle-0.2.2/tests/test_types.py
```

### Comparing `invenio-moodle-0.2.1/.editorconfig` & `invenio-moodle-0.2.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/CONTRIBUTING.rst` & `invenio-moodle-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/LICENSE` & `invenio-moodle-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/MANIFEST.in` & `invenio-moodle-0.2.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/PKG-INFO` & `invenio-moodle-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-moodle
-Version: 0.2.1
+Version: 0.2.2
 Summary: "Provides API for Moodle."
 Home-page: https://github.com/tu-graz-library/invenio-moodle
 Author: "Graz University of Technology"
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio_moodle invenio moodle teachcenter
 Platform: any
@@ -54,14 +54,19 @@
     invenio-moodle is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.2.2 (release 2023-07-25)
+
+- setup: fix typo, prevent correct build
+
+
 Version v0.2.1 (release 2023-07-25)
 
 - setup: change to reusable workflows
 
 
 Version v0.2.0 (release 2023-07-25)
```

### Comparing `invenio-moodle-0.2.1/README.rst` & `invenio-moodle-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/docs/conf.py` & `invenio-moodle-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/docs/index.rst` & `invenio-moodle-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/docs/make.bat` & `invenio-moodle-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/invenio_moodle.egg-info/PKG-INFO` & `invenio-moodle-0.2.2/invenio_moodle.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-moodle
-Version: 0.2.1
+Version: 0.2.2
 Summary: "Provides API for Moodle."
 Home-page: https://github.com/tu-graz-library/invenio-moodle
 Author: "Graz University of Technology"
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio_moodle invenio moodle teachcenter
 Platform: any
@@ -54,14 +54,19 @@
     invenio-moodle is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.2.2 (release 2023-07-25)
+
+- setup: fix typo, prevent correct build
+
+
 Version v0.2.1 (release 2023-07-25)
 
 - setup: change to reusable workflows
 
 
 Version v0.2.0 (release 2023-07-25)
```

### Comparing `invenio-moodle-0.2.1/invenio_moodle.egg-info/requires.txt` & `invenio-moodle-0.2.2/invenio_moodle.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/run-tests.sh` & `invenio-moodle-0.2.2/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/setup.cfg` & `invenio-moodle-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	Programming Language :: Python
 	Topic :: Software Development :: Libraries :: Python Modules
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 include_package_data = True
-pacakges = find:
+packages = find:
 python_requires = >=3.9
 zip_safe = False
 install_requires = 
 	click>=8.0.0
 	click-params>=0.4.0
 	invenio-records-lom>=0.10.0
```

### Comparing `invenio-moodle-0.2.1/tests/conftest.py` & `invenio-moodle-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/tests/data/lom_metadata.json` & `invenio-moodle-0.2.2/tests/data/lom_metadata.json`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/tests/data/minimal_record.json` & `invenio-moodle-0.2.2/tests/data/minimal_record.json`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/tests/test_convert.py` & `invenio-moodle-0.2.2/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/tests/test_invenio_moodle.py` & `invenio-moodle-0.2.2/tests/test_invenio_moodle.py`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/tests/test_schema.py` & `invenio-moodle-0.2.2/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.1/tests/test_types.py` & `invenio-moodle-0.2.2/tests/test_types.py`

 * *Files identical despite different names*

