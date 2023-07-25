# Comparing `tmp/voltools-0.5.0.tar.gz` & `tmp/voltools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voltools-0.5.0.tar", last modified: Thu Jul 20 14:18:47 2023, max compression
+gzip compressed data, was "voltools-0.6.0.tar", last modified: Tue Jul 25 17:32:35 2023, max compression
```

## Comparing `voltools-0.5.0.tar` & `voltools-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-20 14:18:47.826735 voltools-0.5.0/
--rw-r--r--   0 ilya       (501) staff       (20)     1050 2022-03-11 21:56:02.000000 voltools-0.5.0/LICENSE.md
--rw-r--r--   0 ilya       (501) staff       (20)       42 2022-03-11 21:56:02.000000 voltools-0.5.0/MANIFEST.in
--rw-r--r--   0 ilya       (501) staff       (20)     6501 2023-07-20 14:18:47.826595 voltools-0.5.0/PKG-INFO
--rw-r--r--   0 ilya       (501) staff       (20)     5869 2022-03-11 21:56:02.000000 voltools-0.5.0/README.md
--rw-r--r--   0 ilya       (501) staff       (20)       38 2023-07-20 14:18:47.826778 voltools-0.5.0/setup.cfg
--rw-r--r--   0 ilya       (501) staff       (20)     1073 2023-07-20 13:38:18.000000 voltools-0.5.0/setup.py
-drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-20 14:18:47.824139 voltools-0.5.0/tests/
--rw-r--r--   0 ilya       (501) staff       (20)     2614 2022-03-11 21:56:02.000000 voltools-0.5.0/tests/benchmark.py
--rw-r--r--   0 ilya       (501) staff       (20)     2188 2022-03-11 21:56:02.000000 voltools-0.5.0/tests/test_devices.py
--rw-r--r--   0 ilya       (501) staff       (20)      127 2022-03-11 21:56:02.000000 voltools-0.5.0/tests/test_scripts.py
--rw-r--r--   0 ilya       (501) staff       (20)      127 2022-03-11 21:56:02.000000 voltools-0.5.0/tests/test_tools.py
--rw-r--r--   0 ilya       (501) staff       (20)      127 2022-03-11 21:56:02.000000 voltools-0.5.0/tests/test_transforms.py
--rw-r--r--   0 ilya       (501) staff       (20)      127 2022-03-11 21:56:02.000000 voltools-0.5.0/tests/test_volume.py
-drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-20 14:18:47.824843 voltools-0.5.0/voltools/
--rw-r--r--   0 ilya       (501) staff       (20)      196 2023-07-20 14:14:08.000000 voltools-0.5.0/voltools/__init__.py
-drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-20 14:18:47.825999 voltools-0.5.0/voltools/kernels/
--rw-r--r--   0 ilya       (501) staff       (20)     4483 2022-03-11 21:56:02.000000 voltools-0.5.0/voltools/kernels/bspline.h
--rw-r--r--   0 ilya       (501) staff       (20)     3070 2022-03-11 21:56:02.000000 voltools-0.5.0/voltools/kernels/helper_interpolation.h
--rw-r--r--   0 ilya       (501) staff       (20)    37970 2022-03-11 21:56:02.000000 voltools-0.5.0/voltools/kernels/helper_math.h
--rw-r--r--   0 ilya       (501) staff       (20)    11599 2023-07-20 13:36:34.000000 voltools-0.5.0/voltools/transforms.py
-drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-20 14:18:47.826430 voltools-0.5.0/voltools/utils/
--rw-r--r--   0 ilya       (501) staff       (20)      316 2023-07-20 13:34:11.000000 voltools-0.5.0/voltools/utils/__init__.py
--rw-r--r--   0 ilya       (501) staff       (20)     4075 2023-07-20 13:34:11.000000 voltools-0.5.0/voltools/utils/general.py
--rw-r--r--   0 ilya       (501) staff       (20)     5116 2022-03-11 21:56:02.000000 voltools-0.5.0/voltools/utils/matrices.py
--rw-r--r--   0 ilya       (501) staff       (20)     6219 2023-07-20 13:34:11.000000 voltools-0.5.0/voltools/volume.py
-drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-20 14:18:47.825595 voltools-0.5.0/voltools.egg-info/
--rw-r--r--   0 ilya       (501) staff       (20)     6501 2023-07-20 14:18:47.000000 voltools-0.5.0/voltools.egg-info/PKG-INFO
--rw-r--r--   0 ilya       (501) staff       (20)      601 2023-07-20 14:18:47.000000 voltools-0.5.0/voltools.egg-info/SOURCES.txt
--rw-r--r--   0 ilya       (501) staff       (20)        1 2023-07-20 14:18:47.000000 voltools-0.5.0/voltools.egg-info/dependency_links.txt
--rw-r--r--   0 ilya       (501) staff       (20)        1 2023-07-20 14:18:47.000000 voltools-0.5.0/voltools.egg-info/not-zip-safe
--rw-r--r--   0 ilya       (501) staff       (20)       19 2023-07-20 14:18:47.000000 voltools-0.5.0/voltools.egg-info/requires.txt
--rw-r--r--   0 ilya       (501) staff       (20)        9 2023-07-20 14:18:47.000000 voltools-0.5.0/voltools.egg-info/top_level.txt
+drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-25 17:32:35.551052 voltools-0.6.0/
+-rw-r--r--   0 ilya       (501) staff       (20)     1050 2022-03-11 21:56:02.000000 voltools-0.6.0/LICENSE.md
+-rw-r--r--   0 ilya       (501) staff       (20)       42 2022-03-11 21:56:02.000000 voltools-0.6.0/MANIFEST.in
+-rw-r--r--   0 ilya       (501) staff       (20)     6503 2023-07-25 17:32:35.550942 voltools-0.6.0/PKG-INFO
+-rw-r--r--   0 ilya       (501) staff       (20)     5869 2022-03-11 21:56:02.000000 voltools-0.6.0/README.md
+-rw-r--r--   0 ilya       (501) staff       (20)       38 2023-07-25 17:32:35.551088 voltools-0.6.0/setup.cfg
+-rw-r--r--   0 ilya       (501) staff       (20)     1055 2023-07-25 17:30:11.000000 voltools-0.6.0/setup.py
+drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-25 17:32:35.548984 voltools-0.6.0/tests/
+-rw-r--r--   0 ilya       (501) staff       (20)     2614 2022-03-11 21:56:02.000000 voltools-0.6.0/tests/benchmark.py
+-rw-r--r--   0 ilya       (501) staff       (20)     2188 2022-03-11 21:56:02.000000 voltools-0.6.0/tests/test_devices.py
+-rw-r--r--   0 ilya       (501) staff       (20)      127 2022-03-11 21:56:02.000000 voltools-0.6.0/tests/test_scripts.py
+-rw-r--r--   0 ilya       (501) staff       (20)      127 2022-03-11 21:56:02.000000 voltools-0.6.0/tests/test_tools.py
+-rw-r--r--   0 ilya       (501) staff       (20)      127 2022-03-11 21:56:02.000000 voltools-0.6.0/tests/test_transforms.py
+-rw-r--r--   0 ilya       (501) staff       (20)      127 2022-03-11 21:56:02.000000 voltools-0.6.0/tests/test_volume.py
+drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-25 17:32:35.549317 voltools-0.6.0/voltools/
+-rw-r--r--   0 ilya       (501) staff       (20)      196 2023-07-25 17:32:06.000000 voltools-0.6.0/voltools/__init__.py
+drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-25 17:32:35.550400 voltools-0.6.0/voltools/kernels/
+-rw-r--r--   0 ilya       (501) staff       (20)     4483 2022-03-11 21:56:02.000000 voltools-0.6.0/voltools/kernels/bspline.h
+-rw-r--r--   0 ilya       (501) staff       (20)     3070 2022-03-11 21:56:02.000000 voltools-0.6.0/voltools/kernels/helper_interpolation.h
+-rw-r--r--   0 ilya       (501) staff       (20)    37970 2022-03-11 21:56:02.000000 voltools-0.6.0/voltools/kernels/helper_math.h
+-rw-r--r--   0 ilya       (501) staff       (20)    11599 2023-07-20 13:36:34.000000 voltools-0.6.0/voltools/transforms.py
+drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-25 17:32:35.550788 voltools-0.6.0/voltools/utils/
+-rw-r--r--   0 ilya       (501) staff       (20)      316 2023-07-20 13:34:11.000000 voltools-0.6.0/voltools/utils/__init__.py
+-rw-r--r--   0 ilya       (501) staff       (20)     4013 2023-07-25 17:30:11.000000 voltools-0.6.0/voltools/utils/general.py
+-rw-r--r--   0 ilya       (501) staff       (20)     5116 2022-03-11 21:56:02.000000 voltools-0.6.0/voltools/utils/matrices.py
+-rw-r--r--   0 ilya       (501) staff       (20)     6464 2023-07-25 17:30:11.000000 voltools-0.6.0/voltools/volume.py
+drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-25 17:32:35.550038 voltools-0.6.0/voltools.egg-info/
+-rw-r--r--   0 ilya       (501) staff       (20)     6503 2023-07-25 17:32:35.000000 voltools-0.6.0/voltools.egg-info/PKG-INFO
+-rw-r--r--   0 ilya       (501) staff       (20)      601 2023-07-25 17:32:35.000000 voltools-0.6.0/voltools.egg-info/SOURCES.txt
+-rw-r--r--   0 ilya       (501) staff       (20)        1 2023-07-25 17:32:35.000000 voltools-0.6.0/voltools.egg-info/dependency_links.txt
+-rw-r--r--   0 ilya       (501) staff       (20)        1 2023-07-20 14:18:47.000000 voltools-0.6.0/voltools.egg-info/not-zip-safe
+-rw-r--r--   0 ilya       (501) staff       (20)       12 2023-07-25 17:32:35.000000 voltools-0.6.0/voltools.egg-info/requires.txt
+-rw-r--r--   0 ilya       (501) staff       (20)        9 2023-07-25 17:32:35.000000 voltools-0.6.0/voltools.egg-info/top_level.txt
```

### Comparing `voltools-0.5.0/LICENSE.md` & `voltools-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voltools-0.5.0/PKG-INFO` & `voltools-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voltools
-Version: 0.5.0
+Version: 0.6.0
 Summary: CUDA-accelerated 3D affine transformations for NumPy and CuPy
 Home-page: https://github.com/the-lay/voltools
 Author: the-lay
 Author-email: ilja.gubin@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -113,7 +113,9 @@
                    scipy      np_transform   np_transform_out  cp_transform  cp_transform_out  static_vol  static_vol_out
 5, 5, 5           0.201232      4.528787          0.207631      0.195885          0.163193    0.109361         0.059611
 25, 25, 25        5.240529      0.332447          0.238356      0.217309          0.194111    0.138756         0.09321
 50, 50, 50       43.515086      0.804508          0.632981      0.560689          0.527334    0.474820         0.416062
 100, 100, 100   375.886700      4.232868          4.114524      3.454444          3.390018    3.091396         2.999451
 250, 250, 250  6189.052927     95.083083         94.479406     85.200392         84.435548    81.808363       80.959284
 ```
+
+
```

### Comparing `voltools-0.5.0/README.md` & `voltools-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `voltools-0.5.0/setup.py` & `voltools-0.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,15 @@
     license='MIT',
     author='the-lay',
     author_email='ilja.gubin@gmail.com',
     url='https://github.com/the-lay/voltools',
     platforms=['any'],
     install_requires=[
         'numpy',
-        'scipy',
-        'gputil'
+        'scipy'
     ],
     packages=setuptools.find_packages(),
     include_package_data=True,
     zip_safe=False,
     test_suite='tests',
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `voltools-0.5.0/tests/benchmark.py` & `voltools-0.6.0/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `voltools-0.5.0/tests/test_devices.py` & `voltools-0.6.0/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `voltools-0.5.0/voltools/kernels/bspline.h` & `voltools-0.6.0/voltools/kernels/bspline.h`

 * *Files identical despite different names*

### Comparing `voltools-0.5.0/voltools/kernels/helper_interpolation.h` & `voltools-0.6.0/voltools/kernels/helper_interpolation.h`

 * *Files identical despite different names*

### Comparing `voltools-0.5.0/voltools/kernels/helper_math.h` & `voltools-0.6.0/voltools/kernels/helper_math.h`

 * *Files identical despite different names*

### Comparing `voltools-0.5.0/voltools/transforms.py` & `voltools-0.6.0/voltools/transforms.py`

 * *Files identical despite different names*

### Comparing `voltools-0.5.0/voltools/utils/general.py` & `voltools-0.6.0/voltools/utils/general.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 from typing import Tuple
-import GPUtil
 try:
     import cupy
 except ImportError:
     pass
 
 
 def compute_prefilter_workgroup_dims(shape: Tuple[int, int, int]) -> Tuple[Tuple, Tuple]:
@@ -66,19 +65,16 @@
     # check if cupy is installed
     try:
         import cupy
 
         # add auto gpu
         available_devices.append('gpu')
 
-        # get all available gpus
-        gpu_ids = GPUtil.getAvailable()
-
-        # add gpus to list of available devices
-        for i in gpu_ids:
+        # make list of possible devices
+        for i in range(cupy.cuda.runtime.getDeviceCount()):
             available_devices.append(f'gpu:{i}')
 
     except ImportError:
         print('Warning: cupy is not found. Therefore, the only available device is "cpu".\n'
               'Please install cupy>=7.0.0b4:\npip install cupy>=7.0.0b4')
 
     return available_devices
```

### Comparing `voltools-0.5.0/voltools/utils/matrices.py` & `voltools-0.6.0/voltools/utils/matrices.py`

 * *Files identical despite different names*

### Comparing `voltools-0.5.0/voltools/volume.py` & `voltools-0.6.0/voltools/volume.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 try:
     import cupy as cp
 except ImportError:
     pass
 
 
 class StaticVolume:
-
+    """
+    For StaticVolume transforms the boolean reshape cannot be given as an argument.
+    """
     def __init__(self, data: np.ndarray, interpolation: str = 'linear', device: str = 'gpu'):
 
         if data.ndim != 3:
             raise ValueError('Expected a 3D array')
 
         if device not in get_available_devices():
             raise ValueError(f'Unknown device ({device}), must be one of {get_available_devices()}')
@@ -85,15 +87,22 @@
             del xform
             if output is None:
                 return output_vol.get()
             else:
                 return None
 
         elif self.device == 'cpu':
-            return affine(self.data, transform_m, self.interpolation, profile, output, self.device)
+            return affine(
+                self.data,
+                transform_m,
+                interpolation=self.interpolation,
+                profile=profile,
+                output=output,
+                device=self.device
+            )
 
     def transform(self, scale: Union[float, Tuple[float, float, float], np.ndarray] = None,
                   shear: Union[float, Tuple[float, float, float], np.ndarray] = None,
                   rotation: Union[Tuple[float, float, float], np.ndarray] = None,
                   rotation_units: str = 'deg', rotation_order: str = 'rzxz',
                   translation: Union[Tuple[float, float, float], np.ndarray] = None,
                   center: Union[Tuple[float, float, float], np.ndarray] = None,
```

### Comparing `voltools-0.5.0/voltools.egg-info/PKG-INFO` & `voltools-0.6.0/voltools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voltools
-Version: 0.5.0
+Version: 0.6.0
 Summary: CUDA-accelerated 3D affine transformations for NumPy and CuPy
 Home-page: https://github.com/the-lay/voltools
 Author: the-lay
 Author-email: ilja.gubin@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -113,7 +113,9 @@
                    scipy      np_transform   np_transform_out  cp_transform  cp_transform_out  static_vol  static_vol_out
 5, 5, 5           0.201232      4.528787          0.207631      0.195885          0.163193    0.109361         0.059611
 25, 25, 25        5.240529      0.332447          0.238356      0.217309          0.194111    0.138756         0.09321
 50, 50, 50       43.515086      0.804508          0.632981      0.560689          0.527334    0.474820         0.416062
 100, 100, 100   375.886700      4.232868          4.114524      3.454444          3.390018    3.091396         2.999451
 250, 250, 250  6189.052927     95.083083         94.479406     85.200392         84.435548    81.808363       80.959284
 ```
+
+
```

### Comparing `voltools-0.5.0/voltools.egg-info/SOURCES.txt` & `voltools-0.6.0/voltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

