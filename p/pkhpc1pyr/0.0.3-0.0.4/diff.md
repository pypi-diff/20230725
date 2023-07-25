# Comparing `tmp/pkhpc1pyr-0.0.3.tar.gz` & `tmp/pkhpc1pyr-0.0.4.tar.gz`

## Comparing `pkhpc1pyr-0.0.3.tar` & `pkhpc1pyr-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/requirements.txt
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/P2L1.py
--rw-r--r--   0        0        0     7208 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/P2L2.py
--rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/P2L3.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/__init__.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/tests/TestP2L1.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/tests/TestP2L2.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/tests/TestP2L3.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/tests/__init__.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L1Err.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L1Plot.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L2Err.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L2Plot.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L3Err.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L3Plot.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/__init__.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/helperFunctions.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/LICENSE
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/README.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/P2L1.py
+-rw-r--r--   0        0        0     7208 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/P2L2.py
+-rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/P2L3.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/__init__.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/tests/TestP2L1.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/tests/TestP2L2.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/tests/TestP2L3.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/tests/__init__.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/P2L1Err.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/P2L1Plot.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/P2L2Err.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/P2L2Plot.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/P2L3Err.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/P2L3Plot.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/__init__.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/helperFunctions.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/README.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.4/PKG-INFO
```

### Comparing `pkhpc1pyr-0.0.3/src/pkhpc1pyr/P2L1.py` & `pkhpc1pyr-0.0.4/src/pkhpc1pyr/P2L1.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.3/src/pkhpc1pyr/P2L2.py` & `pkhpc1pyr-0.0.4/src/pkhpc1pyr/P2L2.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.3/src/pkhpc1pyr/P2L3.py` & `pkhpc1pyr-0.0.4/src/pkhpc1pyr/P2L3.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.3/src/pkhpc1pyr/tests/TestP2L1.py` & `pkhpc1pyr-0.0.4/src/pkhpc1pyr/tests/TestP2L1.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.3/src/pkhpc1pyr/tests/TestP2L2.py` & `pkhpc1pyr-0.0.4/src/pkhpc1pyr/tests/TestP2L2.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.3/src/pkhpc1pyr/tests/TestP2L3.py` & `pkhpc1pyr-0.0.4/src/pkhpc1pyr/tests/TestP2L3.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L1Err.py` & `pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/P2L1Err.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L1Plot.py` & `pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/P2L1Plot.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L2Err.py` & `pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/P2L2Err.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L2Plot.py` & `pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/P2L2Plot.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L3Err.py` & `pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/P2L3Err.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/P2L3Plot.py` & `pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/P2L3Plot.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.3/src/pkhpc1pyr/utils/helperFunctions.py` & `pkhpc1pyr-0.0.4/src/pkhpc1pyr/utils/helperFunctions.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.3/LICENSE` & `pkhpc1pyr-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.3/README.md` & `pkhpc1pyr-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 <ul> Running requires python version 3.10 or compatible </ul>
 
 <ul>
 Can be installed from Pypi repository with pip
 <br> <i> pip install pkhpc1pyr </i>
 <br> The required dependencies can be found in the file requirements.txt and installed with the command 
-<br> <i> pip install numpy==1.24.3 </i>
+<br> <i> pip install -r requirements.txt </i>
 </ul>
 
 <ul>
 The installation can be tested by calling the TestP2L* functions without any arguments. For example:
 <br> <i> import pkhpc1pyr as pk 
 <br> pk.tests.TestP2L3() </i>
 </ul>
```

### Comparing `pkhpc1pyr-0.0.3/pyproject.toml` & `pkhpc1pyr-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pkhpc1pyr"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Ryan Boyce", email="ryty.boyce@gmail.com" },
 ]
 description = "Scripts and functions for the pharmacokinetic modeling of hyperpolarized [1-13C]-pyruvate."
 readme = "README.md"
 requires-python = "~=3.10"
 classifiers = [
```

### Comparing `pkhpc1pyr-0.0.3/PKG-INFO` & `pkhpc1pyr-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkhpc1pyr
-Version: 0.0.3
+Version: 0.0.4
 Summary: Scripts and functions for the pharmacokinetic modeling of hyperpolarized [1-13C]-pyruvate.
 Project-URL: Homepage, https://github.com/RytyB/HP-C1Pyr-PK-Python
 Author-email: Ryan Boyce <ryty.boyce@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -67,15 +67,15 @@
 
 <ul> Running requires python version 3.10 or compatible </ul>
 
 <ul>
 Can be installed from Pypi repository with pip
 <br> <i> pip install pkhpc1pyr </i>
 <br> The required dependencies can be found in the file requirements.txt and installed with the command 
-<br> <i> pip install numpy==1.24.3 </i>
+<br> <i> pip install -r requirements.txt </i>
 </ul>
 
 <ul>
 The installation can be tested by calling the TestP2L* functions without any arguments. For example:
 <br> <i> import pkhpc1pyr as pk 
 <br> pk.tests.TestP2L3() </i>
 </ul>
```

