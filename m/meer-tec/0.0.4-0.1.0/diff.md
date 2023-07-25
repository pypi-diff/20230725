# Comparing `tmp/meer_tec-0.0.4.tar.gz` & `tmp/meer_tec-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meer_tec-0.0.4.tar", last modified: Fri Jul 21 13:50:28 2023, max compression
+gzip compressed data, was "meer_tec-0.1.0.tar", last modified: Tue Jul 25 13:54:00 2023, max compression
```

## Comparing `meer_tec-0.0.4.tar` & `meer_tec-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:50:28.272042 meer_tec-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-21 13:50:18.000000 meer_tec-0.0.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:50:28.272042 meer_tec-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:50:28.272042 meer_tec-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-21 13:50:18.000000 meer_tec-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-21 13:50:18.000000 meer_tec-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-21 13:50:18.000000 meer_tec-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 13:50:18.000000 meer_tec-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43437 2023-07-21 13:50:28.272042 meer_tec-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-21 13:50:18.000000 meer_tec-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:50:28.272042 meer_tec-0.0.4/meer_tec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:50:18.000000 meer_tec-0.0.4/meer_tec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 13:50:28.000000 meer_tec-0.0.4/meer_tec/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-07-21 13:50:18.000000 meer_tec-0.0.4/meer_tec/meer_tec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:50:28.272042 meer_tec-0.0.4/meer_tec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43437 2023-07-21 13:50:28.000000 meer_tec-0.0.4/meer_tec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-21 13:50:28.000000 meer_tec-0.0.4/meer_tec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:50:28.000000 meer_tec-0.0.4/meer_tec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-21 13:50:28.000000 meer_tec-0.0.4/meer_tec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 13:50:28.000000 meer_tec-0.0.4/meer_tec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-21 13:50:18.000000 meer_tec-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:50:28.272042 meer_tec-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:54:00.698021 meer_tec-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-25 13:53:48.000000 meer_tec-0.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:54:00.694020 meer_tec-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:54:00.694020 meer_tec-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-25 13:53:48.000000 meer_tec-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-25 13:53:48.000000 meer_tec-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-25 13:53:48.000000 meer_tec-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 13:53:48.000000 meer_tec-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43507 2023-07-25 13:54:00.698021 meer_tec-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-25 13:53:48.000000 meer_tec-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:54:00.698021 meer_tec-0.1.0/meer_tec/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 13:53:48.000000 meer_tec-0.1.0/meer_tec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 13:54:00.000000 meer_tec-0.1.0/meer_tec/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-07-25 13:53:48.000000 meer_tec-0.1.0/meer_tec/meer_tec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:54:00.698021 meer_tec-0.1.0/meer_tec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43507 2023-07-25 13:54:00.000000 meer_tec-0.1.0/meer_tec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-25 13:54:00.000000 meer_tec-0.1.0/meer_tec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:54:00.000000 meer_tec-0.1.0/meer_tec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-25 13:54:00.000000 meer_tec-0.1.0/meer_tec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 13:54:00.000000 meer_tec-0.1.0/meer_tec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-25 13:53:48.000000 meer_tec-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 13:54:00.698021 meer_tec-0.1.0/setup.cfg
```

### Comparing `meer_tec-0.0.4/.github/workflows/python-publish.yml` & `meer_tec-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `meer_tec-0.0.4/.gitignore` & `meer_tec-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `meer_tec-0.0.4/LICENSE` & `meer_tec-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meer_tec-0.0.4/PKG-INFO` & `meer_tec-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meer_tec
-Version: 0.0.4
+Version: 0.1.0
 Summary: MeCom for Python
 Author: Bastian Leykauf
 Author-email: leykauf@physik.hu-berlin.de
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -681,15 +681,15 @@
         
 Project-URL: homepage, https://github.com/bleykauf/meer_tec/
 Project-URL: repository, https://github.com/bleykauf/meer_tec/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # MeerTEC -- Python implemenation of the MeCom interface for Meerstetter TECs.
 
 <!---
@@ -702,14 +702,22 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Currently, only communication via ethernet is supported (tested only with [Lantronix XPort](https://www.lantronix.com/products/xport/)).
 Note that only a small subset of [MeCom](https://www.meerstetter.ch/customer-center/compendium/64-tec-controller-remote-control) is implemented at this time.
 
 ## Usage
 
+### USB
+
+```python
+usb = USB("COM3")
+tec = TEC(usb, 0)
+```
+
+### XPort
 Create a connection to the XPort and pass it as an argument to one of the TECs
 
 ```python
 xp = XPort('192.168.1.123')
 tec3 = TEC(xp, 3)
 ```
```

### Comparing `meer_tec-0.0.4/README.md` & `meer_tec-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Currently, only communication via ethernet is supported (tested only with [Lantronix XPort](https://www.lantronix.com/products/xport/)).
 Note that only a small subset of [MeCom](https://www.meerstetter.ch/customer-center/compendium/64-tec-controller-remote-control) is implemented at this time.
 
 ## Usage
 
+### USB
+
+```python
+usb = USB("COM3")
+tec = TEC(usb, 0)
+```
+
+### XPort
 Create a connection to the XPort and pass it as an argument to one of the TECs
 
 ```python
 xp = XPort('192.168.1.123')
 tec3 = TEC(xp, 3)
 ```
```

### Comparing `meer_tec-0.0.4/meer_tec.egg-info/PKG-INFO` & `meer_tec-0.1.0/meer_tec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meer-tec
-Version: 0.0.4
+Version: 0.1.0
 Summary: MeCom for Python
 Author: Bastian Leykauf
 Author-email: leykauf@physik.hu-berlin.de
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -681,15 +681,15 @@
         
 Project-URL: homepage, https://github.com/bleykauf/meer_tec/
 Project-URL: repository, https://github.com/bleykauf/meer_tec/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # MeerTEC -- Python implemenation of the MeCom interface for Meerstetter TECs.
 
 <!---
@@ -702,14 +702,22 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Currently, only communication via ethernet is supported (tested only with [Lantronix XPort](https://www.lantronix.com/products/xport/)).
 Note that only a small subset of [MeCom](https://www.meerstetter.ch/customer-center/compendium/64-tec-controller-remote-control) is implemented at this time.
 
 ## Usage
 
+### USB
+
+```python
+usb = USB("COM3")
+tec = TEC(usb, 0)
+```
+
+### XPort
 Create a connection to the XPort and pass it as an argument to one of the TECs
 
 ```python
 xp = XPort('192.168.1.123')
 tec3 = TEC(xp, 3)
 ```
```

### Comparing `meer_tec-0.0.4/pyproject.toml` & `meer_tec-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 description = "MeCom for Python"
 authors = [
   { name = "Bastian Leykauf" },
   { email = "leykauf@physik.hu-berlin.de" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
   "Intended Audience :: Science/Research",
 ]
-dependencies = ["pythoncrc>=0.10.0"]
+dependencies = ["pythoncrc>=0.10.0", "pyserial>=3.5"]
 dynamic = ["version"]
 
 [tool.setuptools_scm]
 write_to = "meer_tec/_version.py"
 
 [project.optional-dependencies]
 dev = [
```

