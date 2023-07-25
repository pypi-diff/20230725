# Comparing `tmp/cuquantum_cu11-23.6.0-py3-none-manylinux2014_x86_64.whl.zip` & `tmp/cuquantum_cu11-23.6.1-py3-none-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 7002 bytes, number of entries: 5
--rw-r--r--  2.0 unx    11004 b- defN 23-Jul-11 03:30 cuquantum_cu11-23.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2678 b- defN 23-Jul-11 03:30 cuquantum_cu11-23.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx      109 b- defN 23-Jul-11 03:30 cuquantum_cu11-23.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-11 03:30 cuquantum_cu11-23.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      427 b- defN 23-Jul-11 03:30 cuquantum_cu11-23.6.0.dist-info/RECORD
-5 files, 14219 bytes uncompressed, 6202 bytes compressed:  56.4%
+Zip file size: 7003 bytes, number of entries: 5
+-rw-r--r--  2.0 unx    11004 b- defN 23-Jul-20 16:40 cuquantum_cu11-23.6.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2678 b- defN 23-Jul-20 16:40 cuquantum_cu11-23.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      109 b- defN 23-Jul-20 16:40 cuquantum_cu11-23.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-20 16:40 cuquantum_cu11-23.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      427 b- defN 23-Jul-20 16:40 cuquantum_cu11-23.6.1.dist-info/RECORD
+5 files, 14219 bytes uncompressed, 6203 bytes compressed:  56.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: cuquantum_cu11-23.6.0.dist-info/LICENSE
+Filename: cuquantum_cu11-23.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: cuquantum_cu11-23.6.0.dist-info/METADATA
+Filename: cuquantum_cu11-23.6.1.dist-info/METADATA
 Comment: 
 
-Filename: cuquantum_cu11-23.6.0.dist-info/WHEEL
+Filename: cuquantum_cu11-23.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: cuquantum_cu11-23.6.0.dist-info/top_level.txt
+Filename: cuquantum_cu11-23.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: cuquantum_cu11-23.6.0.dist-info/RECORD
+Filename: cuquantum_cu11-23.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cuquantum_cu11-23.6.0.dist-info/LICENSE` & `cuquantum_cu11-23.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cuquantum_cu11-23.6.0.dist-info/METADATA` & `cuquantum_cu11-23.6.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: cuquantum-cu11
-Version: 23.6.0
+Version: 23.6.1
 Summary: NVIDIA cuQuantum SDK
 Home-page: https://developer.nvidia.com/cuquantum-sdk
 Author: NVIDIA Corporation
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Project-URL: Bug Tracker, https://github.com/NVIDIA/cuQuantum/issues
 Project-URL: User Forum, https://github.com/NVIDIA/cuQuantum/discussions
 Project-URL: Documentation, https://docs.nvidia.com/cuda/cuquantum/
 Keywords: cuda,nvidia,state vector,tensor network,high-performance computing,quantum computing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: custatevec-cu11 (==1.4.0)
-Requires-Dist: cutensornet-cu11 (==2.2.0)
+Requires-Dist: custatevec-cu11 (==1.4.1)
+Requires-Dist: cutensornet-cu11 (==2.2.1)
 
 **************************************************************************************
 cuQuantum SDK: A High-Performance Library for Accelerating Quantum Information Science
 **************************************************************************************
 
 `NVIDIA cuQuantum SDK <https://developer.nvidia.com/cuquantum-sdk>`_ is a high-performance library for quantum information science and beyond.
 Currently its primary target is *quantum circuit simulations* and it consists of two major components:
```

