# Comparing `tmp/ebcpy-0.3.6.tar.gz` & `tmp/ebcpy-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebcpy-0.3.6.tar", last modified: Mon Jul 17 14:05:50 2023, max compression
+gzip compressed data, was "ebcpy-0.3.7.tar", last modified: Tue Jul 25 14:58:08 2023, max compression
```

## Comparing `ebcpy-0.3.6.tar` & `ebcpy-0.3.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:05:50.615875 ebcpy-0.3.6/
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-07-17 06:41:21.000000 ebcpy-0.3.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6552 2023-07-17 14:05:50.615875 ebcpy-0.3.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5514 2023-07-17 06:41:21.000000 ebcpy-0.3.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:05:50.611875 ebcpy-0.3.6/ebcpy/
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22850 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/data_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:05:50.615875 ebcpy-0.3.6/ebcpy/modelica/
--rw-rw-rw-   0 root         (0) root         (0)     5695 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/modelica/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5817 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/modelica/manipulate_ds.py
--rw-rw-rw-   0 root         (0) root         (0)    13625 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/modelica/simres.py
--rw-rw-rw-   0 root         (0) root         (0)    19180 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/optimization.py
--rw-rw-rw-   0 root         (0) root         (0)    24847 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/preprocessing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:05:50.615875 ebcpy-0.3.6/ebcpy/simulationapi/
--rw-rw-rw-   0 root         (0) root         (0)    22023 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/simulationapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    49673 2023-07-17 08:02:29.000000 ebcpy-0.3.6/ebcpy/simulationapi/dymola_api.py
--rw-rw-rw-   0 root         (0) root         (0)    15299 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/simulationapi/fmu.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:05:50.615875 ebcpy-0.3.6/ebcpy/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1384 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8478 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/utils/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)    13536 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/utils/reproduction.py
--rw-rw-rw-   0 root         (0) root         (0)     6736 2023-07-17 06:41:21.000000 ebcpy-0.3.6/ebcpy/utils/statistics_analyzer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:05:50.615875 ebcpy-0.3.6/ebcpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6552 2023-07-17 14:05:50.000000 ebcpy-0.3.6/ebcpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      553 2023-07-17 14:05:50.000000 ebcpy-0.3.6/ebcpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 14:05:50.000000 ebcpy-0.3.6/ebcpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2023-07-17 14:05:50.000000 ebcpy-0.3.6/ebcpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-17 14:05:50.000000 ebcpy-0.3.6/ebcpy.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-17 14:05:50.615875 ebcpy-0.3.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2649 2023-07-17 13:55:15.000000 ebcpy-0.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:58:08.861879 ebcpy-0.3.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-07-25 14:47:18.000000 ebcpy-0.3.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6552 2023-07-25 14:58:08.861879 ebcpy-0.3.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5514 2023-07-25 14:47:18.000000 ebcpy-0.3.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:58:08.861879 ebcpy-0.3.7/ebcpy/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-07-25 14:47:18.000000 ebcpy-0.3.7/ebcpy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22850 2023-07-25 14:47:18.000000 ebcpy-0.3.7/ebcpy/data_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:58:08.861879 ebcpy-0.3.7/ebcpy/modelica/
+-rw-rw-rw-   0 root         (0) root         (0)     5695 2023-07-25 14:47:18.000000 ebcpy-0.3.7/ebcpy/modelica/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5817 2023-07-25 14:47:18.000000 ebcpy-0.3.7/ebcpy/modelica/manipulate_ds.py
+-rw-rw-rw-   0 root         (0) root         (0)    13625 2023-07-25 14:47:18.000000 ebcpy-0.3.7/ebcpy/modelica/simres.py
+-rw-rw-rw-   0 root         (0) root         (0)    19180 2023-07-25 14:47:18.000000 ebcpy-0.3.7/ebcpy/optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)    24847 2023-07-25 14:47:18.000000 ebcpy-0.3.7/ebcpy/preprocessing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:58:08.861879 ebcpy-0.3.7/ebcpy/simulationapi/
+-rw-rw-rw-   0 root         (0) root         (0)    22023 2023-07-25 14:47:18.000000 ebcpy-0.3.7/ebcpy/simulationapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    49673 2023-07-25 14:47:18.000000 ebcpy-0.3.7/ebcpy/simulationapi/dymola_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    15299 2023-07-25 14:47:18.000000 ebcpy-0.3.7/ebcpy/simulationapi/fmu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:58:08.861879 ebcpy-0.3.7/ebcpy/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1384 2023-07-25 14:47:18.000000 ebcpy-0.3.7/ebcpy/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8478 2023-07-25 14:47:18.000000 ebcpy-0.3.7/ebcpy/utils/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)    13536 2023-07-25 14:47:18.000000 ebcpy-0.3.7/ebcpy/utils/reproduction.py
+-rw-rw-rw-   0 root         (0) root         (0)     6736 2023-07-25 14:47:18.000000 ebcpy-0.3.7/ebcpy/utils/statistics_analyzer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 14:58:08.861879 ebcpy-0.3.7/ebcpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6552 2023-07-25 14:58:08.000000 ebcpy-0.3.7/ebcpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      553 2023-07-25 14:58:08.000000 ebcpy-0.3.7/ebcpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 14:58:08.000000 ebcpy-0.3.7/ebcpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-25 14:58:08.000000 ebcpy-0.3.7/ebcpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-25 14:58:08.000000 ebcpy-0.3.7/ebcpy.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-25 14:58:08.861879 ebcpy-0.3.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2646 2023-07-25 14:47:18.000000 ebcpy-0.3.7/setup.py
```

### Comparing `ebcpy-0.3.6/LICENSE` & `ebcpy-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/PKG-INFO` & `ebcpy-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ebcpy
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python Library used for different python modules for the analysis and optimization of energy systems, buildings and indoor climate 
 Home-page: https://github.com/RWTH-EBC/ebcpy
 Author: RWTH Aachen University, E.ON Energy Research Center, Institute of Energy Efficient Buildings and Indoor Climate
 Author-email: fabian.wuellhorst@eonerc.rwth-aachen.de
 License: BSD 3-Clause
-Download-URL: https://github.com/RWTH-EBC/ebcpy/archive/refs/tags/0.3.6.tar.gz
+Download-URL: https://github.com/RWTH-EBC/ebcpy/archive/refs/tags/0.3.7.tar.gz
 Keywords: simulation,building,energy,time-series-data,comfort,black-box optimization
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ebcpy-0.3.6/README.md` & `ebcpy-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/ebcpy/data_types.py` & `ebcpy-0.3.7/ebcpy/data_types.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/ebcpy/modelica/__init__.py` & `ebcpy-0.3.7/ebcpy/modelica/__init__.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/ebcpy/modelica/manipulate_ds.py` & `ebcpy-0.3.7/ebcpy/modelica/manipulate_ds.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/ebcpy/modelica/simres.py` & `ebcpy-0.3.7/ebcpy/modelica/simres.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/ebcpy/optimization.py` & `ebcpy-0.3.7/ebcpy/optimization.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/ebcpy/preprocessing.py` & `ebcpy-0.3.7/ebcpy/preprocessing.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/ebcpy/simulationapi/__init__.py` & `ebcpy-0.3.7/ebcpy/simulationapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/ebcpy/simulationapi/dymola_api.py` & `ebcpy-0.3.7/ebcpy/simulationapi/dymola_api.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/ebcpy/simulationapi/fmu.py` & `ebcpy-0.3.7/ebcpy/simulationapi/fmu.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/ebcpy/utils/__init__.py` & `ebcpy-0.3.7/ebcpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/ebcpy/utils/conversion.py` & `ebcpy-0.3.7/ebcpy/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/ebcpy/utils/reproduction.py` & `ebcpy-0.3.7/ebcpy/utils/reproduction.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/ebcpy/utils/statistics_analyzer.py` & `ebcpy-0.3.7/ebcpy/utils/statistics_analyzer.py`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/ebcpy.egg-info/PKG-INFO` & `ebcpy-0.3.7/ebcpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ebcpy
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python Library used for different python modules for the analysis and optimization of energy systems, buildings and indoor climate 
 Home-page: https://github.com/RWTH-EBC/ebcpy
 Author: RWTH Aachen University, E.ON Energy Research Center, Institute of Energy Efficient Buildings and Indoor Climate
 Author-email: fabian.wuellhorst@eonerc.rwth-aachen.de
 License: BSD 3-Clause
-Download-URL: https://github.com/RWTH-EBC/ebcpy/archive/refs/tags/0.3.6.tar.gz
+Download-URL: https://github.com/RWTH-EBC/ebcpy/archive/refs/tags/0.3.7.tar.gz
 Keywords: simulation,building,energy,time-series-data,comfort,black-box optimization
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ebcpy-0.3.6/ebcpy.egg-info/SOURCES.txt` & `ebcpy-0.3.7/ebcpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebcpy-0.3.6/setup.py` & `ebcpy-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 INSTALL_REQUIRES = [
     'numpy>=1.19.5',
     'matplotlib>=3.3.4',
     'scipy>=1.5.4',
     'pandas>=1.1.5',
     'scikit-learn>=0.24.2',
     'fmpy>=0.2.27',
-    'pydantic>=1.8.2',
+    'pydantic<2.0',
     'h5py>=3.1.0',
     'tables>=3.6.1'
 ]
     
 if sys.version_info.minor >= 9 and sys.version_info.major == 3:
     EXTRAS_REQUIRE['full'].append('fastparquet>=2023.1.0')
```

