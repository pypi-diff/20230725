# Comparing `tmp/cudagrad-0.0.20.tar.gz` & `tmp/cudagrad-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudagrad-0.0.20.tar", last modified: Tue Jul 18 06:48:24 2023, max compression
+gzip compressed data, was "cudagrad-0.0.22.tar", last modified: Mon Jul 24 23:20:33 2023, max compression
```

## Comparing `cudagrad-0.0.20.tar` & `cudagrad-0.0.22.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-18 06:48:24.911379 cudagrad-0.0.20/
--rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-18 06:47:23.000000 cudagrad-0.0.20/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3615 2023-07-18 06:48:24.911257 cudagrad-0.0.20/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     3113 2023-07-18 03:03:04.000000 cudagrad-0.0.20/README.md
--rw-r--r--   0 ryan       (501) staff       (20)      724 2023-07-18 06:47:35.000000 cudagrad-0.0.20/pyproject.toml
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-18 06:48:24.911420 cudagrad-0.0.20/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     1592 2023-07-18 02:40:23.000000 cudagrad-0.0.20/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-18 06:48:24.909853 cudagrad-0.0.20/src/
--rw-r--r--   0 ryan       (501) staff       (20)     3414 2023-07-18 06:13:07.000000 cudagrad-0.0.20/src/bindings.cpp
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-18 06:48:24.910767 cudagrad-0.0.20/src/cudagrad.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3615 2023-07-18 06:48:24.000000 cudagrad-0.0.20/src/cudagrad.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      318 2023-07-18 06:48:24.000000 cudagrad-0.0.20/src/cudagrad.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-18 06:48:24.000000 cudagrad-0.0.20/src/cudagrad.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-18 02:46:33.000000 cudagrad-0.0.20/src/cudagrad.egg-info/not-zip-safe
--rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-18 06:48:24.000000 cudagrad-0.0.20/src/cudagrad.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-18 06:48:24.000000 cudagrad-0.0.20/src/cudagrad.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)    23491 2023-07-18 06:45:54.000000 cudagrad-0.0.20/src/cudagrad.hpp
--rw-r--r--   0 ryan       (501) staff       (20)      171 2023-07-18 06:46:23.000000 cudagrad-0.0.20/src/ops.cu
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-18 06:48:24.910937 cudagrad-0.0.20/tests/
--rw-r--r--   0 ryan       (501) staff       (20)     1046 2023-07-18 02:40:23.000000 cudagrad-0.0.20/tests/test.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:20:33.060223 cudagrad-0.0.22/
+-rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-18 06:47:23.000000 cudagrad-0.0.22/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3619 2023-07-24 23:20:33.060103 cudagrad-0.0.22/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     3117 2023-07-19 01:34:52.000000 cudagrad-0.0.22/README.md
+-rw-r--r--   0 ryan       (501) staff       (20)      724 2023-07-24 23:10:08.000000 cudagrad-0.0.22/pyproject.toml
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-24 23:20:33.060257 cudagrad-0.0.22/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     1592 2023-07-18 02:40:23.000000 cudagrad-0.0.22/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:20:33.058239 cudagrad-0.0.22/src/
+-rw-r--r--   0 ryan       (501) staff       (20)     3857 2023-07-24 23:18:51.000000 cudagrad-0.0.22/src/bindings.cpp
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:20:33.059698 cudagrad-0.0.22/src/cudagrad.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3619 2023-07-24 23:20:33.000000 cudagrad-0.0.22/src/cudagrad.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      318 2023-07-24 23:20:33.000000 cudagrad-0.0.22/src/cudagrad.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-24 23:20:33.000000 cudagrad-0.0.22/src/cudagrad.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-18 02:46:33.000000 cudagrad-0.0.22/src/cudagrad.egg-info/not-zip-safe
+-rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-24 23:20:33.000000 cudagrad-0.0.22/src/cudagrad.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-24 23:20:33.000000 cudagrad-0.0.22/src/cudagrad.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)    23491 2023-07-18 06:45:54.000000 cudagrad-0.0.22/src/cudagrad.hpp
+-rw-r--r--   0 ryan       (501) staff       (20)      171 2023-07-18 06:46:23.000000 cudagrad-0.0.22/src/ops.cu
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:20:33.059829 cudagrad-0.0.22/tests/
+-rw-r--r--   0 ryan       (501) staff       (20)     1050 2023-07-19 01:21:03.000000 cudagrad-0.0.22/tests/test.py
```

### Comparing `cudagrad-0.0.20/PKG-INFO` & `cudagrad-0.0.22/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.20
+Version: 0.0.22
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <moorethreads@hey.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
@@ -40,15 +40,15 @@
   for (auto& x : b.get()->grad_) {cout<<x<<" ";} // 66 66 88 88
 }
 ```
 
 Available on [PyPI](https://pypi.org/project/cudagrad/), use `pip install cudagrad` to get the Python bindings
 
 ```py
-# pip install cudagrad; py ./examples/example.py
+# pip install cudagrad; python ./examples/example.py
 import cudagrad as cg
 
 a = cg.tensor([2, 2], [2.0, 3.0, 4.0, 5.0])
 b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
 c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
 d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
 e = ((a @ b) + c) * d
```

### Comparing `cudagrad-0.0.20/README.md` & `cudagrad-0.0.22/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   for (auto& x : b.get()->grad_) {cout<<x<<" ";} // 66 66 88 88
 }
 ```
 
 Available on [PyPI](https://pypi.org/project/cudagrad/), use `pip install cudagrad` to get the Python bindings
 
 ```py
-# pip install cudagrad; py ./examples/example.py
+# pip install cudagrad; python ./examples/example.py
 import cudagrad as cg
 
 a = cg.tensor([2, 2], [2.0, 3.0, 4.0, 5.0])
 b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
 c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
 d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
 e = ((a @ b) + c) * d
```

### Comparing `cudagrad-0.0.20/pyproject.toml` & `cudagrad-0.0.22/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=40.8.0", "wheel", "pybind11>=2.10.1", "toml",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cudagrad"
-version = "0.0.20"
+version = "0.0.22"
 description = "A small autograd engine"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
 dependencies = [ "micrograd",]
 [[project.authors]]
 name = "Ryan Moore"
```

### Comparing `cudagrad-0.0.20/setup.py` & `cudagrad-0.0.22/setup.py`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.20/src/bindings.cpp` & `cudagrad-0.0.22/src/bindings.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#include <sstream>
 #include "cudagrad.hpp"
 
 #include <pybind11/stl.h>
 #include <pybind11/pybind11.h>
 
 #define STRINGIFY(x) #x
 #define MACRO_STRINGIFY(x) STRINGIFY(x)
@@ -53,14 +54,16 @@
     m.def("tensor", [](std::vector<int> sizes, std::vector<float> values) {
         // cast the function pointer to resolve the ambiguity
         auto func = static_cast<std::shared_ptr<cg::Tensor> (*)(std::vector<int>, std::vector<float>)>(&cg::tensor);
         return func(sizes, values);
     }, R"pbdoc(Magic tensor)pbdoc",
     py::arg("sizes"), py::arg("values"));
 
+    // TODO(yrom1): When doing C++ bindings does repr
+    //              override str when no str present?
     py::class_<cg::Tensor, std::shared_ptr<cg::Tensor>>(m, "Tensor")
         .def(py::init<std::vector<int>, std::vector<float>>())
         .def("get_shared", &cg::Tensor::get_shared)
         .def("backward", &cg::Tensor::backward)
         .def("zero_grad", &cg::Tensor::zero_grad)
         .def("sum", &cg::Tensor::sum)
         .def("matmul", &cg::matmul)
@@ -72,17 +75,27 @@
         .def_static("zeros", &cg::Tensor::zeros)
         .def_static("explode", &cg::Tensor::explode)
         .def_static("rand", &cg::Tensor::rand)
         .def("__add__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return a + b; })
         .def("__sub__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return a - b; })
         .def("__mul__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return a * b; })
         .def("__truediv__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return a / b; })
-        .def("__matmul__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return cg::matmul(a, b); });
+        .def("__matmul__", [](std::shared_ptr<cg::Tensor> a, std::shared_ptr<cg::Tensor> b) { return cg::matmul(a, b); })
+        .def("__str__", [](std::shared_ptr<cg::Tensor> t) {
+            std::ostringstream os;
+            os << t;
+            return os.str();
+        })
+        .def("__repr__", [](std::shared_ptr<cg::Tensor> t) {
+            std::ostringstream os;
+            os << t;
+            return os.str();
+        });
 
-    // Add the stream output operator if you want to print your Tensor object in Python.
+    // // Add the stream output operator if you want to print your Tensor object in Python.
     // py::class_<std::ostream>(m, "ostream")
     //     .def(py::self_ns::str(py::self_ns::self))
     //     .def(py::self_ns::repr(py::self_ns::self));
 
     // m.def("__lshift__", [](std::ostream &os, const std::shared_ptr<cg::Tensor> &t) -> std::ostream& {
     //     os << t; return os;
     // }, py::is_operator());
```

### Comparing `cudagrad-0.0.20/src/cudagrad.egg-info/PKG-INFO` & `cudagrad-0.0.22/src/cudagrad.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.20
+Version: 0.0.22
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <moorethreads@hey.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
@@ -40,15 +40,15 @@
   for (auto& x : b.get()->grad_) {cout<<x<<" ";} // 66 66 88 88
 }
 ```
 
 Available on [PyPI](https://pypi.org/project/cudagrad/), use `pip install cudagrad` to get the Python bindings
 
 ```py
-# pip install cudagrad; py ./examples/example.py
+# pip install cudagrad; python ./examples/example.py
 import cudagrad as cg
 
 a = cg.tensor([2, 2], [2.0, 3.0, 4.0, 5.0])
 b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
 c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
 d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
 e = ((a @ b) + c) * d
```

### Comparing `cudagrad-0.0.20/src/cudagrad.hpp` & `cudagrad-0.0.22/src/cudagrad.hpp`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.20/tests/test.py` & `cudagrad-0.0.22/tests/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# py tests/test.py
+# python tests/test.py
 
 import cudagrad as cg
 import torch
 
 # assert cg.__version__ == '0.0.1'
 assert cg.add(1, 2) == 3
 assert cg.subtract(1, 2) == -1
```

