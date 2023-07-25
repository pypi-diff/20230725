# Comparing `tmp/indexed_gzip-1.7.1.tar.gz` & `tmp/indexed_gzip-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexed_gzip-1.7.1.tar", last modified: Fri Mar 31 14:49:11 2023, max compression
+gzip compressed data, was "indexed_gzip-1.8.3.tar", last modified: Tue Jul 25 09:44:48 2023, max compression
```

## Comparing `indexed_gzip-1.7.1.tar` & `indexed_gzip-1.8.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:49:11.587317 indexed_gzip-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-03-31 14:49:11.583317 indexed_gzip-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:49:11.583317 indexed_gzip-1.7.1/indexed_gzip/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39575 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/indexed_gzip.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:49:11.583317 indexed_gzip-1.7.1/indexed_gzip/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/tests/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/tests/benchmark_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    34718 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/tests/ctest_indexed_gzip.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    48696 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/tests/ctest_zran.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/tests/test_indexed_gzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/tests/test_indexed_gzip_threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/tests/test_nibabel_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/tests/test_zran.py
--rw-r--r--   0 runner    (1001) docker     (123)   110980 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/zran.c
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/zran.h
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/zran.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/zran_file_util.c
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/zran_file_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/indexed_gzip/zran_file_util.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:49:11.583317 indexed_gzip-1.7.1/indexed_gzip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-03-31 14:49:11.000000 indexed_gzip-1.7.1/indexed_gzip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-31 14:49:11.000000 indexed_gzip-1.7.1/indexed_gzip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 14:49:11.000000 indexed_gzip-1.7.1/indexed_gzip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-31 14:49:11.000000 indexed_gzip-1.7.1/indexed_gzip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 14:49:11.587317 indexed_gzip-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-03-31 14:49:09.000000 indexed_gzip-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:44:48.961101 indexed_gzip-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-07-25 09:44:48.957103 indexed_gzip-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:44:48.957103 indexed_gzip-1.8.3/indexed_gzip/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39647 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/indexed_gzip.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:44:48.957103 indexed_gzip-1.8.3/indexed_gzip/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/tests/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/tests/benchmark_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34723 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/tests/ctest_indexed_gzip.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    48704 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/tests/ctest_zran.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/tests/test_indexed_gzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/tests/test_indexed_gzip_threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/tests/test_nibabel_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/tests/test_zran.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110980 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/zran.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/zran.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/zran.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/zran_file_util.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/zran_file_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/indexed_gzip/zran_file_util.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:44:48.957103 indexed_gzip-1.8.3/indexed_gzip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-07-25 09:44:48.000000 indexed_gzip-1.8.3/indexed_gzip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-25 09:44:48.000000 indexed_gzip-1.8.3/indexed_gzip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:44:48.000000 indexed_gzip-1.8.3/indexed_gzip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 09:44:48.000000 indexed_gzip-1.8.3/indexed_gzip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 09:44:48.000000 indexed_gzip-1.8.3/indexed_gzip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:44:48.961101 indexed_gzip-1.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-25 09:44:47.000000 indexed_gzip-1.8.3/setup.py
```

### Comparing `indexed_gzip-1.7.1/LICENSE` & `indexed_gzip-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/PKG-INFO` & `indexed_gzip-1.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: indexed_gzip
-Version: 1.7.1
+Version: 1.8.3
 Summary: Fast random access of gzip files in Python
-Home-page: https://github.com/pauldmccarthy/indexed_gzip
-Author: Paul McCarthy
-Author-email: pauldmccarthy@gmail.com
+Maintainer-email: Paul McCarthy <pauldmccarthy@gmail.com>
 License: zlib
+Project-URL: Repository, https://github.com/pauldmccarthy/indexed_gzip
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: zlib/libpng License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Archiving :: Compression
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # indexed_gzip
 
 
 [![PyPi version](https://img.shields.io/pypi/v/indexed_gzip.svg)](https://pypi.python.org/pypi/indexed_gzip/) [![Anaconda version](https://anaconda.org/conda-forge/indexed_gzip/badges/version.svg)](https://anaconda.org/conda-forge/indexed_gzip/)![Test status](https://github.com/pauldmccarthy/indexed_gzip/actions/workflows/master.yaml/badge.svg)
 
@@ -325,14 +326,15 @@
  - Ashwin Ramaswami (@epicfaace): Support for in-memory file objects (#55),
    bug fixes (#63, #64, #65).
  - Michał Górny (@mgorny): Remove hard dependency on `nibabel` from test suite
    (#78).
  - Alexander Gorban (@alexgorban) Fix memory leak (#82, #83).
  - Maximilian Knespel (@mxmlnkn) Change default read buffer size to
    improve performance (#90).
+ - Ben Beasley (@musicinmybrain) Python 3.12 compatibility (#126).
 
 
 ## License
 
 
 `indexed_gzip` inherits the [zlib](http://www.zlib.net) license, available for
 perusal in the [LICENSE](LICENSE) file.
```

### Comparing `indexed_gzip-1.7.1/README.md` & `indexed_gzip-1.8.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -306,14 +306,15 @@
  - Ashwin Ramaswami (@epicfaace): Support for in-memory file objects (#55),
    bug fixes (#63, #64, #65).
  - Michał Górny (@mgorny): Remove hard dependency on `nibabel` from test suite
    (#78).
  - Alexander Gorban (@alexgorban) Fix memory leak (#82, #83).
  - Maximilian Knespel (@mxmlnkn) Change default read buffer size to
    improve performance (#90).
+ - Ben Beasley (@musicinmybrain) Python 3.12 compatibility (#126).
 
 
 ## License
 
 
 `indexed_gzip` inherits the [zlib](http://www.zlib.net) license, available for
 perusal in the [LICENSE](LICENSE) file.
```

### Comparing `indexed_gzip-1.7.1/indexed_gzip/__init__.py` & `indexed_gzip-1.8.3/indexed_gzip/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 
 SafeIndexedGzipFile = IndexedGzipFile
 """Alias for ``IndexedGzipFile``, to preserve compatibility with older
 versions of ``nibabel``.
 """
 
 
-__version__ = '1.7.1'
+__version__ = '1.8.3'
```

### Comparing `indexed_gzip-1.7.1/indexed_gzip/indexed_gzip.pyx` & `indexed_gzip-1.8.3/indexed_gzip/indexed_gzip.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -165,17 +165,19 @@
         The calls to seek and read are protected by a ``threading.RLock``.
         """
         with self.__file_lock:
             self.seek(offset)
             return self.read(nbytes)
 
 
-    def __reduce__(self):
+    def __reduce_ex__(self, protocol):
         """Used to pickle an ``IndexedGzipFile``.
 
+        :arg protocol:         Pickle protocol version
+
         Returns a tuple containing:
           - a reference to the ``unpickle`` function
           - a tuple containing a "state" object, which can be passed
             to ``unpickle``.
         """
 
         fobj = self.__igz_fobj
@@ -1089,15 +1091,15 @@
         log.debug('ReadBuffer.__dealloc__()')
 
 
 def unpickle(state):
     """Create a new ``IndexedGzipFile`` from a pickled state.
 
     :arg state: State of a pickled object, as returned by the
-                ``IndexedGzipFile.__reduce__`` method.
+                ``IndexedGzipFile.__reduce_ex__`` method.
 
     :returns:   A new ``IndexedGzipFile`` object.
     """
 
     tell  = state.pop('tell')
     index = state.pop('index')
     gzobj = IndexedGzipFile(**state)
```

### Comparing `indexed_gzip-1.7.1/indexed_gzip/tests/__init__.py` & `indexed_gzip-1.8.3/indexed_gzip/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip/tests/__main__.py` & `indexed_gzip-1.8.3/indexed_gzip/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip/tests/benchmark.py` & `indexed_gzip-1.8.3/indexed_gzip/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip/tests/benchmark_bandwidth.py` & `indexed_gzip-1.8.3/indexed_gzip/tests/benchmark_bandwidth.py`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip/tests/conftest.py` & `indexed_gzip-1.8.3/indexed_gzip/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip/tests/ctest_indexed_gzip.pyx` & `indexed_gzip-1.8.3/indexed_gzip/tests/ctest_indexed_gzip.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1154,15 +1154,15 @@
         data = np.arange(10000000, dtype=np.uint32)
         with gzip.open(fname, 'wb') as f:
             f.write(data.tobytes())
         del f
 
         gzf = igzip.IndexedGzipFile(fname)
 
-        size    = len(data) / 16
+        size    = int(len(data) / 16)
         offsets = np.arange(0, len(data), size)
         func    = ft.partial(_mpfunc, gzf, size * 4)
 
         pool = mp.Pool(8)
         results = pool.map(func, offsets * 4)
         pool.close()
         pool.join()
```

### Comparing `indexed_gzip-1.7.1/indexed_gzip/tests/ctest_zran.pyx` & `indexed_gzip-1.8.3/indexed_gzip/tests/ctest_zran.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -792,15 +792,15 @@
         nbytes = zran.zran_read(&index, buffer, filesize)
 
         assert nbytes                 == filesize
         assert zran.zran_tell(&index) == nbytes
 
         zran.zran_free(&index)
 
-    nelemsp = nbytes / 8.
+    nelemsp = int(nbytes / 8)
     data    = np.PyArray_SimpleNewFromData(1, &nelemsp,  np.NPY_UINT64, buffer)
 
     assert check_data_valid(data, 0)
 
 
 def test_seek_then_read_block(testfile, no_fds, nelems, niters, seed, use_mmap):
 
@@ -851,15 +851,15 @@
                 print('readelems:   {}'.format(readelems))
                 print('nbytes:      {}'.format(nbytes))
                 print('  should be: {}'.format(readelems * 8))
                 print('ftell:       {}'.format(zran.zran_tell(&index)))
                 print('  should be: {}'.format((se + readelems) * 8))
                 raise
 
-            nelemsp = nbytes / 8.
+            nelemsp = int(nbytes / 8)
             data    = np.PyArray_SimpleNewFromData(1, &nelemsp,  np.NPY_UINT64, buffer)
 
             assert check_data_valid(data, se, se + readelems)
 
             end = time.time()
 
             print("{:0.2f} seconds".format(end - start))
```

### Comparing `indexed_gzip-1.7.1/indexed_gzip/tests/test_indexed_gzip.py` & `indexed_gzip-1.8.3/indexed_gzip/tests/test_indexed_gzip.py`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip/tests/test_indexed_gzip_threading.py` & `indexed_gzip-1.8.3/indexed_gzip/tests/test_indexed_gzip_threading.py`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip/tests/test_nibabel_integration.py` & `indexed_gzip-1.8.3/indexed_gzip/tests/test_nibabel_integration.py`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip/tests/test_zran.py` & `indexed_gzip-1.8.3/indexed_gzip/tests/test_zran.py`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip/zran.c` & `indexed_gzip-1.8.3/indexed_gzip/zran.c`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip/zran.h` & `indexed_gzip-1.8.3/indexed_gzip/zran.h`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip/zran.pxd` & `indexed_gzip-1.8.3/indexed_gzip/zran.pxd`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip/zran_file_util.c` & `indexed_gzip-1.8.3/indexed_gzip/zran_file_util.c`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip/zran_file_util.h` & `indexed_gzip-1.8.3/indexed_gzip/zran_file_util.h`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip/zran_file_util.pxd` & `indexed_gzip-1.8.3/indexed_gzip/zran_file_util.pxd`

 * *Files identical despite different names*

### Comparing `indexed_gzip-1.7.1/indexed_gzip.egg-info/PKG-INFO` & `indexed_gzip-1.8.3/indexed_gzip.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: indexed-gzip
-Version: 1.7.1
+Version: 1.8.3
 Summary: Fast random access of gzip files in Python
-Home-page: https://github.com/pauldmccarthy/indexed_gzip
-Author: Paul McCarthy
-Author-email: pauldmccarthy@gmail.com
+Maintainer-email: Paul McCarthy <pauldmccarthy@gmail.com>
 License: zlib
+Project-URL: Repository, https://github.com/pauldmccarthy/indexed_gzip
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: zlib/libpng License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Archiving :: Compression
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # indexed_gzip
 
 
 [![PyPi version](https://img.shields.io/pypi/v/indexed_gzip.svg)](https://pypi.python.org/pypi/indexed_gzip/) [![Anaconda version](https://anaconda.org/conda-forge/indexed_gzip/badges/version.svg)](https://anaconda.org/conda-forge/indexed_gzip/)![Test status](https://github.com/pauldmccarthy/indexed_gzip/actions/workflows/master.yaml/badge.svg)
 
@@ -325,14 +326,15 @@
  - Ashwin Ramaswami (@epicfaace): Support for in-memory file objects (#55),
    bug fixes (#63, #64, #65).
  - Michał Górny (@mgorny): Remove hard dependency on `nibabel` from test suite
    (#78).
  - Alexander Gorban (@alexgorban) Fix memory leak (#82, #83).
  - Maximilian Knespel (@mxmlnkn) Change default read buffer size to
    improve performance (#90).
+ - Ben Beasley (@musicinmybrain) Python 3.12 compatibility (#126).
 
 
 ## License
 
 
 `indexed_gzip` inherits the [zlib](http://www.zlib.net) license, available for
 perusal in the [LICENSE](LICENSE) file.
```

### Comparing `indexed_gzip-1.7.1/indexed_gzip.egg-info/SOURCES.txt` & `indexed_gzip-1.8.3/indexed_gzip.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 indexed_gzip/zran.pxd
 indexed_gzip/zran_file_util.c
 indexed_gzip/zran_file_util.h
 indexed_gzip/zran_file_util.pxd
 indexed_gzip.egg-info/PKG-INFO
 indexed_gzip.egg-info/SOURCES.txt
 indexed_gzip.egg-info/dependency_links.txt
+indexed_gzip.egg-info/requires.txt
 indexed_gzip.egg-info/top_level.txt
 indexed_gzip/tests/__init__.py
 indexed_gzip/tests/__main__.py
 indexed_gzip/tests/benchmark.py
 indexed_gzip/tests/benchmark_bandwidth.py
 indexed_gzip/tests/conftest.py
 indexed_gzip/tests/ctest_indexed_gzip.pyx
```

### Comparing `indexed_gzip-1.7.1/setup.py` & `indexed_gzip-1.8.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -72,30 +72,25 @@
         for f in files:
             for g in glob.glob(f):
                 try:            os.remove(g)
                 except OSError: pass
 
 
 # Platform information
-python2   = sys.version_info[0] == 2
-noc99     = python2 or (sys.version_info[0] == 3 and sys.version_info[1] <= 4)
+noc99     = sys.version_info[0] == 3 and sys.version_info[1] <= 4
 windows   = sys.platform.startswith("win")
 testing   = 'INDEXED_GZIP_TESTING' in os.environ
+thisdir   = op.dirname(__file__)
 
 # compile ZLIB source?
 ZLIB_HOME = os.environ.get("ZLIB_HOME", None)
-
-# Load README description
-readme = op.join(op.dirname(__file__), 'README.md')
-if python2:
-    openreadme = ft.partial(open, readme, 'rt')
-else:
-    openreadme = ft.partial(open, readme, 'rt', encoding='utf-8')
-with openreadme() as f:
-    readme = f.read().strip()
+# setuptools may complain about
+# absolute paths in some circumstances
+if ZLIB_HOME is not None:
+    ZLIB_HOME = op.relpath(ZLIB_HOME, thisdir)
 
 # If cython is present, we'll compile
 # the pyx files from scratch. Otherwise,
 # we'll compile the pre-generated c
 # files (which are assumed to be present).
 have_cython = True
 have_numpy  = True
@@ -141,19 +136,14 @@
 if have_numpy:
     include_dirs.append(np.get_include())
 
 if windows:
     if ZLIB_HOME is None:
         libs.append('zlib')
 
-    # For stdint.h which is not included in the old Visual C
-    # compiler used for Python 2
-    if python2:
-        include_dirs.append('compat')
-
     # Some C functions might not be present when compiling against
     # older versions of python
     if noc99:
         extra_compile_args += ['-DNO_C99']
 
 # linux / macOS
 else:
@@ -215,50 +205,12 @@
 else:          extensions = [igzip_ext]
 
 
 # Cythonize if we can
 if have_cython:
     extensions = cythonize(extensions, compiler_directives=compiler_directives)
 
-
-# find the version number
-def readVersion():
-    version  = {}
-    initfile = op.join(op.dirname(__file__), 'indexed_gzip', '__init__.py')
-    with open(initfile, 'rt') as f:
-        for line in f:
-            if line.startswith('__version__'):
-                exec(line, version)
-                break
-    return version.get('__version__')
-
-
 setup(
     name='indexed_gzip',
-    packages=['indexed_gzip', 'indexed_gzip.tests'],
-    version=readVersion(),
-    author='Paul McCarthy',
-    author_email='pauldmccarthy@gmail.com',
-    description='Fast random access of gzip files in Python',
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    url='https://github.com/pauldmccarthy/indexed_gzip',
-    license='zlib',
-
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: zlib/libpng License',
-        'Programming Language :: C',
-        'Programming Language :: Cython',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 3',
-        'Topic :: System :: Archiving :: Compression',
-    ],
-
     cmdclass={'clean' : Clean},
-
     ext_modules=extensions,
-
-    tests_require=['pytest', 'numpy', 'nibabel'],
-    test_suite='tests',
 )
```

