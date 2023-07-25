# Comparing `tmp/pointnext-0.0.2.tar.gz` & `tmp/pointnext-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointnext-0.0.2.tar", last modified: Mon Jul 24 18:59:13 2023, max compression
+gzip compressed data, was "pointnext-0.0.3.tar", last modified: Mon Jul 24 19:11:58 2023, max compression
```

## Comparing `pointnext-0.0.2.tar` & `pointnext-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2023-07-24 18:59:13.923180 pointnext-0.0.2/
--rw-rw-r--   0 kent      (1000) kent      (1000)     1065 2023-07-11 18:10:13.000000 pointnext-0.0.2/LICENSE
--rw-rw-r--   0 kent      (1000) kent      (1000)      465 2023-07-24 18:59:13.923180 pointnext-0.0.2/PKG-INFO
--rw-rw-r--   0 kent      (1000) kent      (1000)      492 2023-07-19 17:53:45.000000 pointnext-0.0.2/README.md
-drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2023-07-24 18:59:13.923180 pointnext-0.0.2/csrc/
--rw-rw-r--   0 kent      (1000) kent      (1000)     1209 2022-12-05 18:42:02.000000 pointnext-0.0.2/csrc/ball_query.cpp
--rw-rw-r--   0 kent      (1000) kent      (1000)     2178 2022-12-05 18:42:02.000000 pointnext-0.0.2/csrc/ball_query_gpu.cu
--rw-rw-r--   0 kent      (1000) kent      (1000)     1204 2022-12-05 18:42:02.000000 pointnext-0.0.2/csrc/group_points.cpp
--rw-rw-r--   0 kent      (1000) kent      (1000)     3406 2022-12-05 18:42:02.000000 pointnext-0.0.2/csrc/group_points_gpu.cu
--rw-rw-r--   0 kent      (1000) kent      (1000)     1948 2022-12-05 18:42:02.000000 pointnext-0.0.2/csrc/interpolate.cpp
--rw-rw-r--   0 kent      (1000) kent      (1000)     5405 2022-12-05 18:42:02.000000 pointnext-0.0.2/csrc/interpolate_gpu.cu
--rw-rw-r--   0 kent      (1000) kent      (1000)     1148 2022-12-05 18:42:02.000000 pointnext-0.0.2/csrc/pointnet2_api.cpp
--rw-rw-r--   0 kent      (1000) kent      (1000)     1478 2022-12-05 18:42:02.000000 pointnext-0.0.2/csrc/sampling.cpp
--rw-rw-r--   0 kent      (1000) kent      (1000)     7895 2022-12-05 18:42:02.000000 pointnext-0.0.2/csrc/sampling_gpu.cu
-drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2023-07-24 18:59:13.923180 pointnext-0.0.2/pointnext/
--rw-rw-r--   0 kent      (1000) kent      (1000)       68 2023-07-19 16:39:01.000000 pointnext-0.0.2/pointnext/__init__.py
--rw-rw-r--   0 kent      (1000) kent      (1000)     2191 2023-07-24 18:41:23.000000 pointnext-0.0.2/pointnext/ops.py
--rw-rw-r--   0 kent      (1000) kent      (1000)     9548 2023-07-19 17:53:23.000000 pointnext-0.0.2/pointnext/pointnext.py
--rw-rw-r--   0 kent      (1000) kent      (1000)     1401 2023-07-19 17:42:28.000000 pointnext-0.0.2/pointnext/taichi.py
--rw-rw-r--   0 kent      (1000) kent      (1000)     1659 2023-07-23 18:55:17.000000 pointnext-0.0.2/pointnext/utils.py
-drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2023-07-24 18:59:13.923180 pointnext-0.0.2/pointnext.egg-info/
--rw-rw-r--   0 kent      (1000) kent      (1000)      465 2023-07-24 18:59:13.000000 pointnext-0.0.2/pointnext.egg-info/PKG-INFO
--rw-rw-r--   0 kent      (1000) kent      (1000)      488 2023-07-24 18:59:13.000000 pointnext-0.0.2/pointnext.egg-info/SOURCES.txt
--rw-rw-r--   0 kent      (1000) kent      (1000)        1 2023-07-24 18:59:13.000000 pointnext-0.0.2/pointnext.egg-info/dependency_links.txt
--rw-rw-r--   0 kent      (1000) kent      (1000)       41 2023-07-24 18:59:13.000000 pointnext-0.0.2/pointnext.egg-info/requires.txt
--rw-rw-r--   0 kent      (1000) kent      (1000)       10 2023-07-24 18:59:13.000000 pointnext-0.0.2/pointnext.egg-info/top_level.txt
--rw-rw-r--   0 kent      (1000) kent      (1000)       38 2023-07-24 18:59:13.923180 pointnext-0.0.2/setup.cfg
--rw-rw-r--   0 kent      (1000) kent      (1000)     1364 2023-07-24 18:54:45.000000 pointnext-0.0.2/setup.py
+drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2023-07-24 19:11:58.680156 pointnext-0.0.3/
+-rw-rw-r--   0 kent      (1000) kent      (1000)     1065 2023-07-11 18:10:13.000000 pointnext-0.0.3/LICENSE
+-rw-rw-r--   0 kent      (1000) kent      (1000)       26 2023-07-24 19:11:57.000000 pointnext-0.0.3/MANIFEST.in
+-rw-rw-r--   0 kent      (1000) kent      (1000)      465 2023-07-24 19:11:58.680156 pointnext-0.0.3/PKG-INFO
+-rw-rw-r--   0 kent      (1000) kent      (1000)      492 2023-07-19 17:53:45.000000 pointnext-0.0.3/README.md
+drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2023-07-24 19:11:58.680156 pointnext-0.0.3/csrc/
+-rw-rw-r--   0 kent      (1000) kent      (1000)     1209 2022-12-05 18:42:02.000000 pointnext-0.0.3/csrc/ball_query.cpp
+-rw-rw-r--   0 kent      (1000) kent      (1000)     2178 2022-12-05 18:42:02.000000 pointnext-0.0.3/csrc/ball_query_gpu.cu
+-rw-rw-r--   0 kent      (1000) kent      (1000)      455 2022-12-05 18:42:02.000000 pointnext-0.0.3/csrc/ball_query_gpu.h
+-rw-rw-r--   0 kent      (1000) kent      (1000)      353 2022-12-05 18:42:02.000000 pointnext-0.0.3/csrc/cuda_utils.h
+-rw-rw-r--   0 kent      (1000) kent      (1000)     1204 2022-12-05 18:42:02.000000 pointnext-0.0.3/csrc/group_points.cpp
+-rw-rw-r--   0 kent      (1000) kent      (1000)     3406 2022-12-05 18:42:02.000000 pointnext-0.0.3/csrc/group_points_gpu.cu
+-rw-rw-r--   0 kent      (1000) kent      (1000)      794 2022-12-05 18:42:02.000000 pointnext-0.0.3/csrc/group_points_gpu.h
+-rw-rw-r--   0 kent      (1000) kent      (1000)     1948 2022-12-05 18:42:02.000000 pointnext-0.0.3/csrc/interpolate.cpp
+-rw-rw-r--   0 kent      (1000) kent      (1000)     5405 2022-12-05 18:42:02.000000 pointnext-0.0.3/csrc/interpolate_gpu.cu
+-rw-rw-r--   0 kent      (1000) kent      (1000)     1111 2022-12-05 18:42:02.000000 pointnext-0.0.3/csrc/interpolate_gpu.h
+-rw-rw-r--   0 kent      (1000) kent      (1000)     1148 2022-12-05 18:42:02.000000 pointnext-0.0.3/csrc/pointnet2_api.cpp
+-rw-rw-r--   0 kent      (1000) kent      (1000)     1478 2022-12-05 18:42:02.000000 pointnext-0.0.3/csrc/sampling.cpp
+-rw-rw-r--   0 kent      (1000) kent      (1000)     7895 2022-12-05 18:42:02.000000 pointnext-0.0.3/csrc/sampling_gpu.cu
+-rw-rw-r--   0 kent      (1000) kent      (1000)      982 2022-12-05 18:42:02.000000 pointnext-0.0.3/csrc/sampling_gpu.h
+drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2023-07-24 19:11:58.680156 pointnext-0.0.3/pointnext/
+-rw-rw-r--   0 kent      (1000) kent      (1000)       68 2023-07-19 16:39:01.000000 pointnext-0.0.3/pointnext/__init__.py
+-rw-rw-r--   0 kent      (1000) kent      (1000)     2191 2023-07-24 18:41:23.000000 pointnext-0.0.3/pointnext/ops.py
+-rw-rw-r--   0 kent      (1000) kent      (1000)     9548 2023-07-19 17:53:23.000000 pointnext-0.0.3/pointnext/pointnext.py
+-rw-rw-r--   0 kent      (1000) kent      (1000)     1401 2023-07-19 17:42:28.000000 pointnext-0.0.3/pointnext/taichi.py
+-rw-rw-r--   0 kent      (1000) kent      (1000)     1659 2023-07-23 18:55:17.000000 pointnext-0.0.3/pointnext/utils.py
+drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2023-07-24 19:11:58.680156 pointnext-0.0.3/pointnext.egg-info/
+-rw-rw-r--   0 kent      (1000) kent      (1000)      465 2023-07-24 19:11:58.000000 pointnext-0.0.3/pointnext.egg-info/PKG-INFO
+-rw-rw-r--   0 kent      (1000) kent      (1000)      607 2023-07-24 19:11:58.000000 pointnext-0.0.3/pointnext.egg-info/SOURCES.txt
+-rw-rw-r--   0 kent      (1000) kent      (1000)        1 2023-07-24 19:11:58.000000 pointnext-0.0.3/pointnext.egg-info/dependency_links.txt
+-rw-rw-r--   0 kent      (1000) kent      (1000)       41 2023-07-24 19:11:58.000000 pointnext-0.0.3/pointnext.egg-info/requires.txt
+-rw-rw-r--   0 kent      (1000) kent      (1000)       10 2023-07-24 19:11:58.000000 pointnext-0.0.3/pointnext.egg-info/top_level.txt
+-rw-rw-r--   0 kent      (1000) kent      (1000)       38 2023-07-24 19:11:58.680156 pointnext-0.0.3/setup.cfg
+-rw-rw-r--   0 kent      (1000) kent      (1000)     1469 2023-07-24 19:05:13.000000 pointnext-0.0.3/setup.py
```

### Comparing `pointnext-0.0.2/LICENSE` & `pointnext-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.2/csrc/ball_query.cpp` & `pointnext-0.0.3/csrc/ball_query.cpp`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.2/csrc/ball_query_gpu.cu` & `pointnext-0.0.3/csrc/ball_query_gpu.cu`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.2/csrc/group_points.cpp` & `pointnext-0.0.3/csrc/group_points.cpp`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.2/csrc/group_points_gpu.cu` & `pointnext-0.0.3/csrc/group_points_gpu.cu`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.2/csrc/interpolate.cpp` & `pointnext-0.0.3/csrc/interpolate.cpp`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.2/csrc/interpolate_gpu.cu` & `pointnext-0.0.3/csrc/interpolate_gpu.cu`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.2/csrc/pointnet2_api.cpp` & `pointnext-0.0.3/csrc/pointnet2_api.cpp`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.2/csrc/sampling.cpp` & `pointnext-0.0.3/csrc/sampling.cpp`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.2/csrc/sampling_gpu.cu` & `pointnext-0.0.3/csrc/sampling_gpu.cu`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.2/pointnext/ops.py` & `pointnext-0.0.3/pointnext/ops.py`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.2/pointnext/pointnext.py` & `pointnext-0.0.3/pointnext/pointnext.py`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.2/pointnext/taichi.py` & `pointnext-0.0.3/pointnext/taichi.py`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.2/pointnext/utils.py` & `pointnext-0.0.3/pointnext/utils.py`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.2/setup.py` & `pointnext-0.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,36 @@
+from pathlib import Path
 from setuptools import setup, find_packages
 from torch.utils.cpp_extension import BuildExtension, CppExtension, CUDAExtension, CUDA_HOME
 
+thisdir = Path(__file__).parent
+
 ext_modules = [
     CUDAExtension(
         'pointnext._C',
         [
             'csrc/pointnet2_api.cpp',
             'csrc/ball_query.cpp',
             'csrc/ball_query_gpu.cu',
             'csrc/group_points.cpp',
             'csrc/group_points_gpu.cu',
             'csrc/interpolate.cpp',
             'csrc/interpolate_gpu.cu',
             'csrc/sampling.cpp',
             'csrc/sampling_gpu.cu',
         ],
-        extra_compile_args={'nvcc': ['-O3']})
+        extra_compile_args={'nvcc': ['-O3']},
+        include_dirs=[thisdir / 'csrc'],
+    )
 ]
 
 setup(
     name='pointnext',
     packages=find_packages(exclude=("csrc")),
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     description='PointNext - Pytorch',
     author='Kaidi Shen',
     url='https://github.com/kentechx/pointnext',
     long_description_content_type='text/markdown',
     keywords=[
         '3D segmentation',
```

