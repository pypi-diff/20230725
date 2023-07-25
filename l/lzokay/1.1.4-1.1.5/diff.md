# Comparing `tmp/lzokay-1.1.4.tar.gz` & `tmp/lzokay-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lzokay-1.1.4.tar", last modified: Mon Jul 24 18:57:33 2023, max compression
+gzip compressed data, was "lzokay-1.1.5.tar", last modified: Tue Jul 25 11:13:23 2023, max compression
```

## Comparing `lzokay-1.1.4.tar` & `lzokay-1.1.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/.github/
--rw-rw-rw-   0        0        0      730 2023-07-24 18:55:58.000000 lzokay-1.1.4/.github/dependabot.yml
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/.github/workflows/
--rw-rw-rw-   0        0        0      618 2023-07-24 18:55:58.000000 lzokay-1.1.4/.github/workflows/dependabot.yml
--rw-rw-rw-   0        0        0     4572 2023-07-24 18:55:58.000000 lzokay-1.1.4/.github/workflows/python.yml
--rw-rw-rw-   0        0        0     1992 2023-07-24 18:55:58.000000 lzokay-1.1.4/.gitignore
--rw-rw-rw-   0        0        0       96 2023-07-24 18:55:58.000000 lzokay-1.1.4/.gitmodules
--rw-rw-rw-   0        0        0      432 2023-07-24 18:55:58.000000 lzokay-1.1.4/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1108 2023-07-24 18:55:58.000000 lzokay-1.1.4/LICENSE
--rw-rw-rw-   0        0        0       58 2023-07-24 18:55:58.000000 lzokay-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      786 2023-07-24 18:57:33.831189 lzokay-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-07-24 18:55:58.000000 lzokay-1.1.4/README.md
--rw-rw-rw-   0        0        0   438217 2023-07-24 18:57:31.000000 lzokay-1.1.4/_lzokay.cpp
--rw-rw-rw-   0        0        0     2329 2023-07-24 18:55:58.000000 lzokay-1.1.4/_lzokay.pyx
--rw-rw-rw-   0        0        0      541 2023-07-24 18:55:58.000000 lzokay-1.1.4/lzokay_wrap.pxd
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.815564 lzokay-1.1.4/native/
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/native/lzokay/
--rw-rw-rw-   0        0        0       41 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/.git
--rw-rw-rw-   0        0        0     1705 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/CMakeLists.txt
--rw-rw-rw-   0        0        0      111 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/Config.cmake.in
--rw-rw-rw-   0        0        0     1097 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/LICENSE
--rw-rw-rw-   0        0        0     1892 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/native/lzokay/lzokay-c/
--rw-rw-rw-   0        0        0      204 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/lzokay-c/CMakeLists.txt
--rw-rw-rw-   0        0        0     1084 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/lzokay-c/lzokay-c.cpp
--rw-rw-rw-   0        0        0      566 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/lzokay-c/lzokay-c.h
--rw-rw-rw-   0        0        0    21184 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/lzokay.cpp
--rw-rw-rw-   0        0        0     2558 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/lzokay.hpp
--rw-rw-rw-   0        0        0     1305 2023-07-24 18:56:00.000000 lzokay-1.1.4/native/lzokay/test.cpp
--rw-rw-rw-   0        0        0     1495 2023-07-24 18:55:58.000000 lzokay-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      137 2023-07-24 18:57:33.831189 lzokay-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1165 2023-07-24 18:55:58.000000 lzokay-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.815564 lzokay-1.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/src/lzokay/
--rw-rw-rw-   0        0        0      275 2023-07-24 18:55:58.000000 lzokay-1.1.4/src/lzokay/__init__.py
--rw-rw-rw-   0        0        0      164 2023-07-24 18:57:33.000000 lzokay-1.1.4/src/lzokay/version.py
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/src/lzokay.egg-info/
--rw-rw-rw-   0        0        0      786 2023-07-24 18:57:33.000000 lzokay-1.1.4/src/lzokay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      775 2023-07-24 18:57:33.000000 lzokay-1.1.4/src/lzokay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 18:57:33.000000 lzokay-1.1.4/src/lzokay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-24 18:57:33.000000 lzokay-1.1.4/src/lzokay.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-24 18:57:33.000000 lzokay-1.1.4/src/lzokay.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:33.831189 lzokay-1.1.4/tests/
--rw-rw-rw-   0        0        0      493 2023-07-24 18:55:58.000000 lzokay-1.1.4/tests/test_native.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:13:23.826550 lzokay-1.1.5/
+drwxrwxrwx   0        0        0        0 2023-07-25 11:13:23.795192 lzokay-1.1.5/.github/
+-rw-rw-rw-   0        0        0      730 2023-07-25 11:12:21.000000 lzokay-1.1.5/.github/dependabot.yml
+drwxrwxrwx   0        0        0        0 2023-07-25 11:13:23.810818 lzokay-1.1.5/.github/workflows/
+-rw-rw-rw-   0        0        0      618 2023-07-25 11:12:21.000000 lzokay-1.1.5/.github/workflows/dependabot.yml
+-rw-rw-rw-   0        0        0     4572 2023-07-25 11:12:21.000000 lzokay-1.1.5/.github/workflows/python.yml
+-rw-rw-rw-   0        0        0     1992 2023-07-25 11:12:21.000000 lzokay-1.1.5/.gitignore
+-rw-rw-rw-   0        0        0       96 2023-07-25 11:12:21.000000 lzokay-1.1.5/.gitmodules
+-rw-rw-rw-   0        0        0      432 2023-07-25 11:12:21.000000 lzokay-1.1.5/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1108 2023-07-25 11:12:21.000000 lzokay-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0       58 2023-07-25 11:12:21.000000 lzokay-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      786 2023-07-25 11:13:23.826550 lzokay-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-07-25 11:12:21.000000 lzokay-1.1.5/README.md
+-rw-rw-rw-   0        0        0   402406 2023-07-25 11:13:21.000000 lzokay-1.1.5/_lzokay.cpp
+-rw-rw-rw-   0        0        0     2329 2023-07-25 11:12:21.000000 lzokay-1.1.5/_lzokay.pyx
+-rw-rw-rw-   0        0        0      540 2023-07-25 11:12:21.000000 lzokay-1.1.5/lzokay_wrap.pxd
+drwxrwxrwx   0        0        0        0 2023-07-25 11:13:23.795192 lzokay-1.1.5/native/
+drwxrwxrwx   0        0        0        0 2023-07-25 11:13:23.810818 lzokay-1.1.5/native/lzokay/
+-rw-rw-rw-   0        0        0       41 2023-07-25 11:12:23.000000 lzokay-1.1.5/native/lzokay/.git
+-rw-rw-rw-   0        0        0     1705 2023-07-25 11:12:23.000000 lzokay-1.1.5/native/lzokay/CMakeLists.txt
+-rw-rw-rw-   0        0        0      111 2023-07-25 11:12:23.000000 lzokay-1.1.5/native/lzokay/Config.cmake.in
+-rw-rw-rw-   0        0        0     1097 2023-07-25 11:12:23.000000 lzokay-1.1.5/native/lzokay/LICENSE
+-rw-rw-rw-   0        0        0     1892 2023-07-25 11:12:23.000000 lzokay-1.1.5/native/lzokay/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 11:13:23.810818 lzokay-1.1.5/native/lzokay/lzokay-c/
+-rw-rw-rw-   0        0        0      204 2023-07-25 11:12:23.000000 lzokay-1.1.5/native/lzokay/lzokay-c/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1084 2023-07-25 11:12:23.000000 lzokay-1.1.5/native/lzokay/lzokay-c/lzokay-c.cpp
+-rw-rw-rw-   0        0        0      566 2023-07-25 11:12:23.000000 lzokay-1.1.5/native/lzokay/lzokay-c/lzokay-c.h
+-rw-rw-rw-   0        0        0    21184 2023-07-25 11:12:23.000000 lzokay-1.1.5/native/lzokay/lzokay.cpp
+-rw-rw-rw-   0        0        0     2558 2023-07-25 11:12:23.000000 lzokay-1.1.5/native/lzokay/lzokay.hpp
+-rw-rw-rw-   0        0        0     1305 2023-07-25 11:12:23.000000 lzokay-1.1.5/native/lzokay/test.cpp
+-rw-rw-rw-   0        0        0     1553 2023-07-25 11:12:21.000000 lzokay-1.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      137 2023-07-25 11:13:23.826550 lzokay-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2023-07-25 11:12:21.000000 lzokay-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:13:23.795192 lzokay-1.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 11:13:23.810818 lzokay-1.1.5/src/lzokay/
+-rw-rw-rw-   0        0        0      275 2023-07-25 11:12:21.000000 lzokay-1.1.5/src/lzokay/__init__.py
+-rw-rw-rw-   0        0        0      164 2023-07-25 11:13:23.000000 lzokay-1.1.5/src/lzokay/version.py
+drwxrwxrwx   0        0        0        0 2023-07-25 11:13:23.826550 lzokay-1.1.5/src/lzokay.egg-info/
+-rw-rw-rw-   0        0        0      786 2023-07-25 11:13:23.000000 lzokay-1.1.5/src/lzokay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2023-07-25 11:13:23.000000 lzokay-1.1.5/src/lzokay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 11:13:23.000000 lzokay-1.1.5/src/lzokay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-25 11:13:23.000000 lzokay-1.1.5/src/lzokay.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-25 11:13:23.000000 lzokay-1.1.5/src/lzokay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 11:13:23.826550 lzokay-1.1.5/tests/
+-rw-rw-rw-   0        0        0      493 2023-07-25 11:12:21.000000 lzokay-1.1.5/tests/test_native.py
```

### Comparing `lzokay-1.1.4/.github/dependabot.yml` & `lzokay-1.1.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/.github/workflows/dependabot.yml` & `lzokay-1.1.5/.github/workflows/dependabot.yml`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/.github/workflows/python.yml` & `lzokay-1.1.5/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/.gitignore` & `lzokay-1.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/LICENSE` & `lzokay-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/PKG-INFO` & `lzokay-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lzokay
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python bindings for LZ👌, a LZO compression/decompression algorithm.
 Author: Henrique Gemignani
 Project-URL: Homepage, https://github.com/henriquegemignani/py-lzokay
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lzokay-1.1.4/_lzokay.cpp` & `lzokay-1.1.5/_lzokay.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1400,15 +1400,14 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "<stringsource>",
   "contextvars.pxd",
   "array.pxd",
   "_lzokay.pyx",
   "type.pxd",
   "bool.pxd",
   "complex.pxd",
 };
@@ -1538,14 +1537,56 @@
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
+/* TupleAndListFromArray.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
+#endif
+
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* fastcall.proto */
+#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
+#define __Pyx_KwValues_VARARGS(args, nargs) NULL
+#define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
+#define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
+#if CYTHON_METH_FASTCALL
+    #define __Pyx_Arg_FASTCALL(args, i) args[i]
+    #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
+    #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
+    static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+    #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+#else
+    #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
+    #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
+    #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
+    #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
+    #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
+#else
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#endif
+
 /* PyErrExceptionMatches.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
 static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
 #define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
@@ -1602,179 +1643,14 @@
 
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
-/* Import.proto */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
-
-/* ImportFrom.proto */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
-
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
-#endif
-
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
-#endif
-
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
-#endif
-
-/* ImportDottedModule.proto */
-static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
-#if PY_MAJOR_VERSION >= 3
-static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
-#endif
-
-/* PyFunctionFastCall.proto */
-#if CYTHON_FAST_PYCALL
-#if !CYTHON_VECTORCALL
-#define __Pyx_PyFunction_FastCall(func, args, nargs)\
-    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#endif
-#define __Pyx_BUILD_ASSERT_EXPR(cond)\
-    (sizeof(char [1 - 2*!(cond)]) - 1)
-#ifndef Py_MEMBER_SIZE
-#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
-#endif
-#if !CYTHON_VECTORCALL
-#if PY_VERSION_HEX >= 0x03080000
-  #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
-  #define __Pxy_PyFrame_Initialize_Offsets()
-  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
-#else
-  static size_t __pyx_pyframe_localsplus_offset = 0;
-  #include "frameobject.h"
-  #define __Pxy_PyFrame_Initialize_Offsets()\
-    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
-     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
-  #define __Pyx_PyFrame_GetLocalsplus(frame)\
-    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif
-#endif
-#endif
-
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
-#else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
-#endif
-
-/* PyObjectCallMethO.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
-#endif
-
-/* PyObjectFastCall.proto */
-#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
-static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
-
-/* GCCDiagnostics.proto */
-#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
-#define __Pyx_HAS_GCC_DIAGNOSTIC
-#endif
-
-/* BuildPyUnicode.proto */
-static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
-                                                int prepend_sign, char padding_char);
-
-/* IncludeStringH.proto */
-#include <string.h>
-
-/* CIntToPyUnicode.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char);
-
-/* UnicodeConcatInPlace.proto */
-# if CYTHON_COMPILING_IN_CPYTHON && PY_MAJOR_VERSION >= 3
-    #if CYTHON_REFNANNY
-        #define __Pyx_PyUnicode_ConcatInPlace(left, right) __Pyx_PyUnicode_ConcatInPlaceImpl(&left, right, __pyx_refnanny)
-    #else
-        #define __Pyx_PyUnicode_ConcatInPlace(left, right) __Pyx_PyUnicode_ConcatInPlaceImpl(&left, right)
-    #endif
-    static CYTHON_INLINE PyObject *__Pyx_PyUnicode_ConcatInPlaceImpl(PyObject **p_left, PyObject *right
-        #if CYTHON_REFNANNY
-        , void* __pyx_refnanny
-        #endif
-    );
-#else
-#define __Pyx_PyUnicode_ConcatInPlace __Pyx_PyUnicode_Concat
-#endif
-#define __Pyx_PyUnicode_ConcatInPlaceSafe(left, right) ((unlikely((left) == Py_None) || unlikely((right) == Py_None)) ?\
-    PyNumber_InPlaceAdd(left, right) : __Pyx_PyUnicode_ConcatInPlace(left, right))
-
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
-
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
-/* TupleAndListFromArray.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
-static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
-#endif
-
-/* BytesEquals.proto */
-static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
-
-/* UnicodeEquals.proto */
-static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
-
-/* fastcall.proto */
-#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
-#define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
-#define __Pyx_KwValues_VARARGS(args, nargs) NULL
-#define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
-#define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
-#if CYTHON_METH_FASTCALL
-    #define __Pyx_Arg_FASTCALL(args, i) args[i]
-    #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
-    #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
-    static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
-    #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
-#else
-    #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
-    #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
-    #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
-    #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
-    #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
-#endif
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
-#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
-#else
-#define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
-#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
-#endif
-
 /* PyIntBinop.proto */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
 #else
 #define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
 #endif
@@ -1794,14 +1670,21 @@
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -1869,21 +1752,71 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
+/* PyFunctionFastCall.proto */
+#if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
+#define __Pyx_PyFunction_FastCall(func, args, nargs)\
+    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
+#endif
+#define __Pyx_BUILD_ASSERT_EXPR(cond)\
+    (sizeof(char [1 - 2*!(cond)]) - 1)
+#ifndef Py_MEMBER_SIZE
+#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
+#endif
+#if !CYTHON_VECTORCALL
+#if PY_VERSION_HEX >= 0x03080000
+  #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #define __Pxy_PyFrame_Initialize_Offsets()
+  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
+#else
+  static size_t __pyx_pyframe_localsplus_offset = 0;
+  #include "frameobject.h"
+  #define __Pxy_PyFrame_Initialize_Offsets()\
+    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
+     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
+  #define __Pyx_PyFrame_GetLocalsplus(frame)\
+    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif
+#endif
+#endif
+
+/* PyObjectCallMethO.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
+#endif
+
+/* PyObjectFastCall.proto */
+#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
+
+/* PyObjectCallOneArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+
 /* ObjectGetItem.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key);
 #else
 #define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
 #endif
 
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
 /* RaiseUnexpectedTypeError.proto */
 static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
 #define __PYX_HAVE_RT_ImportType_proto_3_0_0
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
@@ -1898,14 +1831,23 @@
    __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
    __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
    __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
 };
 static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
 #endif
 
+/* Import.proto */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
+
+/* ImportDottedModule.proto */
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
+#endif
+
 /* Py3UpdateBases.proto */
 static PyObject* __Pyx_PEP560_update_bases(PyObject *bases);
 
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
 
 /* PyObjectCall2Args.proto */
@@ -2192,35 +2134,40 @@
     self->data.ob_item = (char*) items;
     __Pyx_SET_SIZE(self, n);
     self->allocated = newsize;
     return 0;
 }
 #endif
 
+/* GCCDiagnostics.proto */
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
+
 /* None.proto */
 #include <new>
 
 /* EnumClassDecl.proto */
 #if defined (_MSC_VER)
   #if _MSC_VER >= 1910
     #define __PYX_ENUM_CLASS_DECL enum
   #else
     #define __PYX_ENUM_CLASS_DECL
   #endif
 #else
   #define __PYX_ENUM_CLASS_DECL enum
 #endif
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
-
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
+
+/* CIntFromPy.proto */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
 
 /* FormatTypeName.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
 typedef PyObject *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%U"
 static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
@@ -2356,67 +2303,56 @@
 
 /* Module declarations from "libc.stdint" */
 
 /* Module declarations from "lzokay_wrap" */
 
 /* Module declarations from "lzokay._lzokay" */
 static int __pyx_f_6lzokay_7_lzokay_compress_worst_size(PyObject *, int __pyx_skip_dispatch); /*proto*/
-static PyObject *__Pyx_Enum_EResult_to_py(__PYX_ENUM_CLASS_DECL lzokay::EResult); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "lzokay._lzokay"
 extern int __pyx_module_is_main_lzokay___lzokay;
 int __pyx_module_is_main_lzokay___lzokay = 0;
 
 /* Implementation of "lzokay._lzokay" */
 /* #### Code section: global_var ### */
-static PyObject *__pyx_builtin_ImportError;
-static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_MemoryError;
 /* #### Code section: string_decls ### */
-static const char __pyx_k_[] = ".";
 static const char __pyx_k_B[] = "B";
 static const char __pyx_k_b[] = "b";
 static const char __pyx_k_s[] = "s";
 static const char __pyx_k__2[] = "*";
-static const char __pyx_k__11[] = "?";
+static const char __pyx_k__10[] = "?";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_code[] = "code";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
-static const char __pyx_k_warn[] = "warn";
 static const char __pyx_k_Error[] = "Error";
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_bytes[] = "bytes";
 static const char __pyx_k_super[] = "super";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_return[] = "return";
-static const char __pyx_k_EResult[] = "EResult";
-static const char __pyx_k_Success[] = "Success";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_tobytes[] = "tobytes";
 static const char __pyx_k_compress[] = "compress";
 static const char __pyx_k_qualname[] = "__qualname__";
 static const char __pyx_k_set_name[] = "__set_name__";
-static const char __pyx_k_warnings[] = "warnings";
 static const char __pyx_k_data_size[] = "data_size";
 static const char __pyx_k_metaclass[] = "__metaclass__";
-static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_data_bytes[] = "data_bytes";
 static const char __pyx_k_decompress[] = "decompress";
 static const char __pyx_k_lzokay_pyx[] = "_lzokay.pyx";
-static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
-static const char __pyx_k_lzokay_wrap[] = "lzokay_wrap";
 static const char __pyx_k_mro_entries[] = "__mro_entries__";
 static const char __pyx_k_InputOverrun[] = "InputOverrun";
 static const char __pyx_k_initializing[] = "_initializing";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_OutputOverrun[] = "OutputOverrun";
 static const char __pyx_k_class_getitem[] = "__class_getitem__";
 static const char __pyx_k_init_subclass[] = "__init_subclass__";
@@ -2427,16 +2363,14 @@
 static const char __pyx_k_LookbehindOverrun[] = "LookbehindOverrun";
 static const char __pyx_k_curren_array_size[] = "curren_array_size";
 static const char __pyx_k_expected_out_size[] = "expected_out_size";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_compress_worst_size[] = "compress_worst_size";
 static const char __pyx_k_expected_output_size[] = "expected_output_size";
-static const char __pyx_k_is_not_a_valid_EResult[] = " is not a valid EResult";
-static const char __pyx_k_enum_class_EResult_not_importabl[] = "enum class EResult not importable from lzokay_wrap. You are probably using a cpdef enum declared in a .pxd file that does not have a .py  or .pyx file.";
 /* #### Code section: decls ### */
 static int __pyx_pf_7cpython_5array_5array___getbuffer__(arrayobject *__pyx_v_self, Py_buffer *__pyx_v_info, CYTHON_UNUSED int __pyx_v_flags); /* proto */
 static void __pyx_pf_7cpython_5array_5array_2__releasebuffer__(CYTHON_UNUSED arrayobject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
 static PyObject *__pyx_pf_6lzokay_7_lzokay_compress_worst_size(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s); /* proto */
 static PyObject *__pyx_pf_6lzokay_7_lzokay_2decompress(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data, PyObject *__pyx_v_expected_output_size); /* proto */
 static PyObject *__pyx_pf_6lzokay_7_lzokay_4compress(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data); /* proto */
 /* #### Code section: late_includes ### */
@@ -2560,27 +2494,22 @@
   PyTypeObject *__pyx_ptype_7cpython_5array_array;
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
-  PyObject *__pyx_kp_u_;
   PyObject *__pyx_n_u_B;
-  PyObject *__pyx_n_s_EResult;
   PyObject *__pyx_n_s_Error;
-  PyObject *__pyx_n_s_ImportError;
   PyObject *__pyx_n_s_InputNotConsumed;
   PyObject *__pyx_n_s_InputOverrun;
   PyObject *__pyx_n_s_LookbehindOverrun;
   PyObject *__pyx_n_s_MemoryError;
   PyObject *__pyx_n_s_OutputOverrun;
-  PyObject *__pyx_n_s_Success;
-  PyObject *__pyx_n_s_ValueError;
-  PyObject *__pyx_n_s__11;
+  PyObject *__pyx_n_s__10;
   PyObject *__pyx_n_s__2;
   PyObject *__pyx_n_s_actual_out_size;
   PyObject *__pyx_n_s_array;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_b;
   PyObject *__pyx_n_s_bytes;
   PyObject *__pyx_n_s_class_getitem;
@@ -2591,26 +2520,23 @@
   PyObject *__pyx_n_s_curren_array_size;
   PyObject *__pyx_n_s_data;
   PyObject *__pyx_n_s_data_bytes;
   PyObject *__pyx_n_s_data_size;
   PyObject *__pyx_n_s_decompress;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_n_s_doc;
-  PyObject *__pyx_kp_u_enum_class_EResult_not_importabl;
   PyObject *__pyx_n_s_expected_out_size;
   PyObject *__pyx_n_s_expected_output_size;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_init_subclass;
   PyObject *__pyx_n_s_initializing;
   PyObject *__pyx_n_s_int;
   PyObject *__pyx_n_s_is_coroutine;
-  PyObject *__pyx_kp_u_is_not_a_valid_EResult;
   PyObject *__pyx_n_s_lzokay__lzokay;
   PyObject *__pyx_kp_s_lzokay_pyx;
-  PyObject *__pyx_n_s_lzokay_wrap;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_metaclass;
   PyObject *__pyx_n_s_module;
   PyObject *__pyx_n_s_mro_entries;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_prepare;
   PyObject *__pyx_n_s_qualname;
@@ -2618,27 +2544,25 @@
   PyObject *__pyx_n_s_return;
   PyObject *__pyx_n_s_s;
   PyObject *__pyx_n_s_set_name;
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_n_s_super;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_tobytes;
-  PyObject *__pyx_n_s_warn;
-  PyObject *__pyx_n_s_warnings;
   PyObject *__pyx_int_3;
   PyObject *__pyx_int_16;
   PyObject *__pyx_int_64;
+  PyObject *__pyx_tuple_;
   PyObject *__pyx_tuple__3;
-  PyObject *__pyx_tuple__4;
-  PyObject *__pyx_tuple__6;
+  PyObject *__pyx_tuple__5;
+  PyObject *__pyx_tuple__7;
   PyObject *__pyx_tuple__8;
-  PyObject *__pyx_tuple__9;
-  PyObject *__pyx_codeobj__5;
-  PyObject *__pyx_codeobj__7;
-  PyObject *__pyx_codeobj__10;
+  PyObject *__pyx_codeobj__4;
+  PyObject *__pyx_codeobj__6;
+  PyObject *__pyx_codeobj__9;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2677,27 +2601,22 @@
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
   Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4type_type);
   Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4bool_bool);
   Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_7complex_complex);
   Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_5array_array);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_);
   Py_CLEAR(clear_module_state->__pyx_n_u_B);
-  Py_CLEAR(clear_module_state->__pyx_n_s_EResult);
   Py_CLEAR(clear_module_state->__pyx_n_s_Error);
-  Py_CLEAR(clear_module_state->__pyx_n_s_ImportError);
   Py_CLEAR(clear_module_state->__pyx_n_s_InputNotConsumed);
   Py_CLEAR(clear_module_state->__pyx_n_s_InputOverrun);
   Py_CLEAR(clear_module_state->__pyx_n_s_LookbehindOverrun);
   Py_CLEAR(clear_module_state->__pyx_n_s_MemoryError);
   Py_CLEAR(clear_module_state->__pyx_n_s_OutputOverrun);
-  Py_CLEAR(clear_module_state->__pyx_n_s_Success);
-  Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
-  Py_CLEAR(clear_module_state->__pyx_n_s__11);
+  Py_CLEAR(clear_module_state->__pyx_n_s__10);
   Py_CLEAR(clear_module_state->__pyx_n_s__2);
   Py_CLEAR(clear_module_state->__pyx_n_s_actual_out_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_array);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_b);
   Py_CLEAR(clear_module_state->__pyx_n_s_bytes);
   Py_CLEAR(clear_module_state->__pyx_n_s_class_getitem);
@@ -2708,26 +2627,23 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_curren_array_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_data_bytes);
   Py_CLEAR(clear_module_state->__pyx_n_s_data_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_decompress);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_doc);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_enum_class_EResult_not_importabl);
   Py_CLEAR(clear_module_state->__pyx_n_s_expected_out_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_expected_output_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_init_subclass);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
   Py_CLEAR(clear_module_state->__pyx_n_s_int);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_is_not_a_valid_EResult);
   Py_CLEAR(clear_module_state->__pyx_n_s_lzokay__lzokay);
   Py_CLEAR(clear_module_state->__pyx_kp_s_lzokay_pyx);
-  Py_CLEAR(clear_module_state->__pyx_n_s_lzokay_wrap);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_metaclass);
   Py_CLEAR(clear_module_state->__pyx_n_s_module);
   Py_CLEAR(clear_module_state->__pyx_n_s_mro_entries);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_prepare);
   Py_CLEAR(clear_module_state->__pyx_n_s_qualname);
@@ -2735,27 +2651,25 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_return);
   Py_CLEAR(clear_module_state->__pyx_n_s_s);
   Py_CLEAR(clear_module_state->__pyx_n_s_set_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_n_s_super);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_tobytes);
-  Py_CLEAR(clear_module_state->__pyx_n_s_warn);
-  Py_CLEAR(clear_module_state->__pyx_n_s_warnings);
   Py_CLEAR(clear_module_state->__pyx_int_3);
   Py_CLEAR(clear_module_state->__pyx_int_16);
   Py_CLEAR(clear_module_state->__pyx_int_64);
+  Py_CLEAR(clear_module_state->__pyx_tuple_);
   Py_CLEAR(clear_module_state->__pyx_tuple__3);
-  Py_CLEAR(clear_module_state->__pyx_tuple__4);
-  Py_CLEAR(clear_module_state->__pyx_tuple__6);
+  Py_CLEAR(clear_module_state->__pyx_tuple__5);
+  Py_CLEAR(clear_module_state->__pyx_tuple__7);
   Py_CLEAR(clear_module_state->__pyx_tuple__8);
-  Py_CLEAR(clear_module_state->__pyx_tuple__9);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__5);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__7);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__10);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__4);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__6);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__9);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -2772,27 +2686,22 @@
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
   Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4type_type);
   Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4bool_bool);
   Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_7complex_complex);
   Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_5array_array);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_);
   Py_VISIT(traverse_module_state->__pyx_n_u_B);
-  Py_VISIT(traverse_module_state->__pyx_n_s_EResult);
   Py_VISIT(traverse_module_state->__pyx_n_s_Error);
-  Py_VISIT(traverse_module_state->__pyx_n_s_ImportError);
   Py_VISIT(traverse_module_state->__pyx_n_s_InputNotConsumed);
   Py_VISIT(traverse_module_state->__pyx_n_s_InputOverrun);
   Py_VISIT(traverse_module_state->__pyx_n_s_LookbehindOverrun);
   Py_VISIT(traverse_module_state->__pyx_n_s_MemoryError);
   Py_VISIT(traverse_module_state->__pyx_n_s_OutputOverrun);
-  Py_VISIT(traverse_module_state->__pyx_n_s_Success);
-  Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
-  Py_VISIT(traverse_module_state->__pyx_n_s__11);
+  Py_VISIT(traverse_module_state->__pyx_n_s__10);
   Py_VISIT(traverse_module_state->__pyx_n_s__2);
   Py_VISIT(traverse_module_state->__pyx_n_s_actual_out_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_array);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_b);
   Py_VISIT(traverse_module_state->__pyx_n_s_bytes);
   Py_VISIT(traverse_module_state->__pyx_n_s_class_getitem);
@@ -2803,26 +2712,23 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_curren_array_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_data_bytes);
   Py_VISIT(traverse_module_state->__pyx_n_s_data_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_decompress);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_doc);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_enum_class_EResult_not_importabl);
   Py_VISIT(traverse_module_state->__pyx_n_s_expected_out_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_expected_output_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_init_subclass);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
   Py_VISIT(traverse_module_state->__pyx_n_s_int);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_is_not_a_valid_EResult);
   Py_VISIT(traverse_module_state->__pyx_n_s_lzokay__lzokay);
   Py_VISIT(traverse_module_state->__pyx_kp_s_lzokay_pyx);
-  Py_VISIT(traverse_module_state->__pyx_n_s_lzokay_wrap);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_metaclass);
   Py_VISIT(traverse_module_state->__pyx_n_s_module);
   Py_VISIT(traverse_module_state->__pyx_n_s_mro_entries);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_prepare);
   Py_VISIT(traverse_module_state->__pyx_n_s_qualname);
@@ -2830,27 +2736,25 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_return);
   Py_VISIT(traverse_module_state->__pyx_n_s_s);
   Py_VISIT(traverse_module_state->__pyx_n_s_set_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_n_s_super);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_tobytes);
-  Py_VISIT(traverse_module_state->__pyx_n_s_warn);
-  Py_VISIT(traverse_module_state->__pyx_n_s_warnings);
   Py_VISIT(traverse_module_state->__pyx_int_3);
   Py_VISIT(traverse_module_state->__pyx_int_16);
   Py_VISIT(traverse_module_state->__pyx_int_64);
+  Py_VISIT(traverse_module_state->__pyx_tuple_);
   Py_VISIT(traverse_module_state->__pyx_tuple__3);
-  Py_VISIT(traverse_module_state->__pyx_tuple__4);
-  Py_VISIT(traverse_module_state->__pyx_tuple__6);
+  Py_VISIT(traverse_module_state->__pyx_tuple__5);
+  Py_VISIT(traverse_module_state->__pyx_tuple__7);
   Py_VISIT(traverse_module_state->__pyx_tuple__8);
-  Py_VISIT(traverse_module_state->__pyx_tuple__9);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__5);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__7);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__10);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__4);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__6);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__9);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -2969,27 +2873,22 @@
 #define __pyx_ptype_7cpython_5array_array __pyx_mstate_global->__pyx_ptype_7cpython_5array_array
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
-#define __pyx_kp_u_ __pyx_mstate_global->__pyx_kp_u_
 #define __pyx_n_u_B __pyx_mstate_global->__pyx_n_u_B
-#define __pyx_n_s_EResult __pyx_mstate_global->__pyx_n_s_EResult
 #define __pyx_n_s_Error __pyx_mstate_global->__pyx_n_s_Error
-#define __pyx_n_s_ImportError __pyx_mstate_global->__pyx_n_s_ImportError
 #define __pyx_n_s_InputNotConsumed __pyx_mstate_global->__pyx_n_s_InputNotConsumed
 #define __pyx_n_s_InputOverrun __pyx_mstate_global->__pyx_n_s_InputOverrun
 #define __pyx_n_s_LookbehindOverrun __pyx_mstate_global->__pyx_n_s_LookbehindOverrun
 #define __pyx_n_s_MemoryError __pyx_mstate_global->__pyx_n_s_MemoryError
 #define __pyx_n_s_OutputOverrun __pyx_mstate_global->__pyx_n_s_OutputOverrun
-#define __pyx_n_s_Success __pyx_mstate_global->__pyx_n_s_Success
-#define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
-#define __pyx_n_s__11 __pyx_mstate_global->__pyx_n_s__11
+#define __pyx_n_s__10 __pyx_mstate_global->__pyx_n_s__10
 #define __pyx_n_s__2 __pyx_mstate_global->__pyx_n_s__2
 #define __pyx_n_s_actual_out_size __pyx_mstate_global->__pyx_n_s_actual_out_size
 #define __pyx_n_s_array __pyx_mstate_global->__pyx_n_s_array
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_b __pyx_mstate_global->__pyx_n_s_b
 #define __pyx_n_s_bytes __pyx_mstate_global->__pyx_n_s_bytes
 #define __pyx_n_s_class_getitem __pyx_mstate_global->__pyx_n_s_class_getitem
@@ -3000,26 +2899,23 @@
 #define __pyx_n_s_curren_array_size __pyx_mstate_global->__pyx_n_s_curren_array_size
 #define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
 #define __pyx_n_s_data_bytes __pyx_mstate_global->__pyx_n_s_data_bytes
 #define __pyx_n_s_data_size __pyx_mstate_global->__pyx_n_s_data_size
 #define __pyx_n_s_decompress __pyx_mstate_global->__pyx_n_s_decompress
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_n_s_doc __pyx_mstate_global->__pyx_n_s_doc
-#define __pyx_kp_u_enum_class_EResult_not_importabl __pyx_mstate_global->__pyx_kp_u_enum_class_EResult_not_importabl
 #define __pyx_n_s_expected_out_size __pyx_mstate_global->__pyx_n_s_expected_out_size
 #define __pyx_n_s_expected_output_size __pyx_mstate_global->__pyx_n_s_expected_output_size
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_init_subclass __pyx_mstate_global->__pyx_n_s_init_subclass
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
 #define __pyx_n_s_int __pyx_mstate_global->__pyx_n_s_int
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
-#define __pyx_kp_u_is_not_a_valid_EResult __pyx_mstate_global->__pyx_kp_u_is_not_a_valid_EResult
 #define __pyx_n_s_lzokay__lzokay __pyx_mstate_global->__pyx_n_s_lzokay__lzokay
 #define __pyx_kp_s_lzokay_pyx __pyx_mstate_global->__pyx_kp_s_lzokay_pyx
-#define __pyx_n_s_lzokay_wrap __pyx_mstate_global->__pyx_n_s_lzokay_wrap
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_metaclass __pyx_mstate_global->__pyx_n_s_metaclass
 #define __pyx_n_s_module __pyx_mstate_global->__pyx_n_s_module
 #define __pyx_n_s_mro_entries __pyx_mstate_global->__pyx_n_s_mro_entries
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_prepare __pyx_mstate_global->__pyx_n_s_prepare
 #define __pyx_n_s_qualname __pyx_mstate_global->__pyx_n_s_qualname
@@ -3027,465 +2923,27 @@
 #define __pyx_n_s_return __pyx_mstate_global->__pyx_n_s_return
 #define __pyx_n_s_s __pyx_mstate_global->__pyx_n_s_s
 #define __pyx_n_s_set_name __pyx_mstate_global->__pyx_n_s_set_name
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_n_s_super __pyx_mstate_global->__pyx_n_s_super
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_tobytes __pyx_mstate_global->__pyx_n_s_tobytes
-#define __pyx_n_s_warn __pyx_mstate_global->__pyx_n_s_warn
-#define __pyx_n_s_warnings __pyx_mstate_global->__pyx_n_s_warnings
 #define __pyx_int_3 __pyx_mstate_global->__pyx_int_3
 #define __pyx_int_16 __pyx_mstate_global->__pyx_int_16
 #define __pyx_int_64 __pyx_mstate_global->__pyx_int_64
+#define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
-#define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
-#define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
+#define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
+#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
-#define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
-#define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
-#define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
-#define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
+#define __pyx_codeobj__4 __pyx_mstate_global->__pyx_codeobj__4
+#define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
+#define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
 /* #### Code section: module_code ### */
 
-/* "EnumTypeToPy":132
- * 
- * @cname("__Pyx_Enum_EResult_to_py")
- * cdef __Pyx_Enum_EResult_to_py(EResult c_val):             # <<<<<<<<<<<<<<
- *     cdef object __pyx_enum
- * 
- */
-
-static PyObject *__Pyx_Enum_EResult_to_py(__PYX_ENUM_CLASS_DECL lzokay::EResult __pyx_v_c_val) {
-  PyObject *__pyx_v___pyx_enum = 0;
-  PyObject *__pyx_v_warnings = NULL;
-  int __pyx_v_underlying_c_val;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
-  PyObject *__pyx_t_10 = NULL;
-  int __pyx_t_11;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__Pyx_Enum_EResult_to_py", 0);
-
-  /* "EnumTypeToPy":137
- * 
- * 
- *     try:             # <<<<<<<<<<<<<<
- *         from lzokay_wrap import EResult as __pyx_enum
- *     except ImportError:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "EnumTypeToPy":138
- * 
- *     try:
- *         from lzokay_wrap import EResult as __pyx_enum             # <<<<<<<<<<<<<<
- *     except ImportError:
- *         import warnings
- */
-      __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 138, __pyx_L3_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_INCREF(__pyx_n_s_EResult);
-      __Pyx_GIVEREF(__pyx_n_s_EResult);
-      PyList_SET_ITEM(__pyx_t_4, 0, __pyx_n_s_EResult);
-      __pyx_t_5 = __Pyx_Import(__pyx_n_s_lzokay_wrap, __pyx_t_4, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 138, __pyx_L3_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_ImportFrom(__pyx_t_5, __pyx_n_s_EResult); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 138, __pyx_L3_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_4);
-      __pyx_v___pyx_enum = __pyx_t_4;
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-
-      /* "EnumTypeToPy":137
- * 
- * 
- *     try:             # <<<<<<<<<<<<<<
- *         from lzokay_wrap import EResult as __pyx_enum
- *     except ImportError:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-
-    /* "EnumTypeToPy":139
- *     try:
- *         from lzokay_wrap import EResult as __pyx_enum
- *     except ImportError:             # <<<<<<<<<<<<<<
- *         import warnings
- *         warnings.warn(
- */
-    __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ImportError);
-    if (__pyx_t_6) {
-      __Pyx_AddTraceback("EnumTypeToPy.__Pyx_Enum_EResult_to_py", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(0, 139, __pyx_L5_except_error)
-      __Pyx_XGOTREF(__pyx_t_5);
-      __Pyx_XGOTREF(__pyx_t_4);
-      __Pyx_XGOTREF(__pyx_t_7);
-
-      /* "EnumTypeToPy":140
- *         from lzokay_wrap import EResult as __pyx_enum
- *     except ImportError:
- *         import warnings             # <<<<<<<<<<<<<<
- *         warnings.warn(
- *             f"enum class EResult not importable from lzokay_wrap. "
- */
-      __pyx_t_8 = __Pyx_ImportDottedModule(__pyx_n_s_warnings, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 140, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __pyx_v_warnings = __pyx_t_8;
-      __pyx_t_8 = 0;
-
-      /* "EnumTypeToPy":141
- *     except ImportError:
- *         import warnings
- *         warnings.warn(             # <<<<<<<<<<<<<<
- *             f"enum class EResult not importable from lzokay_wrap. "
- *             "You are probably using a cpdef enum declared in a .pxd file that "
- */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_warnings, __pyx_n_s_warn); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 141, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_10 = NULL;
-      __pyx_t_6 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
-        __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
-        if (likely(__pyx_t_10)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-          __Pyx_INCREF(__pyx_t_10);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_9, function);
-          __pyx_t_6 = 1;
-        }
-      }
-      {
-        PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_kp_u_enum_class_EResult_not_importabl};
-        __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
-        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 141, __pyx_L5_except_error)
-        __Pyx_GOTREF(__pyx_t_8);
-        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-
-      /* "EnumTypeToPy":145
- *             "You are probably using a cpdef enum declared in a .pxd file that "
- *             "does not have a .py  or .pyx file.")
- *         return <int>c_val             # <<<<<<<<<<<<<<
- * 
- *     if 0:
- */
-      __Pyx_XDECREF(__pyx_r);
-      __pyx_t_8 = __Pyx_PyInt_From_int(((int)__pyx_v_c_val)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 145, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __pyx_r = __pyx_t_8;
-      __pyx_t_8 = 0;
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      goto __pyx_L6_except_return;
-    }
-    goto __pyx_L5_except_error;
-
-    /* "EnumTypeToPy":137
- * 
- * 
- *     try:             # <<<<<<<<<<<<<<
- *         from lzokay_wrap import EResult as __pyx_enum
- *     except ImportError:
- */
-    __pyx_L5_except_error:;
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L6_except_return:;
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L0;
-    __pyx_L8_try_end:;
-  }
-
-  /* "EnumTypeToPy":149
- *     if 0:
- *         pass
- *     elif c_val == EResult.LookbehindOverrun:             # <<<<<<<<<<<<<<
- *         return __pyx_enum.LookbehindOverrun
- *     elif c_val == EResult.OutputOverrun:
- */
-  __pyx_t_11 = (__pyx_v_c_val == lzokay::EResult::LookbehindOverrun);
-  if (__pyx_t_11) {
-
-    /* "EnumTypeToPy":150
- *         pass
- *     elif c_val == EResult.LookbehindOverrun:
- *         return __pyx_enum.LookbehindOverrun             # <<<<<<<<<<<<<<
- *     elif c_val == EResult.OutputOverrun:
- *         return __pyx_enum.OutputOverrun
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_LookbehindOverrun); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 150, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_r = __pyx_t_7;
-    __pyx_t_7 = 0;
-    goto __pyx_L0;
-
-    /* "EnumTypeToPy":149
- *     if 0:
- *         pass
- *     elif c_val == EResult.LookbehindOverrun:             # <<<<<<<<<<<<<<
- *         return __pyx_enum.LookbehindOverrun
- *     elif c_val == EResult.OutputOverrun:
- */
-  }
-
-  /* "EnumTypeToPy":151
- *     elif c_val == EResult.LookbehindOverrun:
- *         return __pyx_enum.LookbehindOverrun
- *     elif c_val == EResult.OutputOverrun:             # <<<<<<<<<<<<<<
- *         return __pyx_enum.OutputOverrun
- *     elif c_val == EResult.InputOverrun:
- */
-  __pyx_t_11 = (__pyx_v_c_val == lzokay::EResult::OutputOverrun);
-  if (__pyx_t_11) {
-
-    /* "EnumTypeToPy":152
- *         return __pyx_enum.LookbehindOverrun
- *     elif c_val == EResult.OutputOverrun:
- *         return __pyx_enum.OutputOverrun             # <<<<<<<<<<<<<<
- *     elif c_val == EResult.InputOverrun:
- *         return __pyx_enum.InputOverrun
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_OutputOverrun); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_r = __pyx_t_7;
-    __pyx_t_7 = 0;
-    goto __pyx_L0;
-
-    /* "EnumTypeToPy":151
- *     elif c_val == EResult.LookbehindOverrun:
- *         return __pyx_enum.LookbehindOverrun
- *     elif c_val == EResult.OutputOverrun:             # <<<<<<<<<<<<<<
- *         return __pyx_enum.OutputOverrun
- *     elif c_val == EResult.InputOverrun:
- */
-  }
-
-  /* "EnumTypeToPy":153
- *     elif c_val == EResult.OutputOverrun:
- *         return __pyx_enum.OutputOverrun
- *     elif c_val == EResult.InputOverrun:             # <<<<<<<<<<<<<<
- *         return __pyx_enum.InputOverrun
- *     elif c_val == EResult.Error:
- */
-  __pyx_t_11 = (__pyx_v_c_val == lzokay::EResult::InputOverrun);
-  if (__pyx_t_11) {
-
-    /* "EnumTypeToPy":154
- *         return __pyx_enum.OutputOverrun
- *     elif c_val == EResult.InputOverrun:
- *         return __pyx_enum.InputOverrun             # <<<<<<<<<<<<<<
- *     elif c_val == EResult.Error:
- *         return __pyx_enum.Error
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_InputOverrun); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 154, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_r = __pyx_t_7;
-    __pyx_t_7 = 0;
-    goto __pyx_L0;
-
-    /* "EnumTypeToPy":153
- *     elif c_val == EResult.OutputOverrun:
- *         return __pyx_enum.OutputOverrun
- *     elif c_val == EResult.InputOverrun:             # <<<<<<<<<<<<<<
- *         return __pyx_enum.InputOverrun
- *     elif c_val == EResult.Error:
- */
-  }
-
-  /* "EnumTypeToPy":155
- *     elif c_val == EResult.InputOverrun:
- *         return __pyx_enum.InputOverrun
- *     elif c_val == EResult.Error:             # <<<<<<<<<<<<<<
- *         return __pyx_enum.Error
- *     elif c_val == EResult.Success:
- */
-  __pyx_t_11 = (__pyx_v_c_val == lzokay::EResult::Error);
-  if (__pyx_t_11) {
-
-    /* "EnumTypeToPy":156
- *         return __pyx_enum.InputOverrun
- *     elif c_val == EResult.Error:
- *         return __pyx_enum.Error             # <<<<<<<<<<<<<<
- *     elif c_val == EResult.Success:
- *         return __pyx_enum.Success
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_Error); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 156, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_r = __pyx_t_7;
-    __pyx_t_7 = 0;
-    goto __pyx_L0;
-
-    /* "EnumTypeToPy":155
- *     elif c_val == EResult.InputOverrun:
- *         return __pyx_enum.InputOverrun
- *     elif c_val == EResult.Error:             # <<<<<<<<<<<<<<
- *         return __pyx_enum.Error
- *     elif c_val == EResult.Success:
- */
-  }
-
-  /* "EnumTypeToPy":157
- *     elif c_val == EResult.Error:
- *         return __pyx_enum.Error
- *     elif c_val == EResult.Success:             # <<<<<<<<<<<<<<
- *         return __pyx_enum.Success
- *     elif c_val == EResult.InputNotConsumed:
- */
-  __pyx_t_11 = (__pyx_v_c_val == lzokay::EResult::Success);
-  if (__pyx_t_11) {
-
-    /* "EnumTypeToPy":158
- *         return __pyx_enum.Error
- *     elif c_val == EResult.Success:
- *         return __pyx_enum.Success             # <<<<<<<<<<<<<<
- *     elif c_val == EResult.InputNotConsumed:
- *         return __pyx_enum.InputNotConsumed
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_Success); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 158, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_r = __pyx_t_7;
-    __pyx_t_7 = 0;
-    goto __pyx_L0;
-
-    /* "EnumTypeToPy":157
- *     elif c_val == EResult.Error:
- *         return __pyx_enum.Error
- *     elif c_val == EResult.Success:             # <<<<<<<<<<<<<<
- *         return __pyx_enum.Success
- *     elif c_val == EResult.InputNotConsumed:
- */
-  }
-
-  /* "EnumTypeToPy":159
- *     elif c_val == EResult.Success:
- *         return __pyx_enum.Success
- *     elif c_val == EResult.InputNotConsumed:             # <<<<<<<<<<<<<<
- *         return __pyx_enum.InputNotConsumed
- *     else:
- */
-  __pyx_t_11 = (__pyx_v_c_val == lzokay::EResult::InputNotConsumed);
-  if (likely(__pyx_t_11)) {
-
-    /* "EnumTypeToPy":160
- *         return __pyx_enum.Success
- *     elif c_val == EResult.InputNotConsumed:
- *         return __pyx_enum.InputNotConsumed             # <<<<<<<<<<<<<<
- *     else:
- *         underlying_c_val = <int>c_val
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v___pyx_enum, __pyx_n_s_InputNotConsumed); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_r = __pyx_t_7;
-    __pyx_t_7 = 0;
-    goto __pyx_L0;
-
-    /* "EnumTypeToPy":159
- *     elif c_val == EResult.Success:
- *         return __pyx_enum.Success
- *     elif c_val == EResult.InputNotConsumed:             # <<<<<<<<<<<<<<
- *         return __pyx_enum.InputNotConsumed
- *     else:
- */
-  }
-
-  /* "EnumTypeToPy":162
- *         return __pyx_enum.InputNotConsumed
- *     else:
- *         underlying_c_val = <int>c_val             # <<<<<<<<<<<<<<
- *         raise ValueError(f"{underlying_c_val} is not a valid EResult")
- * 
- */
-  /*else*/ {
-    __pyx_v_underlying_c_val = ((int)__pyx_v_c_val);
-
-    /* "EnumTypeToPy":163
- *     else:
- *         underlying_c_val = <int>c_val
- *         raise ValueError(f"{underlying_c_val} is not a valid EResult")             # <<<<<<<<<<<<<<
- * 
- */
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_underlying_c_val, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 163, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_7, __pyx_kp_u_is_not_a_valid_EResult); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 163, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_Raise(__pyx_t_7, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __PYX_ERR(0, 163, __pyx_L1_error)
-  }
-
-  /* "EnumTypeToPy":132
- * 
- * @cname("__Pyx_Enum_EResult_to_py")
- * cdef __Pyx_Enum_EResult_to_py(EResult c_val):             # <<<<<<<<<<<<<<
- *     cdef object __pyx_enum
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_AddTraceback("EnumTypeToPy.__Pyx_Enum_EResult_to_py", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v___pyx_enum);
-  __Pyx_XDECREF(__pyx_v_warnings);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 /* "cpython/complex.pxd":19
  * 
  *         @property
  *         cdef inline double real(self):             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
@@ -3595,15 +3053,15 @@
   /* "cpython/contextvars.pxd":118
  *     """
  *     cdef PyObject *value = NULL
  *     PyContextVar_Get(var, NULL, &value)             # <<<<<<<<<<<<<<
  *     if value is NULL:
  *         # context variable does not have a default
  */
-  __pyx_t_1 = PyContextVar_Get(__pyx_v_var, NULL, (&__pyx_v_value)); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 118, __pyx_L1_error)
+  __pyx_t_1 = PyContextVar_Get(__pyx_v_var, NULL, (&__pyx_v_value)); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 118, __pyx_L1_error)
 
   /* "cpython/contextvars.pxd":119
  *     cdef PyObject *value = NULL
  *     PyContextVar_Get(var, NULL, &value)
  *     if value is NULL:             # <<<<<<<<<<<<<<
  *         # context variable does not have a default
  *         pyvalue = default_value
@@ -3725,15 +3183,15 @@
   /* "cpython/contextvars.pxd":136
  *     """
  *     cdef PyObject *value = NULL
  *     PyContextVar_Get(var, <PyObject*>default_value, &value)             # <<<<<<<<<<<<<<
  *     # value of context variable or 'default_value'
  *     pyvalue = <object>value
  */
-  __pyx_t_1 = PyContextVar_Get(__pyx_v_var, ((PyObject *)__pyx_v_default_value), (&__pyx_v_value)); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 136, __pyx_L1_error)
+  __pyx_t_1 = PyContextVar_Get(__pyx_v_var, ((PyObject *)__pyx_v_default_value), (&__pyx_v_value)); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 136, __pyx_L1_error)
 
   /* "cpython/contextvars.pxd":138
  *     PyContextVar_Get(var, <PyObject*>default_value, &value)
  *     # value of context variable or 'default_value'
  *     pyvalue = <object>value             # <<<<<<<<<<<<<<
  *     Py_XDECREF(value)  # PyContextVar_Get() returned an owned reference as 'PyObject*'
  *     return pyvalue
@@ -3828,15 +3286,15 @@
   /* "array.pxd":109
  *             # In particular strided access is always provided regardless
  *             # of flags
  *             item_count = Py_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *             info.suboffsets = NULL
  */
-  __pyx_t_1 = PyInt_FromSsize_t(Py_SIZE(((PyObject *)__pyx_v_self))); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 109, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(Py_SIZE(((PyObject *)__pyx_v_self))); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_item_count = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "array.pxd":111
  *             item_count = Py_SIZE(self)
  * 
@@ -3887,20 +3345,20 @@
   /* "array.pxd":116
  *             info.ndim = 1
  *             info.itemsize = self.ob_descr.itemsize   # e.g. sizeof(float)
  *             info.len = info.itemsize * item_count             # <<<<<<<<<<<<<<
  * 
  *             info.shape = <Py_ssize_t*> PyObject_Malloc(sizeof(Py_ssize_t) + 2)
  */
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_info->itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 116, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_info->itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyNumber_Multiply(__pyx_t_1, __pyx_v_item_count); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 116, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Multiply(__pyx_t_1, __pyx_v_item_count); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_4); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 116, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_4); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 116, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_info->len = __pyx_t_5;
 
   /* "array.pxd":118
  *             info.len = info.itemsize * item_count
  * 
  *             info.shape = <Py_ssize_t*> PyObject_Malloc(sizeof(Py_ssize_t) + 2)             # <<<<<<<<<<<<<<
@@ -3922,15 +3380,15 @@
     /* "array.pxd":120
  *             info.shape = <Py_ssize_t*> PyObject_Malloc(sizeof(Py_ssize_t) + 2)
  *             if not info.shape:
  *                 raise MemoryError()             # <<<<<<<<<<<<<<
  *             info.shape[0] = item_count      # constant regardless of resizing
  *             info.strides = &info.itemsize
  */
-    PyErr_NoMemory(); __PYX_ERR(2, 120, __pyx_L1_error)
+    PyErr_NoMemory(); __PYX_ERR(1, 120, __pyx_L1_error)
 
     /* "array.pxd":119
  * 
  *             info.shape = <Py_ssize_t*> PyObject_Malloc(sizeof(Py_ssize_t) + 2)
  *             if not info.shape:             # <<<<<<<<<<<<<<
  *                 raise MemoryError()
  *             info.shape[0] = item_count      # constant regardless of resizing
@@ -3940,15 +3398,15 @@
   /* "array.pxd":121
  *             if not info.shape:
  *                 raise MemoryError()
  *             info.shape[0] = item_count      # constant regardless of resizing             # <<<<<<<<<<<<<<
  *             info.strides = &info.itemsize
  * 
  */
-  __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_v_item_count); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 121, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_v_item_count); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 121, __pyx_L1_error)
   (__pyx_v_info->shape[0]) = __pyx_t_5;
 
   /* "array.pxd":122
  *                 raise MemoryError()
  *             info.shape[0] = item_count      # constant regardless of resizing
  *             info.strides = &info.itemsize             # <<<<<<<<<<<<<<
  * 
@@ -4097,15 +3555,15 @@
   /* "array.pxd":145
  *     type will be same as template.
  *     if zero is true, new array will be initialized with zeroes."""
  *     cdef array op = newarrayobject(Py_TYPE(template), length, template.ob_descr)             # <<<<<<<<<<<<<<
  *     if zero and op is not None:
  *         memset(op.data.as_chars, 0, length * op.ob_descr.itemsize)
  */
-  __pyx_t_1 = ((PyObject *)newarrayobject(Py_TYPE(((PyObject *)__pyx_v_template)), __pyx_v_length, __pyx_v_template->ob_descr)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 145, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)newarrayobject(Py_TYPE(((PyObject *)__pyx_v_template)), __pyx_v_length, __pyx_v_template->ob_descr)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_op = ((arrayobject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "array.pxd":146
  *     if zero is true, new array will be initialized with zeroes."""
  *     cdef array op = newarrayobject(Py_TYPE(template), length, template.ob_descr)
@@ -4194,15 +3652,15 @@
   /* "array.pxd":152
  * cdef inline array copy(array self):
  *     """ make a copy of an array. """
  *     cdef array op = newarrayobject(Py_TYPE(self), Py_SIZE(self), self.ob_descr)             # <<<<<<<<<<<<<<
  *     memcpy(op.data.as_chars, self.data.as_chars, Py_SIZE(op) * op.ob_descr.itemsize)
  *     return op
  */
-  __pyx_t_1 = ((PyObject *)newarrayobject(Py_TYPE(((PyObject *)__pyx_v_self)), Py_SIZE(((PyObject *)__pyx_v_self)), __pyx_v_self->ob_descr)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 152, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)newarrayobject(Py_TYPE(((PyObject *)__pyx_v_self)), Py_SIZE(((PyObject *)__pyx_v_self)), __pyx_v_self->ob_descr)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_op = ((arrayobject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "array.pxd":153
  *     """ make a copy of an array. """
  *     cdef array op = newarrayobject(Py_TYPE(self), Py_SIZE(self), self.ob_descr)
@@ -4285,15 +3743,15 @@
   /* "array.pxd":162
  *     cdef Py_ssize_t itemsize = self.ob_descr.itemsize
  *     cdef Py_ssize_t origsize = Py_SIZE(self)
  *     resize_smart(self, origsize + n)             # <<<<<<<<<<<<<<
  *     memcpy(self.data.as_chars + origsize * itemsize, stuff, n * itemsize)
  *     return 0
  */
-  __pyx_t_1 = resize_smart(__pyx_v_self, (__pyx_v_origsize + __pyx_v_n)); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 162, __pyx_L1_error)
+  __pyx_t_1 = resize_smart(__pyx_v_self, (__pyx_v_origsize + __pyx_v_n)); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 162, __pyx_L1_error)
 
   /* "array.pxd":163
  *     cdef Py_ssize_t origsize = Py_SIZE(self)
  *     resize_smart(self, origsize + n)
  *     memcpy(self.data.as_chars + origsize * itemsize, stuff, n * itemsize)             # <<<<<<<<<<<<<<
  *     return 0
  * 
@@ -4358,15 +3816,15 @@
     /* "array.pxd":169
  *     """ extend array with data from another array; types must match. """
  *     if self.ob_descr.typecode != other.ob_descr.typecode:
  *         PyErr_BadArgument()             # <<<<<<<<<<<<<<
  *     return extend_buffer(self, other.data.as_chars, Py_SIZE(other))
  * 
  */
-    __pyx_t_2 = PyErr_BadArgument(); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(2, 169, __pyx_L1_error)
+    __pyx_t_2 = PyErr_BadArgument(); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 169, __pyx_L1_error)
 
     /* "array.pxd":168
  * cdef inline int extend(array self, array other) except -1:
  *     """ extend array with data from another array; types must match. """
  *     if self.ob_descr.typecode != other.ob_descr.typecode:             # <<<<<<<<<<<<<<
  *         PyErr_BadArgument()
  *     return extend_buffer(self, other.data.as_chars, Py_SIZE(other))
@@ -4376,15 +3834,15 @@
   /* "array.pxd":170
  *     if self.ob_descr.typecode != other.ob_descr.typecode:
  *         PyErr_BadArgument()
  *     return extend_buffer(self, other.data.as_chars, Py_SIZE(other))             # <<<<<<<<<<<<<<
  * 
  * cdef inline void zero(array self):
  */
-  __pyx_t_2 = __pyx_f_7cpython_5array_extend_buffer(__pyx_v_self, __pyx_v_other->data.as_chars, Py_SIZE(((PyObject *)__pyx_v_other))); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(2, 170, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_7cpython_5array_extend_buffer(__pyx_v_self, __pyx_v_other->data.as_chars, Py_SIZE(((PyObject *)__pyx_v_other))); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 170, __pyx_L1_error)
   __pyx_r = __pyx_t_2;
   goto __pyx_L0;
 
   /* "array.pxd":166
  *     return 0
  * 
  * cdef inline int extend(array self, array other) except -1:             # <<<<<<<<<<<<<<
@@ -4461,26 +3919,26 @@
   /* "lzokay/_lzokay.pyx":42
  * 
  * cpdef int compress_worst_size(s: int):
  *     return s + s // 16 + 64 + 3             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = PyNumber_FloorDivide(__pyx_v_s, __pyx_int_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 42, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_FloorDivide(__pyx_v_s, __pyx_int_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Add(__pyx_v_s, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 42, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_v_s, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_64, 64, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 42, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_64, 64, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_3, 3, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 42, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_3, 3, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(3, 42, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   goto __pyx_L0;
 
   /* "lzokay/_lzokay.pyx":41
  * 
  * 
@@ -4539,37 +3997,37 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_s)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(3, 41, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 41, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compress_worst_size") < 0)) __PYX_ERR(3, 41, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compress_worst_size") < 0)) __PYX_ERR(2, 41, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_s = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("compress_worst_size", 1, 1, 1, __pyx_nargs); __PYX_ERR(3, 41, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("compress_worst_size", 1, 1, 1, __pyx_nargs); __PYX_ERR(2, 41, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lzokay._lzokay.compress_worst_size", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_s), (&PyInt_Type), 0, "s", 1))) __PYX_ERR(3, 41, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_s), (&PyInt_Type), 0, "s", 1))) __PYX_ERR(2, 41, __pyx_L1_error)
   __pyx_r = __pyx_pf_6lzokay_7_lzokay_compress_worst_size(__pyx_self, __pyx_v_s);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4583,16 +4041,16 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compress_worst_size", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_6lzokay_7_lzokay_compress_worst_size(__pyx_v_s, 0); if (unlikely(__pyx_t_1 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(3, 41, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 41, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_6lzokay_7_lzokay_compress_worst_size(__pyx_v_s, 0); if (unlikely(__pyx_t_1 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(2, 41, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4656,27 +4114,27 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(3, 45, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 45, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_expected_output_size);
           if (value) { values[1] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(3, 45, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 45, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decompress") < 0)) __PYX_ERR(3, 45, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decompress") < 0)) __PYX_ERR(2, 45, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
@@ -4684,22 +4142,22 @@
       }
     }
     __pyx_v_data = ((PyObject*)values[0]);
     __pyx_v_expected_output_size = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("decompress", 0, 1, 2, __pyx_nargs); __PYX_ERR(3, 45, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("decompress", 0, 1, 2, __pyx_nargs); __PYX_ERR(2, 45, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lzokay._lzokay.decompress", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 0, "data", 1))) __PYX_ERR(3, 45, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_expected_output_size), (&PyInt_Type), 1, "expected_output_size", 1))) __PYX_ERR(3, 45, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 0, "data", 1))) __PYX_ERR(2, 45, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_expected_output_size), (&PyInt_Type), 1, "expected_output_size", 1))) __PYX_ERR(2, 45, __pyx_L1_error)
   __pyx_r = __pyx_pf_6lzokay_7_lzokay_2decompress(__pyx_self, __pyx_v_data, __pyx_v_expected_output_size);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4733,15 +4191,15 @@
   /* "lzokay/_lzokay.pyx":46
  * 
  * def decompress(data: bytes, expected_output_size: int = None) -> bytes:
  *     data_size = len(data)             # <<<<<<<<<<<<<<
  * 
  *     cdef size_t curren_array_size = data_size
  */
-  __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(3, 46, __pyx_L1_error)
+  __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(2, 46, __pyx_L1_error)
   __pyx_v_data_size = __pyx_t_1;
 
   /* "lzokay/_lzokay.pyx":48
  *     data_size = len(data)
  * 
  *     cdef size_t curren_array_size = data_size             # <<<<<<<<<<<<<<
  *     if expected_output_size is not None:
@@ -4762,15 +4220,15 @@
     /* "lzokay/_lzokay.pyx":50
  *     cdef size_t curren_array_size = data_size
  *     if expected_output_size is not None:
  *         curren_array_size = expected_output_size             # <<<<<<<<<<<<<<
  * 
  *     cdef size_t actual_out_size = 0
  */
-    __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_v_expected_output_size); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(3, 50, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_v_expected_output_size); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 50, __pyx_L1_error)
     __pyx_v_curren_array_size = __pyx_t_3;
 
     /* "lzokay/_lzokay.pyx":49
  * 
  *     cdef size_t curren_array_size = data_size
  *     if expected_output_size is not None:             # <<<<<<<<<<<<<<
  *         curren_array_size = expected_output_size
@@ -4790,27 +4248,27 @@
   /* "lzokay/_lzokay.pyx":53
  * 
  *     cdef size_t actual_out_size = 0
  *     cdef array.array b = array.array('B')             # <<<<<<<<<<<<<<
  *     array.resize(b, curren_array_size)
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 53, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_tuple_, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_v_b = ((arrayobject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "lzokay/_lzokay.pyx":54
  *     cdef size_t actual_out_size = 0
  *     cdef array.array b = array.array('B')
  *     array.resize(b, curren_array_size)             # <<<<<<<<<<<<<<
  * 
  *     cdef c_EResult code = c_EResult.OutputOverrun
  */
-  __pyx_t_5 = resize(__pyx_v_b, __pyx_v_curren_array_size); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(3, 54, __pyx_L1_error)
+  __pyx_t_5 = resize(__pyx_v_b, __pyx_v_curren_array_size); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(2, 54, __pyx_L1_error)
 
   /* "lzokay/_lzokay.pyx":56
  *     array.resize(b, curren_array_size)
  * 
  *     cdef c_EResult code = c_EResult.OutputOverrun             # <<<<<<<<<<<<<<
  *     cdef const uint8_t* data_bytes = data
  *     while code == c_EResult.OutputOverrun:
@@ -4820,15 +4278,15 @@
   /* "lzokay/_lzokay.pyx":57
  * 
  *     cdef c_EResult code = c_EResult.OutputOverrun
  *     cdef const uint8_t* data_bytes = data             # <<<<<<<<<<<<<<
  *     while code == c_EResult.OutputOverrun:
  *         with nogil:
  */
-  __pyx_t_6 = __Pyx_PyBytes_AsUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(3, 57, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyBytes_AsUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(2, 57, __pyx_L1_error)
   __pyx_v_data_bytes = __pyx_t_6;
 
   /* "lzokay/_lzokay.pyx":58
  *     cdef c_EResult code = c_EResult.OutputOverrun
  *     cdef const uint8_t* data_bytes = data
  *     while code == c_EResult.OutputOverrun:             # <<<<<<<<<<<<<<
  *         with nogil:
@@ -4905,15 +4363,15 @@
       /* "lzokay/_lzokay.pyx":64
  *         if code == c_EResult.OutputOverrun:
  *             curren_array_size *= 2
  *             array.resize(b, curren_array_size)             # <<<<<<<<<<<<<<
  * 
  *     array.resize(b, actual_out_size)
  */
-      __pyx_t_5 = resize(__pyx_v_b, __pyx_v_curren_array_size); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(3, 64, __pyx_L1_error)
+      __pyx_t_5 = resize(__pyx_v_b, __pyx_v_curren_array_size); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(2, 64, __pyx_L1_error)
 
       /* "lzokay/_lzokay.pyx":62
  *             code = c_decompress(data_bytes, data_size, b.data.as_uchars, curren_array_size, actual_out_size)
  * 
  *         if code == c_EResult.OutputOverrun:             # <<<<<<<<<<<<<<
  *             curren_array_size *= 2
  *             array.resize(b, curren_array_size)
@@ -4924,44 +4382,44 @@
   /* "lzokay/_lzokay.pyx":66
  *             array.resize(b, curren_array_size)
  * 
  *     array.resize(b, actual_out_size)             # <<<<<<<<<<<<<<
  * 
  *     if code in result_mapping:
  */
-  __pyx_t_5 = resize(__pyx_v_b, __pyx_v_actual_out_size); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(3, 66, __pyx_L1_error)
+  __pyx_t_5 = resize(__pyx_v_b, __pyx_v_actual_out_size); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(2, 66, __pyx_L1_error)
 
   /* "lzokay/_lzokay.pyx":68
  *     array.resize(b, actual_out_size)
  * 
  *     if code in result_mapping:             # <<<<<<<<<<<<<<
  *         raise result_mapping[code]()
  * 
  */
-  __pyx_t_4 = __Pyx_Enum_EResult_to_py(__pyx_v_code); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 68, __pyx_L1_error)
+  __pyx_t_4 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(__pyx_v_code); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 68, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_4, __pyx_t_7, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(3, 68, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_4, __pyx_t_7, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(2, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (unlikely(__pyx_t_2)) {
 
     /* "lzokay/_lzokay.pyx":69
  * 
  *     if code in result_mapping:
  *         raise result_mapping[code]()             # <<<<<<<<<<<<<<
  * 
  *     return b.tobytes()
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 69, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = __Pyx_Enum_EResult_to_py(__pyx_v_code); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 69, __pyx_L1_error)
+    __pyx_t_8 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(__pyx_v_code); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(3, 69, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_8 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
@@ -4973,21 +4431,21 @@
         __pyx_t_5 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[1] = {__pyx_t_8, };
       __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 69, __pyx_L1_error)
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 69, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __Pyx_Raise(__pyx_t_7, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __PYX_ERR(3, 69, __pyx_L1_error)
+    __PYX_ERR(2, 69, __pyx_L1_error)
 
     /* "lzokay/_lzokay.pyx":68
  *     array.resize(b, actual_out_size)
  * 
  *     if code in result_mapping:             # <<<<<<<<<<<<<<
  *         raise result_mapping[code]()
  * 
@@ -4998,15 +4456,15 @@
  *         raise result_mapping[code]()
  * 
  *     return b.tobytes()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_b), __pyx_n_s_tobytes); if (unlikely(!__pyx_t_9)) __PYX_ERR(3, 71, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_b), __pyx_n_s_tobytes); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_8 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
@@ -5016,19 +4474,19 @@
       __pyx_t_5 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_8, };
     __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 71, __pyx_L1_error)
+    if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
-  if (!(likely(PyBytes_CheckExact(__pyx_t_7))||((__pyx_t_7) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_7))) __PYX_ERR(3, 71, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_t_7))||((__pyx_t_7) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_7))) __PYX_ERR(2, 71, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_7);
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
   /* "lzokay/_lzokay.pyx":45
  * 
  * 
@@ -5099,37 +4557,37 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(3, 74, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 74, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compress") < 0)) __PYX_ERR(3, 74, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compress") < 0)) __PYX_ERR(2, 74, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_data = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("compress", 1, 1, 1, __pyx_nargs); __PYX_ERR(3, 74, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("compress", 1, 1, 1, __pyx_nargs); __PYX_ERR(2, 74, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lzokay._lzokay.compress", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 0, "data", 1))) __PYX_ERR(3, 74, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 0, "data", 1))) __PYX_ERR(2, 74, __pyx_L1_error)
   __pyx_r = __pyx_pf_6lzokay_7_lzokay_4compress(__pyx_self, __pyx_v_data);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5162,61 +4620,61 @@
   /* "lzokay/_lzokay.pyx":75
  * 
  * def compress(data: bytes) -> bytes:
  *     cdef const uint8_t* data_bytes = data             # <<<<<<<<<<<<<<
  *     cdef size_t data_size = len(data)
  *     cdef size_t expected_out_size = compress_worst_size(data_size)
  */
-  __pyx_t_1 = __Pyx_PyBytes_AsUString(__pyx_v_data); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(3, 75, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_AsUString(__pyx_v_data); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(2, 75, __pyx_L1_error)
   __pyx_v_data_bytes = __pyx_t_1;
 
   /* "lzokay/_lzokay.pyx":76
  * def compress(data: bytes) -> bytes:
  *     cdef const uint8_t* data_bytes = data
  *     cdef size_t data_size = len(data)             # <<<<<<<<<<<<<<
  *     cdef size_t expected_out_size = compress_worst_size(data_size)
  * 
  */
-  __pyx_t_2 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(3, 76, __pyx_L1_error)
+  __pyx_t_2 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(2, 76, __pyx_L1_error)
   __pyx_v_data_size = __pyx_t_2;
 
   /* "lzokay/_lzokay.pyx":77
  *     cdef const uint8_t* data_bytes = data
  *     cdef size_t data_size = len(data)
  *     cdef size_t expected_out_size = compress_worst_size(data_size)             # <<<<<<<<<<<<<<
  * 
  *     cdef array.array b = array.array('B')
  */
-  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_data_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 77, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_data_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(3, 77, __pyx_L1_error)
-  __pyx_t_4 = __pyx_f_6lzokay_7_lzokay_compress_worst_size(((PyObject*)__pyx_t_3), 0); if (unlikely(__pyx_t_4 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(3, 77, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_3)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(2, 77, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_6lzokay_7_lzokay_compress_worst_size(((PyObject*)__pyx_t_3), 0); if (unlikely(__pyx_t_4 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(2, 77, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_expected_out_size = __pyx_t_4;
 
   /* "lzokay/_lzokay.pyx":79
  *     cdef size_t expected_out_size = compress_worst_size(data_size)
  * 
  *     cdef array.array b = array.array('B')             # <<<<<<<<<<<<<<
  *     array.resize(b, expected_out_size)
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 79, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_b = ((arrayobject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "lzokay/_lzokay.pyx":80
  * 
  *     cdef array.array b = array.array('B')
  *     array.resize(b, expected_out_size)             # <<<<<<<<<<<<<<
  * 
  *     # Results from c_compress
  */
-  __pyx_t_4 = resize(__pyx_v_b, __pyx_v_expected_out_size); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 80, __pyx_L1_error)
+  __pyx_t_4 = resize(__pyx_v_b, __pyx_v_expected_out_size); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 80, __pyx_L1_error)
 
   /* "lzokay/_lzokay.pyx":84
  *     # Results from c_compress
  *     cdef c_EResult code
  *     cdef size_t actual_out_size = 0             # <<<<<<<<<<<<<<
  * 
  *     with nogil:
@@ -5271,44 +4729,44 @@
   /* "lzokay/_lzokay.pyx":89
  *         code = c_compress(data_bytes, data_size, b.data.as_uchars, expected_out_size, actual_out_size)
  * 
  *     array.resize(b, actual_out_size)             # <<<<<<<<<<<<<<
  * 
  *     if code in result_mapping:
  */
-  __pyx_t_4 = resize(__pyx_v_b, __pyx_v_actual_out_size); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(3, 89, __pyx_L1_error)
+  __pyx_t_4 = resize(__pyx_v_b, __pyx_v_actual_out_size); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 89, __pyx_L1_error)
 
   /* "lzokay/_lzokay.pyx":91
  *     array.resize(b, actual_out_size)
  * 
  *     if code in result_mapping:             # <<<<<<<<<<<<<<
  *         raise result_mapping[code]()
  * 
  */
-  __pyx_t_3 = __Pyx_Enum_EResult_to_py(__pyx_v_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 91, __pyx_L1_error)
+  __pyx_t_3 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(__pyx_v_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 91, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_t_3, __pyx_t_5, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(3, 91, __pyx_L1_error)
+  __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_t_3, __pyx_t_5, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(2, 91, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(__pyx_t_6)) {
 
     /* "lzokay/_lzokay.pyx":92
  * 
  *     if code in result_mapping:
  *         raise result_mapping[code]()             # <<<<<<<<<<<<<<
  * 
  *     return b.tobytes()
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 92, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_result_mapping); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = __Pyx_Enum_EResult_to_py(__pyx_v_code); if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 92, __pyx_L1_error)
+    __pyx_t_7 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(__pyx_v_code); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 92, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = NULL;
     __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
@@ -5320,21 +4778,21 @@
         __pyx_t_4 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[1] = {__pyx_t_7, };
       __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 92, __pyx_L1_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 92, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(3, 92, __pyx_L1_error)
+    __PYX_ERR(2, 92, __pyx_L1_error)
 
     /* "lzokay/_lzokay.pyx":91
  *     array.resize(b, actual_out_size)
  * 
  *     if code in result_mapping:             # <<<<<<<<<<<<<<
  *         raise result_mapping[code]()
  * 
@@ -5345,15 +4803,15 @@
  *         raise result_mapping[code]()
  * 
  *     return b.tobytes()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_b), __pyx_n_s_tobytes); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 94, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_b), __pyx_n_s_tobytes); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_7 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
@@ -5363,19 +4821,19 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_7, };
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 94, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
-  if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_5))) __PYX_ERR(3, 94, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_5))) __PYX_ERR(2, 94, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
   /* "lzokay/_lzokay.pyx":74
  * 
  * 
@@ -5411,27 +4869,22 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
-    {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
     {&__pyx_n_u_B, __pyx_k_B, sizeof(__pyx_k_B), 0, 1, 0, 1},
-    {&__pyx_n_s_EResult, __pyx_k_EResult, sizeof(__pyx_k_EResult), 0, 0, 1, 1},
     {&__pyx_n_s_Error, __pyx_k_Error, sizeof(__pyx_k_Error), 0, 0, 1, 1},
-    {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
     {&__pyx_n_s_InputNotConsumed, __pyx_k_InputNotConsumed, sizeof(__pyx_k_InputNotConsumed), 0, 0, 1, 1},
     {&__pyx_n_s_InputOverrun, __pyx_k_InputOverrun, sizeof(__pyx_k_InputOverrun), 0, 0, 1, 1},
     {&__pyx_n_s_LookbehindOverrun, __pyx_k_LookbehindOverrun, sizeof(__pyx_k_LookbehindOverrun), 0, 0, 1, 1},
     {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
     {&__pyx_n_s_OutputOverrun, __pyx_k_OutputOverrun, sizeof(__pyx_k_OutputOverrun), 0, 0, 1, 1},
-    {&__pyx_n_s_Success, __pyx_k_Success, sizeof(__pyx_k_Success), 0, 0, 1, 1},
-    {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
-    {&__pyx_n_s__11, __pyx_k__11, sizeof(__pyx_k__11), 0, 0, 1, 1},
+    {&__pyx_n_s__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 0, 1, 1},
     {&__pyx_n_s__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 1},
     {&__pyx_n_s_actual_out_size, __pyx_k_actual_out_size, sizeof(__pyx_k_actual_out_size), 0, 0, 1, 1},
     {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
     {&__pyx_n_s_bytes, __pyx_k_bytes, sizeof(__pyx_k_bytes), 0, 0, 1, 1},
     {&__pyx_n_s_class_getitem, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
@@ -5442,26 +4895,23 @@
     {&__pyx_n_s_curren_array_size, __pyx_k_curren_array_size, sizeof(__pyx_k_curren_array_size), 0, 0, 1, 1},
     {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
     {&__pyx_n_s_data_bytes, __pyx_k_data_bytes, sizeof(__pyx_k_data_bytes), 0, 0, 1, 1},
     {&__pyx_n_s_data_size, __pyx_k_data_size, sizeof(__pyx_k_data_size), 0, 0, 1, 1},
     {&__pyx_n_s_decompress, __pyx_k_decompress, sizeof(__pyx_k_decompress), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
     {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
-    {&__pyx_kp_u_enum_class_EResult_not_importabl, __pyx_k_enum_class_EResult_not_importabl, sizeof(__pyx_k_enum_class_EResult_not_importabl), 0, 1, 0, 0},
     {&__pyx_n_s_expected_out_size, __pyx_k_expected_out_size, sizeof(__pyx_k_expected_out_size), 0, 0, 1, 1},
     {&__pyx_n_s_expected_output_size, __pyx_k_expected_output_size, sizeof(__pyx_k_expected_output_size), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_init_subclass, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
     {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
-    {&__pyx_kp_u_is_not_a_valid_EResult, __pyx_k_is_not_a_valid_EResult, sizeof(__pyx_k_is_not_a_valid_EResult), 0, 1, 0, 0},
     {&__pyx_n_s_lzokay__lzokay, __pyx_k_lzokay__lzokay, sizeof(__pyx_k_lzokay__lzokay), 0, 0, 1, 1},
     {&__pyx_kp_s_lzokay_pyx, __pyx_k_lzokay_pyx, sizeof(__pyx_k_lzokay_pyx), 0, 0, 1, 0},
-    {&__pyx_n_s_lzokay_wrap, __pyx_k_lzokay_wrap, sizeof(__pyx_k_lzokay_wrap), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
     {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
     {&__pyx_n_s_mro_entries, __pyx_k_mro_entries, sizeof(__pyx_k_mro_entries), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
     {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
@@ -5469,25 +4919,21 @@
     {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
     {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
     {&__pyx_n_s_set_name, __pyx_k_set_name, sizeof(__pyx_k_set_name), 0, 0, 1, 1},
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
     {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_tobytes, __pyx_k_tobytes, sizeof(__pyx_k_tobytes), 0, 0, 1, 1},
-    {&__pyx_n_s_warn, __pyx_k_warn, sizeof(__pyx_k_warn), 0, 0, 1, 1},
-    {&__pyx_n_s_warnings, __pyx_k_warnings, sizeof(__pyx_k_warnings), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(0, 139, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 163, __pyx_L1_error)
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 120, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 120, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -5497,69 +4943,69 @@
   /* "lzokay/_lzokay.pyx":53
  * 
  *     cdef size_t actual_out_size = 0
  *     cdef array.array b = array.array('B')             # <<<<<<<<<<<<<<
  *     array.resize(b, curren_array_size)
  * 
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_u_B); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(3, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_n_u_B); if (unlikely(!__pyx_tuple_)) __PYX_ERR(2, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
 
   /* "lzokay/_lzokay.pyx":41
  * 
  * 
  * cpdef int compress_worst_size(s: int):             # <<<<<<<<<<<<<<
  *     return s + s // 16 + 64 + 3
  * 
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_n_s_s); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(3, 41, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lzokay_pyx, __pyx_n_s_compress_worst_size, 41, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(3, 41, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_s_s); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lzokay_pyx, __pyx_n_s_compress_worst_size, 41, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(2, 41, __pyx_L1_error)
 
   /* "lzokay/_lzokay.pyx":45
  * 
  * 
  * def decompress(data: bytes, expected_output_size: int = None) -> bytes:             # <<<<<<<<<<<<<<
  *     data_size = len(data)
  * 
  */
-  __pyx_tuple__6 = PyTuple_Pack(8, __pyx_n_s_data, __pyx_n_s_expected_output_size, __pyx_n_s_data_size, __pyx_n_s_curren_array_size, __pyx_n_s_actual_out_size, __pyx_n_s_b, __pyx_n_s_code, __pyx_n_s_data_bytes); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(3, 45, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lzokay_pyx, __pyx_n_s_decompress, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(3, 45, __pyx_L1_error)
-  __pyx_tuple__8 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(3, 45, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__5 = PyTuple_Pack(8, __pyx_n_s_data, __pyx_n_s_expected_output_size, __pyx_n_s_data_size, __pyx_n_s_curren_array_size, __pyx_n_s_actual_out_size, __pyx_n_s_b, __pyx_n_s_code, __pyx_n_s_data_bytes); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 45, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lzokay_pyx, __pyx_n_s_decompress, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(2, 45, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 45, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "lzokay/_lzokay.pyx":74
  * 
  * 
  * def compress(data: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     cdef const uint8_t* data_bytes = data
  *     cdef size_t data_size = len(data)
  */
-  __pyx_tuple__9 = PyTuple_Pack(7, __pyx_n_s_data, __pyx_n_s_data_bytes, __pyx_n_s_data_size, __pyx_n_s_expected_out_size, __pyx_n_s_b, __pyx_n_s_code, __pyx_n_s_actual_out_size); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(3, 74, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lzokay_pyx, __pyx_n_s_compress, 74, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(3, 74, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(7, __pyx_n_s_data, __pyx_n_s_data_bytes, __pyx_n_s_data_size, __pyx_n_s_expected_out_size, __pyx_n_s_b, __pyx_n_s_code, __pyx_n_s_actual_out_size); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 74, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lzokay_pyx, __pyx_n_s_compress, 74, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(2, 74, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
-  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(3, 1, __pyx_L1_error);
-  __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(3, 1, __pyx_L1_error)
-  __pyx_int_16 = PyInt_FromLong(16); if (unlikely(!__pyx_int_16)) __PYX_ERR(3, 1, __pyx_L1_error)
-  __pyx_int_64 = PyInt_FromLong(64); if (unlikely(!__pyx_int_64)) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(2, 1, __pyx_L1_error);
+  __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_int_16 = PyInt_FromLong(16); if (unlikely(!__pyx_int_16)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_int_64 = PyInt_FromLong(64); if (unlikely(!__pyx_int_64)) __PYX_ERR(2, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: init_globals ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
@@ -5611,37 +5057,37 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
-  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
   sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
   sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 69, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_3_0_0(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(arrayobject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 69, __pyx_L1_error)
+  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_3_0_0(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(arrayobject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(1, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5845,414 +5291,414 @@
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("_lzokay", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
-  if (unlikely(!__pyx_m)) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (unlikely(!__pyx_m)) __PYX_ERR(2, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
-  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
     __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to _lzokay pseudovariable */
-    if (unlikely((add_module_result < 0))) __PYX_ERR(3, 1, __pyx_L1_error)
+    if (unlikely((add_module_result < 0))) __PYX_ERR(2, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
-  if (unlikely(!__pyx_m)) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (unlikely(!__pyx_m)) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(2, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(2, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(2, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit__lzokay(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (__Pyx_check_binary_version() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
-  __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(3, 1, __pyx_L1_error)
-  __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(3, 1, __pyx_L1_error)
-  __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(2, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
   #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
   /*--- Initialize various global constants etc. ---*/
-  if (__Pyx_InitConstants() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (__Pyx_InitConstants() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   stringtab_initialized = 1;
-  if (__Pyx_InitGlobals() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (__Pyx_InitGlobals() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
-  if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_lzokay___lzokay) {
-    if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+    if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
-    PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(3, 1, __pyx_L1_error)
+    PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(2, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "lzokay._lzokay")) {
-      if (unlikely((PyDict_SetItemString(modules, "lzokay._lzokay", __pyx_m) < 0))) __PYX_ERR(3, 1, __pyx_L1_error)
+      if (unlikely((PyDict_SetItemString(modules, "lzokay._lzokay", __pyx_m) < 0))) __PYX_ERR(2, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   (void)__Pyx_modinit_type_init_code();
-  if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(2, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
-  if (__Pyx_patch_abc() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (__Pyx_patch_abc() < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   #endif
 
   /* "lzokay/_lzokay.pyx":2
  * from cpython cimport array
  * import array             # <<<<<<<<<<<<<<
  * from libc.stdint cimport uint8_t
  * 
  */
-  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_array, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 2, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_array, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_array, __pyx_t_2) < 0) __PYX_ERR(3, 2, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_array, __pyx_t_2) < 0) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "lzokay/_lzokay.pyx":12
  * 
  * 
  * class LookbehindOverrun(Exception):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_LookbehindOverrun, __pyx_n_s_LookbehindOverrun, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_LookbehindOverrun, __pyx_n_s_LookbehindOverrun, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (__pyx_t_3 != __pyx_t_2) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(3, 12, __pyx_L1_error)
+    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_LookbehindOverrun, __pyx_t_3, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_LookbehindOverrun, __pyx_t_3, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LookbehindOverrun, __pyx_t_2) < 0) __PYX_ERR(3, 12, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LookbehindOverrun, __pyx_t_2) < 0) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "lzokay/_lzokay.pyx":16
  * 
  * 
  * class OutputOverrun(Exception):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 16, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_4 = __Pyx_PEP560_update_bases(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 16, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PEP560_update_bases(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 16, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_5, __pyx_t_4, __pyx_n_s_OutputOverrun, __pyx_n_s_OutputOverrun, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_5, __pyx_t_4, __pyx_n_s_OutputOverrun, __pyx_n_s_OutputOverrun, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__pyx_t_4 != __pyx_t_3) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_2, "__orig_bases__", __pyx_t_3) < 0))) __PYX_ERR(3, 16, __pyx_L1_error)
+    if (unlikely((PyDict_SetItemString(__pyx_t_2, "__orig_bases__", __pyx_t_3) < 0))) __PYX_ERR(2, 16, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_5, __pyx_n_s_OutputOverrun, __pyx_t_4, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_5, __pyx_n_s_OutputOverrun, __pyx_t_4, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_OutputOverrun, __pyx_t_3) < 0) __PYX_ERR(3, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_OutputOverrun, __pyx_t_3) < 0) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "lzokay/_lzokay.pyx":20
  * 
  * 
  * class InputOverrun(Exception):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 20, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_5 = __Pyx_PEP560_update_bases(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 20, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PEP560_update_bases(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 20, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_5, __pyx_n_s_InputOverrun, __pyx_n_s_InputOverrun, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 20, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_5, __pyx_n_s_InputOverrun, __pyx_n_s_InputOverrun, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__pyx_t_5 != __pyx_t_4) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_3, "__orig_bases__", __pyx_t_4) < 0))) __PYX_ERR(3, 20, __pyx_L1_error)
+    if (unlikely((PyDict_SetItemString(__pyx_t_3, "__orig_bases__", __pyx_t_4) < 0))) __PYX_ERR(2, 20, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_InputOverrun, __pyx_t_5, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 20, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_InputOverrun, __pyx_t_5, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InputOverrun, __pyx_t_4) < 0) __PYX_ERR(3, 20, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InputOverrun, __pyx_t_4) < 0) __PYX_ERR(2, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "lzokay/_lzokay.pyx":24
  * 
  * 
  * class Error(Exception):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 24, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_2 = __Pyx_PEP560_update_bases(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 24, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PEP560_update_bases(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 24, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_Py3MetaclassPrepare(__pyx_t_3, __pyx_t_2, __pyx_n_s_Error, __pyx_n_s_Error, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 24, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3MetaclassPrepare(__pyx_t_3, __pyx_t_2, __pyx_n_s_Error, __pyx_n_s_Error, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__pyx_t_2 != __pyx_t_5) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_4, "__orig_bases__", __pyx_t_5) < 0))) __PYX_ERR(3, 24, __pyx_L1_error)
+    if (unlikely((PyDict_SetItemString(__pyx_t_4, "__orig_bases__", __pyx_t_5) < 0))) __PYX_ERR(2, 24, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_3, __pyx_n_s_Error, __pyx_t_2, __pyx_t_4, NULL, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 24, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_3, __pyx_n_s_Error, __pyx_t_2, __pyx_t_4, NULL, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Error, __pyx_t_5) < 0) __PYX_ERR(3, 24, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Error, __pyx_t_5) < 0) __PYX_ERR(2, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "lzokay/_lzokay.pyx":28
  * 
  * 
  * class InputNotConsumed(Exception):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 28, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 28, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 28, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_InputNotConsumed, __pyx_n_s_InputNotConsumed, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 28, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_InputNotConsumed, __pyx_n_s_InputNotConsumed, (PyObject *) NULL, __pyx_n_s_lzokay__lzokay, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (__pyx_t_3 != __pyx_t_2) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(3, 28, __pyx_L1_error)
+    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(2, 28, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_InputNotConsumed, __pyx_t_3, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(3, 28, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_InputNotConsumed, __pyx_t_3, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InputNotConsumed, __pyx_t_2) < 0) __PYX_ERR(3, 28, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InputNotConsumed, __pyx_t_2) < 0) __PYX_ERR(2, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "lzokay/_lzokay.pyx":33
  * 
  * result_mapping = {
  *     c_EResult.LookbehindOverrun: LookbehindOverrun,             # <<<<<<<<<<<<<<
  *     c_EResult.OutputOverrun: OutputOverrun,
  *     c_EResult.InputOverrun: InputOverrun,
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 33, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_Enum_EResult_to_py(lzokay::EResult::LookbehindOverrun); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 33, __pyx_L1_error)
+  __pyx_t_4 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(lzokay::EResult::LookbehindOverrun); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LookbehindOverrun); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 33, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LookbehindOverrun); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_4, __pyx_t_5) < 0) __PYX_ERR(3, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_4, __pyx_t_5) < 0) __PYX_ERR(2, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "lzokay/_lzokay.pyx":34
  * result_mapping = {
  *     c_EResult.LookbehindOverrun: LookbehindOverrun,
  *     c_EResult.OutputOverrun: OutputOverrun,             # <<<<<<<<<<<<<<
  *     c_EResult.InputOverrun: InputOverrun,
  *     c_EResult.Error: Error,
  */
-  __pyx_t_5 = __Pyx_Enum_EResult_to_py(lzokay::EResult::OutputOverrun); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 34, __pyx_L1_error)
+  __pyx_t_5 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(lzokay::EResult::OutputOverrun); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_OutputOverrun); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 34, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_OutputOverrun); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_5, __pyx_t_4) < 0) __PYX_ERR(3, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_5, __pyx_t_4) < 0) __PYX_ERR(2, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "lzokay/_lzokay.pyx":35
  *     c_EResult.LookbehindOverrun: LookbehindOverrun,
  *     c_EResult.OutputOverrun: OutputOverrun,
  *     c_EResult.InputOverrun: InputOverrun,             # <<<<<<<<<<<<<<
  *     c_EResult.Error: Error,
  *     c_EResult.InputNotConsumed: InputNotConsumed,
  */
-  __pyx_t_4 = __Pyx_Enum_EResult_to_py(lzokay::EResult::InputOverrun); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 35, __pyx_L1_error)
+  __pyx_t_4 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(lzokay::EResult::InputOverrun); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InputOverrun); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 35, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InputOverrun); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_4, __pyx_t_5) < 0) __PYX_ERR(3, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_4, __pyx_t_5) < 0) __PYX_ERR(2, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "lzokay/_lzokay.pyx":36
  *     c_EResult.OutputOverrun: OutputOverrun,
  *     c_EResult.InputOverrun: InputOverrun,
  *     c_EResult.Error: Error,             # <<<<<<<<<<<<<<
  *     c_EResult.InputNotConsumed: InputNotConsumed,
  * }
  */
-  __pyx_t_5 = __Pyx_Enum_EResult_to_py(lzokay::EResult::Error); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 36, __pyx_L1_error)
+  __pyx_t_5 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(lzokay::EResult::Error); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Error); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 36, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Error); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_5, __pyx_t_4) < 0) __PYX_ERR(3, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_5, __pyx_t_4) < 0) __PYX_ERR(2, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "lzokay/_lzokay.pyx":37
  *     c_EResult.InputOverrun: InputOverrun,
  *     c_EResult.Error: Error,
  *     c_EResult.InputNotConsumed: InputNotConsumed,             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  __pyx_t_4 = __Pyx_Enum_EResult_to_py(lzokay::EResult::InputNotConsumed); if (unlikely(!__pyx_t_4)) __PYX_ERR(3, 37, __pyx_L1_error)
+  __pyx_t_4 = [](const lzokay::EResult& x){return __Pyx_PyInt_From_int((int)x);}(lzokay::EResult::InputNotConsumed); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InputNotConsumed); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 37, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_InputNotConsumed); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_t_4, __pyx_t_5) < 0) __PYX_ERR(3, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_t_4, __pyx_t_5) < 0) __PYX_ERR(2, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_result_mapping, __pyx_t_3) < 0) __PYX_ERR(3, 32, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_result_mapping, __pyx_t_3) < 0) __PYX_ERR(2, 32, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "lzokay/_lzokay.pyx":41
  * 
  * 
  * cpdef int compress_worst_size(s: int):             # <<<<<<<<<<<<<<
  *     return s + s // 16 + 64 + 3
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 41, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_s, __pyx_n_s_int) < 0) __PYX_ERR(3, 41, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6lzokay_7_lzokay_1compress_worst_size, 0, __pyx_n_s_compress_worst_size, NULL, __pyx_n_s_lzokay__lzokay, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 41, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_s, __pyx_n_s_int) < 0) __PYX_ERR(2, 41, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6lzokay_7_lzokay_1compress_worst_size, 0, __pyx_n_s_compress_worst_size, NULL, __pyx_n_s_lzokay__lzokay, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compress_worst_size, __pyx_t_5) < 0) __PYX_ERR(3, 41, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compress_worst_size, __pyx_t_5) < 0) __PYX_ERR(2, 41, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "lzokay/_lzokay.pyx":45
  * 
  * 
  * def decompress(data: bytes, expected_output_size: int = None) -> bytes:             # <<<<<<<<<<<<<<
  *     data_size = len(data)
  * 
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 45, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_data, __pyx_n_s_bytes) < 0) __PYX_ERR(3, 45, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_expected_output_size, __pyx_n_s_int) < 0) __PYX_ERR(3, 45, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(3, 45, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6lzokay_7_lzokay_3decompress, 0, __pyx_n_s_decompress, NULL, __pyx_n_s_lzokay__lzokay, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_data, __pyx_n_s_bytes) < 0) __PYX_ERR(2, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_expected_output_size, __pyx_n_s_int) < 0) __PYX_ERR(2, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(2, 45, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_6lzokay_7_lzokay_3decompress, 0, __pyx_n_s_decompress, NULL, __pyx_n_s_lzokay__lzokay, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__8);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__7);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_decompress, __pyx_t_3) < 0) __PYX_ERR(3, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_decompress, __pyx_t_3) < 0) __PYX_ERR(2, 45, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "lzokay/_lzokay.pyx":74
  * 
  * 
  * def compress(data: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     cdef const uint8_t* data_bytes = data
  *     cdef size_t data_size = len(data)
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 74, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data, __pyx_n_s_bytes) < 0) __PYX_ERR(3, 74, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(3, 74, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6lzokay_7_lzokay_5compress, 0, __pyx_n_s_compress, NULL, __pyx_n_s_lzokay__lzokay, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 74, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data, __pyx_n_s_bytes) < 0) __PYX_ERR(2, 74, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(2, 74, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6lzokay_7_lzokay_5compress, 0, __pyx_n_s_compress, NULL, __pyx_n_s_lzokay__lzokay, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compress, __pyx_t_5) < 0) __PYX_ERR(3, 74, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compress, __pyx_t_5) < 0) __PYX_ERR(2, 74, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "lzokay/_lzokay.pyx":1
  * from cpython cimport array             # <<<<<<<<<<<<<<
  * import array
  * from libc.stdint cimport uint8_t
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_5) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_5) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -6318,1214 +5764,14 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
-/* PyErrExceptionMatches */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    int result;
-    PyObject *exc_type;
-#if PY_VERSION_HEX >= 0x030C00A6
-    PyObject *current_exception = tstate->current_exception;
-    if (unlikely(!current_exception)) return 0;
-    exc_type = (PyObject*) Py_TYPE(current_exception);
-    if (exc_type == err) return 1;
-#else
-    exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-#endif
-    #if CYTHON_AVOID_BORROWED_REFS
-    Py_INCREF(exc_type);
-    #endif
-    if (unlikely(PyTuple_Check(err))) {
-        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    } else {
-        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
-    }
-    #if CYTHON_AVOID_BORROWED_REFS
-    Py_DECREF(exc_type);
-    #endif
-    return result;
-}
-#endif
-
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-#if PY_VERSION_HEX >= 0x030C00A6
-    PyObject *tmp_value;
-    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
-    if (value) {
-        #if CYTHON_COMPILING_IN_CPYTHON
-        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
-        #endif
-            PyException_SetTraceback(value, tb);
-    }
-    tmp_value = tstate->current_exception;
-    tstate->current_exception = value;
-    Py_XDECREF(tmp_value);
-#else
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#endif
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-#if PY_VERSION_HEX >= 0x030C00A6
-    PyObject* exc_value;
-    exc_value = tstate->current_exception;
-    tstate->current_exception = 0;
-    *value = exc_value;
-    *type = NULL;
-    *tb = NULL;
-    if (exc_value) {
-        *type = (PyObject*) Py_TYPE(exc_value);
-        Py_INCREF(*type);
-        #if CYTHON_COMPILING_IN_CPYTHON
-        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
-        Py_XINCREF(*tb);
-        #else
-        *tb = PyException_GetTraceback(exc_value);
-        #endif
-    }
-#else
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-#endif
-}
-#endif
-
-/* PyObjectGetAttrStr */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro))
-        return tp->tp_getattro(obj, attr_name);
-#if PY_MAJOR_VERSION < 3
-    if (likely(tp->tp_getattr))
-        return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
-#endif
-    return PyObject_GetAttr(obj, attr_name);
-}
-#endif
-
-/* PyObjectGetAttrStrNoError */
-static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        __Pyx_PyErr_Clear();
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
-    PyObject *result;
-#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
-        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
-    }
-#endif
-    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
-    if (unlikely(!result)) {
-        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
-    }
-    return result;
-}
-
-/* GetBuiltinName */
-static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
-    if (unlikely(!result) && !PyErr_Occurred()) {
-        PyErr_Format(PyExc_NameError,
-#if PY_MAJOR_VERSION >= 3
-            "name '%U' is not defined", name);
-#else
-            "name '%.200s' is not defined", PyString_AS_STRING(name));
-#endif
-    }
-    return result;
-}
-
-/* Import */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *module = 0;
-    PyObject *empty_dict = 0;
-    PyObject *empty_list = 0;
-    #if PY_MAJOR_VERSION < 3
-    PyObject *py_import;
-    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (unlikely(!py_import))
-        goto bad;
-    if (!from_list) {
-        empty_list = PyList_New(0);
-        if (unlikely(!empty_list))
-            goto bad;
-        from_list = empty_list;
-    }
-    #endif
-    empty_dict = PyDict_New();
-    if (unlikely(!empty_dict))
-        goto bad;
-    {
-        #if PY_MAJOR_VERSION >= 3
-        if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
-                #if CYTHON_COMPILING_IN_LIMITED_API
-                module = PyImport_ImportModuleLevelObject(
-                    name, empty_dict, empty_dict, from_list, 1);
-                #else
-                module = PyImport_ImportModuleLevelObject(
-                    name, __pyx_d, empty_dict, from_list, 1);
-                #endif
-                if (unlikely(!module)) {
-                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
-                        goto bad;
-                    PyErr_Clear();
-                }
-            }
-            level = 0;
-        }
-        #endif
-        if (!module) {
-            #if PY_MAJOR_VERSION < 3
-            PyObject *py_level = PyInt_FromLong(level);
-            if (unlikely(!py_level))
-                goto bad;
-            module = PyObject_CallFunctionObjArgs(py_import,
-                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
-            Py_DECREF(py_level);
-            #else
-            #if CYTHON_COMPILING_IN_LIMITED_API
-            module = PyImport_ImportModuleLevelObject(
-                name, empty_dict, empty_dict, from_list, level);
-            #else
-            module = PyImport_ImportModuleLevelObject(
-                name, __pyx_d, empty_dict, from_list, level);
-            #endif
-            #endif
-        }
-    }
-bad:
-    Py_XDECREF(empty_dict);
-    Py_XDECREF(empty_list);
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(py_import);
-    #endif
-    return module;
-}
-
-/* ImportFrom */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
-    PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
-    if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
-        const char* module_name_str = 0;
-        PyObject* module_name = 0;
-        PyObject* module_dot = 0;
-        PyObject* full_name = 0;
-        PyErr_Clear();
-        module_name_str = PyModule_GetName(module);
-        if (unlikely(!module_name_str)) { goto modbad; }
-        module_name = PyUnicode_FromString(module_name_str);
-        if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u_);
-        if (unlikely(!module_dot)) { goto modbad; }
-        full_name = PyUnicode_Concat(module_dot, name);
-        if (unlikely(!full_name)) { goto modbad; }
-        #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
-        {
-            PyObject *modules = PyImport_GetModuleDict();
-            if (unlikely(!modules))
-                goto modbad;
-            value = PyObject_GetItem(modules, full_name);
-        }
-        #else
-        value = PyImport_GetModule(full_name);
-        #endif
-      modbad:
-        Py_XDECREF(full_name);
-        Py_XDECREF(module_dot);
-        Py_XDECREF(module_name);
-    }
-    if (unlikely(!value)) {
-        PyErr_Format(PyExc_ImportError,
-        #if PY_MAJOR_VERSION < 3
-            "cannot import name %.230s", PyString_AS_STRING(name));
-        #else
-            "cannot import name %S", name);
-        #endif
-    }
-    return value;
-}
-
-/* GetTopmostException */
-#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
-    }
-    return exc_info;
-}
-#endif
-
-/* SaveResetException */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    PyObject *exc_value = exc_info->exc_value;
-    if (exc_value == NULL || exc_value == Py_None) {
-        *value = NULL;
-        *type = NULL;
-        *tb = NULL;
-    } else {
-        *value = exc_value;
-        Py_INCREF(*value);
-        *type = (PyObject*) Py_TYPE(exc_value);
-        Py_INCREF(*type);
-        *tb = PyException_GetTraceback(exc_value);
-    }
-  #elif CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-  #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-  #endif
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    PyObject *tmp_value = exc_info->exc_value;
-    exc_info->exc_value = value;
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-  #else
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-  #endif
-}
-#endif
-
-/* GetException */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
-#endif
-{
-    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-  #if PY_VERSION_HEX >= 0x030C00A6
-    local_value = tstate->current_exception;
-    tstate->current_exception = 0;
-    if (likely(local_value)) {
-        local_type = (PyObject*) Py_TYPE(local_value);
-        Py_INCREF(local_type);
-        local_tb = PyException_GetTraceback(local_value);
-    }
-  #else
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-  #endif
-#else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
-#endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
-    if (unlikely(tstate->current_exception))
-#elif CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
-#else
-    if (unlikely(PyErr_Occurred()))
-#endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
-    }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
-    {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-      #if PY_VERSION_HEX >= 0x030B00a4
-        tmp_value = exc_info->exc_value;
-        exc_info->exc_value = local_value;
-        tmp_type = NULL;
-        tmp_tb = NULL;
-        Py_XDECREF(local_type);
-        Py_XDECREF(local_tb);
-      #else
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
-      #endif
-    }
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
-#endif
-    return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
-}
-
-/* ImportDottedModule */
-#if PY_MAJOR_VERSION >= 3
-static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
-    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
-    if (unlikely(PyErr_Occurred())) {
-        PyErr_Clear();
-    }
-    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
-        partial_name = name;
-    } else {
-        slice = PySequence_GetSlice(parts_tuple, 0, count);
-        if (unlikely(!slice))
-            goto bad;
-        sep = PyUnicode_FromStringAndSize(".", 1);
-        if (unlikely(!sep))
-            goto bad;
-        partial_name = PyUnicode_Join(sep, slice);
-    }
-    PyErr_Format(
-#if PY_MAJOR_VERSION < 3
-        PyExc_ImportError,
-        "No module named '%s'", PyString_AS_STRING(partial_name));
-#else
-#if PY_VERSION_HEX >= 0x030600B1
-        PyExc_ModuleNotFoundError,
-#else
-        PyExc_ImportError,
-#endif
-        "No module named '%U'", partial_name);
-#endif
-bad:
-    Py_XDECREF(sep);
-    Py_XDECREF(slice);
-    Py_XDECREF(partial_name);
-    return NULL;
-}
-#endif
-#if PY_MAJOR_VERSION >= 3
-static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
-    PyObject *imported_module;
-#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
-    PyObject *modules = PyImport_GetModuleDict();
-    if (unlikely(!modules))
-        return NULL;
-    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
-    Py_XINCREF(imported_module);
-#else
-    imported_module = PyImport_GetModule(name);
-#endif
-    return imported_module;
-}
-#endif
-#if PY_MAJOR_VERSION >= 3
-static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
-    Py_ssize_t i, nparts;
-    nparts = PyTuple_GET_SIZE(parts_tuple);
-    for (i=1; i < nparts && module; i++) {
-        PyObject *part, *submodule;
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        part = PyTuple_GET_ITEM(parts_tuple, i);
-#else
-        part = PySequence_ITEM(parts_tuple, i);
-#endif
-        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
-#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
-        Py_DECREF(part);
-#endif
-        Py_DECREF(module);
-        module = submodule;
-    }
-    if (unlikely(!module)) {
-        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
-    }
-    return module;
-}
-#endif
-static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
-#if PY_MAJOR_VERSION < 3
-    PyObject *module, *from_list, *star = __pyx_n_s__2;
-    CYTHON_UNUSED_VAR(parts_tuple);
-    from_list = PyList_New(1);
-    if (unlikely(!from_list))
-        return NULL;
-    Py_INCREF(star);
-    PyList_SET_ITEM(from_list, 0, star);
-    module = __Pyx_Import(name, from_list, 0);
-    Py_DECREF(from_list);
-    return module;
-#else
-    PyObject *imported_module;
-    PyObject *module = __Pyx_Import(name, NULL, 0);
-    if (!parts_tuple || unlikely(!module))
-        return module;
-    imported_module = __Pyx__ImportDottedModule_Lookup(name);
-    if (likely(imported_module)) {
-        Py_DECREF(module);
-        return imported_module;
-    }
-    PyErr_Clear();
-    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
-#endif
-}
-static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
-    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
-    if (likely(module)) {
-        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
-        if (likely(spec)) {
-            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
-            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
-                Py_DECREF(spec);
-                spec = NULL;
-            }
-            Py_XDECREF(unsafe);
-        }
-        if (likely(!spec)) {
-            PyErr_Clear();
-            return module;
-        }
-        Py_DECREF(spec);
-        Py_DECREF(module);
-    } else if (PyErr_Occurred()) {
-        PyErr_Clear();
-    }
-#endif
-    return __Pyx__ImportDottedModule(name, parts_tuple);
-}
-
-/* PyFunctionFastCall */
-#if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
-static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
-                                               PyObject *globals) {
-    PyFrameObject *f;
-    PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject **fastlocals;
-    Py_ssize_t i;
-    PyObject *result;
-    assert(globals != NULL);
-    /* XXX Perhaps we should create a specialized
-       PyFrame_New() that doesn't take locals, but does
-       take builtins without sanity checking them.
-       */
-    assert(tstate != NULL);
-    f = PyFrame_New(tstate, co, globals, NULL);
-    if (f == NULL) {
-        return NULL;
-    }
-    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
-    for (i = 0; i < na; i++) {
-        Py_INCREF(*args);
-        fastlocals[i] = *args++;
-    }
-    result = PyEval_EvalFrameEx(f,0);
-    ++tstate->recursion_depth;
-    Py_DECREF(f);
-    --tstate->recursion_depth;
-    return result;
-}
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
-    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
-    PyObject *globals = PyFunction_GET_GLOBALS(func);
-    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
-    PyObject *closure;
-#if PY_MAJOR_VERSION >= 3
-    PyObject *kwdefs;
-#endif
-    PyObject *kwtuple, **k;
-    PyObject **d;
-    Py_ssize_t nd;
-    Py_ssize_t nk;
-    PyObject *result;
-    assert(kwargs == NULL || PyDict_Check(kwargs));
-    nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
-        return NULL;
-    }
-    if (
-#if PY_MAJOR_VERSION >= 3
-            co->co_kwonlyargcount == 0 &&
-#endif
-            likely(kwargs == NULL || nk == 0) &&
-            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
-        if (argdefs == NULL && co->co_argcount == nargs) {
-            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
-            goto done;
-        }
-        else if (nargs == 0 && argdefs != NULL
-                 && co->co_argcount == Py_SIZE(argdefs)) {
-            /* function called with no arguments, but all parameters have
-               a default value: use default values as arguments .*/
-            args = &PyTuple_GET_ITEM(argdefs, 0);
-            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
-            goto done;
-        }
-    }
-    if (kwargs != NULL) {
-        Py_ssize_t pos, i;
-        kwtuple = PyTuple_New(2 * nk);
-        if (kwtuple == NULL) {
-            result = NULL;
-            goto done;
-        }
-        k = &PyTuple_GET_ITEM(kwtuple, 0);
-        pos = i = 0;
-        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
-            Py_INCREF(k[i]);
-            Py_INCREF(k[i+1]);
-            i += 2;
-        }
-        nk = i / 2;
-    }
-    else {
-        kwtuple = NULL;
-        k = NULL;
-    }
-    closure = PyFunction_GET_CLOSURE(func);
-#if PY_MAJOR_VERSION >= 3
-    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
-#endif
-    if (argdefs != NULL) {
-        d = &PyTuple_GET_ITEM(argdefs, 0);
-        nd = Py_SIZE(argdefs);
-    }
-    else {
-        d = NULL;
-        nd = 0;
-    }
-#if PY_MAJOR_VERSION >= 3
-    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
-                               k, (int)nk,
-                               d, (int)nd, kwdefs, closure);
-#else
-    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
-                               k, (int)nk,
-                               d, (int)nd, closure);
-#endif
-    Py_XDECREF(kwtuple);
-done:
-    Py_LeaveRecursiveCall();
-    return result;
-}
-#endif
-
-/* PyObjectCall */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
-    if (unlikely(!call))
-        return PyObject_Call(func, arg, kw);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = (*call)(func, arg, kw);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
-/* PyObjectCallMethO */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
-    PyObject *self, *result;
-    PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = cfunc(self, arg);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
-/* PyObjectFastCall */
-static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
-    PyObject *argstuple;
-    PyObject *result;
-    size_t i;
-    argstuple = PyTuple_New((Py_ssize_t)nargs);
-    if (unlikely(!argstuple)) return NULL;
-    for (i = 0; i < nargs; i++) {
-        Py_INCREF(args[i]);
-        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
-    }
-    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
-    Py_DECREF(argstuple);
-    return result;
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
-    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
-#if CYTHON_COMPILING_IN_CPYTHON
-    if (nargs == 0 && kwargs == NULL) {
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-        if (__Pyx_IsCyOrPyCFunction(func))
-#else
-        if (PyCFunction_Check(func))
-#endif
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-                return __Pyx_PyObject_CallMethO(func, NULL);
-            }
-        }
-    }
-    else if (nargs == 1 && kwargs == NULL) {
-        if (PyCFunction_Check(func))
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-                return __Pyx_PyObject_CallMethO(func, args[0]);
-            }
-        }
-    }
-#endif
-    #if PY_VERSION_HEX < 0x030800B1
-    #if CYTHON_FAST_PYCCALL
-    if (PyCFunction_Check(func)) {
-        if (kwargs) {
-            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
-        } else {
-            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
-        }
-    }
-    #if PY_VERSION_HEX >= 0x030700A1
-    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
-        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
-    }
-    #endif
-    #endif
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
-    }
-    #endif
-    #endif
-    #if CYTHON_VECTORCALL
-    vectorcallfunc f = _PyVectorcall_Function(func);
-    if (f) {
-        return f(func, args, (size_t)nargs, kwargs);
-    }
-    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
-    if (__Pyx_CyFunction_CheckExact(func)) {
-        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
-        if (f) return f(func, args, (size_t)nargs, kwargs);
-    }
-    #endif
-    if (nargs == 0) {
-        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
-    }
-    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
-}
-
-/* CIntToDigits */
-static const char DIGIT_PAIRS_10[2*10*10+1] = {
-    "00010203040506070809"
-    "10111213141516171819"
-    "20212223242526272829"
-    "30313233343536373839"
-    "40414243444546474849"
-    "50515253545556575859"
-    "60616263646566676869"
-    "70717273747576777879"
-    "80818283848586878889"
-    "90919293949596979899"
-};
-static const char DIGIT_PAIRS_8[2*8*8+1] = {
-    "0001020304050607"
-    "1011121314151617"
-    "2021222324252627"
-    "3031323334353637"
-    "4041424344454647"
-    "5051525354555657"
-    "6061626364656667"
-    "7071727374757677"
-};
-static const char DIGITS_HEX[2*16+1] = {
-    "0123456789abcdef"
-    "0123456789ABCDEF"
-};
-
-/* BuildPyUnicode */
-static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
-                                                int prepend_sign, char padding_char) {
-    PyObject *uval;
-    Py_ssize_t uoffset = ulength - clength;
-#if CYTHON_USE_UNICODE_INTERNALS
-    Py_ssize_t i;
-#if CYTHON_PEP393_ENABLED
-    void *udata;
-    uval = PyUnicode_New(ulength, 127);
-    if (unlikely(!uval)) return NULL;
-    udata = PyUnicode_DATA(uval);
-#else
-    Py_UNICODE *udata;
-    uval = PyUnicode_FromUnicode(NULL, ulength);
-    if (unlikely(!uval)) return NULL;
-    udata = PyUnicode_AS_UNICODE(uval);
-#endif
-    if (uoffset > 0) {
-        i = 0;
-        if (prepend_sign) {
-            __Pyx_PyUnicode_WRITE(PyUnicode_1BYTE_KIND, udata, 0, '-');
-            i++;
-        }
-        for (; i < uoffset; i++) {
-            __Pyx_PyUnicode_WRITE(PyUnicode_1BYTE_KIND, udata, i, padding_char);
-        }
-    }
-    for (i=0; i < clength; i++) {
-        __Pyx_PyUnicode_WRITE(PyUnicode_1BYTE_KIND, udata, uoffset+i, chars[i]);
-    }
-#else
-    {
-        PyObject *sign = NULL, *padding = NULL;
-        uval = NULL;
-        if (uoffset > 0) {
-            prepend_sign = !!prepend_sign;
-            if (uoffset > prepend_sign) {
-                padding = PyUnicode_FromOrdinal(padding_char);
-                if (likely(padding) && uoffset > prepend_sign + 1) {
-                    PyObject *tmp;
-                    PyObject *repeat = PyInt_FromSsize_t(uoffset - prepend_sign);
-                    if (unlikely(!repeat)) goto done_or_error;
-                    tmp = PyNumber_Multiply(padding, repeat);
-                    Py_DECREF(repeat);
-                    Py_DECREF(padding);
-                    padding = tmp;
-                }
-                if (unlikely(!padding)) goto done_or_error;
-            }
-            if (prepend_sign) {
-                sign = PyUnicode_FromOrdinal('-');
-                if (unlikely(!sign)) goto done_or_error;
-            }
-        }
-        uval = PyUnicode_DecodeASCII(chars, clength, NULL);
-        if (likely(uval) && padding) {
-            PyObject *tmp = PyNumber_Add(padding, uval);
-            Py_DECREF(uval);
-            uval = tmp;
-        }
-        if (likely(uval) && sign) {
-            PyObject *tmp = PyNumber_Add(sign, uval);
-            Py_DECREF(uval);
-            uval = tmp;
-        }
-done_or_error:
-        Py_XDECREF(padding);
-        Py_XDECREF(sign);
-    }
-#endif
-    return uval;
-}
-
-/* CIntToPyUnicode */
-static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char) {
-    char digits[sizeof(int)*3+2];
-    char *dpos, *end = digits + sizeof(int)*3+2;
-    const char *hex_digits = DIGITS_HEX;
-    Py_ssize_t length, ulength;
-    int prepend_sign, last_one_off;
-    int remaining;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (format_char == 'X') {
-        hex_digits += 16;
-        format_char = 'x';
-    }
-    remaining = value;
-    last_one_off = 0;
-    dpos = end;
-    do {
-        int digit_pos;
-        switch (format_char) {
-        case 'o':
-            digit_pos = abs((int)(remaining % (8*8)));
-            remaining = (int) (remaining / (8*8));
-            dpos -= 2;
-            memcpy(dpos, DIGIT_PAIRS_8 + digit_pos * 2, 2);
-            last_one_off = (digit_pos < 8);
-            break;
-        case 'd':
-            digit_pos = abs((int)(remaining % (10*10)));
-            remaining = (int) (remaining / (10*10));
-            dpos -= 2;
-            memcpy(dpos, DIGIT_PAIRS_10 + digit_pos * 2, 2);
-            last_one_off = (digit_pos < 10);
-            break;
-        case 'x':
-            *(--dpos) = hex_digits[abs((int)(remaining % 16))];
-            remaining = (int) (remaining / 16);
-            break;
-        default:
-            assert(0);
-            break;
-        }
-    } while (unlikely(remaining != 0));
-    assert(!last_one_off || *dpos == '0');
-    dpos += last_one_off;
-    length = end - dpos;
-    ulength = length;
-    prepend_sign = 0;
-    if (!is_unsigned && value <= neg_one) {
-        if (padding_char == ' ' || width <= length + 1) {
-            *(--dpos) = '-';
-            ++length;
-        } else {
-            prepend_sign = 1;
-        }
-        ++ulength;
-    }
-    if (width > ulength) {
-        ulength = width;
-    }
-    if (ulength == 1) {
-        return PyUnicode_FromOrdinal(*dpos);
-    }
-    return __Pyx_PyUnicode_BuildFromAscii(ulength, dpos, (int) length, prepend_sign, padding_char);
-}
-
-/* UnicodeConcatInPlace */
-# if CYTHON_COMPILING_IN_CPYTHON && PY_MAJOR_VERSION >= 3
-static int
-__Pyx_unicode_modifiable(PyObject *unicode)
-{
-    if (Py_REFCNT(unicode) != 1)
-        return 0;
-    if (!PyUnicode_CheckExact(unicode))
-        return 0;
-    if (PyUnicode_CHECK_INTERNED(unicode))
-        return 0;
-    return 1;
-}
-static CYTHON_INLINE PyObject *__Pyx_PyUnicode_ConcatInPlaceImpl(PyObject **p_left, PyObject *right
-        #if CYTHON_REFNANNY
-        , void* __pyx_refnanny
-        #endif
-    ) {
-    PyObject *left = *p_left;
-    Py_ssize_t left_len, right_len, new_len;
-    if (unlikely(__Pyx_PyUnicode_READY(left) == -1))
-        return NULL;
-    if (unlikely(__Pyx_PyUnicode_READY(right) == -1))
-        return NULL;
-    left_len = PyUnicode_GET_LENGTH(left);
-    if (left_len == 0) {
-        Py_INCREF(right);
-        return right;
-    }
-    right_len = PyUnicode_GET_LENGTH(right);
-    if (right_len == 0) {
-        Py_INCREF(left);
-        return left;
-    }
-    if (unlikely(left_len > PY_SSIZE_T_MAX - right_len)) {
-        PyErr_SetString(PyExc_OverflowError,
-                        "strings are too large to concat");
-        return NULL;
-    }
-    new_len = left_len + right_len;
-    if (__Pyx_unicode_modifiable(left)
-            && PyUnicode_CheckExact(right)
-            && PyUnicode_KIND(right) <= PyUnicode_KIND(left)
-            && !(PyUnicode_IS_ASCII(left) && !PyUnicode_IS_ASCII(right))) {
-        __Pyx_GIVEREF(*p_left);
-        if (unlikely(PyUnicode_Resize(p_left, new_len) != 0)) {
-            __Pyx_GOTREF(*p_left);
-            return NULL;
-        }
-        __Pyx_INCREF(*p_left);
-        _PyUnicode_FastCopyCharacters(*p_left, left_len, right, 0, right_len);
-        return *p_left;
-    } else {
-        return __Pyx_PyUnicode_Concat(left, right);
-    }
-  }
-#endif
-
-/* PyObjectCallOneArg */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *args[2] = {NULL, arg};
-    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
-}
-
-/* RaiseException */
-#if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    CYTHON_UNUSED_VAR(cause);
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
-    }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
-        }
-    }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
-}
-#else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
-                }
-            }
-        }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
-        }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
-    }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
-    }
-    PyErr_SetObject(type, value);
-    if (tb) {
-      #if PY_VERSION_HEX >= 0x030C00A6
-        PyException_SetTraceback(value, tb);
-      #elif CYTHON_FAST_THREAD_STATE
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
-        }
-#else
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#endif
-    }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
-}
-#endif
-
 /* TupleAndListFromArray */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
     PyObject *v;
     Py_ssize_t i;
     for (i = 0; i < length; i++) {
         v = dest[i] = src[i];
@@ -7725,14 +5971,164 @@
             return kwvalues[i];
         }
     }
     return NULL;  // not found (no exception set)
 }
 #endif
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    int result;
+    PyObject *exc_type;
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *current_exception = tstate->current_exception;
+    if (unlikely(!current_exception)) return 0;
+    exc_type = (PyObject*) Py_TYPE(current_exception);
+    if (exc_type == err) return 1;
+#else
+    exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+#endif
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_INCREF(exc_type);
+    #endif
+    if (unlikely(PyTuple_Check(err))) {
+        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    } else {
+        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+    }
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_DECREF(exc_type);
+    #endif
+    return result;
+}
+#endif
+
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *tmp_value;
+    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
+    if (value) {
+        #if CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
+        #endif
+            PyException_SetTraceback(value, tb);
+    }
+    tmp_value = tstate->current_exception;
+    tstate->current_exception = value;
+    Py_XDECREF(tmp_value);
+#else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#endif
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject* exc_value;
+    exc_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    *value = exc_value;
+    *type = NULL;
+    *tb = NULL;
+    if (exc_value) {
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
+        Py_XINCREF(*tb);
+        #else
+        *tb = PyException_GetTraceback(exc_value);
+        #endif
+    }
+#else
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#endif
+}
+#endif
+
+/* PyObjectGetAttrStr */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro))
+        return tp->tp_getattro(obj, attr_name);
+#if PY_MAJOR_VERSION < 3
+    if (likely(tp->tp_getattr))
+        return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
+#endif
+    return PyObject_GetAttr(obj, attr_name);
+}
+#endif
+
+/* PyObjectGetAttrStrNoError */
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
+    }
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    }
+    return result;
+}
+
+/* GetBuiltinName */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
+    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
+    if (unlikely(!result) && !PyErr_Occurred()) {
+        PyErr_Format(PyExc_NameError,
+#if PY_MAJOR_VERSION >= 3
+            "name '%U' is not defined", name);
+#else
+            "name '%.200s' is not defined", PyString_AS_STRING(name));
+#endif
+    }
+    return result;
+}
+
 /* PyIntBinop */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
     CYTHON_MAYBE_UNUSED_VAR(intval);
     CYTHON_MAYBE_UNUSED_VAR(inplace);
     CYTHON_UNUSED_VAR(zerodivision_check);
     #if PY_MAJOR_VERSION < 3
@@ -8041,14 +6437,34 @@
         "Argument '%.200s' has incorrect type (expected " __Pyx_FMT_TYPENAME
         ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
     __Pyx_DECREF_TypeName(type_name);
     __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
+/* PyObjectCall */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *result;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
+    if (unlikely(!call))
+        return PyObject_Call(func, arg, kw);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = (*call)(func, arg, kw);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
@@ -8205,14 +6621,234 @@
     if (is_list || PySequence_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
+/* PyFunctionFastCall */
+#if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
+static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
+                                               PyObject *globals) {
+    PyFrameObject *f;
+    PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject **fastlocals;
+    Py_ssize_t i;
+    PyObject *result;
+    assert(globals != NULL);
+    /* XXX Perhaps we should create a specialized
+       PyFrame_New() that doesn't take locals, but does
+       take builtins without sanity checking them.
+       */
+    assert(tstate != NULL);
+    f = PyFrame_New(tstate, co, globals, NULL);
+    if (f == NULL) {
+        return NULL;
+    }
+    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
+    for (i = 0; i < na; i++) {
+        Py_INCREF(*args);
+        fastlocals[i] = *args++;
+    }
+    result = PyEval_EvalFrameEx(f,0);
+    ++tstate->recursion_depth;
+    Py_DECREF(f);
+    --tstate->recursion_depth;
+    return result;
+}
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
+    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
+    PyObject *globals = PyFunction_GET_GLOBALS(func);
+    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
+    PyObject *closure;
+#if PY_MAJOR_VERSION >= 3
+    PyObject *kwdefs;
+#endif
+    PyObject *kwtuple, **k;
+    PyObject **d;
+    Py_ssize_t nd;
+    Py_ssize_t nk;
+    PyObject *result;
+    assert(kwargs == NULL || PyDict_Check(kwargs));
+    nk = kwargs ? PyDict_Size(kwargs) : 0;
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
+        return NULL;
+    }
+    if (
+#if PY_MAJOR_VERSION >= 3
+            co->co_kwonlyargcount == 0 &&
+#endif
+            likely(kwargs == NULL || nk == 0) &&
+            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
+        if (argdefs == NULL && co->co_argcount == nargs) {
+            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
+            goto done;
+        }
+        else if (nargs == 0 && argdefs != NULL
+                 && co->co_argcount == Py_SIZE(argdefs)) {
+            /* function called with no arguments, but all parameters have
+               a default value: use default values as arguments .*/
+            args = &PyTuple_GET_ITEM(argdefs, 0);
+            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
+            goto done;
+        }
+    }
+    if (kwargs != NULL) {
+        Py_ssize_t pos, i;
+        kwtuple = PyTuple_New(2 * nk);
+        if (kwtuple == NULL) {
+            result = NULL;
+            goto done;
+        }
+        k = &PyTuple_GET_ITEM(kwtuple, 0);
+        pos = i = 0;
+        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
+            Py_INCREF(k[i]);
+            Py_INCREF(k[i+1]);
+            i += 2;
+        }
+        nk = i / 2;
+    }
+    else {
+        kwtuple = NULL;
+        k = NULL;
+    }
+    closure = PyFunction_GET_CLOSURE(func);
+#if PY_MAJOR_VERSION >= 3
+    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
+#endif
+    if (argdefs != NULL) {
+        d = &PyTuple_GET_ITEM(argdefs, 0);
+        nd = Py_SIZE(argdefs);
+    }
+    else {
+        d = NULL;
+        nd = 0;
+    }
+#if PY_MAJOR_VERSION >= 3
+    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
+                               args, (int)nargs,
+                               k, (int)nk,
+                               d, (int)nd, kwdefs, closure);
+#else
+    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
+                               args, (int)nargs,
+                               k, (int)nk,
+                               d, (int)nd, closure);
+#endif
+    Py_XDECREF(kwtuple);
+done:
+    Py_LeaveRecursiveCall();
+    return result;
+}
+#endif
+
+/* PyObjectCallMethO */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
+    PyObject *self, *result;
+    PyCFunction cfunc;
+    cfunc = PyCFunction_GET_FUNCTION(func);
+    self = PyCFunction_GET_SELF(func);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = cfunc(self, arg);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
+/* PyObjectFastCall */
+static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+    PyObject *argstuple;
+    PyObject *result;
+    size_t i;
+    argstuple = PyTuple_New((Py_ssize_t)nargs);
+    if (unlikely(!argstuple)) return NULL;
+    for (i = 0; i < nargs; i++) {
+        Py_INCREF(args[i]);
+        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
+    }
+    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+    Py_DECREF(argstuple);
+    return result;
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
+    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (nargs == 0 && kwargs == NULL) {
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
+        if (__Pyx_IsCyOrPyCFunction(func))
+#else
+        if (PyCFunction_Check(func))
+#endif
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+                return __Pyx_PyObject_CallMethO(func, NULL);
+            }
+        }
+    }
+    else if (nargs == 1 && kwargs == NULL) {
+        if (PyCFunction_Check(func))
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+                return __Pyx_PyObject_CallMethO(func, args[0]);
+            }
+        }
+    }
+#endif
+    #if PY_VERSION_HEX < 0x030800B1
+    #if CYTHON_FAST_PYCCALL
+    if (PyCFunction_Check(func)) {
+        if (kwargs) {
+            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
+        } else {
+            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
+        }
+    }
+    #if PY_VERSION_HEX >= 0x030700A1
+    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
+        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
+    }
+    #endif
+    #endif
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
+    }
+    #endif
+    #endif
+    #if CYTHON_VECTORCALL
+    vectorcallfunc f = _PyVectorcall_Function(func);
+    if (f) {
+        return f(func, args, (size_t)nargs, kwargs);
+    }
+    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+    if (__Pyx_CyFunction_CheckExact(func)) {
+        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+        if (f) return f(func, args, (size_t)nargs, kwargs);
+    }
+    #endif
+    if (nargs == 0) {
+        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
+    }
+    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
+}
+
+/* PyObjectCallOneArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *args[2] = {NULL, arg};
+    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject *index) {
     PyObject *runerr = NULL;
     Py_ssize_t key_value;
     key_value = __Pyx_PyIndex_AsSsize_t(index);
     if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
@@ -8253,14 +6889,175 @@
     if (likely(sm && sm->sq_item)) {
         return __Pyx_PyObject_GetIndex(obj, key);
     }
     return __Pyx_PyObject_GetItem_Slow(obj, key);
 }
 #endif
 
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    CYTHON_UNUSED_VAR(cause);
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+      #if PY_VERSION_HEX >= 0x030C00A6
+        PyException_SetTraceback(value, tb);
+      #elif CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
 /* RaiseUnexpectedTypeError */
 static int
 __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
 {
     __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
                  expected, obj_type_name);
@@ -8344,14 +7141,210 @@
     return (PyTypeObject *)result;
 bad:
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
+/* Import */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+    PyObject *module = 0;
+    PyObject *empty_dict = 0;
+    PyObject *empty_list = 0;
+    #if PY_MAJOR_VERSION < 3
+    PyObject *py_import;
+    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
+    if (unlikely(!py_import))
+        goto bad;
+    if (!from_list) {
+        empty_list = PyList_New(0);
+        if (unlikely(!empty_list))
+            goto bad;
+        from_list = empty_list;
+    }
+    #endif
+    empty_dict = PyDict_New();
+    if (unlikely(!empty_dict))
+        goto bad;
+    {
+        #if PY_MAJOR_VERSION >= 3
+        if (level == -1) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+                #if CYTHON_COMPILING_IN_LIMITED_API
+                module = PyImport_ImportModuleLevelObject(
+                    name, empty_dict, empty_dict, from_list, 1);
+                #else
+                module = PyImport_ImportModuleLevelObject(
+                    name, __pyx_d, empty_dict, from_list, 1);
+                #endif
+                if (unlikely(!module)) {
+                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
+                        goto bad;
+                    PyErr_Clear();
+                }
+            }
+            level = 0;
+        }
+        #endif
+        if (!module) {
+            #if PY_MAJOR_VERSION < 3
+            PyObject *py_level = PyInt_FromLong(level);
+            if (unlikely(!py_level))
+                goto bad;
+            module = PyObject_CallFunctionObjArgs(py_import,
+                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
+            Py_DECREF(py_level);
+            #else
+            #if CYTHON_COMPILING_IN_LIMITED_API
+            module = PyImport_ImportModuleLevelObject(
+                name, empty_dict, empty_dict, from_list, level);
+            #else
+            module = PyImport_ImportModuleLevelObject(
+                name, __pyx_d, empty_dict, from_list, level);
+            #endif
+            #endif
+        }
+    }
+bad:
+    Py_XDECREF(empty_dict);
+    Py_XDECREF(empty_list);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_import);
+    #endif
+    return module;
+}
+
+/* ImportDottedModule */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
+    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
+    if (unlikely(PyErr_Occurred())) {
+        PyErr_Clear();
+    }
+    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
+        partial_name = name;
+    } else {
+        slice = PySequence_GetSlice(parts_tuple, 0, count);
+        if (unlikely(!slice))
+            goto bad;
+        sep = PyUnicode_FromStringAndSize(".", 1);
+        if (unlikely(!sep))
+            goto bad;
+        partial_name = PyUnicode_Join(sep, slice);
+    }
+    PyErr_Format(
+#if PY_MAJOR_VERSION < 3
+        PyExc_ImportError,
+        "No module named '%s'", PyString_AS_STRING(partial_name));
+#else
+#if PY_VERSION_HEX >= 0x030600B1
+        PyExc_ModuleNotFoundError,
+#else
+        PyExc_ImportError,
+#endif
+        "No module named '%U'", partial_name);
+#endif
+bad:
+    Py_XDECREF(sep);
+    Py_XDECREF(slice);
+    Py_XDECREF(partial_name);
+    return NULL;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
+    PyObject *imported_module;
+#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+    PyObject *modules = PyImport_GetModuleDict();
+    if (unlikely(!modules))
+        return NULL;
+    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
+    Py_XINCREF(imported_module);
+#else
+    imported_module = PyImport_GetModule(name);
+#endif
+    return imported_module;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
+    }
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
+}
+#endif
+static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if PY_MAJOR_VERSION < 3
+    PyObject *module, *from_list, *star = __pyx_n_s__2;
+    CYTHON_UNUSED_VAR(parts_tuple);
+    from_list = PyList_New(1);
+    if (unlikely(!from_list))
+        return NULL;
+    Py_INCREF(star);
+    PyList_SET_ITEM(from_list, 0, star);
+    module = __Pyx_Import(name, from_list, 0);
+    Py_DECREF(from_list);
+    return module;
+#else
+    PyObject *imported_module;
+    PyObject *module = __Pyx_Import(name, NULL, 0);
+    if (!parts_tuple || unlikely(!module))
+        return module;
+    imported_module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(imported_module)) {
+        Py_DECREF(module);
+        return imported_module;
+    }
+    PyErr_Clear();
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
+#endif
+}
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
+    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(module)) {
+        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
+        if (likely(spec)) {
+            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
+            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
+                Py_DECREF(spec);
+                spec = NULL;
+            }
+            Py_XDECREF(unsafe);
+        }
+        if (likely(!spec)) {
+            PyErr_Clear();
+            return module;
+        }
+        Py_DECREF(spec);
+        Py_DECREF(module);
+    } else if (PyErr_Occurred()) {
+        PyErr_Clear();
+    }
+#endif
+    return __Pyx__ImportDottedModule(name, parts_tuple);
+}
+
 /* Py3UpdateBases */
 static PyObject*
 __Pyx_PEP560_update_bases(PyObject *bases)
 {
     Py_ssize_t i, j, size_bases;
     PyObject *base, *meth, *new_base, *result, *new_bases = NULL;
     size_bases = PyTuple_GET_SIZE(bases);
@@ -10076,14 +9069,52 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
@@ -10349,52 +9380,14 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const size_t neg_one = (size_t) -1, const_zero = (size_t) 0;
@@ -10669,15 +9662,15 @@
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__11));
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__10));
     }
     return name;
 }
 #endif
 
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
```

### Comparing `lzokay-1.1.4/_lzokay.pyx` & `lzokay-1.1.5/_lzokay.pyx`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/lzokay_wrap.pxd` & `lzokay-1.1.5/lzokay_wrap.pxd`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from libc.stdint cimport uint8_t
 
 
 cdef extern from "lzokay.hpp" namespace "lzokay":
-    cpdef enum class EResult(int):
+    cdef enum class EResult(int):
         LookbehindOverrun,
         OutputOverrun,
         InputOverrun,
         Error,
         Success,
         InputNotConsumed,
```

### Comparing `lzokay-1.1.4/native/lzokay/CMakeLists.txt` & `lzokay-1.1.5/native/lzokay/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/native/lzokay/LICENSE` & `lzokay-1.1.5/native/lzokay/LICENSE`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/native/lzokay/README.md` & `lzokay-1.1.5/native/lzokay/README.md`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/native/lzokay/lzokay-c/lzokay-c.cpp` & `lzokay-1.1.5/native/lzokay/lzokay-c/lzokay-c.cpp`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/native/lzokay/lzokay-c/lzokay-c.h` & `lzokay-1.1.5/native/lzokay/lzokay-c/lzokay-c.h`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/native/lzokay/lzokay.cpp` & `lzokay-1.1.5/native/lzokay/lzokay.cpp`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/native/lzokay/lzokay.hpp` & `lzokay-1.1.5/native/lzokay/lzokay.hpp`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/native/lzokay/test.cpp` & `lzokay-1.1.5/native/lzokay/test.cpp`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/pyproject.toml` & `lzokay-1.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,18 @@
 [tool.setuptools_scm]
 version_scheme = "guess-next-dev"
 local_scheme = "no-local-version"
 write_to = "src/lzokay/version.py"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
+filterwarnings = [
+    "error",
+]
+xfail_strict = true
 
 [tool.ruff]
 line-length = 120
 select = [
     "E", "F", "W", "C90", "I", "UP", "C4",
     "RSE",
     "TCH",
```

### Comparing `lzokay-1.1.4/setup.py` & `lzokay-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `lzokay-1.1.4/src/lzokay.egg-info/PKG-INFO` & `lzokay-1.1.5/src/lzokay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lzokay
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python bindings for LZ👌, a LZO compression/decompression algorithm.
 Author: Henrique Gemignani
 Project-URL: Homepage, https://github.com/henriquegemignani/py-lzokay
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lzokay-1.1.4/src/lzokay.egg-info/SOURCES.txt` & `lzokay-1.1.5/src/lzokay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

