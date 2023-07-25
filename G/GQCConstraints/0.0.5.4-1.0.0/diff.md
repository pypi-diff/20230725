# Comparing `tmp/GQCConstraints-0.0.5.4.tar.gz` & `tmp/GQCConstraints-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GQCConstraints-0.0.5.4.tar", last modified: Tue Jul 25 14:15:40 2023, max compression
+gzip compressed data, was "GQCConstraints-1.0.0.tar", last modified: Tue Jul 25 15:59:01 2023, max compression
```

## Comparing `GQCConstraints-0.0.5.4.tar` & `GQCConstraints-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:15:40.142091 GQCConstraints-0.0.5.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:15:39.866186 GQCConstraints-0.0.5.4/GQCC/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:15:39.908198 GQCConstraints-0.0.5.4/GQCC/Methods/
--rw-r--r--   0 root         (0) root         (0)    14754 2023-07-14 14:04:07.000000 GQCConstraints-0.0.5.4/GQCC/Methods/EntanglementStudy.py
--rw-r--r--   0 root         (0) root         (0)    10437 2023-07-14 13:50:26.000000 GQCConstraints-0.0.5.4/GQCC/Methods/ExpectationValueSearch.py
--rw-r--r--   0 root         (0) root         (0)     4808 2023-07-14 13:50:40.000000 GQCConstraints-0.0.5.4/GQCC/Methods/MultiplierScan.py
--rw-r--r--   0 root         (0) root         (0)     6262 2023-07-25 10:55:49.000000 GQCConstraints-0.0.5.4/GQCC/Methods/PotentialEnergySurface.py
--rw-r--r--   0 root         (0) root         (0)      135 2022-08-11 13:30:31.000000 GQCConstraints-0.0.5.4/GQCC/Methods/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:15:39.958682 GQCConstraints-0.0.5.4/GQCC/Optimization/
--rw-r--r--   0 root         (0) root         (0)     9917 2022-09-01 08:47:56.000000 GQCConstraints-0.0.5.4/GQCC/Optimization/SpinResolvedOptimizationFunctions.py
--rw-r--r--   0 root         (0) root         (0)     6573 2023-07-14 13:52:03.000000 GQCConstraints-0.0.5.4/GQCC/Optimization/SpinResolvedOptimizer.py
--rw-r--r--   0 root         (0) root         (0)    11825 2022-12-15 16:22:25.000000 GQCConstraints-0.0.5.4/GQCC/Optimization/SpinUnresolvedOptimizationFunctions.py
--rw-r--r--   0 root         (0) root         (0)     5066 2023-07-14 13:53:15.000000 GQCConstraints-0.0.5.4/GQCC/Optimization/SpinUnresolvedOptimizer.py
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-14 14:06:03.000000 GQCConstraints-0.0.5.4/GQCC/Optimization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:15:40.014456 GQCConstraints-0.0.5.4/GQCC/SpinResolvedConstraints/
--rw-r--r--   0 root         (0) root         (0)     8314 2023-07-14 13:54:09.000000 GQCConstraints-0.0.5.4/GQCC/SpinResolvedConstraints/FCI.py
--rw-r--r--   0 root         (0) root         (0)     6196 2023-07-25 08:31:03.000000 GQCConstraints-0.0.5.4/GQCC/SpinResolvedConstraints/HubbardFCI.py
--rw-r--r--   0 root         (0) root         (0)    11662 2023-07-14 13:53:51.000000 GQCConstraints-0.0.5.4/GQCC/SpinResolvedConstraints/UHF.py
--rw-r--r--   0 root         (0) root         (0)     8580 2023-07-14 13:53:59.000000 GQCConstraints-0.0.5.4/GQCC/SpinResolvedConstraints/UNOCI.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-14 08:57:26.000000 GQCConstraints-0.0.5.4/GQCC/SpinResolvedConstraints/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:15:40.072373 GQCConstraints-0.0.5.4/GQCC/SpinUnresolvedConstraints/
--rw-r--r--   0 root         (0) root         (0)     7797 2023-07-25 09:00:15.000000 GQCConstraints-0.0.5.4/GQCC/SpinUnresolvedConstraints/FCI.py
--rw-r--r--   0 root         (0) root         (0)     9889 2023-07-25 09:00:14.000000 GQCConstraints-0.0.5.4/GQCC/SpinUnresolvedConstraints/GHF.py
--rw-r--r--   0 root         (0) root         (0)     6505 2023-07-14 13:53:33.000000 GQCConstraints-0.0.5.4/GQCC/SpinUnresolvedConstraints/GNOCI.py
--rw-r--r--   0 root         (0) root         (0)     5929 2023-07-25 08:35:29.000000 GQCConstraints-0.0.5.4/GQCC/SpinUnresolvedConstraints/HubbardFCI.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-14 13:19:50.000000 GQCConstraints-0.0.5.4/GQCC/SpinUnresolvedConstraints/__init__.py
--rw-r--r--   0 root         (0) root         (0)      928 2023-07-14 13:52:47.000000 GQCConstraints-0.0.5.4/GQCC/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:15:40.128697 GQCConstraints-0.0.5.4/GQCConstraints.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1796 2023-07-25 14:15:39.000000 GQCConstraints-0.0.5.4/GQCConstraints.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2023-07-25 14:15:39.000000 GQCConstraints-0.0.5.4/GQCConstraints.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 14:15:39.000000 GQCConstraints-0.0.5.4/GQCConstraints.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-25 14:15:39.000000 GQCConstraints-0.0.5.4/GQCConstraints.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-25 14:15:39.000000 GQCConstraints-0.0.5.4/GQCConstraints.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     7651 2022-08-11 13:30:31.000000 GQCConstraints-0.0.5.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1796 2023-07-25 14:15:40.139948 GQCConstraints-0.0.5.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1631 2023-07-25 13:57:42.000000 GQCConstraints-0.0.5.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 14:15:40.143549 GQCConstraints-0.0.5.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1075 2023-07-25 14:15:22.000000 GQCConstraints-0.0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:59:01.542950 GQCConstraints-1.0.0/GQCC/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/GQCC/Methods/
+-rw-r--r--   0 runner    (1001) docker     (122)    14754 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Methods/EntanglementStudy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10437 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Methods/ExpectationValueSearch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4808 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Methods/MultiplierScan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Methods/PotentialEnergySurface.py
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/GQCC/Optimization/
+-rw-r--r--   0 runner    (1001) docker     (122)     9917 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Optimization/SpinResolvedOptimizationFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6573 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Optimization/SpinResolvedOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11825 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Optimization/SpinUnresolvedOptimizationFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5066 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Optimization/SpinUnresolvedOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/Optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/
+-rw-r--r--   0 runner    (1001) docker     (122)     8314 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/FCI.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6196 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/HubbardFCI.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11662 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/UHF.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8580 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/UNOCI.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/
+-rw-r--r--   0 runner    (1001) docker     (122)     7797 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/FCI.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9889 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/GHF.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6505 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/GNOCI.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5929 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/HubbardFCI.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/GQCC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/GQCConstraints.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-07-25 15:59:01.000000 GQCConstraints-1.0.0/GQCConstraints.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-07-25 15:59:01.000000 GQCConstraints-1.0.0/GQCConstraints.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 15:59:01.000000 GQCConstraints-1.0.0/GQCConstraints.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-25 15:59:01.000000 GQCConstraints-1.0.0/GQCConstraints.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-25 15:59:01.000000 GQCConstraints-1.0.0/GQCConstraints.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-25 15:59:01.546950 GQCConstraints-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-07-25 15:58:48.000000 GQCConstraints-1.0.0/setup.py
```

### Comparing `GQCConstraints-0.0.5.4/GQCC/Methods/EntanglementStudy.py` & `GQCConstraints-1.0.0/GQCC/Methods/EntanglementStudy.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/Methods/ExpectationValueSearch.py` & `GQCConstraints-1.0.0/GQCC/Methods/ExpectationValueSearch.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/Methods/MultiplierScan.py` & `GQCConstraints-1.0.0/GQCC/Methods/MultiplierScan.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/Methods/PotentialEnergySurface.py` & `GQCConstraints-1.0.0/GQCC/Methods/PotentialEnergySurface.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/Optimization/SpinResolvedOptimizationFunctions.py` & `GQCConstraints-1.0.0/GQCC/Optimization/SpinResolvedOptimizationFunctions.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/Optimization/SpinResolvedOptimizer.py` & `GQCConstraints-1.0.0/GQCC/Optimization/SpinResolvedOptimizer.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/Optimization/SpinUnresolvedOptimizationFunctions.py` & `GQCConstraints-1.0.0/GQCC/Optimization/SpinUnresolvedOptimizationFunctions.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/Optimization/SpinUnresolvedOptimizer.py` & `GQCConstraints-1.0.0/GQCC/Optimization/SpinUnresolvedOptimizer.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/SpinResolvedConstraints/FCI.py` & `GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/FCI.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/SpinResolvedConstraints/HubbardFCI.py` & `GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/HubbardFCI.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/SpinResolvedConstraints/UHF.py` & `GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/UHF.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/SpinResolvedConstraints/UNOCI.py` & `GQCConstraints-1.0.0/GQCC/SpinResolvedConstraints/UNOCI.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/SpinUnresolvedConstraints/FCI.py` & `GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/FCI.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/SpinUnresolvedConstraints/GHF.py` & `GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/GHF.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/SpinUnresolvedConstraints/GNOCI.py` & `GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/GNOCI.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/SpinUnresolvedConstraints/HubbardFCI.py` & `GQCConstraints-1.0.0/GQCC/SpinUnresolvedConstraints/HubbardFCI.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCC/__init__.py` & `GQCConstraints-1.0.0/GQCC/__init__.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/GQCConstraints.egg-info/PKG-INFO` & `GQCConstraints-1.0.0/GQCConstraints.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GQCConstraints
-Version: 0.0.5.4
+Version: 1.0.0
 Summary: This library build on GQCP provides easy to work with utilities in order to perform constrained quantum chemical calculations.
 Author: The Ghent Quantum Chemistry Group
 Keywords: quantum chemistry,constraints,GQCP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GQCConstraints
```

### Comparing `GQCConstraints-0.0.5.4/GQCConstraints.egg-info/SOURCES.txt` & `GQCConstraints-1.0.0/GQCConstraints.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/LICENSE` & `GQCConstraints-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.4/PKG-INFO` & `GQCConstraints-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GQCConstraints
-Version: 0.0.5.4
+Version: 1.0.0
 Summary: This library build on GQCP provides easy to work with utilities in order to perform constrained quantum chemical calculations.
 Author: The Ghent Quantum Chemistry Group
 Keywords: quantum chemistry,constraints,GQCP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GQCConstraints
```

### Comparing `GQCConstraints-0.0.5.4/README.md` & `GQCConstraints-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <p align="center">
 <img src="./media/logo.jpg" width="700">
 </p>
 
 [![PyPI Version](https://img.shields.io/pypi/v/GQCConstraints.svg)](https://pypi.python.org/pypi/GQCConstraints)
-
+[![Examples](https://img.shields.io/badge/tutorials-green.svg)](/examples)
 
 
 # GQCConstraints
 GQCConstraints or GQCC for short is a python library, based on [GQCP](https://github.com/GQCG/GQCP), that can be used to run several constrained quantum chemical calculations.
 
 Constraint and symmetries are closely related and as such, applying different kind of constraints on quantum chemical calculations can lead to some very interesting insights.
```

### Comparing `GQCConstraints-0.0.5.4/setup.py` & `GQCConstraints-1.0.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import setuptools
 import os
 import sys
 
-if not os.path.exists('/gqcpy'):
-    sys.exit("This software is meant to be installed as an extension on top of a GQCPy docker container and needs gqcpy to work. \nSee https://gqcg.github.io/GQCP/user-documentation/installing-gqcp.html in order to get started.")
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 long_description = long_description.split('\n', 8)[8]
 
 setuptools.setup(
       name='GQCConstraints',
-      version='0.0.5.4',
+      version='1.0.0',
       description='This library build on GQCP provides easy to work with utilities in order to perform constrained quantum chemical calculations.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='The Ghent Quantum Chemistry Group',
       packages=setuptools.find_packages(),
       install_requires=['pandas==1.2.5', 'numpy==1.22.4', 'scipy==1.7.0'],
       keywords=['quantum chemistry', 'constraints', 'GQCP']
```

