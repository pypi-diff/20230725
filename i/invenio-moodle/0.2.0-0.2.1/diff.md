# Comparing `tmp/invenio-moodle-0.2.0.tar.gz` & `tmp/invenio-moodle-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-moodle-0.2.0.tar", last modified: Tue Jul 25 11:40:33 2023, max compression
+gzip compressed data, was "invenio-moodle-0.2.1.tar", last modified: Tue Jul 25 12:37:37 2023, max compression
```

## Comparing `invenio-moodle-0.2.0.tar` & `invenio-moodle-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:40:33.745651 invenio-moodle-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-25 11:40:33.745651 invenio-moodle-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:40:33.741650 invenio-moodle-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10163 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:40:33.741650 invenio-moodle-0.2.0/invenio_moodle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-25 11:40:33.000000 invenio-moodle-0.2.0/invenio_moodle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-25 11:40:33.000000 invenio-moodle-0.2.0/invenio_moodle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:40:33.000000 invenio-moodle-0.2.0/invenio_moodle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 11:40:33.000000 invenio-moodle-0.2.0/invenio_moodle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:40:33.000000 invenio-moodle-0.2.0/invenio_moodle.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-25 11:40:33.000000 invenio-moodle-0.2.0/invenio_moodle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:40:33.000000 invenio-moodle-0.2.0/invenio_moodle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-25 11:40:33.745651 invenio-moodle-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:40:33.745651 invenio-moodle-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:40:33.745651 invenio-moodle-0.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/tests/data/lom_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/tests/data/minimal_record.json
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/tests/test_invenio_moodle.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-25 11:40:28.000000 invenio-moodle-0.2.0/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:37:37.644982 invenio-moodle-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-25 12:37:37.644982 invenio-moodle-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:37:37.640982 invenio-moodle-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10163 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:37:37.640982 invenio-moodle-0.2.1/invenio_moodle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-25 12:37:37.000000 invenio-moodle-0.2.1/invenio_moodle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-25 12:37:37.000000 invenio-moodle-0.2.1/invenio_moodle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:37:37.000000 invenio-moodle-0.2.1/invenio_moodle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 12:37:37.000000 invenio-moodle-0.2.1/invenio_moodle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:37:37.000000 invenio-moodle-0.2.1/invenio_moodle.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-25 12:37:37.000000 invenio-moodle-0.2.1/invenio_moodle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:37:37.000000 invenio-moodle-0.2.1/invenio_moodle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-25 12:37:37.644982 invenio-moodle-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:37:37.640982 invenio-moodle-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:37:37.640982 invenio-moodle-0.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/tests/data/lom_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/tests/data/minimal_record.json
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/tests/test_invenio_moodle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-25 12:37:31.000000 invenio-moodle-0.2.1/tests/test_types.py
```

### Comparing `invenio-moodle-0.2.0/.editorconfig` & `invenio-moodle-0.2.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/CONTRIBUTING.rst` & `invenio-moodle-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/LICENSE` & `invenio-moodle-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/MANIFEST.in` & `invenio-moodle-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/PKG-INFO` & `invenio-moodle-0.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,71 @@
 Metadata-Version: 2.1
 Name: invenio-moodle
-Version: 0.2.0
+Version: 0.2.1
 Summary: "Provides API for Moodle."
 Home-page: https://github.com/tu-graz-library/invenio-moodle
 Author: "Graz University of Technology"
 Author-email: info@tugraz.at
 License: MIT
-Description: ..
-            Copyright (C) 2022 Graz University of Technology.
-        
-            invenio-moodle is free software; you can redistribute it and/or
-            modify it under the terms of the MIT License; see LICENSE file for more
-            details.
-        
-        ===============
-         invenio-moodle
-        ===============
-        
-        .. image:: https://github.com/tu-graz-library/invenio-moodle/workflows/CI/badge.svg
-                :target: https://github.com/tu-graz-library/invenio-moodle/actions?query=workflow%3ACI
-        
-        .. image:: https://img.shields.io/github/tag/tu-graz-library/invenio-moodle.svg
-                :target: https://github.com/tu-graz-library/invenio-moodle/releases
-        
-        .. image:: https://img.shields.io/pypi/dm/invenio-moodle.svg
-                :target: https://pypi.python.org/pypi/invenio-moodle
-        
-        .. image:: https://img.shields.io/github/license/tu-graz-library/invenio-moodle.svg
-                :target: https://github.com/tu-graz-library/invenio-moodle/blob/master/LICENSE
-        
-        Provides API for Moodle.
-        
-        Further documentation is available on
-        https://invenio-moodle.readthedocs.io/
-        
-        ..
-            Copyright (C) 2022 Graz University of Technology.
-        
-            invenio-moodle is free software; you can redistribute it and/or
-            modify it under the terms of the MIT License; see LICENSE file for more
-            details.
-        
-        Changes
-        =======
-        
-        Version v0.2.0 (release 2023-07-25)
-        
-        
-        
-        
 Keywords: invenio_moodle invenio moodle teachcenter
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Provides-Extra: tests
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+..
+    Copyright (C) 2022 Graz University of Technology.
+
+    invenio-moodle is free software; you can redistribute it and/or
+    modify it under the terms of the MIT License; see LICENSE file for more
+    details.
+
+===============
+ invenio-moodle
+===============
+
+.. image:: https://github.com/tu-graz-library/invenio-moodle/workflows/CI/badge.svg
+        :target: https://github.com/tu-graz-library/invenio-moodle/actions?query=workflow%3ACI
+
+.. image:: https://img.shields.io/github/tag/tu-graz-library/invenio-moodle.svg
+        :target: https://github.com/tu-graz-library/invenio-moodle/releases
+
+.. image:: https://img.shields.io/pypi/dm/invenio-moodle.svg
+        :target: https://pypi.python.org/pypi/invenio-moodle
+
+.. image:: https://img.shields.io/github/license/tu-graz-library/invenio-moodle.svg
+        :target: https://github.com/tu-graz-library/invenio-moodle/blob/master/LICENSE
+
+Provides API for Moodle.
+
+Further documentation is available on
+https://invenio-moodle.readthedocs.io/
+
+..
+    Copyright (C) 2022 Graz University of Technology.
+
+    invenio-moodle is free software; you can redistribute it and/or
+    modify it under the terms of the MIT License; see LICENSE file for more
+    details.
+
+Changes
+=======
+
+Version v0.2.1 (release 2023-07-25)
+
+- setup: change to reusable workflows
+
+
+Version v0.2.0 (release 2023-07-25)
+
+
+
+
+
```

### Comparing `invenio-moodle-0.2.0/README.rst` & `invenio-moodle-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/docs/conf.py` & `invenio-moodle-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/docs/index.rst` & `invenio-moodle-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/docs/make.bat` & `invenio-moodle-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/invenio_moodle.egg-info/PKG-INFO` & `invenio-moodle-0.2.1/invenio_moodle.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,71 @@
 Metadata-Version: 2.1
 Name: invenio-moodle
-Version: 0.2.0
+Version: 0.2.1
 Summary: "Provides API for Moodle."
 Home-page: https://github.com/tu-graz-library/invenio-moodle
 Author: "Graz University of Technology"
 Author-email: info@tugraz.at
 License: MIT
-Description: ..
-            Copyright (C) 2022 Graz University of Technology.
-        
-            invenio-moodle is free software; you can redistribute it and/or
-            modify it under the terms of the MIT License; see LICENSE file for more
-            details.
-        
-        ===============
-         invenio-moodle
-        ===============
-        
-        .. image:: https://github.com/tu-graz-library/invenio-moodle/workflows/CI/badge.svg
-                :target: https://github.com/tu-graz-library/invenio-moodle/actions?query=workflow%3ACI
-        
-        .. image:: https://img.shields.io/github/tag/tu-graz-library/invenio-moodle.svg
-                :target: https://github.com/tu-graz-library/invenio-moodle/releases
-        
-        .. image:: https://img.shields.io/pypi/dm/invenio-moodle.svg
-                :target: https://pypi.python.org/pypi/invenio-moodle
-        
-        .. image:: https://img.shields.io/github/license/tu-graz-library/invenio-moodle.svg
-                :target: https://github.com/tu-graz-library/invenio-moodle/blob/master/LICENSE
-        
-        Provides API for Moodle.
-        
-        Further documentation is available on
-        https://invenio-moodle.readthedocs.io/
-        
-        ..
-            Copyright (C) 2022 Graz University of Technology.
-        
-            invenio-moodle is free software; you can redistribute it and/or
-            modify it under the terms of the MIT License; see LICENSE file for more
-            details.
-        
-        Changes
-        =======
-        
-        Version v0.2.0 (release 2023-07-25)
-        
-        
-        
-        
 Keywords: invenio_moodle invenio moodle teachcenter
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Provides-Extra: tests
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+..
+    Copyright (C) 2022 Graz University of Technology.
+
+    invenio-moodle is free software; you can redistribute it and/or
+    modify it under the terms of the MIT License; see LICENSE file for more
+    details.
+
+===============
+ invenio-moodle
+===============
+
+.. image:: https://github.com/tu-graz-library/invenio-moodle/workflows/CI/badge.svg
+        :target: https://github.com/tu-graz-library/invenio-moodle/actions?query=workflow%3ACI
+
+.. image:: https://img.shields.io/github/tag/tu-graz-library/invenio-moodle.svg
+        :target: https://github.com/tu-graz-library/invenio-moodle/releases
+
+.. image:: https://img.shields.io/pypi/dm/invenio-moodle.svg
+        :target: https://pypi.python.org/pypi/invenio-moodle
+
+.. image:: https://img.shields.io/github/license/tu-graz-library/invenio-moodle.svg
+        :target: https://github.com/tu-graz-library/invenio-moodle/blob/master/LICENSE
+
+Provides API for Moodle.
+
+Further documentation is available on
+https://invenio-moodle.readthedocs.io/
+
+..
+    Copyright (C) 2022 Graz University of Technology.
+
+    invenio-moodle is free software; you can redistribute it and/or
+    modify it under the terms of the MIT License; see LICENSE file for more
+    details.
+
+Changes
+=======
+
+Version v0.2.1 (release 2023-07-25)
+
+- setup: change to reusable workflows
+
+
+Version v0.2.0 (release 2023-07-25)
+
+
+
+
+
```

### Comparing `invenio-moodle-0.2.0/invenio_moodle.egg-info/SOURCES.txt` & `invenio-moodle-0.2.1/invenio_moodle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/invenio_moodle.egg-info/requires.txt` & `invenio-moodle-0.2.1/invenio_moodle.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/run-tests.sh` & `invenio-moodle-0.2.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/setup.cfg` & `invenio-moodle-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/tests/conftest.py` & `invenio-moodle-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/tests/data/lom_metadata.json` & `invenio-moodle-0.2.1/tests/data/lom_metadata.json`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/tests/data/minimal_record.json` & `invenio-moodle-0.2.1/tests/data/minimal_record.json`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/tests/test_convert.py` & `invenio-moodle-0.2.1/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/tests/test_invenio_moodle.py` & `invenio-moodle-0.2.1/tests/test_invenio_moodle.py`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/tests/test_schema.py` & `invenio-moodle-0.2.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `invenio-moodle-0.2.0/tests/test_types.py` & `invenio-moodle-0.2.1/tests/test_types.py`

 * *Files identical despite different names*

