# Comparing `tmp/metrapy-0.1.0.tar.gz` & `tmp/metrapy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metrapy-0.1.0.tar", last modified: Wed Jul 19 20:03:35 2023, max compression
+gzip compressed data, was "metrapy-0.1.1.tar", last modified: Tue Jul 25 04:44:40 2023, max compression
```

## Comparing `metrapy-0.1.0.tar` & `metrapy-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 20:03:35.956573 metrapy-0.1.0/
--rw-rw-rw-   0        0        0     2670 2023-07-19 20:03:35.955610 metrapy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2347 2023-07-19 20:01:09.000000 metrapy-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 20:03:35.924492 metrapy-0.1.0/metrapy/
--rw-rw-rw-   0        0        0    13702 2023-07-19 19:30:36.000000 metrapy-0.1.0/metrapy/connector.py
-drwxrwxrwx   0        0        0        0 2023-07-19 20:03:35.954575 metrapy-0.1.0/metrapy/metrapy.egg-info/
--rw-rw-rw-   0        0        0     2670 2023-07-19 20:03:35.000000 metrapy-0.1.0/metrapy/metrapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-07-19 20:03:35.000000 metrapy-0.1.0/metrapy/metrapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 20:03:35.000000 metrapy-0.1.0/metrapy/metrapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-19 20:03:35.000000 metrapy-0.1.0/metrapy/metrapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-19 20:03:35.000000 metrapy-0.1.0/metrapy/metrapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1877 2023-07-19 19:33:47.000000 metrapy-0.1.0/metrapy/sync.py
--rw-rw-rw-   0        0        0       42 2023-07-19 20:03:35.956573 metrapy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1079 2023-07-19 19:33:45.000000 metrapy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 04:44:40.037428 metrapy-0.1.1/
+-rw-rw-rw-   0        0        0     2670 2023-07-25 04:44:40.036433 metrapy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2347 2023-07-19 20:01:09.000000 metrapy-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 04:44:40.007860 metrapy-0.1.1/metrapy/
+-rw-rw-rw-   0        0        0        0 2023-07-25 03:44:41.000000 metrapy-0.1.1/metrapy/__init__.py
+-rw-rw-rw-   0        0        0    13702 2023-07-19 19:30:36.000000 metrapy-0.1.1/metrapy/connector.py
+-rw-rw-rw-   0        0        0      205 2023-07-19 19:33:58.000000 metrapy-0.1.1/metrapy/defaults.py
+-rw-rw-rw-   0        0        0     2414 2023-07-19 19:32:18.000000 metrapy-0.1.1/metrapy/maps.py
+-rw-rw-rw-   0        0        0     1877 2023-07-19 19:33:47.000000 metrapy-0.1.1/metrapy/sync.py
+-rw-rw-rw-   0        0        0      607 2023-07-19 19:33:51.000000 metrapy-0.1.1/metrapy/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 04:44:40.035431 metrapy-0.1.1/metrapy.egg-info/
+-rw-rw-rw-   0        0        0     2670 2023-07-25 04:44:39.000000 metrapy-0.1.1/metrapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-07-25 04:44:39.000000 metrapy-0.1.1/metrapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 04:44:39.000000 metrapy-0.1.1/metrapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-25 04:44:39.000000 metrapy-0.1.1/metrapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-25 04:44:39.000000 metrapy-0.1.1/metrapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 04:44:40.037428 metrapy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-07-25 04:44:37.000000 metrapy-0.1.1/setup.py
```

### Comparing `metrapy-0.1.0/PKG-INFO` & `metrapy-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrapy
-Version: 0.1.0
+Version: 0.1.1
 Summary: batteries included wrapper utility for MetaTrader5's python integration
 Author: pavittarx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `metrapy-0.1.0/README.md` & `metrapy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.0/metrapy/connector.py` & `metrapy-0.1.1/metrapy/connector.py`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.0/metrapy/metrapy.egg-info/PKG-INFO` & `metrapy-0.1.1/metrapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrapy
-Version: 0.1.0
+Version: 0.1.1
 Summary: batteries included wrapper utility for MetaTrader5's python integration
 Author: pavittarx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `metrapy-0.1.0/metrapy/sync.py` & `metrapy-0.1.1/metrapy/sync.py`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.0/setup.py` & `metrapy-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="metrapy",  # This is the name of the package
-    version="0.1.0",  # The initial release version
+    version="0.1.1",  # The initial release version
     author="pavittarx",  # Full name of the author
     description="batteries included wrapper utility for MetaTrader5's python integration",
     long_description=long_description,  # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),  # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],  # Information to filter the project on PyPi website
     python_requires=">=3.6",  # Minimum version requirement of the package
     py_modules=["connector", "sync"],  # Name of the python package
-    package_dir={"": "metrapy"},  # Directory of the source code of the package
+    # package_dir={"": "metrapy"},  # Directory of the source code of the package
     install_requires=["MetaTrader5"],  # Install other dependencies if any
 )
```

