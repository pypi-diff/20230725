# Comparing `tmp/pysndlib-0.5.0.tar.gz` & `tmp/pysndlib-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysndlib-0.5.0.tar", last modified: Tue Jul 25 03:27:47 2023, max compression
+gzip compressed data, was "pysndlib-0.5.1.tar", last modified: Tue Jul 25 04:26:04 2023, max compression
```

## Comparing `pysndlib-0.5.0.tar` & `pysndlib-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-25 03:27:47.791834 pysndlib-0.5.0/
--rw-r--r--   0 runner     (501) staff       (20)     1068 2023-07-25 03:27:09.000000 pysndlib-0.5.0/LICENSE.md
--rw-r--r--   0 runner     (501) staff       (20)     1020 2023-07-25 03:27:47.791416 pysndlib-0.5.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      516 2023-07-25 03:27:09.000000 pysndlib-0.5.0/README.md
--rw-r--r--   0 runner     (501) staff       (20)      659 2023-07-25 03:27:09.000000 pysndlib-0.5.0/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-25 03:27:47.792010 pysndlib-0.5.0/setup.cfg
--rwxr-xr-x   0 runner     (501) staff       (20)     2728 2023-07-25 03:27:09.000000 pysndlib-0.5.0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-25 03:27:47.751649 pysndlib-0.5.0/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-25 03:27:47.788911 pysndlib-0.5.0/src/pysndlib/
--rw-r--r--   0 runner     (501) staff       (20)        2 2023-07-25 03:27:09.000000 pysndlib-0.5.0/src/pysndlib/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      213 2023-07-25 03:27:09.000000 pysndlib-0.5.0/src/pysndlib/analog_filter.py
--rw-r--r--   0 runner     (501) staff       (20)  6402117 2023-07-25 03:27:43.000000 pysndlib-0.5.0/src/pysndlib/clm.c
--rwxr-xr-x   0 runner     (501) staff       (20)    81331 2023-07-25 03:27:09.000000 pysndlib-0.5.0/src/pysndlib/clm_ins.py
--rwxr-xr-x   0 runner     (501) staff       (20)     6664 2023-07-25 03:27:09.000000 pysndlib-0.5.0/src/pysndlib/dsp.py
--rwxr-xr-x   0 runner     (501) staff       (20)     6286 2023-07-25 03:27:09.000000 pysndlib-0.5.0/src/pysndlib/env.py
--rwxr-xr-x   0 runner     (501) staff       (20)    46172 2023-07-25 03:27:09.000000 pysndlib-0.5.0/src/pysndlib/generators.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1735 2023-07-25 03:27:09.000000 pysndlib-0.5.0/src/pysndlib/jcrev.py
--rw-r--r--   0 runner     (501) staff       (20)      985 2023-07-25 03:27:09.000000 pysndlib-0.5.0/src/pysndlib/musx.py
--rw-r--r--   0 runner     (501) staff       (20)  2542556 2023-07-25 03:27:46.000000 pysndlib-0.5.0/src/pysndlib/sndlib.c
--rw-r--r--   0 runner     (501) staff       (20)     2978 2023-07-25 03:27:09.000000 pysndlib-0.5.0/src/pysndlib/v.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-25 03:27:47.790877 pysndlib-0.5.0/src/pysndlib.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     1020 2023-07-25 03:27:47.000000 pysndlib-0.5.0/src/pysndlib.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      436 2023-07-25 03:27:47.000000 pysndlib-0.5.0/src/pysndlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-25 03:27:47.000000 pysndlib-0.5.0/src/pysndlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2023-07-25 03:27:47.000000 pysndlib-0.5.0/src/pysndlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-25 04:26:04.298030 pysndlib-0.5.1/
+-rw-r--r--   0 runner     (501) staff       (20)     1068 2023-07-25 04:25:28.000000 pysndlib-0.5.1/LICENSE.md
+-rw-r--r--   0 runner     (501) staff       (20)     1020 2023-07-25 04:26:04.297616 pysndlib-0.5.1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      516 2023-07-25 04:25:28.000000 pysndlib-0.5.1/README.md
+-rw-r--r--   0 runner     (501) staff       (20)      704 2023-07-25 04:25:28.000000 pysndlib-0.5.1/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-25 04:26:04.298131 pysndlib-0.5.1/setup.cfg
+-rwxr-xr-x   0 runner     (501) staff       (20)     2728 2023-07-25 04:25:28.000000 pysndlib-0.5.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-25 04:26:04.262664 pysndlib-0.5.1/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-25 04:26:04.294260 pysndlib-0.5.1/src/pysndlib/
+-rw-r--r--   0 runner     (501) staff       (20)        2 2023-07-25 04:25:28.000000 pysndlib-0.5.1/src/pysndlib/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      213 2023-07-25 04:25:28.000000 pysndlib-0.5.1/src/pysndlib/analog_filter.py
+-rw-r--r--   0 runner     (501) staff       (20)  6402117 2023-07-25 04:26:00.000000 pysndlib-0.5.1/src/pysndlib/clm.c
+-rwxr-xr-x   0 runner     (501) staff       (20)    81331 2023-07-25 04:25:28.000000 pysndlib-0.5.1/src/pysndlib/clm_ins.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     6664 2023-07-25 04:25:28.000000 pysndlib-0.5.1/src/pysndlib/dsp.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     6286 2023-07-25 04:25:28.000000 pysndlib-0.5.1/src/pysndlib/env.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    46172 2023-07-25 04:25:28.000000 pysndlib-0.5.1/src/pysndlib/generators.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1735 2023-07-25 04:25:28.000000 pysndlib-0.5.1/src/pysndlib/jcrev.py
+-rw-r--r--   0 runner     (501) staff       (20)      985 2023-07-25 04:25:28.000000 pysndlib-0.5.1/src/pysndlib/musx.py
+-rw-r--r--   0 runner     (501) staff       (20)  2542556 2023-07-25 04:26:03.000000 pysndlib-0.5.1/src/pysndlib/sndlib.c
+-rw-r--r--   0 runner     (501) staff       (20)     2978 2023-07-25 04:25:28.000000 pysndlib-0.5.1/src/pysndlib/v.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-25 04:26:04.296975 pysndlib-0.5.1/src/pysndlib.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     1020 2023-07-25 04:26:04.000000 pysndlib-0.5.1/src/pysndlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      471 2023-07-25 04:26:04.000000 pysndlib-0.5.1/src/pysndlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-25 04:26:04.000000 pysndlib-0.5.1/src/pysndlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       20 2023-07-25 04:26:04.000000 pysndlib-0.5.1/src/pysndlib.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2023-07-25 04:26:04.000000 pysndlib-0.5.1/src/pysndlib.egg-info/top_level.txt
```

### Comparing `pysndlib-0.5.0/LICENSE.md` & `pysndlib-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysndlib-0.5.0/PKG-INFO` & `pysndlib-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysndlib
-Version: 0.5.0
+Version: 0.5.1
 Summary: A python wrapper around sndlib
 Author-email: Todd Ingalls <testcase@asu.edu>
 Project-URL: Homepage, https://github.com/testcase/pysndlib
 Project-URL: Bug Tracker, https://github.com/testcase/pysndlib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pysndlib-0.5.0/README.md` & `pysndlib-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pysndlib-0.5.0/pyproject.toml` & `pysndlib-0.5.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [project]
 name = "pysndlib"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="Todd Ingalls", email="testcase@asu.edu" },
 ]
 description = "A python wrapper around sndlib"
+dependencies = ["numpy", "Cython>=3.0.0"]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -19,7 +20,10 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "Cython>=3.0.0", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
+
+
+
```

### Comparing `pysndlib-0.5.0/setup.py` & `pysndlib-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `pysndlib-0.5.0/src/pysndlib/clm.c` & `pysndlib-0.5.1/src/pysndlib/clm.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,28 +6,28 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-Wno-parentheses-equality"
         ],
         "extra_objects": [
             "./sndlib/libsndlib.a"
         ],
         "include_dirs": [
-            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/core/include",
+            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/core/include",
             "./sndlib"
         ],
         "name": "pysndlib.clm",
         "sources": [
             "src/pysndlib/clm.pyx"
         ]
     },
@@ -1565,177 +1565,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1779,42 +1779,42 @@
 struct __pyx_obj_8pysndlib_3clm___pyx_scope_struct_6_array_reader;
 struct __pyx_obj___Pyx_EnumMeta;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -29139,261 +29139,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -29402,29 +29402,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -29435,15 +29435,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -29452,29 +29452,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -29485,15 +29485,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -29502,29 +29502,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -29535,15 +29535,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -29552,29 +29552,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -29585,15 +29585,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -29602,29 +29602,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -29635,89 +29635,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -29725,33 +29725,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -29759,96 +29759,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -29864,15 +29864,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -29880,68 +29880,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 983, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -29949,15 +29949,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -29972,15 +29972,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -29996,15 +29996,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -30012,68 +30012,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 989, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -30081,15 +30081,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -30104,15 +30104,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -30128,15 +30128,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -30144,68 +30144,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 995, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -30213,15 +30213,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -30236,176 +30236,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -117246,26 +117246,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__10 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 983, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 989, __pyx_L1_error)
```

### Comparing `pysndlib-0.5.0/src/pysndlib/clm_ins.py` & `pysndlib-0.5.1/src/pysndlib/clm_ins.py`

 * *Files identical despite different names*

### Comparing `pysndlib-0.5.0/src/pysndlib/dsp.py` & `pysndlib-0.5.1/src/pysndlib/dsp.py`

 * *Files identical despite different names*

### Comparing `pysndlib-0.5.0/src/pysndlib/env.py` & `pysndlib-0.5.1/src/pysndlib/env.py`

 * *Files identical despite different names*

### Comparing `pysndlib-0.5.0/src/pysndlib/generators.py` & `pysndlib-0.5.1/src/pysndlib/generators.py`

 * *Files identical despite different names*

### Comparing `pysndlib-0.5.0/src/pysndlib/jcrev.py` & `pysndlib-0.5.1/src/pysndlib/jcrev.py`

 * *Files identical despite different names*

### Comparing `pysndlib-0.5.0/src/pysndlib/musx.py` & `pysndlib-0.5.1/src/pysndlib/musx.py`

 * *Files identical despite different names*

### Comparing `pysndlib-0.5.0/src/pysndlib/sndlib.c` & `pysndlib-0.5.1/src/pysndlib/sndlib.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,28 +6,28 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-Wno-parentheses-equality"
         ],
         "extra_objects": [
             "./sndlib/libsndlib.a"
         ],
         "include_dirs": [
-            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/core/include",
+            "/private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/core/include",
             "./sndlib"
         ],
         "name": "pysndlib.sndlib",
         "sources": [
             "src/pysndlib/sndlib.pyx"
         ]
     },
@@ -1552,177 +1552,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1756,42 +1756,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj___Pyx_EnumMeta;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -24394,261 +24394,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -24657,29 +24657,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -24690,15 +24690,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -24707,29 +24707,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -24740,15 +24740,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -24757,29 +24757,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -24790,15 +24790,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -24807,29 +24807,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -24840,15 +24840,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -24857,29 +24857,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -24890,89 +24890,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -24980,33 +24980,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -25014,96 +25014,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -25119,15 +25119,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -25135,68 +25135,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 983, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -25204,15 +25204,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -25227,15 +25227,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -25251,15 +25251,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -25267,68 +25267,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 989, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -25336,15 +25336,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -25359,15 +25359,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -25383,15 +25383,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -25399,68 +25399,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 995, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -25468,15 +25468,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -25491,176 +25491,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -33875,26 +33875,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__10 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 983, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-shgxn5mo/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../private/var/folders/24/8k48jl6d249_n_qfxwsl6xvm0000gn/T/build-env-pxzqgnlt/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 989, __pyx_L1_error)
```

### Comparing `pysndlib-0.5.0/src/pysndlib/v.py` & `pysndlib-0.5.1/src/pysndlib/v.py`

 * *Files identical despite different names*

### Comparing `pysndlib-0.5.0/src/pysndlib.egg-info/PKG-INFO` & `pysndlib-0.5.1/src/pysndlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysndlib
-Version: 0.5.0
+Version: 0.5.1
 Summary: A python wrapper around sndlib
 Author-email: Todd Ingalls <testcase@asu.edu>
 Project-URL: Homepage, https://github.com/testcase/pysndlib
 Project-URL: Bug Tracker, https://github.com/testcase/pysndlib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

