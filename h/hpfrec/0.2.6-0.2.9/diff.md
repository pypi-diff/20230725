# Comparing `tmp/hpfrec-0.2.6.tar.gz` & `tmp/hpfrec-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpfrec-0.2.6.tar", last modified: Mon Jul  3 18:27:48 2023, max compression
+gzip compressed data, was "hpfrec-0.2.9.tar", last modified: Tue Jul 18 20:45:01 2023, max compression
```

## Comparing `hpfrec-0.2.6.tar` & `hpfrec-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:27:48.958666 hpfrec-0.2.6/
--rw-r--r--   0 david     (1000) david     (1000)     1317 2020-07-07 19:42:30.000000 hpfrec-0.2.6/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)       86 2020-07-07 19:42:22.000000 hpfrec-0.2.6/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      323 2023-07-03 18:27:48.958666 hpfrec-0.2.6/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     9089 2023-03-28 18:57:18.000000 hpfrec-0.2.6/README.md
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:27:48.958666 hpfrec-0.2.6/hpfrec/
--rw-r--r--   0 david     (1000) david     (1000)    58449 2023-07-03 18:23:35.000000 hpfrec-0.2.6/hpfrec/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      619 2023-03-19 16:26:27.000000 hpfrec-0.2.6/hpfrec/cython_double.pyx
--rw-r--r--   0 david     (1000) david     (1000)      785 2023-03-19 16:26:45.000000 hpfrec-0.2.6/hpfrec/cython_float.pyx
--rw-r--r--   0 david     (1000) david     (1000)    32584 2023-07-03 18:24:17.000000 hpfrec-0.2.6/hpfrec/cython_loops.pxi
--rw-r--r--   0 david     (1000) david     (1000)       50 2023-03-19 16:26:48.000000 hpfrec-0.2.6/hpfrec/return0.pyx
--rw-r--r--   0 david     (1000) david     (1000)       50 2023-03-19 16:26:50.000000 hpfrec-0.2.6/hpfrec/return1.pyx
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:27:48.958666 hpfrec-0.2.6/hpfrec.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      323 2023-07-03 18:27:48.000000 hpfrec-0.2.6/hpfrec.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      342 2023-07-03 18:27:48.000000 hpfrec-0.2.6/hpfrec.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-03 18:27:48.000000 hpfrec-0.2.6/hpfrec.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       38 2023-07-03 18:27:48.000000 hpfrec-0.2.6/hpfrec.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)        7 2023-07-03 18:27:48.000000 hpfrec-0.2.6/hpfrec.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       95 2021-04-15 15:58:17.000000 hpfrec-0.2.6/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)       79 2023-07-03 18:27:48.958666 hpfrec-0.2.6/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)    10273 2023-07-03 18:26:58.000000 hpfrec-0.2.6/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 20:45:01.981991 hpfrec-0.2.9/
+-rw-r--r--   0 david     (1000) david     (1000)     1317 2020-07-07 19:42:30.000000 hpfrec-0.2.9/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)       86 2020-07-07 19:42:22.000000 hpfrec-0.2.9/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      310 2023-07-18 20:45:01.981991 hpfrec-0.2.9/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     9089 2023-03-28 18:57:18.000000 hpfrec-0.2.9/README.md
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 20:45:01.981991 hpfrec-0.2.9/hpfrec/
+-rw-r--r--   0 david     (1000) david     (1000)    58449 2023-07-03 18:23:35.000000 hpfrec-0.2.9/hpfrec/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      449 2023-07-18 20:11:22.000000 hpfrec-0.2.9/hpfrec/cython_double.pxi
+-rw-r--r--   0 david     (1000) david     (1000)      532 2023-07-18 20:41:57.000000 hpfrec-0.2.9/hpfrec/cython_double_nonwindows.pyx
+-rw-r--r--   0 david     (1000) david     (1000)      527 2023-07-18 20:42:02.000000 hpfrec-0.2.9/hpfrec/cython_double_windows.pyx
+-rw-r--r--   0 david     (1000) david     (1000)      565 2023-07-18 20:12:23.000000 hpfrec-0.2.9/hpfrec/cython_float.pxi
+-rw-r--r--   0 david     (1000) david     (1000)      531 2023-07-18 20:42:13.000000 hpfrec-0.2.9/hpfrec/cython_float_nonwindows.pyx
+-rw-r--r--   0 david     (1000) david     (1000)      526 2023-07-18 20:42:04.000000 hpfrec-0.2.9/hpfrec/cython_float_windows.pyx
+-rw-r--r--   0 david     (1000) david     (1000)    31934 2023-07-18 20:42:18.000000 hpfrec-0.2.9/hpfrec/cython_loops.pxi
+-rw-r--r--   0 david     (1000) david     (1000)       50 2023-03-19 16:26:48.000000 hpfrec-0.2.9/hpfrec/return0.pyx
+-rw-r--r--   0 david     (1000) david     (1000)       50 2023-03-19 16:26:50.000000 hpfrec-0.2.9/hpfrec/return1.pyx
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 20:45:01.981991 hpfrec-0.2.9/hpfrec.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      310 2023-07-18 20:45:01.000000 hpfrec-0.2.9/hpfrec.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      439 2023-07-18 20:45:01.000000 hpfrec-0.2.9/hpfrec.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-18 20:45:01.000000 hpfrec-0.2.9/hpfrec.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)        7 2023-07-18 20:45:01.000000 hpfrec-0.2.9/hpfrec.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       99 2023-07-18 20:07:44.000000 hpfrec-0.2.9/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)       38 2023-07-18 20:45:01.981991 hpfrec-0.2.9/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)    10675 2023-07-18 20:41:33.000000 hpfrec-0.2.9/setup.py
```

### Comparing `hpfrec-0.2.6/LICENSE` & `hpfrec-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hpfrec-0.2.6/README.md` & `hpfrec-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `hpfrec-0.2.6/hpfrec/__init__.py` & `hpfrec-0.2.9/hpfrec/__init__.py`

 * *Files identical despite different names*

### Comparing `hpfrec-0.2.6/hpfrec/cython_double.pyx` & `hpfrec-0.2.9/hpfrec/cython_float.pxi`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 #cython: language_level=3
-from scipy.linalg.cython_blas cimport ddot
+import numpy as np
+cimport numpy as np
+from scipy.linalg.cython_blas cimport sdot
+from scipy.special.cython_special cimport psi, gamma
 import ctypes
 
-## TODO: use libc.math once Cython 0.30 is released
-# from libc.math cimport log, exp
-cdef extern from "<math.h>":
-	double log(double x) nogil
-	double exp(double x) nogil
-	const double HUGE_VAL
-	const long double HUGE_VALL
+from libc.math cimport log, exp, logf, expf, HUGE_VALF, HUGE_VAL, HUGE_VALL
 
-c_real_t = ctypes.c_double
-ctypedef double real_t
+c_real_t = ctypes.c_float
+ctypedef float real_t
 
 ctypedef real_t (*blas_dot)(int*, real_t*, int*, real_t*, int*) nogil
-cdef blas_dot tdot = ddot
+cdef blas_dot tdot = sdot
 
 ctypedef real_t (*real_t_fun)(real_t) nogil
-cdef real_t_fun exp_t = exp
-cdef real_t_fun log_t = log
+cdef real_t_fun exp_t = expf
+cdef real_t_fun log_t = logf
 
-cdef real_t HUGE_VAL_T = HUGE_VAL
+cdef real_t HUGE_VAL_T = HUGE_VALF
 
 include "cython_loops.pxi"
```

### Comparing `hpfrec-0.2.6/hpfrec/cython_loops.pxi` & `hpfrec-0.2.9/hpfrec/cython_loops.pxi`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,14 @@
 cimport numpy as np
 cimport cython
 from cython.parallel cimport prange
 from scipy.special.cython_special cimport psi, gamma, loggamma
 import time, os
 import ctypes
 
-## Note: As of the end of 2018, MSVC is still stuck with OpenMP 2.0 (released 2002), which does not support
-## parallel for loops with unsigend iterators. If you are using a different compiler, this part can be safely removed
-## See also: https://github.com/cython/cython/issues/3136
-IF UNAME_SYSNAME == "Windows":
-	obj_ind_type = ctypes.c_longlong
-	ctypedef long long ind_type
-	ctypedef double long_double_type
-	obj_long_double_type = ctypes.c_double
-	LD_HUGE_VAL = HUGE_VAL
-ELSE:
-	obj_ind_type = ctypes.c_size_t
-	ctypedef size_t ind_type
-	ctypedef long double long_double_type
-	obj_long_double_type = ctypes.c_longdouble
-	LD_HUGE_VAL = HUGE_VALL
-
-
 ### Helper functions
 ####################
 def cast_real_t(n):
 	return <real_t> n
 
 def cast_int(n):
 	return <int> n
```

### Comparing `hpfrec-0.2.6/setup.py` & `hpfrec-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     from setuptools import Extension
 except ImportError:
     from distutils.core import setup
     from distutils.extension import Extension
 from Cython.Distutils import build_ext
 import numpy
 import sys, os, subprocess, warnings, re
+import platform
 
 found_omp = True
 def set_omp_false():
     global found_omp
     found_omp = False
 
 ## Modify this to make the output of the compilation tests more verbose
@@ -21,14 +22,16 @@
 
 ## Workaround for python<=3.9 on windows
 try:
     EXIT_SUCCESS = os.EX_OK
 except AttributeError:
     EXIT_SUCCESS = 0
 
+IS_WINDOWS = platform.system() == "Windows"
+
 ## https://stackoverflow.com/questions/724664/python-distutils-how-to-get-a-compiler-that-is-going-to-be-used
 class build_ext_subclass( build_ext ):
     def build_extensions(self):
         if self.compiler.compiler_type == 'msvc':
             for e in self.extensions:
                 e.extra_compile_args += ['/openmp', '/O2', '/GL', '/fp:fast']
         else:
@@ -203,41 +206,45 @@
             pass
         return is_supported
 
 
 setup(
     name = 'hpfrec',
     packages = ['hpfrec'],
-    install_requires=[
-     'pandas>=0.24',
-     'numpy>=1.18',
-     'scipy',
-     'cython'
-],
-    version = '0.2.6',
+    version = '0.2.9',
     description = 'Hierarchical Poisson matrix factorization for recommender systems',
     author = 'David Cortes',
     url = 'https://github.com/david-cortes/hpfrec',
-    keywords = ['poisson', 'probabilistic', 'non-negative', 'factorization', 'variational inference', 'collaborative filtering'],
+    keywords = ['poisson', 'probabilistic', 'factorization', 'variational inference', 'collaborative filtering'],
     classifiers = [],
 
     cmdclass = {'build_ext': build_ext_subclass},
     ext_modules = [ Extension(
                         "hpfrec.cython_loops_float",
-                        sources=["hpfrec/cython_float.pyx"],
+                        sources=[
+                            "hpfrec/cython_float_nonwindows.pyx"
+                            if not IS_WINDOWS
+                            else
+                            "hpfrec/cython_float_windows.pyx"
+                        ],
                         include_dirs=[numpy.get_include()]
                     ),
                     Extension(
                         "hpfrec.cython_loops_double",
-                        sources=["hpfrec/cython_double.pyx"],
+                        sources=[
+                            "hpfrec/cython_double_nonwindows.pyx"
+                            if not IS_WINDOWS
+                            else
+                            "hpfrec/cython_double_windows.pyx"
+                        ],
                         include_dirs=[numpy.get_include()]
                     ),
                     Extension(
                         "hpfrec._check_openmp",
-                        sources=["hpfrec/return1.pyx"],
+                        sources=["hpfrec/return1.pyx" if found_omp else "hpfrec/return0.pyx"],
                         include_dirs=[numpy.get_include()]
                     ) ]
 )
 
 if not found_omp:
     omp_msg  = "\n\n\nCould not detect OpenMP. Package will be built without multi-threading capabilities. "
     omp_msg += " To enable multi-threading, first install OpenMP"
```

