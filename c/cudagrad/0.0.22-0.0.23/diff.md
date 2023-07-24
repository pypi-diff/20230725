# Comparing `tmp/cudagrad-0.0.22.tar.gz` & `tmp/cudagrad-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudagrad-0.0.22.tar", last modified: Mon Jul 24 23:20:33 2023, max compression
+gzip compressed data, was "cudagrad-0.0.23.tar", last modified: Mon Jul 24 23:48:40 2023, max compression
```

## Comparing `cudagrad-0.0.22.tar` & `cudagrad-0.0.23.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:20:33.060223 cudagrad-0.0.22/
--rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-18 06:47:23.000000 cudagrad-0.0.22/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3619 2023-07-24 23:20:33.060103 cudagrad-0.0.22/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     3117 2023-07-19 01:34:52.000000 cudagrad-0.0.22/README.md
--rw-r--r--   0 ryan       (501) staff       (20)      724 2023-07-24 23:10:08.000000 cudagrad-0.0.22/pyproject.toml
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-24 23:20:33.060257 cudagrad-0.0.22/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     1592 2023-07-18 02:40:23.000000 cudagrad-0.0.22/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:20:33.058239 cudagrad-0.0.22/src/
--rw-r--r--   0 ryan       (501) staff       (20)     3857 2023-07-24 23:18:51.000000 cudagrad-0.0.22/src/bindings.cpp
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:20:33.059698 cudagrad-0.0.22/src/cudagrad.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3619 2023-07-24 23:20:33.000000 cudagrad-0.0.22/src/cudagrad.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      318 2023-07-24 23:20:33.000000 cudagrad-0.0.22/src/cudagrad.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-24 23:20:33.000000 cudagrad-0.0.22/src/cudagrad.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-18 02:46:33.000000 cudagrad-0.0.22/src/cudagrad.egg-info/not-zip-safe
--rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-24 23:20:33.000000 cudagrad-0.0.22/src/cudagrad.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-24 23:20:33.000000 cudagrad-0.0.22/src/cudagrad.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)    23491 2023-07-18 06:45:54.000000 cudagrad-0.0.22/src/cudagrad.hpp
--rw-r--r--   0 ryan       (501) staff       (20)      171 2023-07-18 06:46:23.000000 cudagrad-0.0.22/src/ops.cu
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:20:33.059829 cudagrad-0.0.22/tests/
--rw-r--r--   0 ryan       (501) staff       (20)     1050 2023-07-19 01:21:03.000000 cudagrad-0.0.22/tests/test.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:48:40.841282 cudagrad-0.0.23/
+-rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-18 06:47:23.000000 cudagrad-0.0.23/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3619 2023-07-24 23:48:40.841146 cudagrad-0.0.23/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     3117 2023-07-19 01:34:52.000000 cudagrad-0.0.23/README.md
+-rw-r--r--   0 ryan       (501) staff       (20)      724 2023-07-24 23:47:25.000000 cudagrad-0.0.23/pyproject.toml
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-24 23:48:40.841332 cudagrad-0.0.23/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     1592 2023-07-18 02:40:23.000000 cudagrad-0.0.23/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:48:40.839745 cudagrad-0.0.23/src/
+-rw-r--r--   0 ryan       (501) staff       (20)     3857 2023-07-24 23:43:55.000000 cudagrad-0.0.23/src/bindings.cpp
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:48:40.840749 cudagrad-0.0.23/src/cudagrad.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3619 2023-07-24 23:48:40.000000 cudagrad-0.0.23/src/cudagrad.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      318 2023-07-24 23:48:40.000000 cudagrad-0.0.23/src/cudagrad.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-24 23:48:40.000000 cudagrad-0.0.23/src/cudagrad.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-18 02:46:33.000000 cudagrad-0.0.23/src/cudagrad.egg-info/not-zip-safe
+-rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-24 23:48:40.000000 cudagrad-0.0.23/src/cudagrad.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-24 23:48:40.000000 cudagrad-0.0.23/src/cudagrad.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)    23588 2023-07-24 23:47:23.000000 cudagrad-0.0.23/src/cudagrad.hpp
+-rw-r--r--   0 ryan       (501) staff       (20)      171 2023-07-18 06:46:23.000000 cudagrad-0.0.23/src/ops.cu
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:48:40.840868 cudagrad-0.0.23/tests/
+-rw-r--r--   0 ryan       (501) staff       (20)     1050 2023-07-19 01:21:03.000000 cudagrad-0.0.23/tests/test.py
```

### Comparing `cudagrad-0.0.22/PKG-INFO` & `cudagrad-0.0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.22
+Version: 0.0.23
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <moorethreads@hey.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cudagrad-0.0.22/README.md` & `cudagrad-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.22/pyproject.toml` & `cudagrad-0.0.23/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=40.8.0", "wheel", "pybind11>=2.10.1", "toml",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cudagrad"
-version = "0.0.22"
+version = "0.0.23"
 description = "A small autograd engine"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
 dependencies = [ "micrograd",]
 [[project.authors]]
 name = "Ryan Moore"
```

### Comparing `cudagrad-0.0.22/setup.py` & `cudagrad-0.0.23/setup.py`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.22/src/bindings.cpp` & `cudagrad-0.0.23/src/bindings.cpp`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.22/src/cudagrad.egg-info/PKG-INFO` & `cudagrad-0.0.23/src/cudagrad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.22
+Version: 0.0.23
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <moorethreads@hey.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cudagrad-0.0.22/src/cudagrad.hpp` & `cudagrad-0.0.23/src/cudagrad.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -142,24 +142,29 @@
 
   std::vector<int> get_size() const { return size_; }
 
   std::vector<float> get_data() const { return data_; }
 
   std::vector<float> get_grad() const { return grad_; }
 
-  void graph(int depth = 0) {
+  void graph() {
+    // this is to compensate for no default args pybind11
+    _graph(0);
+  }
+
+  void _graph(int depth = 0) {
     auto print_if_not_leaf = [this](char c) -> const char {
       if (c != '?') return c;
       return ' ';
     };
     std::string tab(depth, ' ');
     char displayed_op = print_if_not_leaf(op_);
     std::cout << tab << this << " " << displayed_op << std::endl;
     for (auto c : children_) {
-      c.get()->graph(depth + 2);
+      c.get()->_graph(depth + 2);
     }
   }
 
   float &data(const std::vector<size_t> &indices) {
     // checkIndicesBounds(indices);
 
     size_t idx = offset_;
```

### Comparing `cudagrad-0.0.22/tests/test.py` & `cudagrad-0.0.23/tests/test.py`

 * *Files identical despite different names*

