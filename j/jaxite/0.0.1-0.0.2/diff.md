# Comparing `tmp/jaxite-0.0.1.tar.gz` & `tmp/jaxite-0.0.2.tar.gz`

## Comparing `jaxite-0.0.1.tar` & `jaxite-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_bool/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_bool/bool_encoding.py
--rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_bool/bool_params.py
--rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_bool/jaxite_bool.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_bool/lut.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_bool/type_converters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_lib/__init__.py
--rw-r--r--   0        0        0    19262 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_lib/bootstrap.py
--rw-r--r--   0        0        0    12766 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_lib/decomposition.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_lib/encoding.py
--rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_lib/key_switch.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_lib/lwe.py
--rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_lib/matrix_utils.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_lib/parameters.py
--rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_lib/random_source.py
--rw-r--r--   0        0        0    11359 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_lib/rgsw.py
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_lib/rlwe.py
--rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_lib/test_polynomial.py
--rw-r--r--   0        0        0     9278 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_lib/test_utils.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jaxite-0.0.1/jaxite/jaxite_lib/types.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 jaxite-0.0.1/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jaxite-0.0.1/LICENSE
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 jaxite-0.0.1/README.md
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 jaxite-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 jaxite-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_bool/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_bool/bool_encoding.py
+-rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_bool/bool_params.py
+-rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_bool/jaxite_bool.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_bool/lut.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_bool/type_converters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_lib/__init__.py
+-rw-r--r--   0        0        0    19262 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_lib/bootstrap.py
+-rw-r--r--   0        0        0    12766 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_lib/decomposition.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_lib/encoding.py
+-rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_lib/key_switch.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_lib/lwe.py
+-rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_lib/matrix_utils.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_lib/parameters.py
+-rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_lib/random_source.py
+-rw-r--r--   0        0        0    11359 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_lib/rgsw.py
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_lib/rlwe.py
+-rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_lib/test_polynomial.py
+-rw-r--r--   0        0        0     9278 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_lib/test_utils.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jaxite-0.0.2/jaxite/jaxite_lib/types.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 jaxite-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jaxite-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 jaxite-0.0.2/README.md
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 jaxite-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 jaxite-0.0.2/PKG-INFO
```

### Comparing `jaxite-0.0.1/jaxite/jaxite_bool/bool_encoding.py` & `jaxite-0.0.2/jaxite/jaxite_bool/bool_encoding.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_bool/bool_params.py` & `jaxite-0.0.2/jaxite/jaxite_bool/bool_params.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_bool/jaxite_bool.py` & `jaxite-0.0.2/jaxite/jaxite_bool/jaxite_bool.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_bool/lut.py` & `jaxite-0.0.2/jaxite/jaxite_bool/lut.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_bool/type_converters.py` & `jaxite-0.0.2/jaxite/jaxite_bool/type_converters.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_lib/bootstrap.py` & `jaxite-0.0.2/jaxite/jaxite_lib/bootstrap.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_lib/decomposition.py` & `jaxite-0.0.2/jaxite/jaxite_lib/decomposition.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_lib/encoding.py` & `jaxite-0.0.2/jaxite/jaxite_lib/encoding.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_lib/key_switch.py` & `jaxite-0.0.2/jaxite/jaxite_lib/key_switch.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_lib/lwe.py` & `jaxite-0.0.2/jaxite/jaxite_lib/lwe.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_lib/matrix_utils.py` & `jaxite-0.0.2/jaxite/jaxite_lib/matrix_utils.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_lib/parameters.py` & `jaxite-0.0.2/jaxite/jaxite_lib/parameters.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_lib/random_source.py` & `jaxite-0.0.2/jaxite/jaxite_lib/random_source.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_lib/rgsw.py` & `jaxite-0.0.2/jaxite/jaxite_lib/rgsw.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_lib/rlwe.py` & `jaxite-0.0.2/jaxite/jaxite_lib/rlwe.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_lib/test_polynomial.py` & `jaxite-0.0.2/jaxite/jaxite_lib/test_polynomial.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/jaxite/jaxite_lib/test_utils.py` & `jaxite-0.0.2/jaxite/jaxite_lib/test_utils.py`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/LICENSE` & `jaxite-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/README.md` & `jaxite-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jaxite-0.0.1/pyproject.toml` & `jaxite-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jaxite"
-version = "0.0.1"
+version = "0.0.2"
 description = 'A Homomorphic Encryption implementation (CGGI) written in JAX'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Asra Ali" },
@@ -24,25 +24,24 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "jax==0.4.13",
-  "jaxlib==0.4.13",
-  "numpy==1.25.1",
+  "jax~=0.4.13",
+  "jaxlib~=0.4.13",
 ]
 
 [project.urls]
 Documentation = "https://github.com/google/jaxite"
 Issues = "https://github.com/google/jaxite/issues"
 Source = "https://github.com/google/jaxite"
 
 [tool.hatch.build]
 include = [
   "jaxite/**/*.py",
 ]
 exclude = [
   "jaxite/**/*_test.py",
   "jaxite/**/test_util.py",
-]
+]
```

### Comparing `jaxite-0.0.1/PKG-INFO` & `jaxite-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxite
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Homomorphic Encryption implementation (CGGI) written in JAX
 Project-URL: Documentation, https://github.com/google/jaxite
 Project-URL: Issues, https://github.com/google/jaxite/issues
 Project-URL: Source, https://github.com/google/jaxite
 Author: Asra Ali, Cathie Yun, Jeremy Kun, Shruthi Gorantala
 License-Expression: MIT
 License-File: LICENSE
@@ -14,17 +14,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Requires-Dist: jax==0.4.13
-Requires-Dist: jaxlib==0.4.13
-Requires-Dist: numpy==1.25.1
+Requires-Dist: jaxlib~=0.4.13
+Requires-Dist: jax~=0.4.13
 Description-Content-Type: text/markdown
 
 # Jaxite
 
 Jaxite is a fully homomorphic encryption backend targeting TPUs and GPUs,
 written in [JAX](https://github.com/google/jax).
```

