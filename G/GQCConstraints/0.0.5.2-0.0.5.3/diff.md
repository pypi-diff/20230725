# Comparing `tmp/GQCConstraints-0.0.5.2.tar.gz` & `tmp/GQCConstraints-0.0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GQCConstraints-0.0.5.2.tar", last modified: Tue Jul 25 14:00:45 2023, max compression
+gzip compressed data, was "GQCConstraints-0.0.5.3.tar", last modified: Tue Jul 25 14:03:42 2023, max compression
```

## Comparing `GQCConstraints-0.0.5.2.tar` & `GQCConstraints-0.0.5.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:00:45.724746 GQCConstraints-0.0.5.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:00:45.395499 GQCConstraints-0.0.5.2/GQCC/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:00:45.437212 GQCConstraints-0.0.5.2/GQCC/Methods/
--rw-r--r--   0 root         (0) root         (0)    14754 2023-07-14 14:04:07.000000 GQCConstraints-0.0.5.2/GQCC/Methods/EntanglementStudy.py
--rw-r--r--   0 root         (0) root         (0)    10437 2023-07-14 13:50:26.000000 GQCConstraints-0.0.5.2/GQCC/Methods/ExpectationValueSearch.py
--rw-r--r--   0 root         (0) root         (0)     4808 2023-07-14 13:50:40.000000 GQCConstraints-0.0.5.2/GQCC/Methods/MultiplierScan.py
--rw-r--r--   0 root         (0) root         (0)     6262 2023-07-25 10:55:49.000000 GQCConstraints-0.0.5.2/GQCC/Methods/PotentialEnergySurface.py
--rw-r--r--   0 root         (0) root         (0)      135 2022-08-11 13:30:31.000000 GQCConstraints-0.0.5.2/GQCC/Methods/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:00:45.479540 GQCConstraints-0.0.5.2/GQCC/Optimization/
--rw-r--r--   0 root         (0) root         (0)     9917 2022-09-01 08:47:56.000000 GQCConstraints-0.0.5.2/GQCC/Optimization/SpinResolvedOptimizationFunctions.py
--rw-r--r--   0 root         (0) root         (0)     6573 2023-07-14 13:52:03.000000 GQCConstraints-0.0.5.2/GQCC/Optimization/SpinResolvedOptimizer.py
--rw-r--r--   0 root         (0) root         (0)    11825 2022-12-15 16:22:25.000000 GQCConstraints-0.0.5.2/GQCC/Optimization/SpinUnresolvedOptimizationFunctions.py
--rw-r--r--   0 root         (0) root         (0)     5066 2023-07-14 13:53:15.000000 GQCConstraints-0.0.5.2/GQCC/Optimization/SpinUnresolvedOptimizer.py
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-14 14:06:03.000000 GQCConstraints-0.0.5.2/GQCC/Optimization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:00:45.545167 GQCConstraints-0.0.5.2/GQCC/SpinResolvedConstraints/
--rw-r--r--   0 root         (0) root         (0)     8314 2023-07-14 13:54:09.000000 GQCConstraints-0.0.5.2/GQCC/SpinResolvedConstraints/FCI.py
--rw-r--r--   0 root         (0) root         (0)     6196 2023-07-25 08:31:03.000000 GQCConstraints-0.0.5.2/GQCC/SpinResolvedConstraints/HubbardFCI.py
--rw-r--r--   0 root         (0) root         (0)    11662 2023-07-14 13:53:51.000000 GQCConstraints-0.0.5.2/GQCC/SpinResolvedConstraints/UHF.py
--rw-r--r--   0 root         (0) root         (0)     8580 2023-07-14 13:53:59.000000 GQCConstraints-0.0.5.2/GQCC/SpinResolvedConstraints/UNOCI.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-14 08:57:26.000000 GQCConstraints-0.0.5.2/GQCC/SpinResolvedConstraints/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:00:45.602816 GQCConstraints-0.0.5.2/GQCC/SpinUnresolvedConstraints/
--rw-r--r--   0 root         (0) root         (0)     7797 2023-07-25 09:00:15.000000 GQCConstraints-0.0.5.2/GQCC/SpinUnresolvedConstraints/FCI.py
--rw-r--r--   0 root         (0) root         (0)     9889 2023-07-25 09:00:14.000000 GQCConstraints-0.0.5.2/GQCC/SpinUnresolvedConstraints/GHF.py
--rw-r--r--   0 root         (0) root         (0)     6505 2023-07-14 13:53:33.000000 GQCConstraints-0.0.5.2/GQCC/SpinUnresolvedConstraints/GNOCI.py
--rw-r--r--   0 root         (0) root         (0)     5929 2023-07-25 08:35:29.000000 GQCConstraints-0.0.5.2/GQCC/SpinUnresolvedConstraints/HubbardFCI.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-14 13:19:50.000000 GQCConstraints-0.0.5.2/GQCC/SpinUnresolvedConstraints/__init__.py
--rw-r--r--   0 root         (0) root         (0)      928 2023-07-14 13:52:47.000000 GQCConstraints-0.0.5.2/GQCC/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:00:45.703441 GQCConstraints-0.0.5.2/GQCConstraints.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1938 2023-07-25 14:00:45.000000 GQCConstraints-0.0.5.2/GQCConstraints.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2023-07-25 14:00:45.000000 GQCConstraints-0.0.5.2/GQCConstraints.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 14:00:45.000000 GQCConstraints-0.0.5.2/GQCConstraints.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-25 14:00:45.000000 GQCConstraints-0.0.5.2/GQCConstraints.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-25 14:00:45.000000 GQCConstraints-0.0.5.2/GQCConstraints.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     7651 2022-08-11 13:30:31.000000 GQCConstraints-0.0.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1938 2023-07-25 14:00:45.718459 GQCConstraints-0.0.5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1631 2023-07-25 13:57:42.000000 GQCConstraints-0.0.5.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 14:00:45.727072 GQCConstraints-0.0.5.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      968 2023-07-25 14:00:31.000000 GQCConstraints-0.0.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:03:42.748006 GQCConstraints-0.0.5.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:03:42.481922 GQCConstraints-0.0.5.3/GQCC/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:03:42.518181 GQCConstraints-0.0.5.3/GQCC/Methods/
+-rw-r--r--   0 root         (0) root         (0)    14754 2023-07-14 14:04:07.000000 GQCConstraints-0.0.5.3/GQCC/Methods/EntanglementStudy.py
+-rw-r--r--   0 root         (0) root         (0)    10437 2023-07-14 13:50:26.000000 GQCConstraints-0.0.5.3/GQCC/Methods/ExpectationValueSearch.py
+-rw-r--r--   0 root         (0) root         (0)     4808 2023-07-14 13:50:40.000000 GQCConstraints-0.0.5.3/GQCC/Methods/MultiplierScan.py
+-rw-r--r--   0 root         (0) root         (0)     6262 2023-07-25 10:55:49.000000 GQCConstraints-0.0.5.3/GQCC/Methods/PotentialEnergySurface.py
+-rw-r--r--   0 root         (0) root         (0)      135 2022-08-11 13:30:31.000000 GQCConstraints-0.0.5.3/GQCC/Methods/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:03:42.569134 GQCConstraints-0.0.5.3/GQCC/Optimization/
+-rw-r--r--   0 root         (0) root         (0)     9917 2022-09-01 08:47:56.000000 GQCConstraints-0.0.5.3/GQCC/Optimization/SpinResolvedOptimizationFunctions.py
+-rw-r--r--   0 root         (0) root         (0)     6573 2023-07-14 13:52:03.000000 GQCConstraints-0.0.5.3/GQCC/Optimization/SpinResolvedOptimizer.py
+-rw-r--r--   0 root         (0) root         (0)    11825 2022-12-15 16:22:25.000000 GQCConstraints-0.0.5.3/GQCC/Optimization/SpinUnresolvedOptimizationFunctions.py
+-rw-r--r--   0 root         (0) root         (0)     5066 2023-07-14 13:53:15.000000 GQCConstraints-0.0.5.3/GQCC/Optimization/SpinUnresolvedOptimizer.py
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-14 14:06:03.000000 GQCConstraints-0.0.5.3/GQCC/Optimization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:03:42.632544 GQCConstraints-0.0.5.3/GQCC/SpinResolvedConstraints/
+-rw-r--r--   0 root         (0) root         (0)     8314 2023-07-14 13:54:09.000000 GQCConstraints-0.0.5.3/GQCC/SpinResolvedConstraints/FCI.py
+-rw-r--r--   0 root         (0) root         (0)     6196 2023-07-25 08:31:03.000000 GQCConstraints-0.0.5.3/GQCC/SpinResolvedConstraints/HubbardFCI.py
+-rw-r--r--   0 root         (0) root         (0)    11662 2023-07-14 13:53:51.000000 GQCConstraints-0.0.5.3/GQCC/SpinResolvedConstraints/UHF.py
+-rw-r--r--   0 root         (0) root         (0)     8580 2023-07-14 13:53:59.000000 GQCConstraints-0.0.5.3/GQCC/SpinResolvedConstraints/UNOCI.py
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-14 08:57:26.000000 GQCConstraints-0.0.5.3/GQCC/SpinResolvedConstraints/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:03:42.672908 GQCConstraints-0.0.5.3/GQCC/SpinUnresolvedConstraints/
+-rw-r--r--   0 root         (0) root         (0)     7797 2023-07-25 09:00:15.000000 GQCConstraints-0.0.5.3/GQCC/SpinUnresolvedConstraints/FCI.py
+-rw-r--r--   0 root         (0) root         (0)     9889 2023-07-25 09:00:14.000000 GQCConstraints-0.0.5.3/GQCC/SpinUnresolvedConstraints/GHF.py
+-rw-r--r--   0 root         (0) root         (0)     6505 2023-07-14 13:53:33.000000 GQCConstraints-0.0.5.3/GQCC/SpinUnresolvedConstraints/GNOCI.py
+-rw-r--r--   0 root         (0) root         (0)     5929 2023-07-25 08:35:29.000000 GQCConstraints-0.0.5.3/GQCC/SpinUnresolvedConstraints/HubbardFCI.py
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-14 13:19:50.000000 GQCConstraints-0.0.5.3/GQCC/SpinUnresolvedConstraints/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      928 2023-07-14 13:52:47.000000 GQCConstraints-0.0.5.3/GQCC/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:03:42.726039 GQCConstraints-0.0.5.3/GQCConstraints.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-07-25 14:03:42.000000 GQCConstraints-0.0.5.3/GQCConstraints.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-07-25 14:03:42.000000 GQCConstraints-0.0.5.3/GQCConstraints.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 14:03:42.000000 GQCConstraints-0.0.5.3/GQCConstraints.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-25 14:03:42.000000 GQCConstraints-0.0.5.3/GQCConstraints.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-25 14:03:42.000000 GQCConstraints-0.0.5.3/GQCConstraints.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     7651 2022-08-11 13:30:31.000000 GQCConstraints-0.0.5.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-07-25 14:03:42.744097 GQCConstraints-0.0.5.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-07-25 13:57:42.000000 GQCConstraints-0.0.5.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 14:03:42.750223 GQCConstraints-0.0.5.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-07-25 14:03:03.000000 GQCConstraints-0.0.5.3/setup.py
```

### Comparing `GQCConstraints-0.0.5.2/GQCC/Methods/EntanglementStudy.py` & `GQCConstraints-0.0.5.3/GQCC/Methods/EntanglementStudy.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/Methods/ExpectationValueSearch.py` & `GQCConstraints-0.0.5.3/GQCC/Methods/ExpectationValueSearch.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/Methods/MultiplierScan.py` & `GQCConstraints-0.0.5.3/GQCC/Methods/MultiplierScan.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/Methods/PotentialEnergySurface.py` & `GQCConstraints-0.0.5.3/GQCC/Methods/PotentialEnergySurface.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/Optimization/SpinResolvedOptimizationFunctions.py` & `GQCConstraints-0.0.5.3/GQCC/Optimization/SpinResolvedOptimizationFunctions.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/Optimization/SpinResolvedOptimizer.py` & `GQCConstraints-0.0.5.3/GQCC/Optimization/SpinResolvedOptimizer.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/Optimization/SpinUnresolvedOptimizationFunctions.py` & `GQCConstraints-0.0.5.3/GQCC/Optimization/SpinUnresolvedOptimizationFunctions.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/Optimization/SpinUnresolvedOptimizer.py` & `GQCConstraints-0.0.5.3/GQCC/Optimization/SpinUnresolvedOptimizer.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/SpinResolvedConstraints/FCI.py` & `GQCConstraints-0.0.5.3/GQCC/SpinResolvedConstraints/FCI.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/SpinResolvedConstraints/HubbardFCI.py` & `GQCConstraints-0.0.5.3/GQCC/SpinResolvedConstraints/HubbardFCI.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/SpinResolvedConstraints/UHF.py` & `GQCConstraints-0.0.5.3/GQCC/SpinResolvedConstraints/UHF.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/SpinResolvedConstraints/UNOCI.py` & `GQCConstraints-0.0.5.3/GQCC/SpinResolvedConstraints/UNOCI.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/SpinUnresolvedConstraints/FCI.py` & `GQCConstraints-0.0.5.3/GQCC/SpinUnresolvedConstraints/FCI.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/SpinUnresolvedConstraints/GHF.py` & `GQCConstraints-0.0.5.3/GQCC/SpinUnresolvedConstraints/GHF.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/SpinUnresolvedConstraints/GNOCI.py` & `GQCConstraints-0.0.5.3/GQCC/SpinUnresolvedConstraints/GNOCI.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/SpinUnresolvedConstraints/HubbardFCI.py` & `GQCConstraints-0.0.5.3/GQCC/SpinUnresolvedConstraints/HubbardFCI.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCC/__init__.py` & `GQCConstraints-0.0.5.3/GQCC/__init__.py`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/GQCConstraints.egg-info/PKG-INFO` & `GQCConstraints-0.0.5.3/GQCConstraints.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: GQCConstraints
-Version: 0.0.5.2
+Version: 0.0.5.3
 Summary: This library build on GQCP provides easy to work with utilities in order to perform constrained quantum chemical calculations.
 Author: The Ghent Quantum Chemistry Group
 Keywords: quantum chemistry,constraints,GQCP
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 <img src="./media/logo.jpg" width="700">
 </p>
 
 [![PyPI Version](https://img.shields.io/pypi/v/GQCConstraints.svg)](https://pypi.python.org/pypi/GQCConstraints)
```

### Comparing `GQCConstraints-0.0.5.2/GQCConstraints.egg-info/SOURCES.txt` & `GQCConstraints-0.0.5.3/GQCConstraints.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/LICENSE` & `GQCConstraints-0.0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/PKG-INFO` & `GQCConstraints-0.0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: GQCConstraints
-Version: 0.0.5.2
+Version: 0.0.5.3
 Summary: This library build on GQCP provides easy to work with utilities in order to perform constrained quantum chemical calculations.
 Author: The Ghent Quantum Chemistry Group
 Keywords: quantum chemistry,constraints,GQCP
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 <img src="./media/logo.jpg" width="700">
 </p>
 
 [![PyPI Version](https://img.shields.io/pypi/v/GQCConstraints.svg)](https://pypi.python.org/pypi/GQCConstraints)
```

### Comparing `GQCConstraints-0.0.5.2/README.md` & `GQCConstraints-0.0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `GQCConstraints-0.0.5.2/setup.py` & `GQCConstraints-0.0.5.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
       name='GQCConstraints',
-      version='0.0.5.2',
+      version='0.0.5.3',
       description='This library build on GQCP provides easy to work with utilities in order to perform constrained quantum chemical calculations.',
       long_description=long_description,
+      long_description_content_type='text/markdown',
       author='The Ghent Quantum Chemistry Group',
       packages=setuptools.find_packages(),
       install_requires=['pandas==1.2.5', 'numpy==1.22.4', 'scipy==1.7.0'],
       keywords=['quantum chemistry', 'constraints', 'GQCP']
       )
```

