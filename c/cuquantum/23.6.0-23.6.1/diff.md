# Comparing `tmp/cuquantum-23.6.0.tar.gz` & `tmp/cuquantum-23.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuquantum-23.6.0.tar", last modified: Tue Jul 11 03:38:41 2023, max compression
+gzip compressed data, was "cuquantum-23.6.1.tar", last modified: Thu Jul 20 16:49:26 2023, max compression
```

## Comparing `cuquantum-23.6.0.tar` & `cuquantum-23.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:38:41.020473 cuquantum-23.6.0/
--rw-r--r--   0 root         (0) root         (0)    11004 2023-07-11 03:36:36.000000 cuquantum-23.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2853 2023-07-11 03:38:41.020473 cuquantum-23.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2052 2023-07-11 03:36:36.000000 cuquantum-23.6.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     8953 2023-07-11 03:36:36.000000 cuquantum-23.6.0/cuda_autodetect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:38:41.016473 cuquantum-23.6.0/cuquantum.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2853 2023-07-11 03:38:40.000000 cuquantum-23.6.0/cuquantum.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      210 2023-07-11 03:38:40.000000 cuquantum-23.6.0/cuquantum.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 03:38:40.000000 cuquantum-23.6.0/cuquantum.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 03:38:40.000000 cuquantum-23.6.0/cuquantum.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-11 03:38:40.000000 cuquantum-23.6.0/cuquantum.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 03:38:41.020473 cuquantum-23.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2525 2023-07-11 03:36:36.000000 cuquantum-23.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:49:26.202466 cuquantum-23.6.1/
+-rw-r--r--   0 root         (0) root         (0)    11004 2023-07-20 16:47:10.000000 cuquantum-23.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-07-20 16:49:26.202466 cuquantum-23.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-07-20 16:47:10.000000 cuquantum-23.6.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)     8953 2023-07-20 16:47:10.000000 cuquantum-23.6.1/cuda_autodetect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:49:26.202466 cuquantum-23.6.1/cuquantum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-07-20 16:49:26.000000 cuquantum-23.6.1/cuquantum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      210 2023-07-20 16:49:26.000000 cuquantum-23.6.1/cuquantum.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:49:26.000000 cuquantum-23.6.1/cuquantum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:49:26.000000 cuquantum-23.6.1/cuquantum.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 16:49:26.000000 cuquantum-23.6.1/cuquantum.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 16:49:26.202466 cuquantum-23.6.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2525 2023-07-20 16:47:10.000000 cuquantum-23.6.1/setup.py
```

### Comparing `cuquantum-23.6.0/LICENSE` & `cuquantum-23.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cuquantum-23.6.0/PKG-INFO` & `cuquantum-23.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuquantum
-Version: 23.6.0
+Version: 23.6.1
 Summary: NVIDIA cuQuantum SDK
 Home-page: https://developer.nvidia.com/cuquantum-sdk
 Author: NVIDIA Corporation
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Project-URL: Bug Tracker, https://github.com/NVIDIA/cuQuantum/issues
 Project-URL: User Forum, https://github.com/NVIDIA/cuQuantum/discussions
```

### Comparing `cuquantum-23.6.0/README.rst` & `cuquantum-23.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `cuquantum-23.6.0/cuda_autodetect.py` & `cuquantum-23.6.1/cuda_autodetect.py`

 * *Files identical despite different names*

### Comparing `cuquantum-23.6.0/cuquantum.egg-info/PKG-INFO` & `cuquantum-23.6.1/cuquantum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuquantum
-Version: 23.6.0
+Version: 23.6.1
 Summary: NVIDIA cuQuantum SDK
 Home-page: https://developer.nvidia.com/cuquantum-sdk
 Author: NVIDIA Corporation
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Project-URL: Bug Tracker, https://github.com/NVIDIA/cuQuantum/issues
 Project-URL: User Forum, https://github.com/NVIDIA/cuQuantum/discussions
```

### Comparing `cuquantum-23.6.0/setup.py` & `cuquantum-23.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from setuptools import setup
 
 from cuda_autodetect import infer_best_package, bdist_wheel
 
 
 # Update this for every release
-package_ver = '23.06.0'
+package_ver = '23.06.1'
 package_name = "cuquantum"
 
 
 # get project long description
 with open("README.rst") as f:
     long_description = f.read()
```

