# Comparing `tmp/dispersenn2-0.0.1.tar.gz` & `tmp/dispersenn2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dispersenn2-0.0.1.tar", max compression
+gzip compressed data, was "dispersenn2-0.0.2.tar", max compression
```

## Comparing `dispersenn2-0.0.1.tar` & `dispersenn2-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      366 2023-07-25 00:18:01.284112 dispersenn2-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-25 00:18:01.284112 dispersenn2-0.0.1/dispersenn2/__init__.py
--rw-r--r--   0        0        0     2129 2023-07-25 00:18:01.284112 dispersenn2-0.0.1/dispersenn2/check_params.py
--rw-r--r--   0        0        0    13167 2023-07-25 00:18:01.284112 dispersenn2-0.0.1/dispersenn2/data_generation.py
--rw-r--r--   0        0        0    23908 2023-07-25 00:18:01.284112 dispersenn2-0.0.1/dispersenn2/disperseNN2.py
--rw-r--r--   0        0        0     7097 2023-07-25 00:18:01.284112 dispersenn2-0.0.1/dispersenn2/process_input.py
--rw-r--r--   0        0        0     3824 2023-07-25 00:18:01.284112 dispersenn2-0.0.1/dispersenn2/read_input.py
--rw-r--r--   0        0        0      554 2023-07-25 18:22:53.482874 dispersenn2-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 dispersenn2-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      366 2023-07-25 00:18:01.284112 dispersenn2-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-25 00:18:01.284112 dispersenn2-0.0.2/dispersenn2/__init__.py
+-rw-r--r--   0        0        0     2129 2023-07-25 00:18:01.284112 dispersenn2-0.0.2/dispersenn2/check_params.py
+-rw-r--r--   0        0        0    13167 2023-07-25 00:18:01.284112 dispersenn2-0.0.2/dispersenn2/data_generation.py
+-rw-r--r--   0        0        0    23908 2023-07-25 00:18:01.284112 dispersenn2-0.0.2/dispersenn2/disperseNN2.py
+-rw-r--r--   0        0        0     7097 2023-07-25 00:18:01.284112 dispersenn2-0.0.2/dispersenn2/process_input.py
+-rw-r--r--   0        0        0     3824 2023-07-25 00:18:01.284112 dispersenn2-0.0.2/dispersenn2/read_input.py
+-rw-r--r--   0        0        0      575 2023-07-25 20:39:09.049643 dispersenn2-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 dispersenn2-0.0.2/PKG-INFO
```

### Comparing `dispersenn2-0.0.1/dispersenn2/check_params.py` & `dispersenn2-0.0.2/dispersenn2/check_params.py`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.1/dispersenn2/data_generation.py` & `dispersenn2-0.0.2/dispersenn2/data_generation.py`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.1/dispersenn2/disperseNN2.py` & `dispersenn2-0.0.2/dispersenn2/disperseNN2.py`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.1/dispersenn2/process_input.py` & `dispersenn2-0.0.2/dispersenn2/process_input.py`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.1/dispersenn2/read_input.py` & `dispersenn2-0.0.2/dispersenn2/read_input.py`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.1/pyproject.toml` & `dispersenn2-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "disperseNN2"
-version = "0.0.1"
+version = "0.0.2"
 description = "Neural net for estimating dispersal distance"
 authors = ["chriscrsmith <chriscs@uoregon.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 gpustat = "^1.1"
@@ -12,14 +12,15 @@
 geopy = "^2.3.0"
 attrs = "^23.1.0"
 scikit-learn = "^1.3.0"
 msprime = "^1.2.0"
 tskit = "^0.5.5"
 utm = "^0.7.0"
 matplotlib = "^3.7.2"
+tensorflow = "^2.11"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 disperseNN2 = 'dispersenn2.disperseNN2:run'
```

### Comparing `dispersenn2-0.0.1/PKG-INFO` & `dispersenn2-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dispersenn2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Neural net for estimating dispersal distance
 Author: chriscrsmith
 Author-email: chriscs@uoregon.edu
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,14 +12,15 @@
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: geopy (>=2.3.0,<3.0.0)
 Requires-Dist: gpustat (>=1.1,<2.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: msprime (>=1.2.0,<2.0.0)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
+Requires-Dist: tensorflow (>=2.11,<3.0)
 Requires-Dist: tskit (>=0.5.5,<0.6.0)
 Requires-Dist: utm (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # disperseNN2
 
 [![Documentation Status](https://readthedocs.org/projects/dispersenn2/badge/?version=latest)](https://dispersenn2.readthedocs.io/en/latest/?badge=latest)
```

