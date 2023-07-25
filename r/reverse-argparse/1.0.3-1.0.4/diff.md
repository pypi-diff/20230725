# Comparing `tmp/reverse_argparse-1.0.3.tar.gz` & `tmp/reverse_argparse-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reverse_argparse-1.0.3.tar", max compression
+gzip compressed data, was "reverse_argparse-1.0.4.tar", max compression
```

## Comparing `reverse_argparse-1.0.3.tar` & `reverse_argparse-1.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1723 2023-07-25 17:15:53.922553 reverse_argparse-1.0.3/LICENSE.md
--rw-r--r--   0        0        0     3850 2023-07-25 17:15:53.922553 reverse_argparse-1.0.3/README.md
--rw-r--r--   0        0        0     2480 2023-07-25 17:15:54.910568 reverse_argparse-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      305 2023-07-25 17:15:54.910568 reverse_argparse-1.0.3/reverse_argparse/__init__.py
--rw-r--r--   0        0        0    18712 2023-07-25 17:15:53.922553 reverse_argparse-1.0.3/reverse_argparse/reverse_argparse.py
--rw-r--r--   0        0        0     5469 1970-01-01 00:00:00.000000 reverse_argparse-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1723 2023-07-25 17:30:09.787917 reverse_argparse-1.0.4/LICENSE.md
+-rw-r--r--   0        0        0     3850 2023-07-25 17:30:09.787917 reverse_argparse-1.0.4/README.md
+-rw-r--r--   0        0        0     2480 2023-07-25 17:30:10.763931 reverse_argparse-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      305 2023-07-25 17:30:10.763931 reverse_argparse-1.0.4/reverse_argparse/__init__.py
+-rw-r--r--   0        0        0    18712 2023-07-25 17:30:09.791917 reverse_argparse-1.0.4/reverse_argparse/reverse_argparse.py
+-rw-r--r--   0        0        0     5469 1970-01-01 00:00:00.000000 reverse_argparse-1.0.4/PKG-INFO
```

### Comparing `reverse_argparse-1.0.3/LICENSE.md` & `reverse_argparse-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `reverse_argparse-1.0.3/README.md` & `reverse_argparse-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![codecov](https://codecov.io/gh/sandialabs/reverse_argparse/branch/master/graph/badge.svg?token=FmDStZ6FVR)](https://codecov.io/gh/sandialabs/reverse_argparse)
 [![Continuous Integration](https://github.com/sandialabs/reverse_argparse/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/sandialabs/reverse_argparse/actions/workflows/continuous-integration.yml)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 [![Documentation Status](https://readthedocs.org/projects/reverse-argparse/badge/?version=latest)](https://reverse-argparse.readthedocs.io/en/latest/?badge=latest)
 [![Linting: Pylint](https://img.shields.io/badge/Linting-Pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![pre-commit.ci Status](https://results.pre-commit.ci/badge/github/sandialabs/reverse_argparse/master.svg)](https://results.pre-commit.ci/latest/github/sandialabs/reverse_argparse/master)
-[![PyPI Version](https://badge.fury.io/py/reverse_argparse.svg)](https://badge.fury.io/py/reverse-argparse)
+[![PyPI Version](https://badge.fury.io/py/reverse-argparse.svg)](https://badge.fury.io/py/reverse-argparse)
 ![Python Version](https://img.shields.io/badge/Python-3.8+-blue.svg)
 [![Security: Bandit](https://img.shields.io/badge/Security-Bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 # reverse_argparse
 
 Whereas [`argparse`][argparse] is concerned with taking a bunch of command line
 arguments and parsing them, this package is intended to do the opposite; that
```

### Comparing `reverse_argparse-1.0.3/pyproject.toml` & `reverse_argparse-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [tool.isort]
 profile = "black"
 line_length = 79
 
 
 [tool.poetry]
 name = "reverse_argparse"
-version = "1.0.3"
+version = "1.0.4"
 license = "LICENSE.md"
 readme = "README.md"
 keywords = ["argparse", "argument", "parse", "parsing", "command line"]
 repository = "https://github.com/sandialabs/reverse_argparse"
 description = "Generate the effective command line invocation for a script."
 documentation = "https://reverse-argparse.readthedocs.io"
 authors = [
```

### Comparing `reverse_argparse-1.0.3/reverse_argparse/reverse_argparse.py` & `reverse_argparse-1.0.4/reverse_argparse/reverse_argparse.py`

 * *Files identical despite different names*

### Comparing `reverse_argparse-1.0.3/PKG-INFO` & `reverse_argparse-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reverse-argparse
-Version: 1.0.3
+Version: 1.0.4
 Summary: Generate the effective command line invocation for a script.
 Home-page: https://github.com/sandialabs/reverse_argparse
 License: LICENSE.md
 Keywords: argparse,argument,parse,parsing,command line
 Author: Jason M. Gates
 Author-email: jmgate@sandia.gov
 Requires-Python: >=3.8
@@ -37,15 +37,15 @@
 [![codecov](https://codecov.io/gh/sandialabs/reverse_argparse/branch/master/graph/badge.svg?token=FmDStZ6FVR)](https://codecov.io/gh/sandialabs/reverse_argparse)
 [![Continuous Integration](https://github.com/sandialabs/reverse_argparse/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/sandialabs/reverse_argparse/actions/workflows/continuous-integration.yml)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 [![Documentation Status](https://readthedocs.org/projects/reverse-argparse/badge/?version=latest)](https://reverse-argparse.readthedocs.io/en/latest/?badge=latest)
 [![Linting: Pylint](https://img.shields.io/badge/Linting-Pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![pre-commit.ci Status](https://results.pre-commit.ci/badge/github/sandialabs/reverse_argparse/master.svg)](https://results.pre-commit.ci/latest/github/sandialabs/reverse_argparse/master)
-[![PyPI Version](https://badge.fury.io/py/reverse_argparse.svg)](https://badge.fury.io/py/reverse-argparse)
+[![PyPI Version](https://badge.fury.io/py/reverse-argparse.svg)](https://badge.fury.io/py/reverse-argparse)
 ![Python Version](https://img.shields.io/badge/Python-3.8+-blue.svg)
 [![Security: Bandit](https://img.shields.io/badge/Security-Bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 # reverse_argparse
 
 Whereas [`argparse`][argparse] is concerned with taking a bunch of command line
 arguments and parsing them, this package is intended to do the opposite; that
```

