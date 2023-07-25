# Comparing `tmp/bojaxns-1.0.3.tar.gz` & `tmp/bojaxns-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bojaxns-1.0.3.tar", last modified: Tue Jul 25 15:41:28 2023, max compression
+gzip compressed data, was "bojaxns-1.0.4.tar", last modified: Tue Jul 25 17:11:43 2023, max compression
```

## Comparing `bojaxns-1.0.3.tar` & `bojaxns-1.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 15:41:28.111423 bojaxns-1.0.3/
--rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-07-21 00:04:16.000000 bojaxns-1.0.3/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     2259 2023-07-25 15:41:28.111423 bojaxns-1.0.3/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     1806 2023-07-23 14:37:43.000000 bojaxns-1.0.3/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 15:41:28.111423 bojaxns-1.0.3/bojaxns/
--rw-rw-r--   0 albert    (1000) albert    (1000)      199 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5038 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/base.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2005 2023-07-21 12:38:12.000000 bojaxns-1.0.3/bojaxns/basic.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3282 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/experiment.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 15:41:28.111423 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/
--rw-rw-r--   0 albert    (1000) albert    (1000)       70 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    11415 2023-07-25 15:21:05.000000 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/bayesian_optimiser.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    15665 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/distribution_math.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9088 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/multi_step_lookahead.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 15:41:28.111423 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5288 2023-07-25 15:21:05.000000 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5939 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5069 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/parameter_space.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9505 2023-07-23 14:22:31.000000 bojaxns-1.0.3/bojaxns/service.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 15:41:28.111423 bojaxns-1.0.3/bojaxns/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2181 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/tests/test_experiment.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3508 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/tests/test_parameter_space.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      622 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/tests/test_utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2986 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 15:41:28.111423 bojaxns-1.0.3/bojaxns.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     2259 2023-07-25 15:41:28.000000 bojaxns-1.0.3/bojaxns.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      894 2023-07-25 15:41:28.000000 bojaxns-1.0.3/bojaxns.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-25 15:41:28.000000 bojaxns-1.0.3/bojaxns.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        8 2023-07-25 15:41:28.000000 bojaxns-1.0.3/bojaxns.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-07-21 00:04:16.000000 bojaxns-1.0.3/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-07-25 15:41:28.111423 bojaxns-1.0.3/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      961 2023-07-25 15:21:05.000000 bojaxns-1.0.3/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 17:11:43.346069 bojaxns-1.0.4/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-07-21 00:04:16.000000 bojaxns-1.0.4/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2259 2023-07-25 17:11:43.346069 bojaxns-1.0.4/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1806 2023-07-23 14:37:43.000000 bojaxns-1.0.4/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 17:11:43.342069 bojaxns-1.0.4/bojaxns/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      199 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5038 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/base.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2005 2023-07-21 12:38:12.000000 bojaxns-1.0.4/bojaxns/basic.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3282 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/experiment.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 17:11:43.342069 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/
+-rw-rw-r--   0 albert    (1000) albert    (1000)       70 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    11415 2023-07-25 15:21:05.000000 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/bayesian_optimiser.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15709 2023-07-25 17:10:14.000000 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/distribution_math.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9088 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/multi_step_lookahead.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 17:11:43.342069 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5288 2023-07-25 15:21:05.000000 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5939 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5069 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/parameter_space.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9505 2023-07-25 17:10:14.000000 bojaxns-1.0.4/bojaxns/service.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 17:11:43.342069 bojaxns-1.0.4/bojaxns/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2181 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/tests/test_experiment.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3508 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/tests/test_parameter_space.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      622 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/tests/test_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2986 2023-07-21 00:04:16.000000 bojaxns-1.0.4/bojaxns/utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 17:11:43.342069 bojaxns-1.0.4/bojaxns.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2259 2023-07-25 17:11:43.000000 bojaxns-1.0.4/bojaxns.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      894 2023-07-25 17:11:43.000000 bojaxns-1.0.4/bojaxns.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-25 17:11:43.000000 bojaxns-1.0.4/bojaxns.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        8 2023-07-25 17:11:43.000000 bojaxns-1.0.4/bojaxns.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-07-21 00:04:16.000000 bojaxns-1.0.4/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-07-25 17:11:43.346069 bojaxns-1.0.4/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      961 2023-07-25 17:11:12.000000 bojaxns-1.0.4/setup.py
```

### Comparing `bojaxns-1.0.3/LICENSE` & `bojaxns-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/PKG-INFO` & `bojaxns-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bojaxns
-Version: 1.0.3
+Version: 1.0.4
 Summary: Bayesian Optimisation with JAXNS
 Home-page: https://github.com/joshuaalbert/bojaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bojaxns-1.0.3/README.md` & `bojaxns-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/bojaxns/base.py` & `bojaxns-1.0.4/bojaxns/base.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/bojaxns/basic.py` & `bojaxns-1.0.4/bojaxns/basic.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/bojaxns/experiment.py` & `bojaxns-1.0.4/bojaxns/experiment.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/bojaxns/gaussian_process_formulation/bayesian_optimiser.py` & `bojaxns-1.0.4/bojaxns/gaussian_process_formulation/bayesian_optimiser.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/bojaxns/gaussian_process_formulation/distribution_math.py` & `bojaxns-1.0.4/bojaxns/gaussian_process_formulation/distribution_math.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,22 +54,24 @@
 
 class GaussianProcessData(NamedTuple):
     U: jnp.ndarray
     Y: jnp.ndarray
     Y_var: jnp.ndarray
     sample_size: jnp.ndarray
 
+class NotEnoughData(Exception):
+    pass
 
 def _ensure_gaussian_process_data(data: GaussianProcessData) -> GaussianProcessData:
     data = tree_map(lambda x: jnp.asarray(x, float_type), data)
     _assert_rank(2, U=data.U)
     _assert_rank(1, sample_size=data.sample_size, Y=data.Y, Y_var=data.Y_var)
     _assert_same_leading_dim(*data)
     if data.Y.size < 2:
-        raise ValueError('Need more samples to form mean and variance of data.')
+        raise NotEnoughData('Need more samples to form mean and variance of data.')
     return data
 
 
 class GaussianProcessConditionalPredictive(ConditionalPredictive):
     def __init__(self,
                  data: GaussianProcessData,
                  kernel: tfp.math.psd_kernels.PositiveSemidefiniteKernel,
```

### Comparing `bojaxns-1.0.3/bojaxns/gaussian_process_formulation/multi_step_lookahead.py` & `bojaxns-1.0.4/bojaxns/gaussian_process_formulation/multi_step_lookahead.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py` & `bojaxns-1.0.4/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py` & `bojaxns-1.0.4/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/bojaxns/parameter_space.py` & `bojaxns-1.0.4/bojaxns/parameter_space.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/bojaxns/service.py` & `bojaxns-1.0.4/bojaxns/service.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/bojaxns/tests/test_experiment.py` & `bojaxns-1.0.4/bojaxns/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/bojaxns/tests/test_parameter_space.py` & `bojaxns-1.0.4/bojaxns/tests/test_parameter_space.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/bojaxns/tests/test_utils.py` & `bojaxns-1.0.4/bojaxns/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/bojaxns/utils.py` & `bojaxns-1.0.4/bojaxns/utils.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/bojaxns.egg-info/PKG-INFO` & `bojaxns-1.0.4/bojaxns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bojaxns
-Version: 1.0.3
+Version: 1.0.4
 Summary: Bayesian Optimisation with JAXNS
 Home-page: https://github.com/joshuaalbert/bojaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bojaxns-1.0.3/bojaxns.egg-info/SOURCES.txt` & `bojaxns-1.0.4/bojaxns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.3/setup.py` & `bojaxns-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     'pydantic'
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='bojaxns',
-      version='1.0.3',
+      version='1.0.4',
       description='Bayesian Optimisation with JAXNS',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/bojaxns",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
```

