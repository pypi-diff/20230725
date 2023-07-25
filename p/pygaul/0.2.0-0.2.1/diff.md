# Comparing `tmp/pygaul-0.2.0.tar.gz` & `tmp/pygaul-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygaul-0.2.0.tar", last modified: Mon Jul 24 13:01:00 2023, max compression
+gzip compressed data, was "pygaul-0.2.1.tar", last modified: Tue Jul 25 05:03:15 2023, max compression
```

## Comparing `pygaul-0.2.0.tar` & `pygaul-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:00.593614 pygaul-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-24 13:01:00.593614 pygaul-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-24 13:00:36.000000 pygaul-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:00.589614 pygaul-0.2.0/pygaul/
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-24 13:00:36.000000 pygaul-0.2.0/pygaul/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:00.593614 pygaul-0.2.0/pygaul/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-24 13:00:36.000000 pygaul-0.2.0/pygaul/data/gaul_continent.json
--rw-r--r--   0 runner    (1001) docker     (123)   705454 2023-07-24 13:00:36.000000 pygaul-0.2.0/pygaul/data/gaul_database.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:00.589614 pygaul-0.2.0/pygaul.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-24 13:01:00.000000 pygaul-0.2.0/pygaul.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-24 13:01:00.000000 pygaul-0.2.0/pygaul.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:01:00.000000 pygaul-0.2.0/pygaul.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 13:01:00.000000 pygaul-0.2.0/pygaul.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 13:01:00.000000 pygaul-0.2.0/pygaul.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-24 13:00:36.000000 pygaul-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:01:00.593614 pygaul-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 13:00:36.000000 pygaul-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:00.593614 pygaul-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-24 13:00:36.000000 pygaul-0.2.0/tests/test_get_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-24 13:00:36.000000 pygaul-0.2.0/tests/test_get_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:03:15.971857 pygaul-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 05:03:00.000000 pygaul-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-25 05:03:15.971857 pygaul-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-25 05:03:00.000000 pygaul-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:03:15.967857 pygaul-0.2.1/pygaul/
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-25 05:03:00.000000 pygaul-0.2.1/pygaul/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:03:15.967857 pygaul-0.2.1/pygaul/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-25 05:03:00.000000 pygaul-0.2.1/pygaul/data/gaul_continent.json
+-rw-r--r--   0 runner    (1001) docker     (123)   705454 2023-07-25 05:03:00.000000 pygaul-0.2.1/pygaul/data/gaul_database.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:03:15.967857 pygaul-0.2.1/pygaul.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-25 05:03:15.000000 pygaul-0.2.1/pygaul.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-25 05:03:15.000000 pygaul-0.2.1/pygaul.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:03:15.000000 pygaul-0.2.1/pygaul.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-25 05:03:15.000000 pygaul-0.2.1/pygaul.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 05:03:15.000000 pygaul-0.2.1/pygaul.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-25 05:03:00.000000 pygaul-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 05:03:15.971857 pygaul-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:03:15.971857 pygaul-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-25 05:03:00.000000 pygaul-0.2.1/tests/test_get_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-25 05:03:00.000000 pygaul-0.2.1/tests/test_get_name.py
```

### Comparing `pygaul-0.2.0/PKG-INFO` & `pygaul-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygaul
-Version: 0.2.0
+Version: 0.2.1
 Summary: Easy access to administrative boundary defined by FAO GAUL from a Python script.
 Author-email: Pierrick Rambaud <pierrick.rambaud49@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/12rambau/pygaul
 Keywords: skeleton,Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: doc
+License-File: LICENSE
 
 
 pyGAUL
 ======
 
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg?logo=opensourceinitiative&logoColor=white
     :target: LICENSE
```

### Comparing `pygaul-0.2.0/README.rst` & `pygaul-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `pygaul-0.2.0/pygaul/__init__.py` & `pygaul-0.2.1/pygaul/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pathlib import Path
 from typing import List, Union
 
 import ee
 import numpy as np
 import pandas as pd
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __author__ = "Pierrick Rambaud"
 __email__ = "pierrick.rambaud49@gmail.com"
 
 __gaul_data__ = Path(__file__).parent / "data" / "gaul_database.parquet"
 __gaul_continent__ = Path(__file__).parent / "data" / "gaul_continent.json"
 __gaul_asset__ = "FAO/GAUL/2015/level{}"
```

### Comparing `pygaul-0.2.0/pygaul/data/gaul_continent.json` & `pygaul-0.2.1/pygaul/data/gaul_continent.json`

 * *Files identical despite different names*

### Comparing `pygaul-0.2.0/pygaul/data/gaul_database.parquet` & `pygaul-0.2.1/pygaul/data/gaul_database.parquet`

 * *Files identical despite different names*

### Comparing `pygaul-0.2.0/pygaul.egg-info/PKG-INFO` & `pygaul-0.2.1/pygaul.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygaul
-Version: 0.2.0
+Version: 0.2.1
 Summary: Easy access to administrative boundary defined by FAO GAUL from a Python script.
 Author-email: Pierrick Rambaud <pierrick.rambaud49@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/12rambau/pygaul
 Keywords: skeleton,Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: doc
+License-File: LICENSE
 
 
 pyGAUL
 ======
 
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg?logo=opensourceinitiative&logoColor=white
     :target: LICENSE
```

### Comparing `pygaul-0.2.0/pyproject.toml` & `pygaul-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygaul"
-version = "0.2.0"
+version = "0.2.1"
 description = "Easy access to administrative boundary defined by FAO GAUL from a Python script."
 keywords = ["skeleton", "Python"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
@@ -60,28 +60,28 @@
     "sphinx-autoapi",
     "geemap",
     "jupyter-sphinx",
     "httplib2",
 ]
 
 [tool.setuptools]
+license-files = ["LICENSE"]
 include-package-data = true
-license-files = ["LICENSE.txt"]
 
 [tool.setuptools.package-data]
 pygaul = ["data/gaul_database.parquet", "data/gaul_continent.json"]
 
 [tool.setuptools.packages.find]
 include = ["pygaul*"]
 exclude = ["docs*", "tests*"]
 
 [tool.commitizen]
 tag_format = "v$major.$minor.$patch$prerelease"
 update_changelog_on_bump = false
-version = "0.2.0"
+version = "0.2.1"
 version_files = [
     "pyproject.toml:version",
     "pygaul/__init__.py:__version__",
     "docs/conf.py:release"
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `pygaul-0.2.0/tests/test_get_items.py` & `pygaul-0.2.1/tests/test_get_items.py`

 * *Files identical despite different names*

### Comparing `pygaul-0.2.0/tests/test_get_name.py` & `pygaul-0.2.1/tests/test_get_name.py`

 * *Files identical despite different names*

