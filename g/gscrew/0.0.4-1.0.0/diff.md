# Comparing `tmp/gscrew-0.0.4.tar.gz` & `tmp/gscrew-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gscrew-0.0.4.tar", last modified: Tue Jul 25 08:32:51 2023, max compression
+gzip compressed data, was "gscrew-1.0.0.tar", last modified: Tue Jul 25 09:45:40 2023, max compression
```

## Comparing `gscrew-0.0.4.tar` & `gscrew-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:51.071710 gscrew-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 08:32:37.000000 gscrew-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-25 08:32:51.071710 gscrew-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-25 08:32:37.000000 gscrew-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:51.071710 gscrew-0.0.4/gscrew/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 08:32:37.000000 gscrew-0.0.4/gscrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-07-25 08:32:37.000000 gscrew-0.0.4/gscrew/geometric_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-07-25 08:32:37.000000 gscrew-0.0.4/gscrew/screw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:51.071710 gscrew-0.0.4/gscrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-25 08:32:51.000000 gscrew-0.0.4/gscrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-25 08:32:51.000000 gscrew-0.0.4/gscrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:32:51.000000 gscrew-0.0.4/gscrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 08:32:51.000000 gscrew-0.0.4/gscrew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 08:32:51.000000 gscrew-0.0.4/gscrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-25 08:32:37.000000 gscrew-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 08:32:37.000000 gscrew-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:32:51.071710 gscrew-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 08:32:37.000000 gscrew-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:45:40.700264 gscrew-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 09:45:29.000000 gscrew-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-25 09:45:40.700264 gscrew-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-25 09:45:29.000000 gscrew-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:45:40.700264 gscrew-1.0.0/gscrew/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 09:45:29.000000 gscrew-1.0.0/gscrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-07-25 09:45:29.000000 gscrew-1.0.0/gscrew/geometric_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-25 09:45:29.000000 gscrew-1.0.0/gscrew/screw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:45:40.700264 gscrew-1.0.0/gscrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-25 09:45:40.000000 gscrew-1.0.0/gscrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-25 09:45:40.000000 gscrew-1.0.0/gscrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:45:40.000000 gscrew-1.0.0/gscrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 09:45:40.000000 gscrew-1.0.0/gscrew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 09:45:40.000000 gscrew-1.0.0/gscrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-25 09:45:29.000000 gscrew-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 09:45:29.000000 gscrew-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:45:40.700264 gscrew-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 09:45:29.000000 gscrew-1.0.0/setup.py
```

### Comparing `gscrew-0.0.4/LICENSE` & `gscrew-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gscrew-0.0.4/PKG-INFO` & `gscrew-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscrew
-Version: 0.0.4
+Version: 1.0.0
 Summary: A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
 Author: Antoine Royer, Loris Delafosse
 Project-URL: Homepage, https://github.com/Shadow15510/GScrew
 Project-URL: Documentation, http://gscrew.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
@@ -26,16 +26,16 @@
 
 ## Installation
 A Pypi package is available, please refer to the [Pypi page](https://pypi.org/project/GScrew/) or enter `pip install gscrew` in a terminal.
 
 ## Exemples
 First of all, you need to import the modules:
 ```
-import gscrew.geometric_algebra as ga
-from gscrew.screw import Screw
+import GScrew.geometric_algebra as ga
+from GScrew.screw import Screw
 ```
 The `screw` module also provides a `CoScrew` object and the `comoment` function for calculating the comoment between a coscrew and a screw.
 
 Once these modules have been imported, we can create the geometric algebra in which we will be working. For basic physical applications, a three-dimensionnal algebra should suffice:
 ```
 my_algebra = ga.GeometricAlgebra(3)
 locals().update(my_algebra.blades)
```

### Comparing `gscrew-0.0.4/README.md` & `gscrew-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 ## Installation
 A Pypi package is available, please refer to the [Pypi page](https://pypi.org/project/GScrew/) or enter `pip install gscrew` in a terminal.
 
 ## Exemples
 First of all, you need to import the modules:
 ```
-import gscrew.geometric_algebra as ga
-from gscrew.screw import Screw
+import GScrew.geometric_algebra as ga
+from GScrew.screw import Screw
 ```
 The `screw` module also provides a `CoScrew` object and the `comoment` function for calculating the comoment between a coscrew and a screw.
 
 Once these modules have been imported, we can create the geometric algebra in which we will be working. For basic physical applications, a three-dimensionnal algebra should suffice:
 ```
 my_algebra = ga.GeometricAlgebra(3)
 locals().update(my_algebra.blades)
```

### Comparing `gscrew-0.0.4/gscrew/geometric_algebra.py` & `gscrew-1.0.0/gscrew/geometric_algebra.py`

 * *Files identical despite different names*

### Comparing `gscrew-0.0.4/gscrew/screw.py` & `gscrew-1.0.0/gscrew/screw.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,23 @@
         ----------
         ref_point : MultiVector
             The point of reference of the (co)screw
         direction : MultiVector
             The direction of the (co)screw, usually named S.
         moment : MultiVector
             The moment of the (co)screw, usually named M.
+
+        Raises
+        ------
+        TypeError
+            If ``ref_point`` is not as point.
         """
+        if ref_point(1) != ref_point:
+            raise TypeError("ref_point is not a point")
+
         self.ref_point = ref_point
         self.direction = direction
         self.moment = moment
 
     def __repr__(self):
         """Allow to display the (co)Screw at its reference point.
```

### Comparing `gscrew-0.0.4/gscrew.egg-info/PKG-INFO` & `gscrew-1.0.0/gscrew.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscrew
-Version: 0.0.4
+Version: 1.0.0
 Summary: A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
 Author: Antoine Royer, Loris Delafosse
 Project-URL: Homepage, https://github.com/Shadow15510/GScrew
 Project-URL: Documentation, http://gscrew.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
@@ -26,16 +26,16 @@
 
 ## Installation
 A Pypi package is available, please refer to the [Pypi page](https://pypi.org/project/GScrew/) or enter `pip install gscrew` in a terminal.
 
 ## Exemples
 First of all, you need to import the modules:
 ```
-import gscrew.geometric_algebra as ga
-from gscrew.screw import Screw
+import GScrew.geometric_algebra as ga
+from GScrew.screw import Screw
 ```
 The `screw` module also provides a `CoScrew` object and the `comoment` function for calculating the comoment between a coscrew and a screw.
 
 Once these modules have been imported, we can create the geometric algebra in which we will be working. For basic physical applications, a three-dimensionnal algebra should suffice:
 ```
 my_algebra = ga.GeometricAlgebra(3)
 locals().update(my_algebra.blades)
```

### Comparing `gscrew-0.0.4/pyproject.toml` & `gscrew-1.0.0/pyproject.toml`

 * *Files identical despite different names*

