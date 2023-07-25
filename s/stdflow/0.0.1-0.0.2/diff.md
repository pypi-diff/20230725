# Comparing `tmp/stdflow-0.0.1.tar.gz` & `tmp/stdflow-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdflow-0.0.1.tar", last modified: Mon Jul 24 16:12:47 2023, max compression
+gzip compressed data, was "stdflow-0.0.2.tar", last modified: Tue Jul 25 02:25:11 2023, max compression
```

## Comparing `stdflow-0.0.1.tar` & `stdflow-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,30 @@
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-24 16:12:47.076480 stdflow-0.0.1/
--rw-r--r--   0 cyprien    (501) staff       (20)     1071 2023-07-24 15:57:38.000000 stdflow-0.0.1/LICENSE
--rw-r--r--   0 cyprien    (501) staff       (20)     6498 2023-07-24 16:12:47.076356 stdflow-0.0.1/PKG-INFO
--rw-r--r--   0 cyprien    (501) staff       (20)     5931 2023-07-24 15:39:08.000000 stdflow-0.0.1/README.md
--rw-r--r--   0 cyprien    (501) staff       (20)      748 2023-07-24 16:01:47.000000 stdflow-0.0.1/pyproject.toml
--rw-r--r--   0 cyprien    (501) staff       (20)       38 2023-07-24 16:12:47.076520 stdflow-0.0.1/setup.cfg
--rw-r--r--   0 cyprien    (501) staff       (20)     1030 2023-07-24 16:12:38.000000 stdflow-0.0.1/setup.py
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-24 16:12:47.072892 stdflow-0.0.1/stdflow/
--rw-r--r--   0 cyprien    (501) staff       (20)     3363 2023-07-24 15:26:56.000000 stdflow-0.0.1/stdflow/__init__.py
--rw-r--r--   0 cyprien    (501) staff       (20)       81 2023-07-24 02:46:01.000000 stdflow-0.0.1/stdflow/config.py
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-24 16:12:47.074005 stdflow-0.0.1/stdflow/loaders/
--rw-r--r--   0 cyprien    (501) staff       (20)      339 2023-07-24 02:46:01.000000 stdflow-0.0.1/stdflow/loaders/__init__.py
--rw-r--r--   0 cyprien    (501) staff       (20)     1156 2023-07-24 02:46:01.000000 stdflow-0.0.1/stdflow/loaders/csv.py
--rw-r--r--   0 cyprien    (501) staff       (20)     2980 2023-07-24 15:19:12.000000 stdflow-0.0.1/stdflow/metadata.py
--rw-r--r--   0 cyprien    (501) staff       (20)     6526 2023-07-24 15:58:05.000000 stdflow-0.0.1/stdflow/path.py
--rw-r--r--   0 cyprien    (501) staff       (20)    12681 2023-07-24 15:26:56.000000 stdflow-0.0.1/stdflow/step.py
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-24 16:12:47.074263 stdflow-0.0.1/stdflow/utils/
--rw-r--r--   0 cyprien    (501) staff       (20)     7383 2023-07-24 14:48:55.000000 stdflow-0.0.1/stdflow/utils/__init__.py
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-24 16:12:47.073663 stdflow-0.0.1/stdflow.egg-info/
--rw-r--r--   0 cyprien    (501) staff       (20)     6498 2023-07-24 16:12:47.000000 stdflow-0.0.1/stdflow.egg-info/PKG-INFO
--rw-r--r--   0 cyprien    (501) staff       (20)      507 2023-07-24 16:12:47.000000 stdflow-0.0.1/stdflow.egg-info/SOURCES.txt
--rw-r--r--   0 cyprien    (501) staff       (20)        1 2023-07-24 16:12:47.000000 stdflow-0.0.1/stdflow.egg-info/dependency_links.txt
--rw-r--r--   0 cyprien    (501) staff       (20)       83 2023-07-24 16:12:47.000000 stdflow-0.0.1/stdflow.egg-info/requires.txt
--rw-r--r--   0 cyprien    (501) staff       (20)       14 2023-07-24 16:12:47.000000 stdflow-0.0.1/stdflow.egg-info/top_level.txt
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-24 16:12:47.076036 stdflow-0.0.1/tests/
--rw-r--r--   0 cyprien    (501) staff       (20)        0 2023-07-22 02:06:18.000000 stdflow-0.0.1/tests/__init__.py
--rw-r--r--   0 cyprien    (501) staff       (20)     3430 2023-07-24 08:07:00.000000 stdflow-0.0.1/tests/test_load.py
--rw-r--r--   0 cyprien    (501) staff       (20)      490 2023-07-22 02:45:55.000000 stdflow-0.0.1/tests/test_package_vesion.py
--rw-r--r--   0 cyprien    (501) staff       (20)     5681 2023-07-24 15:20:46.000000 stdflow-0.0.1/tests/test_save.py
--rw-r--r--   0 cyprien    (501) staff       (20)     2089 2023-07-24 08:07:00.000000 stdflow-0.0.1/tests/test_src.py
--rw-r--r--   0 cyprien    (501) staff       (20)      751 2023-07-24 08:07:00.000000 stdflow-0.0.1/tests/test_utils.py
--rw-r--r--   0 cyprien    (501) staff       (20)      628 2023-07-24 03:34:22.000000 stdflow-0.0.1/tests/test_version.py
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 02:25:11.425492 stdflow-0.0.2/
+-rw-r--r--   0 cyprien    (501) staff       (20)     1071 2023-07-24 15:57:38.000000 stdflow-0.0.2/LICENSE
+-rw-r--r--   0 cyprien    (501) staff       (20)     6450 2023-07-25 02:25:11.425347 stdflow-0.0.2/PKG-INFO
+-rw-r--r--   0 cyprien    (501) staff       (20)     5931 2023-07-24 15:39:08.000000 stdflow-0.0.2/README.md
+-rw-r--r--   0 cyprien    (501) staff       (20)      829 2023-07-25 02:25:04.000000 stdflow-0.0.2/pyproject.toml
+-rw-r--r--   0 cyprien    (501) staff       (20)       38 2023-07-25 02:25:11.425539 stdflow-0.0.2/setup.cfg
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 02:25:11.421778 stdflow-0.0.2/stdflow/
+-rw-r--r--   0 cyprien    (501) staff       (20)     3363 2023-07-25 02:24:34.000000 stdflow-0.0.2/stdflow/__init__.py
+-rw-r--r--   0 cyprien    (501) staff       (20)       81 2023-07-24 02:46:01.000000 stdflow-0.0.2/stdflow/config.py
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 02:25:11.422899 stdflow-0.0.2/stdflow/loaders/
+-rw-r--r--   0 cyprien    (501) staff       (20)      339 2023-07-24 02:46:01.000000 stdflow-0.0.2/stdflow/loaders/__init__.py
+-rw-r--r--   0 cyprien    (501) staff       (20)     1156 2023-07-24 02:46:01.000000 stdflow-0.0.2/stdflow/loaders/csv.py
+-rw-r--r--   0 cyprien    (501) staff       (20)     2980 2023-07-24 15:19:12.000000 stdflow-0.0.2/stdflow/metadata.py
+-rw-r--r--   0 cyprien    (501) staff       (20)     6526 2023-07-24 15:58:05.000000 stdflow-0.0.2/stdflow/path.py
+-rw-r--r--   0 cyprien    (501) staff       (20)    12681 2023-07-24 15:26:56.000000 stdflow-0.0.2/stdflow/step.py
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 02:25:11.423211 stdflow-0.0.2/stdflow/utils/
+-rw-r--r--   0 cyprien    (501) staff       (20)     7383 2023-07-24 14:48:55.000000 stdflow-0.0.2/stdflow/utils/__init__.py
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 02:25:11.422557 stdflow-0.0.2/stdflow.egg-info/
+-rw-r--r--   0 cyprien    (501) staff       (20)     6450 2023-07-25 02:25:11.000000 stdflow-0.0.2/stdflow.egg-info/PKG-INFO
+-rw-r--r--   0 cyprien    (501) staff       (20)      480 2023-07-25 02:25:11.000000 stdflow-0.0.2/stdflow.egg-info/SOURCES.txt
+-rw-r--r--   0 cyprien    (501) staff       (20)        1 2023-07-25 02:25:11.000000 stdflow-0.0.2/stdflow.egg-info/dependency_links.txt
+-rw-r--r--   0 cyprien    (501) staff       (20)       83 2023-07-25 02:25:11.000000 stdflow-0.0.2/stdflow.egg-info/requires.txt
+-rw-r--r--   0 cyprien    (501) staff       (20)        8 2023-07-25 02:25:11.000000 stdflow-0.0.2/stdflow.egg-info/top_level.txt
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-25 02:25:11.425055 stdflow-0.0.2/tests/
+-rw-r--r--   0 cyprien    (501) staff       (20)     3430 2023-07-24 08:07:00.000000 stdflow-0.0.2/tests/test_load.py
+-rw-r--r--   0 cyprien    (501) staff       (20)      490 2023-07-22 02:45:55.000000 stdflow-0.0.2/tests/test_package_vesion.py
+-rw-r--r--   0 cyprien    (501) staff       (20)     5681 2023-07-24 15:20:46.000000 stdflow-0.0.2/tests/test_save.py
+-rw-r--r--   0 cyprien    (501) staff       (20)     2089 2023-07-24 08:07:00.000000 stdflow-0.0.2/tests/test_src.py
+-rw-r--r--   0 cyprien    (501) staff       (20)      751 2023-07-24 08:07:00.000000 stdflow-0.0.2/tests/test_utils.py
+-rw-r--r--   0 cyprien    (501) staff       (20)      628 2023-07-25 02:24:34.000000 stdflow-0.0.2/tests/test_version.py
```

### Comparing `stdflow-0.0.1/LICENSE` & `stdflow-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.1/PKG-INFO` & `stdflow-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: stdflow
-Version: 0.0.1
+Version: 0.0.2
 Summary: [alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output.
-Home-page: https://github.com/CyprienRicque/stdflow
-Author: Cyprien Ricque
-Author-email: ricque.cyprien@gmail.com
-License: MIT
+Author-email: Cyprien Ricque <ricque.cyprien@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # stdflow
 
 # README OUTDATED
```

### Comparing `stdflow-0.0.1/README.md` & `stdflow-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.1/pyproject.toml` & `stdflow-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-#[build-system]
-#requires = ["setuptools", "wheel"]
-#build-backend = "setuptools.build_meta"
+[build-system]
+requires = ["setuptools>=61.0", "wheel"]
+build-backend = "setuptools.build_meta"
 
-#[project]
-#name = "stdflow"
-#version = "0.0.1"
-#description = "[alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output."
-#readme = "README.md"
-#authors = [
-#    { name = "Cyprien Ricque", email = "ricque.cyprien@gmail.com" },
-#]
-#license = "MIT"
-#classifiers = [
-#    "Development Status :: First release",
-#    "Programming Language :: Python :: 3.9",
-#]
+[project]
+name = "stdflow"
+version = "0.0.2"
+description = "[alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output."
+readme = "README.md"
+authors = [
+    { name = "Cyprien Ricque", email = "ricque.cyprien@gmail.com" },
+]
+requires-python = ">=3.9"
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    'License :: OSI Approved :: MIT License',
+    "Programming Language :: Python :: 3.9",
+]
 dependencies = [
     "pandas~=2.0.3",
     "datetime~=5.2",
     "python-box[all]~=7.0",
     "openpyxl~=3.1.2",
     "python-box~=7.0.1"
 ]
```

### Comparing `stdflow-0.0.1/stdflow/__init__.py` & `stdflow-0.0.2/stdflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from datetime import datetime
 from typing import Optional, Union
 
 import pandas as pd
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 from stdflow.loaders import DataLoader
 from stdflow.step import GStep, Step
 
 s_step: Step = GStep()  # Singleton Step
```

### Comparing `stdflow-0.0.1/stdflow/loaders/csv.py` & `stdflow-0.0.2/stdflow/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.1/stdflow/metadata.py` & `stdflow-0.0.2/stdflow/metadata.py`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.1/stdflow/path.py` & `stdflow-0.0.2/stdflow/path.py`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.1/stdflow/step.py` & `stdflow-0.0.2/stdflow/step.py`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.1/stdflow/utils/__init__.py` & `stdflow-0.0.2/stdflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.1/stdflow.egg-info/PKG-INFO` & `stdflow-0.0.2/stdflow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: stdflow
-Version: 0.0.1
+Version: 0.0.2
 Summary: [alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output.
-Home-page: https://github.com/CyprienRicque/stdflow
-Author: Cyprien Ricque
-Author-email: ricque.cyprien@gmail.com
-License: MIT
+Author-email: Cyprien Ricque <ricque.cyprien@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # stdflow
 
 # README OUTDATED
```

### Comparing `stdflow-0.0.1/tests/test_load.py` & `stdflow-0.0.2/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.1/tests/test_save.py` & `stdflow-0.0.2/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.1/tests/test_src.py` & `stdflow-0.0.2/tests/test_src.py`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.1/tests/test_utils.py` & `stdflow-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.1/tests/test_version.py` & `stdflow-0.0.2/tests/test_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import stdflow as st
 
 
 def test_exact_version():
-    assert st.__version__ == "0.0.1"
+    assert st.__version__ == "0.0.2"
 
 
 def test_version():
     from stdflow import __version__
 
     assert isinstance(__version__, str), "Version must be a string"
```

