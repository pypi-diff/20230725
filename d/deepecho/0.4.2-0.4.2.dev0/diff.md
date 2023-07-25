# Comparing `tmp/deepecho-0.4.2.tar.gz` & `tmp/deepecho-0.4.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepecho-0.4.2.tar", last modified: Tue Jul 25 17:38:55 2023, max compression
+gzip compressed data, was "deepecho-0.4.2.dev0.tar", last modified: Mon Jul 24 19:41:26 2023, max compression
```

## Comparing `deepecho-0.4.2.tar` & `deepecho-0.4.2.dev0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-25 17:38:55.977950 deepecho-0.4.2/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       61 2023-01-10 22:50:52.000000 deepecho-0.4.2/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8325 2023-01-09 19:52:40.000000 deepecho-0.4.2/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3545 2023-07-25 17:38:53.000000 deepecho-0.4.2/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4825 2023-01-10 22:50:52.000000 deepecho-0.4.2/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      296 2023-01-09 19:52:40.000000 deepecho-0.4.2/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14579 2023-07-25 17:38:55.978116 deepecho-0.4.2/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7897 2023-01-10 22:50:52.000000 deepecho-0.4.2/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-25 17:38:55.975391 deepecho-0.4.2/deepecho/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      382 2023-07-25 17:38:54.000000 deepecho-0.4.2/deepecho/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-25 17:38:55.976297 deepecho-0.4.2/deepecho/data/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    28256 2023-01-09 19:52:40.000000 deepecho-0.4.2/deepecho/data/demo.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      266 2023-01-09 19:52:40.000000 deepecho-0.4.2/deepecho/demo.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-25 17:38:55.977052 deepecho-0.4.2/deepecho/models/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2023-01-09 19:52:40.000000 deepecho-0.4.2/deepecho/models/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10617 2023-05-02 18:08:31.000000 deepecho-0.4.2/deepecho/models/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21506 2023-01-10 22:50:52.000000 deepecho-0.4.2/deepecho/models/basic_gan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22393 2023-01-10 22:50:52.000000 deepecho-0.4.2/deepecho/models/par.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7223 2023-01-10 22:50:52.000000 deepecho-0.4.2/deepecho/sequences.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-25 17:38:55.976174 deepecho-0.4.2/deepecho.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14579 2023-07-25 17:38:55.000000 deepecho-0.4.2/deepecho.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      631 2023-07-25 17:38:55.000000 deepecho-0.4.2/deepecho.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-25 17:38:55.000000 deepecho-0.4.2/deepecho.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-25 17:38:55.000000 deepecho-0.4.2/deepecho.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1176 2023-07-25 17:38:55.000000 deepecho-0.4.2/deepecho.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        9 2023-07-25 17:38:55.000000 deepecho-0.4.2/deepecho.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1665 2023-07-25 17:38:55.978628 deepecho-0.4.2/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3336 2023-07-25 17:38:54.000000 deepecho-0.4.2/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-25 17:38:55.977192 deepecho-0.4.2/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       28 2023-01-10 22:50:52.000000 deepecho-0.4.2/tests/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-25 17:38:55.977589 deepecho-0.4.2/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       44 2023-01-10 22:50:52.000000 deepecho-0.4.2/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3942 2023-01-10 22:50:52.000000 deepecho-0.4.2/tests/integration/test_basic_gan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3886 2023-01-10 22:50:52.000000 deepecho-0.4.2/tests/integration/test_par.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-25 17:38:55.977835 deepecho-0.4.2/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       37 2023-01-10 22:50:52.000000 deepecho-0.4.2/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6642 2023-01-10 22:50:52.000000 deepecho-0.4.2/tests/unit/test_sequences.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-24 19:41:26.764092 deepecho-0.4.2.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       61 2023-01-10 22:50:52.000000 deepecho-0.4.2.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8325 2023-01-09 19:52:40.000000 deepecho-0.4.2.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3220 2023-05-02 18:08:31.000000 deepecho-0.4.2.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4825 2023-01-10 22:50:52.000000 deepecho-0.4.2.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      296 2023-01-09 19:52:40.000000 deepecho-0.4.2.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14187 2023-07-24 19:41:26.764273 deepecho-0.4.2.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7897 2023-01-10 22:50:52.000000 deepecho-0.4.2.dev0/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-24 19:41:26.760842 deepecho-0.4.2.dev0/deepecho/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      387 2023-05-02 18:09:04.000000 deepecho-0.4.2.dev0/deepecho/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-24 19:41:26.762019 deepecho-0.4.2.dev0/deepecho/data/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    28256 2023-01-09 19:52:40.000000 deepecho-0.4.2.dev0/deepecho/data/demo.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      266 2023-01-09 19:52:40.000000 deepecho-0.4.2.dev0/deepecho/demo.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-24 19:41:26.762971 deepecho-0.4.2.dev0/deepecho/models/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2023-01-09 19:52:40.000000 deepecho-0.4.2.dev0/deepecho/models/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10617 2023-05-02 18:08:31.000000 deepecho-0.4.2.dev0/deepecho/models/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21506 2023-01-10 22:50:52.000000 deepecho-0.4.2.dev0/deepecho/models/basic_gan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22393 2023-01-10 22:50:52.000000 deepecho-0.4.2.dev0/deepecho/models/par.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7223 2023-01-10 22:50:52.000000 deepecho-0.4.2.dev0/deepecho/sequences.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-24 19:41:26.761821 deepecho-0.4.2.dev0/deepecho.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14187 2023-07-24 19:41:26.000000 deepecho-0.4.2.dev0/deepecho.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      631 2023-07-24 19:41:26.000000 deepecho-0.4.2.dev0/deepecho.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-24 19:41:26.000000 deepecho-0.4.2.dev0/deepecho.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-24 19:41:26.000000 deepecho-0.4.2.dev0/deepecho.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1176 2023-07-24 19:41:26.000000 deepecho-0.4.2.dev0/deepecho.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        9 2023-07-24 19:41:26.000000 deepecho-0.4.2.dev0/deepecho.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1670 2023-07-24 19:41:26.764833 deepecho-0.4.2.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3341 2023-07-24 19:41:13.000000 deepecho-0.4.2.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-24 19:41:26.763243 deepecho-0.4.2.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       28 2023-01-10 22:50:52.000000 deepecho-0.4.2.dev0/tests/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-24 19:41:26.763704 deepecho-0.4.2.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       44 2023-01-10 22:50:52.000000 deepecho-0.4.2.dev0/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3942 2023-01-10 22:50:52.000000 deepecho-0.4.2.dev0/tests/integration/test_basic_gan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3886 2023-01-10 22:50:52.000000 deepecho-0.4.2.dev0/tests/integration/test_par.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-24 19:41:26.763966 deepecho-0.4.2.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       37 2023-01-10 22:50:52.000000 deepecho-0.4.2.dev0/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6642 2023-01-10 22:50:52.000000 deepecho-0.4.2.dev0/tests/unit/test_sequences.py
```

### Comparing `deepecho-0.4.2/CONTRIBUTING.rst` & `deepecho-0.4.2.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.2/HISTORY.md` & `deepecho-0.4.2.dev0/HISTORY.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,9 @@
 # History
 
-## 0.4.2 - 2023-07-25
-
-This release drops support for Python 3.7 and adds support for Python 3.11.
-
-### Maintenance
-
-* Add support for Python 3.11 - Issue [#74](https://github.com/sdv-dev/DeepEcho/issues/74) by @fealho
-* Drop support for Python 3.7 - Issue [#75](https://github.com/sdv-dev/DeepEcho/issues/75) by @R-Palazzo
-
 ## 0.4.1 - 2023-05-02
 
 This release adds support for Pandas 2.0 and PyTorch 2.0!
 
 ### Maintenance
 
 * Remove upper bound for pandas - Issue [#69](https://github.com/sdv-dev/DeepEcho/issues/69) by @frances-h
```

### Comparing `deepecho-0.4.2/LICENSE` & `deepecho-0.4.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.2/PKG-INFO` & `deepecho-0.4.2.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepecho
-Version: 0.4.2
+Version: 0.4.2.dev0
 Summary: Create sequential synthetic data of mixed types using a GAN.
 Home-page: https://github.com/sdv-dev/DeepEcho
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Description: <div align="center">
         <br/>
@@ -189,23 +189,14 @@
         [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
         integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
         for specific needs.
         
         
         # History
         
-        ## 0.4.2 - 2023-07-25
-        
-        This release drops support for Python 3.7 and adds support for Python 3.11.
-        
-        ### Maintenance
-        
-        * Add support for Python 3.11 - Issue [#74](https://github.com/sdv-dev/DeepEcho/issues/74) by @fealho
-        * Drop support for Python 3.7 - Issue [#75](https://github.com/sdv-dev/DeepEcho/issues/75) by @R-Palazzo
-        
         ## 0.4.1 - 2023-05-02
         
         This release adds support for Pandas 2.0 and PyTorch 2.0!
         
         ### Maintenance
         
         * Remove upper bound for pandas - Issue [#69](https://github.com/sdv-dev/DeepEcho/issues/69) by @frances-h
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: deepecho Version: 0.4.2 Summary: Create sequential
-synthetic data of mixed types using a GAN. Home-page: https://github.com/sdv-
-dev/DeepEcho Author: DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1
-Description:
+Metadata-Version: 2.1 Name: deepecho Version: 0.4.2.dev0 Summary: Create
+sequential synthetic data of mixed types using a GAN. Home-page: https://
+github.com/sdv-dev/DeepEcho Author: DataCebo, Inc. Author-email: info@sdv.dev
+License: BSL-1.1 Description:
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
 [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--
 %20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-
 +Pre-Alpha) [![PyPi Shield](https://img.shields.io/pypi/v/deepecho.svg)](https:
 //pypi.python.org/pypi/deepecho) [![Tests](https://github.com/sdv-dev/DeepEcho/
@@ -97,63 +97,59 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## 0.4.2 - 2023-07-25 This release
-drops support for Python 3.7 and adds support for Python 3.11. ### Maintenance
-* Add support for Python 3.11 - Issue [#74](https://github.com/sdv-dev/
-DeepEcho/issues/74) by @fealho * Drop support for Python 3.7 - Issue [#75]
-(https://github.com/sdv-dev/DeepEcho/issues/75) by @R-Palazzo ## 0.4.1 - 2023-
-05-02 This release adds support for Pandas 2.0 and PyTorch 2.0! ### Maintenance
-* Remove upper bound for pandas - Issue [#69](https://github.com/sdv-dev/
-DeepEcho/issues/69) by @frances-h * Upgrade to Torch 2.0 - Issue [#70](https://
-github.com/sdv-dev/DeepEcho/issues/70) by @frances-h ## 0.4.0 - 2023-01-10 This
-release adds support for python 3.10 and 3.11. It also drops support for python
-3.6. ### Maintenance * Support Python 3.10 and 3.11 - Issue [#63](https://
-github.com/sdv-dev/DeepEcho/issues/63) by @pvk-developer * DeepEcho Package
-Maintenance Updates - Issue [#62](https://github.com/sdv-dev/DeepEcho/issues/
-62) by @pvk-developer ## 0.3.0 - 2021-11-15 This release adds support for
-Python 3.9 and updates dependencies to ensure compatibility with the rest of
-the SDV ecosystem. * Add support for Python 3.9 - Issue [#41](https://
-github.com/sdv-dev/DeepEcho/issues/41) by @fealho * Add pip check to CI
-workflows internal improvements - Issue [#39](https://github.com/sdv-dev/
-DeepEcho/issues/39) by @pvk-developer * Add support for pylint>2.7.2
-housekeeping - Issue [#33](https://github.com/sdv-dev/DeepEcho/issues/33) by
-@fealho * Add support for torch>=1.8 housekeeping - Issue [#32](https://
-github.com/sdv-dev/DeepEcho/issues/32) by @fealho ## 0.2.1 - 2021-10-12 This
-release fixes a bug with how DeepEcho handles NaN values. * Handling NaN's bug
-- Issue [#35](https://github.com/sdv-dev/DeepEcho/issues/35) by @fealho ##
-0.2.0 - 2021-02-24 Maintenance release to update dependencies and ensure
-compatibility with the rest of the SDV ecosystem libraries. ## 0.1.4 - 2020-10-
-16 Minor maintenance version to update dependencies and documentation, and also
-make the demo data loading function parse dates properly. ## 0.1.3 - 2020-10-16
-This version includes several minor improvements to the PAR model and the way
-the sequences are generated: * Sequences can now be generated without dropping
-the sequence index. * The PAR model learns the min and max length of the
-sequence from the input data. * NaN values are properly supported for both
-categorical and numerical columns. * NaN values are generated for numerical
-columns only if there were NaNs in the input data. * Constant columns can now
-be modeled. ## 0.1.2 - 2020-09-15 Add BasicGAN Model and additional
-benchmarking results. ## 0.1.1 - 2020-08-15 This release includes a few new
-features to make DeepEcho work on more types of datasets as well as to making
-it easier to add new datasets to the benchmarking framework. * Add
-`segment_size` and `sequence_index` arguments to `fit` method. * Add
-`sequence_length` as an optional argument to `sample` and `sample_sequence`
-methods. * Update the Dataset storage format to add `sequence_index` and
-versioning. * Separate the sequence assembling process in its own
-`deepecho.sequences` module. * Add function `make_dataset` to create a dataset
-from a dataframe and just a few column names. * Add notebook tutorial to show
-how to create a datasets and use them. ## 0.1.0 - 2020-08-11 First release.
-Included Features: * PARModel * Demo dataset and tutorials * Benchmarking
-Framework * Support and instructions for benchmarking on a Kubernetes cluster.
-Keywords: deepecho deepecho DeepEcho Platform: UNKNOWN Classifier: Development
-Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
-License :: Free for non-commercial use Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: >=3.8,<3.12 Description-Content-Type:
-text/markdown Provides-Extra: test Provides-Extra: dev
+libraries for specific needs. # History ## 0.4.1 - 2023-05-02 This release adds
+support for Pandas 2.0 and PyTorch 2.0! ### Maintenance * Remove upper bound
+for pandas - Issue [#69](https://github.com/sdv-dev/DeepEcho/issues/69) by
+@frances-h * Upgrade to Torch 2.0 - Issue [#70](https://github.com/sdv-dev/
+DeepEcho/issues/70) by @frances-h ## 0.4.0 - 2023-01-10 This release adds
+support for python 3.10 and 3.11. It also drops support for python 3.6. ###
+Maintenance * Support Python 3.10 and 3.11 - Issue [#63](https://github.com/
+sdv-dev/DeepEcho/issues/63) by @pvk-developer * DeepEcho Package Maintenance
+Updates - Issue [#62](https://github.com/sdv-dev/DeepEcho/issues/62) by @pvk-
+developer ## 0.3.0 - 2021-11-15 This release adds support for Python 3.9 and
+updates dependencies to ensure compatibility with the rest of the SDV
+ecosystem. * Add support for Python 3.9 - Issue [#41](https://github.com/sdv-
+dev/DeepEcho/issues/41) by @fealho * Add pip check to CI workflows internal
+improvements - Issue [#39](https://github.com/sdv-dev/DeepEcho/issues/39) by
+@pvk-developer * Add support for pylint>2.7.2 housekeeping - Issue [#33](https:
+//github.com/sdv-dev/DeepEcho/issues/33) by @fealho * Add support for
+torch>=1.8 housekeeping - Issue [#32](https://github.com/sdv-dev/DeepEcho/
+issues/32) by @fealho ## 0.2.1 - 2021-10-12 This release fixes a bug with how
+DeepEcho handles NaN values. * Handling NaN's bug - Issue [#35](https://
+github.com/sdv-dev/DeepEcho/issues/35) by @fealho ## 0.2.0 - 2021-02-24
+Maintenance release to update dependencies and ensure compatibility with the
+rest of the SDV ecosystem libraries. ## 0.1.4 - 2020-10-16 Minor maintenance
+version to update dependencies and documentation, and also make the demo data
+loading function parse dates properly. ## 0.1.3 - 2020-10-16 This version
+includes several minor improvements to the PAR model and the way the sequences
+are generated: * Sequences can now be generated without dropping the sequence
+index. * The PAR model learns the min and max length of the sequence from the
+input data. * NaN values are properly supported for both categorical and
+numerical columns. * NaN values are generated for numerical columns only if
+there were NaNs in the input data. * Constant columns can now be modeled. ##
+0.1.2 - 2020-09-15 Add BasicGAN Model and additional benchmarking results. ##
+0.1.1 - 2020-08-15 This release includes a few new features to make DeepEcho
+work on more types of datasets as well as to making it easier to add new
+datasets to the benchmarking framework. * Add `segment_size` and
+`sequence_index` arguments to `fit` method. * Add `sequence_length` as an
+optional argument to `sample` and `sample_sequence` methods. * Update the
+Dataset storage format to add `sequence_index` and versioning. * Separate the
+sequence assembling process in its own `deepecho.sequences` module. * Add
+function `make_dataset` to create a dataset from a dataframe and just a few
+column names. * Add notebook tutorial to show how to create a datasets and use
+them. ## 0.1.0 - 2020-08-11 First release. Included Features: * PARModel * Demo
+dataset and tutorials * Benchmarking Framework * Support and instructions for
+benchmarking on a Kubernetes cluster. Keywords: deepecho deepecho DeepEcho
+Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+Intended Audience :: Developers Classifier: License :: Free for non-commercial
+use Classifier: Natural Language :: English Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
+>=3.8,<3.12 Description-Content-Type: text/markdown Provides-Extra: test
+Provides-Extra: dev
```

### Comparing `deepecho-0.4.2/README.md` & `deepecho-0.4.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.2/deepecho/data/demo.csv` & `deepecho-0.4.2.dev0/deepecho/data/demo.csv`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.2/deepecho/models/base.py` & `deepecho-0.4.2.dev0/deepecho/models/base.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.2/deepecho/models/basic_gan.py` & `deepecho-0.4.2.dev0/deepecho/models/basic_gan.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.2/deepecho/models/par.py` & `deepecho-0.4.2.dev0/deepecho/models/par.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.2/deepecho/sequences.py` & `deepecho-0.4.2.dev0/deepecho/sequences.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.2/deepecho.egg-info/PKG-INFO` & `deepecho-0.4.2.dev0/deepecho.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepecho
-Version: 0.4.2
+Version: 0.4.2.dev0
 Summary: Create sequential synthetic data of mixed types using a GAN.
 Home-page: https://github.com/sdv-dev/DeepEcho
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Description: <div align="center">
         <br/>
@@ -189,23 +189,14 @@
         [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
         integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
         for specific needs.
         
         
         # History
         
-        ## 0.4.2 - 2023-07-25
-        
-        This release drops support for Python 3.7 and adds support for Python 3.11.
-        
-        ### Maintenance
-        
-        * Add support for Python 3.11 - Issue [#74](https://github.com/sdv-dev/DeepEcho/issues/74) by @fealho
-        * Drop support for Python 3.7 - Issue [#75](https://github.com/sdv-dev/DeepEcho/issues/75) by @R-Palazzo
-        
         ## 0.4.1 - 2023-05-02
         
         This release adds support for Pandas 2.0 and PyTorch 2.0!
         
         ### Maintenance
         
         * Remove upper bound for pandas - Issue [#69](https://github.com/sdv-dev/DeepEcho/issues/69) by @frances-h
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: deepecho Version: 0.4.2 Summary: Create sequential
-synthetic data of mixed types using a GAN. Home-page: https://github.com/sdv-
-dev/DeepEcho Author: DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1
-Description:
+Metadata-Version: 2.1 Name: deepecho Version: 0.4.2.dev0 Summary: Create
+sequential synthetic data of mixed types using a GAN. Home-page: https://
+github.com/sdv-dev/DeepEcho Author: DataCebo, Inc. Author-email: info@sdv.dev
+License: BSL-1.1 Description:
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
 [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--
 %20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-
 +Pre-Alpha) [![PyPi Shield](https://img.shields.io/pypi/v/deepecho.svg)](https:
 //pypi.python.org/pypi/deepecho) [![Tests](https://github.com/sdv-dev/DeepEcho/
@@ -97,63 +97,59 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## 0.4.2 - 2023-07-25 This release
-drops support for Python 3.7 and adds support for Python 3.11. ### Maintenance
-* Add support for Python 3.11 - Issue [#74](https://github.com/sdv-dev/
-DeepEcho/issues/74) by @fealho * Drop support for Python 3.7 - Issue [#75]
-(https://github.com/sdv-dev/DeepEcho/issues/75) by @R-Palazzo ## 0.4.1 - 2023-
-05-02 This release adds support for Pandas 2.0 and PyTorch 2.0! ### Maintenance
-* Remove upper bound for pandas - Issue [#69](https://github.com/sdv-dev/
-DeepEcho/issues/69) by @frances-h * Upgrade to Torch 2.0 - Issue [#70](https://
-github.com/sdv-dev/DeepEcho/issues/70) by @frances-h ## 0.4.0 - 2023-01-10 This
-release adds support for python 3.10 and 3.11. It also drops support for python
-3.6. ### Maintenance * Support Python 3.10 and 3.11 - Issue [#63](https://
-github.com/sdv-dev/DeepEcho/issues/63) by @pvk-developer * DeepEcho Package
-Maintenance Updates - Issue [#62](https://github.com/sdv-dev/DeepEcho/issues/
-62) by @pvk-developer ## 0.3.0 - 2021-11-15 This release adds support for
-Python 3.9 and updates dependencies to ensure compatibility with the rest of
-the SDV ecosystem. * Add support for Python 3.9 - Issue [#41](https://
-github.com/sdv-dev/DeepEcho/issues/41) by @fealho * Add pip check to CI
-workflows internal improvements - Issue [#39](https://github.com/sdv-dev/
-DeepEcho/issues/39) by @pvk-developer * Add support for pylint>2.7.2
-housekeeping - Issue [#33](https://github.com/sdv-dev/DeepEcho/issues/33) by
-@fealho * Add support for torch>=1.8 housekeeping - Issue [#32](https://
-github.com/sdv-dev/DeepEcho/issues/32) by @fealho ## 0.2.1 - 2021-10-12 This
-release fixes a bug with how DeepEcho handles NaN values. * Handling NaN's bug
-- Issue [#35](https://github.com/sdv-dev/DeepEcho/issues/35) by @fealho ##
-0.2.0 - 2021-02-24 Maintenance release to update dependencies and ensure
-compatibility with the rest of the SDV ecosystem libraries. ## 0.1.4 - 2020-10-
-16 Minor maintenance version to update dependencies and documentation, and also
-make the demo data loading function parse dates properly. ## 0.1.3 - 2020-10-16
-This version includes several minor improvements to the PAR model and the way
-the sequences are generated: * Sequences can now be generated without dropping
-the sequence index. * The PAR model learns the min and max length of the
-sequence from the input data. * NaN values are properly supported for both
-categorical and numerical columns. * NaN values are generated for numerical
-columns only if there were NaNs in the input data. * Constant columns can now
-be modeled. ## 0.1.2 - 2020-09-15 Add BasicGAN Model and additional
-benchmarking results. ## 0.1.1 - 2020-08-15 This release includes a few new
-features to make DeepEcho work on more types of datasets as well as to making
-it easier to add new datasets to the benchmarking framework. * Add
-`segment_size` and `sequence_index` arguments to `fit` method. * Add
-`sequence_length` as an optional argument to `sample` and `sample_sequence`
-methods. * Update the Dataset storage format to add `sequence_index` and
-versioning. * Separate the sequence assembling process in its own
-`deepecho.sequences` module. * Add function `make_dataset` to create a dataset
-from a dataframe and just a few column names. * Add notebook tutorial to show
-how to create a datasets and use them. ## 0.1.0 - 2020-08-11 First release.
-Included Features: * PARModel * Demo dataset and tutorials * Benchmarking
-Framework * Support and instructions for benchmarking on a Kubernetes cluster.
-Keywords: deepecho deepecho DeepEcho Platform: UNKNOWN Classifier: Development
-Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
-License :: Free for non-commercial use Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: >=3.8,<3.12 Description-Content-Type:
-text/markdown Provides-Extra: test Provides-Extra: dev
+libraries for specific needs. # History ## 0.4.1 - 2023-05-02 This release adds
+support for Pandas 2.0 and PyTorch 2.0! ### Maintenance * Remove upper bound
+for pandas - Issue [#69](https://github.com/sdv-dev/DeepEcho/issues/69) by
+@frances-h * Upgrade to Torch 2.0 - Issue [#70](https://github.com/sdv-dev/
+DeepEcho/issues/70) by @frances-h ## 0.4.0 - 2023-01-10 This release adds
+support for python 3.10 and 3.11. It also drops support for python 3.6. ###
+Maintenance * Support Python 3.10 and 3.11 - Issue [#63](https://github.com/
+sdv-dev/DeepEcho/issues/63) by @pvk-developer * DeepEcho Package Maintenance
+Updates - Issue [#62](https://github.com/sdv-dev/DeepEcho/issues/62) by @pvk-
+developer ## 0.3.0 - 2021-11-15 This release adds support for Python 3.9 and
+updates dependencies to ensure compatibility with the rest of the SDV
+ecosystem. * Add support for Python 3.9 - Issue [#41](https://github.com/sdv-
+dev/DeepEcho/issues/41) by @fealho * Add pip check to CI workflows internal
+improvements - Issue [#39](https://github.com/sdv-dev/DeepEcho/issues/39) by
+@pvk-developer * Add support for pylint>2.7.2 housekeeping - Issue [#33](https:
+//github.com/sdv-dev/DeepEcho/issues/33) by @fealho * Add support for
+torch>=1.8 housekeeping - Issue [#32](https://github.com/sdv-dev/DeepEcho/
+issues/32) by @fealho ## 0.2.1 - 2021-10-12 This release fixes a bug with how
+DeepEcho handles NaN values. * Handling NaN's bug - Issue [#35](https://
+github.com/sdv-dev/DeepEcho/issues/35) by @fealho ## 0.2.0 - 2021-02-24
+Maintenance release to update dependencies and ensure compatibility with the
+rest of the SDV ecosystem libraries. ## 0.1.4 - 2020-10-16 Minor maintenance
+version to update dependencies and documentation, and also make the demo data
+loading function parse dates properly. ## 0.1.3 - 2020-10-16 This version
+includes several minor improvements to the PAR model and the way the sequences
+are generated: * Sequences can now be generated without dropping the sequence
+index. * The PAR model learns the min and max length of the sequence from the
+input data. * NaN values are properly supported for both categorical and
+numerical columns. * NaN values are generated for numerical columns only if
+there were NaNs in the input data. * Constant columns can now be modeled. ##
+0.1.2 - 2020-09-15 Add BasicGAN Model and additional benchmarking results. ##
+0.1.1 - 2020-08-15 This release includes a few new features to make DeepEcho
+work on more types of datasets as well as to making it easier to add new
+datasets to the benchmarking framework. * Add `segment_size` and
+`sequence_index` arguments to `fit` method. * Add `sequence_length` as an
+optional argument to `sample` and `sample_sequence` methods. * Update the
+Dataset storage format to add `sequence_index` and versioning. * Separate the
+sequence assembling process in its own `deepecho.sequences` module. * Add
+function `make_dataset` to create a dataset from a dataframe and just a few
+column names. * Add notebook tutorial to show how to create a datasets and use
+them. ## 0.1.0 - 2020-08-11 First release. Included Features: * PARModel * Demo
+dataset and tutorials * Benchmarking Framework * Support and instructions for
+benchmarking on a Kubernetes cluster. Keywords: deepecho deepecho DeepEcho
+Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+Intended Audience :: Developers Classifier: License :: Free for non-commercial
+use Classifier: Natural Language :: English Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
+>=3.8,<3.12 Description-Content-Type: text/markdown Provides-Extra: test
+Provides-Extra: dev
```

### Comparing `deepecho-0.4.2/deepecho.egg-info/SOURCES.txt` & `deepecho-0.4.2.dev0/deepecho.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.2/deepecho.egg-info/requires.txt` & `deepecho-0.4.2.dev0/deepecho.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.2/setup.cfg` & `deepecho-0.4.2.dev0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.2
+current_version = 0.4.2.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `deepecho-0.4.2/setup.py` & `deepecho-0.4.2.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,10 +108,10 @@
     name='deepecho',
     packages=find_packages(include=['deepecho', 'deepecho.*']),
     python_requires='>=3.8,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/DeepEcho',
-    version='0.4.2',
+    version='0.4.2.dev0',
     zip_safe=False,
 )
```

### Comparing `deepecho-0.4.2/tests/integration/test_basic_gan.py` & `deepecho-0.4.2.dev0/tests/integration/test_basic_gan.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.2/tests/integration/test_par.py` & `deepecho-0.4.2.dev0/tests/integration/test_par.py`

 * *Files identical despite different names*

### Comparing `deepecho-0.4.2/tests/unit/test_sequences.py` & `deepecho-0.4.2.dev0/tests/unit/test_sequences.py`

 * *Files identical despite different names*

