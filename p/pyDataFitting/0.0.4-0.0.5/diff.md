# Comparing `tmp/pyDataFitting-0.0.4.tar.gz` & `tmp/pyDataFitting-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDataFitting-0.0.4.tar", last modified: Fri Jul 21 14:15:03 2023, max compression
+gzip compressed data, was "pyDataFitting-0.0.5.tar", last modified: Tue Jul 25 14:51:57 2023, max compression
```

## Comparing `pyDataFitting-0.0.4.tar` & `pyDataFitting-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 14:15:03.194839 pyDataFitting-0.0.4/
--rw-rw-rw-   0        0        0     1095 2023-01-17 12:23:36.000000 pyDataFitting-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     5256 2023-07-21 14:15:03.748299 pyDataFitting-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4671 2023-04-14 12:49:18.000000 pyDataFitting-0.0.4/README.md
--rw-rw-rw-   0        0        0      110 2023-01-17 12:23:36.000000 pyDataFitting-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      722 2023-07-21 14:15:03.758595 pyDataFitting-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      273 2023-07-21 14:13:36.000000 pyDataFitting-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 14:15:03.194839 pyDataFitting-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-21 14:15:03.194839 pyDataFitting-0.0.4/src/pyDataFitting/
--rw-rw-rw-   0        0        0      307 2023-04-14 13:25:24.000000 pyDataFitting-0.0.4/src/pyDataFitting/__init__.py
--rw-rw-rw-   0        0        0     4067 2023-01-17 12:23:36.000000 pyDataFitting-0.0.4/src/pyDataFitting/linear_regression.py
--rw-rw-rw-   0        0        0     1669 2023-04-14 09:13:47.000000 pyDataFitting-0.0.4/src/pyDataFitting/model_diagnostics.py
--rw-rw-rw-   0        0        0    13711 2023-04-14 11:10:40.000000 pyDataFitting-0.0.4/src/pyDataFitting/model_tools.py
--rw-rw-rw-   0        0        0     6063 2023-01-17 12:23:36.000000 pyDataFitting-0.0.4/src/pyDataFitting/nonlinear_regression.py
--rw-rw-rw-   0        0        0    11118 2023-04-14 12:54:35.000000 pyDataFitting-0.0.4/src/pyDataFitting/partial_least_squares_regression.py
--rw-rw-rw-   0        0        0    23760 2023-01-17 12:23:36.000000 pyDataFitting-0.0.4/src/pyDataFitting/polynomial_regression.py
--rw-rw-rw-   0        0        0    47982 2023-06-07 14:43:30.000000 pyDataFitting-0.0.4/src/pyDataFitting/principle_component_regression.py
-drwxrwxrwx   0        0        0        0 2023-07-21 14:15:03.198839 pyDataFitting-0.0.4/src/pyDataFitting.egg-info/
--rw-rw-rw-   0        0        0     5256 2023-07-21 14:15:03.000000 pyDataFitting-0.0.4/src/pyDataFitting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      769 2023-07-21 14:15:03.000000 pyDataFitting-0.0.4/src/pyDataFitting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 14:15:03.000000 pyDataFitting-0.0.4/src/pyDataFitting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-07-21 14:15:03.000000 pyDataFitting-0.0.4/src/pyDataFitting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-21 14:15:03.000000 pyDataFitting-0.0.4/src/pyDataFitting.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 14:15:03.202839 pyDataFitting-0.0.4/tests/
--rw-rw-rw-   0        0        0     2989 2023-04-14 11:51:38.000000 pyDataFitting-0.0.4/tests/test_model_tools.py
--rw-rw-rw-   0        0        0     2367 2023-04-14 20:55:16.000000 pyDataFitting-0.0.4/tests/test_nonlinear_regresssion.py
--rw-rw-rw-   0        0        0     3959 2023-01-17 12:23:36.000000 pyDataFitting-0.0.4/tests/test_piecewise_polynomial_fit.py
--rw-rw-rw-   0        0        0     3387 2023-01-17 12:23:36.000000 pyDataFitting-0.0.4/tests/test_polynomial_regression.py
--rw-rw-rw-   0        0        0     2396 2023-04-14 20:50:17.000000 pyDataFitting-0.0.4/tests/test_principal_component_regression.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:51:57.115537 pyDataFitting-0.0.5/
+-rw-rw-rw-   0        0        0     1095 2023-01-17 12:23:36.000000 pyDataFitting-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5256 2023-07-25 14:51:57.623307 pyDataFitting-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4671 2023-04-14 12:49:18.000000 pyDataFitting-0.0.5/README.md
+-rw-rw-rw-   0        0        0      110 2023-01-17 12:23:36.000000 pyDataFitting-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      722 2023-07-25 14:51:57.633345 pyDataFitting-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      273 2023-07-25 14:51:28.000000 pyDataFitting-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:51:57.115537 pyDataFitting-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 14:51:57.115537 pyDataFitting-0.0.5/src/pyDataFitting/
+-rw-rw-rw-   0        0        0      398 2023-07-25 10:37:41.000000 pyDataFitting-0.0.5/src/pyDataFitting/__init__.py
+-rw-rw-rw-   0        0        0     4067 2023-01-17 12:23:36.000000 pyDataFitting-0.0.5/src/pyDataFitting/linear_regression.py
+-rw-rw-rw-   0        0        0      695 2023-07-25 10:43:49.000000 pyDataFitting-0.0.5/src/pyDataFitting/model_diagnostics.py
+-rw-rw-rw-   0        0        0    13711 2023-04-14 11:10:40.000000 pyDataFitting-0.0.5/src/pyDataFitting/model_tools.py
+-rw-rw-rw-   0        0        0     6063 2023-01-17 12:23:36.000000 pyDataFitting-0.0.5/src/pyDataFitting/nonlinear_regression.py
+-rw-rw-rw-   0        0        0    11118 2023-04-14 12:54:35.000000 pyDataFitting-0.0.5/src/pyDataFitting/partial_least_squares_regression.py
+-rw-rw-rw-   0        0        0    23760 2023-01-17 12:23:36.000000 pyDataFitting-0.0.5/src/pyDataFitting/polynomial_regression.py
+-rw-rw-rw-   0        0        0    47982 2023-06-07 14:43:30.000000 pyDataFitting-0.0.5/src/pyDataFitting/principle_component_regression.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:51:57.119536 pyDataFitting-0.0.5/src/pyDataFitting.egg-info/
+-rw-rw-rw-   0        0        0     5256 2023-07-25 14:51:57.000000 pyDataFitting-0.0.5/src/pyDataFitting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      769 2023-07-25 14:51:57.000000 pyDataFitting-0.0.5/src/pyDataFitting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:51:57.000000 pyDataFitting-0.0.5/src/pyDataFitting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-07-25 14:51:57.000000 pyDataFitting-0.0.5/src/pyDataFitting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-25 14:51:57.000000 pyDataFitting-0.0.5/src/pyDataFitting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 14:51:57.123536 pyDataFitting-0.0.5/tests/
+-rw-rw-rw-   0        0        0     2989 2023-04-14 11:51:38.000000 pyDataFitting-0.0.5/tests/test_model_tools.py
+-rw-rw-rw-   0        0        0     2367 2023-04-14 20:55:16.000000 pyDataFitting-0.0.5/tests/test_nonlinear_regresssion.py
+-rw-rw-rw-   0        0        0     3959 2023-01-17 12:23:36.000000 pyDataFitting-0.0.5/tests/test_piecewise_polynomial_fit.py
+-rw-rw-rw-   0        0        0     3387 2023-01-17 12:23:36.000000 pyDataFitting-0.0.5/tests/test_polynomial_regression.py
+-rw-rw-rw-   0        0        0     2396 2023-04-14 20:50:17.000000 pyDataFitting-0.0.5/tests/test_principal_component_regression.py
```

### Comparing `pyDataFitting-0.0.4/LICENSE` & `pyDataFitting-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.4/PKG-INFO` & `pyDataFitting-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDataFitting
-Version: 0.0.4
+Version: 0.0.5
 Summary: package for specialized regression
 Home-page: https://github.com/AlexanderSouthan/pyDataFitting
 Author: Alexander Southan
 Author-email: 72788772+AlexanderSouthan@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/pyDataFitting/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyDataFitting-0.0.4/README.md` & `pyDataFitting-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.4/setup.cfg` & `pyDataFitting-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7944 6174 6146 6974 7469 6e67   = pyDataFitting
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 302e  ..version = 0.0.
-00000030: 340d 0a61 7574 686f 7220 3d20 416c 6578  4..author = Alex
+00000030: 350d 0a61 7574 686f 7220 3d20 416c 6578  5..author = Alex
 00000040: 616e 6465 7220 536f 7574 6861 6e0d 0a61  ander Southan..a
 00000050: 7574 686f 725f 656d 6169 6c20 3d20 3732  uthor_email = 72
 00000060: 3738 3837 3732 2b41 6c65 7861 6e64 6572  788772+Alexander
 00000070: 536f 7574 6861 6e40 7573 6572 732e 6e6f  Southan@users.no
 00000080: 7265 706c 792e 6769 7468 7562 2e63 6f6d  reply.github.com
 00000090: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 000000a0: 7061 636b 6167 6520 666f 7220 7370 6563  package for spec
```

### Comparing `pyDataFitting-0.0.4/src/pyDataFitting/linear_regression.py` & `pyDataFitting-0.0.5/src/pyDataFitting/linear_regression.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.4/src/pyDataFitting/model_tools.py` & `pyDataFitting-0.0.5/src/pyDataFitting/model_tools.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.4/src/pyDataFitting/nonlinear_regression.py` & `pyDataFitting-0.0.5/src/pyDataFitting/nonlinear_regression.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.4/src/pyDataFitting/partial_least_squares_regression.py` & `pyDataFitting-0.0.5/src/pyDataFitting/partial_least_squares_regression.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.4/src/pyDataFitting/polynomial_regression.py` & `pyDataFitting-0.0.5/src/pyDataFitting/polynomial_regression.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.4/src/pyDataFitting/principle_component_regression.py` & `pyDataFitting-0.0.5/src/pyDataFitting/principle_component_regression.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.4/src/pyDataFitting.egg-info/PKG-INFO` & `pyDataFitting-0.0.5/src/pyDataFitting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDataFitting
-Version: 0.0.4
+Version: 0.0.5
 Summary: package for specialized regression
 Home-page: https://github.com/AlexanderSouthan/pyDataFitting
 Author: Alexander Southan
 Author-email: 72788772+AlexanderSouthan@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/pyDataFitting/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyDataFitting-0.0.4/src/pyDataFitting.egg-info/SOURCES.txt` & `pyDataFitting-0.0.5/src/pyDataFitting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.4/tests/test_model_tools.py` & `pyDataFitting-0.0.5/tests/test_model_tools.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.4/tests/test_nonlinear_regresssion.py` & `pyDataFitting-0.0.5/tests/test_nonlinear_regresssion.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.4/tests/test_piecewise_polynomial_fit.py` & `pyDataFitting-0.0.5/tests/test_piecewise_polynomial_fit.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.4/tests/test_polynomial_regression.py` & `pyDataFitting-0.0.5/tests/test_polynomial_regression.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.4/tests/test_principal_component_regression.py` & `pyDataFitting-0.0.5/tests/test_principal_component_regression.py`

 * *Files identical despite different names*

