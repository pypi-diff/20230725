# Comparing `tmp/flimsay-0.2.0.tar.gz` & `tmp/flimsay-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flimsay-0.2.0.tar", last modified: Fri Jul 21 13:36:28 2023, max compression
+gzip compressed data, was "flimsay-0.4.0.tar", last modified: Tue Jul 25 21:18:15 2023, max compression
```

## Comparing `flimsay-0.2.0.tar` & `flimsay-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:36:28.176071 flimsay-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-21 13:36:28.176071 flimsay-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-07-21 13:36:19.000000 flimsay-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:36:28.172071 flimsay-0.2.0/flimsay/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/blib.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/mass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-21 13:31:28.000000 flimsay-0.2.0/flimsay/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:36:28.176071 flimsay-0.2.0/flimsay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-21 13:36:28.000000 flimsay-0.2.0/flimsay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-21 13:36:28.000000 flimsay-0.2.0/flimsay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:36:28.000000 flimsay-0.2.0/flimsay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 13:36:28.000000 flimsay-0.2.0/flimsay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-21 13:36:28.000000 flimsay-0.2.0/flimsay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 13:36:28.000000 flimsay-0.2.0/flimsay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-21 13:31:28.000000 flimsay-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:36:28.176071 flimsay-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:18:15.179916 flimsay-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-25 21:18:15.179916 flimsay-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-07-25 21:18:08.000000 flimsay-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:18:15.175917 flimsay-0.4.0/flimsay/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-25 21:13:56.000000 flimsay-0.4.0/flimsay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-25 21:13:56.000000 flimsay-0.4.0/flimsay/blib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-25 21:13:56.000000 flimsay-0.4.0/flimsay/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-25 21:13:56.000000 flimsay-0.4.0/flimsay/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-07-25 21:13:56.000000 flimsay-0.4.0/flimsay/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-07-25 21:13:56.000000 flimsay-0.4.0/flimsay/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-25 21:13:56.000000 flimsay-0.4.0/flimsay/mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-25 21:13:56.000000 flimsay-0.4.0/flimsay/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:18:15.179916 flimsay-0.4.0/flimsay/weights/
+-rw-r--r--   0 runner    (1001) docker     (123)  1750627 2023-07-25 21:13:56.000000 flimsay-0.4.0/flimsay/weights/ccs_model.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2534003 2023-07-25 21:13:56.000000 flimsay-0.4.0/flimsay/weights/one_over_k0_model.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:18:15.175917 flimsay-0.4.0/flimsay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-25 21:18:15.000000 flimsay-0.4.0/flimsay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-25 21:18:15.000000 flimsay-0.4.0/flimsay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:18:15.000000 flimsay-0.4.0/flimsay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 21:18:15.000000 flimsay-0.4.0/flimsay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-25 21:18:15.000000 flimsay-0.4.0/flimsay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 21:18:15.000000 flimsay-0.4.0/flimsay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-25 21:13:56.000000 flimsay-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:18:15.179916 flimsay-0.4.0/setup.cfg
```

### Comparing `flimsay-0.2.0/PKG-INFO` & `flimsay-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flimsay
-Version: 0.2.0
+Version: 0.4.0
 Summary: A super simple fast IMS predictor
 Author-email: Sebastian Paez <spaez@talus.bio>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/TalusBio/flimsay
 Project-URL: Documentation, https://TalusBio.github.io/flimsay
 Keywords: proteomics,dia,ion mobility
 Classifier: Programming Language :: Python :: 3
@@ -14,18 +14,18 @@
 Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: plot
 Provides-Extra: build
 Provides-Extra: dev
 
-# Flimsy: Fun/Fast Simple IMS Anyone like You can use.
+# Flimsay: Fun/Fast Simple IMS Anyone like You can use.
 Sebastian Paez
 
-version = 0.2.0
+version = 0.4.0
 
 This repository implements a very simple LGBM model to predict ion
 mobility from peptides.
 
 ## Usage
 
 There are two main ways to interact with `flimsay`, one is using python
@@ -82,15 +82,15 @@
     stripped_sequence_name="Stripped_Seqs",
     calc_masses=True,
     default_charge=2,
 )
 df
 ```
 
-    2023-07-21 13:32:38.680 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
+    2023-07-25 21:14:45.792 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
 
 <div>
 <style scoped>
     .dataframe tbody tr th:only-of-type {
         vertical-align: middle;
     }
 &#10;    .dataframe tbody tr th {
@@ -132,15 +132,15 @@
 from flimsay.model import FlimsayModel
 
 model_instance = FlimsayModel()
 
 %timeit model_instance.predict_peptide("MYPEPTIDEK", charge=3)
 ```
 
-    263 µs ± 11.5 µs per loop (mean ± std. dev. of 7 runs, 1,000 loops each)
+    174 µs ± 942 ns per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
 
 In my laptop that takes 133 microseconds per peptide, or roughly 7,500
 peptides per second.
 
 #### Batch Prediction
 
 ``` python
@@ -167,15 +167,15 @@
 df = add_features(df, stripped_sequence_name="Stripped_Seqs")
 
 
 # Now we get to run the prediction!
 %timeit model_instance.predict(df)
 ```
 
-    23.8 s ± 72.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
+    20.6 s ± 76.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 
 In my system every million peptides is predicted in 8.86 seconds, that is  
 113,000 per second.
 
 ## Motivation
 
 There is a fair amount of data on CCS and ion mobility of peptides but
```

### Comparing `flimsay-0.2.0/README.md` & `flimsay-0.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Flimsy: Fun/Fast Simple IMS Anyone like You can use.
+# Flimsay: Fun/Fast Simple IMS Anyone like You can use.
 Sebastian Paez
 
-version = 0.2.0
+version = 0.4.0
 
 This repository implements a very simple LGBM model to predict ion
 mobility from peptides.
 
 ## Usage
 
 There are two main ways to interact with `flimsay`, one is using python
@@ -62,15 +62,15 @@
     stripped_sequence_name="Stripped_Seqs",
     calc_masses=True,
     default_charge=2,
 )
 df
 ```
 
-    2023-07-21 13:32:38.680 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
+    2023-07-25 21:14:45.792 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
 
 <div>
 <style scoped>
     .dataframe tbody tr th:only-of-type {
         vertical-align: middle;
     }
 &#10;    .dataframe tbody tr th {
@@ -112,15 +112,15 @@
 from flimsay.model import FlimsayModel
 
 model_instance = FlimsayModel()
 
 %timeit model_instance.predict_peptide("MYPEPTIDEK", charge=3)
 ```
 
-    263 µs ± 11.5 µs per loop (mean ± std. dev. of 7 runs, 1,000 loops each)
+    174 µs ± 942 ns per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
 
 In my laptop that takes 133 microseconds per peptide, or roughly 7,500
 peptides per second.
 
 #### Batch Prediction
 
 ``` python
@@ -147,15 +147,15 @@
 df = add_features(df, stripped_sequence_name="Stripped_Seqs")
 
 
 # Now we get to run the prediction!
 %timeit model_instance.predict(df)
 ```
 
-    23.8 s ± 72.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
+    20.6 s ± 76.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 
 In my system every million peptides is predicted in 8.86 seconds, that is  
 113,000 per second.
 
 ## Motivation
 
 There is a fair amount of data on CCS and ion mobility of peptides but
```

### Comparing `flimsay-0.2.0/flimsay/blib.py` & `flimsay-0.4.0/flimsay/blib.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.2.0/flimsay/constants.py` & `flimsay-0.4.0/flimsay/constants.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.2.0/flimsay/data.py` & `flimsay-0.4.0/flimsay/data.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.2.0/flimsay/features.py` & `flimsay-0.4.0/flimsay/features.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.2.0/flimsay/mass.py` & `flimsay-0.4.0/flimsay/mass.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.2.0/flimsay/model.py` & `flimsay-0.4.0/flimsay/model.py`

 * *Files identical despite different names*

### Comparing `flimsay-0.2.0/flimsay.egg-info/PKG-INFO` & `flimsay-0.4.0/flimsay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flimsay
-Version: 0.2.0
+Version: 0.4.0
 Summary: A super simple fast IMS predictor
 Author-email: Sebastian Paez <spaez@talus.bio>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/TalusBio/flimsay
 Project-URL: Documentation, https://TalusBio.github.io/flimsay
 Keywords: proteomics,dia,ion mobility
 Classifier: Programming Language :: Python :: 3
@@ -14,18 +14,18 @@
 Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: plot
 Provides-Extra: build
 Provides-Extra: dev
 
-# Flimsy: Fun/Fast Simple IMS Anyone like You can use.
+# Flimsay: Fun/Fast Simple IMS Anyone like You can use.
 Sebastian Paez
 
-version = 0.2.0
+version = 0.4.0
 
 This repository implements a very simple LGBM model to predict ion
 mobility from peptides.
 
 ## Usage
 
 There are two main ways to interact with `flimsay`, one is using python
@@ -82,15 +82,15 @@
     stripped_sequence_name="Stripped_Seqs",
     calc_masses=True,
     default_charge=2,
 )
 df
 ```
 
-    2023-07-21 13:32:38.680 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
+    2023-07-25 21:14:45.792 | WARNING  | flimsay.features:add_features:163 - Charge not provided, using default charge of 2
 
 <div>
 <style scoped>
     .dataframe tbody tr th:only-of-type {
         vertical-align: middle;
     }
 &#10;    .dataframe tbody tr th {
@@ -132,15 +132,15 @@
 from flimsay.model import FlimsayModel
 
 model_instance = FlimsayModel()
 
 %timeit model_instance.predict_peptide("MYPEPTIDEK", charge=3)
 ```
 
-    263 µs ± 11.5 µs per loop (mean ± std. dev. of 7 runs, 1,000 loops each)
+    174 µs ± 942 ns per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
 
 In my laptop that takes 133 microseconds per peptide, or roughly 7,500
 peptides per second.
 
 #### Batch Prediction
 
 ``` python
@@ -167,15 +167,15 @@
 df = add_features(df, stripped_sequence_name="Stripped_Seqs")
 
 
 # Now we get to run the prediction!
 %timeit model_instance.predict(df)
 ```
 
-    23.8 s ± 72.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
+    20.6 s ± 76.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 
 In my system every million peptides is predicted in 8.86 seconds, that is  
 113,000 per second.
 
 ## Motivation
 
 There is a fair amount of data on CCS and ion mobility of peptides but
```

### Comparing `flimsay-0.2.0/pyproject.toml` & `flimsay-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flimsay"
-version = "0.2.0"
+version = "0.4.0"
 authors = [
     {name = "Sebastian Paez", email = "spaez@talus.bio"},
 ]
 description = "A super simple fast IMS predictor"
 requires-python = ">=3.9,<3.12"
 keywords = ["proteomics", "dia", "ion mobility"]
 license = {text = "Apache 2.0"}
@@ -61,19 +61,20 @@
     "black >= 23.1.0",
     "isort >=  5.12.0",
     "pylance >= 0.3.9",
     "jupyter >= 1.0.0",
     "pip-tools >= 7.0.0"
 ]
 
-[tool.setuptools.packages.find]
-include = ["flimsay"]
+[tool.setuptools.package-dir]
+flimsay = "flimsay"
 
 [tool.setuptools.package-data]
 flimsay = ["*.txt"]
+"flimsay.weights" = ["*.txt"]
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--doctest-modules -v --cov=flimsay"
 doctest_optionflags = "NORMALIZE_WHITESPACE"
 testpaths = [
@@ -111,15 +112,15 @@
 target-version = ['py39', 'py310', 'py311']
 preview = true
 
 [tool.isort]
 profile = "black"
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.4.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

