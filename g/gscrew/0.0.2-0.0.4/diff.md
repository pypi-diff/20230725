# Comparing `tmp/GScrew-0.0.2.tar.gz` & `tmp/gscrew-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GScrew-0.0.2.tar", last modified: Tue Jul 25 08:16:47 2023, max compression
+gzip compressed data, was "gscrew-0.0.4.tar", last modified: Tue Jul 25 08:32:51 2023, max compression
```

## Comparing `GScrew-0.0.2.tar` & `gscrew-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:16:47.664974 GScrew-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:16:47.664974 GScrew-0.0.2/GScrew/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 08:16:32.000000 GScrew-0.0.2/GScrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-07-25 08:16:32.000000 GScrew-0.0.2/GScrew/geometric_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-07-25 08:16:32.000000 GScrew-0.0.2/GScrew/screw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:16:47.664974 GScrew-0.0.2/GScrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-25 08:16:47.000000 GScrew-0.0.2/GScrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-25 08:16:47.000000 GScrew-0.0.2/GScrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:16:47.000000 GScrew-0.0.2/GScrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 08:16:47.000000 GScrew-0.0.2/GScrew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 08:16:47.000000 GScrew-0.0.2/GScrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 08:16:32.000000 GScrew-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-25 08:16:47.664974 GScrew-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-25 08:16:32.000000 GScrew-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-25 08:16:32.000000 GScrew-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 08:16:32.000000 GScrew-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:16:47.664974 GScrew-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 08:16:32.000000 GScrew-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:51.071710 gscrew-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 08:32:37.000000 gscrew-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-25 08:32:51.071710 gscrew-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-25 08:32:37.000000 gscrew-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:51.071710 gscrew-0.0.4/gscrew/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 08:32:37.000000 gscrew-0.0.4/gscrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-07-25 08:32:37.000000 gscrew-0.0.4/gscrew/geometric_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-07-25 08:32:37.000000 gscrew-0.0.4/gscrew/screw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:51.071710 gscrew-0.0.4/gscrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-25 08:32:51.000000 gscrew-0.0.4/gscrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-25 08:32:51.000000 gscrew-0.0.4/gscrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:32:51.000000 gscrew-0.0.4/gscrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 08:32:51.000000 gscrew-0.0.4/gscrew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 08:32:51.000000 gscrew-0.0.4/gscrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-25 08:32:37.000000 gscrew-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 08:32:37.000000 gscrew-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:32:51.071710 gscrew-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 08:32:37.000000 gscrew-0.0.4/setup.py
```

### Comparing `GScrew-0.0.2/GScrew/geometric_algebra.py` & `gscrew-0.0.4/gscrew/geometric_algebra.py`

 * *Files identical despite different names*

### Comparing `GScrew-0.0.2/GScrew/screw.py` & `gscrew-0.0.4/gscrew/screw.py`

 * *Files identical despite different names*

### Comparing `GScrew-0.0.2/GScrew.egg-info/PKG-INFO` & `gscrew-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
-Name: GScrew
-Version: 0.0.2
+Name: gscrew
+Version: 0.0.4
 Summary: A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
 Author: Antoine Royer, Loris Delafosse
-Project-URL: Homepage, https://github.com/Shadow15510/SCREW
-Project-URL: Documentation, http://screw.readthedocs.io/
+Project-URL: Homepage, https://github.com/Shadow15510/GScrew
+Project-URL: Documentation, http://gscrew.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
 # GScrew (Generalized Screw Calculus)
 [![Documentation Status](https://readthedocs.org/projects/gscrew/badge/?version=latest)](https://gscrew.readthedocs.io/en/latest/?badge=latest)
 [![Licence](https://img.shields.io/github/license/Shadow15510/GScrew?color=green)](https://github.com/Shadow15510/GScrew/blob/master/LICENSE)
+[![Build Status](https://github.com/Shadow15510/GScrew/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Shadow15510/GScrew/blob/master/.github/workflows/python-publish.yml)
 
 ## Description
 A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
 
-The full documentation is on readthedocs.
-
-If you encounter an issue, feel free to open one.
+- [readthedocs Documentation](https://gscrew.readthedocs.io/en/latest/).
+- [Bug tracker](https://github.com/Shadow15510/GScrew/issues).
 
 ## Installation
-A Pypi package is available, please refer to the Pypi page or enter `pip install gscrew` in a terminal.
+A Pypi package is available, please refer to the [Pypi page](https://pypi.org/project/GScrew/) or enter `pip install gscrew` in a terminal.
 
 ## Exemples
 First of all, you need to import the modules:
 ```
-import geometric_algebra as ga
-from screw import Screw
+import gscrew.geometric_algebra as ga
+from gscrew.screw import Screw
 ```
 The `screw` module also provides a `CoScrew` object and the `comoment` function for calculating the comoment between a coscrew and a screw.
 
 Once these modules have been imported, we can create the geometric algebra in which we will be working. For basic physical applications, a three-dimensionnal algebra should suffice:
 ```
 my_algebra = ga.GeometricAlgebra(3)
 locals().update(my_algebra.blades)
```

### Comparing `GScrew-0.0.2/LICENSE` & `gscrew-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `GScrew-0.0.2/PKG-INFO` & `gscrew-0.0.4/gscrew.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
-Name: GScrew
-Version: 0.0.2
+Name: gscrew
+Version: 0.0.4
 Summary: A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
 Author: Antoine Royer, Loris Delafosse
-Project-URL: Homepage, https://github.com/Shadow15510/SCREW
-Project-URL: Documentation, http://screw.readthedocs.io/
+Project-URL: Homepage, https://github.com/Shadow15510/GScrew
+Project-URL: Documentation, http://gscrew.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
 # GScrew (Generalized Screw Calculus)
 [![Documentation Status](https://readthedocs.org/projects/gscrew/badge/?version=latest)](https://gscrew.readthedocs.io/en/latest/?badge=latest)
 [![Licence](https://img.shields.io/github/license/Shadow15510/GScrew?color=green)](https://github.com/Shadow15510/GScrew/blob/master/LICENSE)
+[![Build Status](https://github.com/Shadow15510/GScrew/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Shadow15510/GScrew/blob/master/.github/workflows/python-publish.yml)
 
 ## Description
 A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
 
-The full documentation is on readthedocs.
-
-If you encounter an issue, feel free to open one.
+- [readthedocs Documentation](https://gscrew.readthedocs.io/en/latest/).
+- [Bug tracker](https://github.com/Shadow15510/GScrew/issues).
 
 ## Installation
-A Pypi package is available, please refer to the Pypi page or enter `pip install gscrew` in a terminal.
+A Pypi package is available, please refer to the [Pypi page](https://pypi.org/project/GScrew/) or enter `pip install gscrew` in a terminal.
 
 ## Exemples
 First of all, you need to import the modules:
 ```
-import geometric_algebra as ga
-from screw import Screw
+import gscrew.geometric_algebra as ga
+from gscrew.screw import Screw
 ```
 The `screw` module also provides a `CoScrew` object and the `comoment` function for calculating the comoment between a coscrew and a screw.
 
 Once these modules have been imported, we can create the geometric algebra in which we will be working. For basic physical applications, a three-dimensionnal algebra should suffice:
 ```
 my_algebra = ga.GeometricAlgebra(3)
 locals().update(my_algebra.blades)
```

### Comparing `GScrew-0.0.2/README.md` & `gscrew-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # GScrew (Generalized Screw Calculus)
 [![Documentation Status](https://readthedocs.org/projects/gscrew/badge/?version=latest)](https://gscrew.readthedocs.io/en/latest/?badge=latest)
 [![Licence](https://img.shields.io/github/license/Shadow15510/GScrew?color=green)](https://github.com/Shadow15510/GScrew/blob/master/LICENSE)
+[![Build Status](https://github.com/Shadow15510/GScrew/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Shadow15510/GScrew/blob/master/.github/workflows/python-publish.yml)
 
 ## Description
 A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
 
-The full documentation is on readthedocs.
-
-If you encounter an issue, feel free to open one.
+- [readthedocs Documentation](https://gscrew.readthedocs.io/en/latest/).
+- [Bug tracker](https://github.com/Shadow15510/GScrew/issues).
 
 ## Installation
-A Pypi package is available, please refer to the Pypi page or enter `pip install gscrew` in a terminal.
+A Pypi package is available, please refer to the [Pypi page](https://pypi.org/project/GScrew/) or enter `pip install gscrew` in a terminal.
 
 ## Exemples
 First of all, you need to import the modules:
 ```
-import geometric_algebra as ga
-from screw import Screw
+import gscrew.geometric_algebra as ga
+from gscrew.screw import Screw
 ```
 The `screw` module also provides a `CoScrew` object and the `comoment` function for calculating the comoment between a coscrew and a screw.
 
 Once these modules have been imported, we can create the geometric algebra in which we will be working. For basic physical applications, a three-dimensionnal algebra should suffice:
 ```
 my_algebra = ga.GeometricAlgebra(3)
 locals().update(my_algebra.blades)
```

### Comparing `GScrew-0.0.2/pyproject.toml` & `gscrew-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "GScrew"
+name = "gscrew"
 authors = [
 	{name="Antoine Royer"},
 	{name="Loris Delafosse"}
 ]
 description = "A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra)."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.7"
@@ -30,15 +30,15 @@
 doc = [
     "sphinx>=7.0.1",
     "sphinx-rtd-theme",
     "sphinx-autodocgen",
 ]
 
 [tool.setuptools.dynamic.version]
-attr = "GScrew.__init__.__version__"
+attr = "gscrew.__init__.__version__"
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
-Homepage = "https://github.com/Shadow15510/SCREW"
-Documentation = "http://screw.readthedocs.io/"
+Homepage = "https://github.com/Shadow15510/GScrew"
+Documentation = "http://gscrew.readthedocs.io/"
```

