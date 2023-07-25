# Comparing `tmp/pyiono-0.0.10.tar.gz` & `tmp/pyiono-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiono-0.0.10.tar", last modified: Tue Jul 25 12:59:19 2023, max compression
+gzip compressed data, was "pyiono-0.1.0.tar", last modified: Tue Jul 25 14:35:42 2023, max compression
```

## Comparing `pyiono-0.0.10.tar` & `pyiono-0.1.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 12:59:19.685361 pyiono-0.0.10/
--rw-rw-r--   0 greg      (1000) greg      (1000)    11348 2023-07-25 08:35:45.000000 pyiono-0.0.10/LICENSE
--rw-rw-r--   0 greg      (1000) greg      (1000)    14935 2023-07-25 12:59:19.685361 pyiono-0.0.10/PKG-INFO
--rw-rw-r--   0 greg      (1000) greg      (1000)     1323 2023-07-25 12:50:49.000000 pyiono-0.0.10/README.md
--rw-rw-r--   0 greg      (1000) greg      (1000)     1576 2023-07-25 12:57:45.000000 pyiono-0.0.10/pyproject.toml
--rw-rw-r--   0 greg      (1000) greg      (1000)       38 2023-07-25 12:59:19.685361 pyiono-0.0.10/setup.cfg
--rw-rw-r--   0 greg      (1000) greg      (1000)       50 2023-07-25 12:36:35.000000 pyiono-0.0.10/setup.py
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 12:59:19.673360 pyiono-0.0.10/src/
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 12:59:19.677360 pyiono-0.0.10/src/pyiono/
--rw-rw-r--   0 greg      (1000) greg      (1000)      125 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/__init__.py
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 12:59:19.681360 pyiono-0.0.10/src/pyiono/cli/
--rw-rw-r--   0 greg      (1000) greg      (1000)     3716 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/cli/GIMs_Helpers.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     7336 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/cli/GTMs.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     9776 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/cli/IPP.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    24364 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/cli/cli.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    23772 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/cli/download_madrigal.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    41247 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/cli/g_gnss.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    55996 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/cli/v_analysis.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    22671 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/cli/v_data.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    19082 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/cli/v_download.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    45639 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/cli/v_lsq.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    15387 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/cli/v_rps_results.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     5234 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/cli/v_vgos.py
--rw-rw-r--   0 greg      (1000) greg      (1000)      118 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/imports.py
--rw-rw-r--   0 greg      (1000) greg      (1000)      143 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/main.py
--rw-rw-r--   0 greg      (1000) greg      (1000)      698 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/math.py
--rw-rw-r--   0 greg      (1000) greg      (1000)      456 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/time.py
--rw-rw-r--   0 greg      (1000) greg      (1000)      543 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/transform.py
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 12:59:19.681360 pyiono-0.0.10/src/pyiono/vgos/
--rw-rw-r--   0 greg      (1000) greg      (1000)     5509 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/vgos/cli.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    23775 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/vgos/download_madrigal.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    26207 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/vgos/madrigalDownload.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    14615 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/vgos/v_download.py
--rw-rw-r--   0 greg      (1000) greg      (1000)   117252 2023-07-25 12:36:35.000000 pyiono-0.0.10/src/pyiono/vgos/v_test.py
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 12:59:19.681360 pyiono-0.0.10/src/pyiono.egg-info/
--rw-rw-r--   0 greg      (1000) greg      (1000)    14935 2023-07-25 12:59:19.000000 pyiono-0.0.10/src/pyiono.egg-info/PKG-INFO
--rw-rw-r--   0 greg      (1000) greg      (1000)      830 2023-07-25 12:59:19.000000 pyiono-0.0.10/src/pyiono.egg-info/SOURCES.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)        1 2023-07-25 12:59:19.000000 pyiono-0.0.10/src/pyiono.egg-info/dependency_links.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)      286 2023-07-25 12:59:19.000000 pyiono-0.0.10/src/pyiono.egg-info/requires.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)        7 2023-07-25 12:59:19.000000 pyiono-0.0.10/src/pyiono.egg-info/top_level.txt
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 12:59:19.681360 pyiono-0.0.10/tests/
--rw-rw-r--   0 greg      (1000) greg      (1000)      181 2023-07-25 12:36:35.000000 pyiono-0.0.10/tests/test_math.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 14:35:42.255078 pyiono-0.1.0/
+-rw-rw-r--   0 greg      (1000) greg      (1000)    11348 2023-07-25 08:35:45.000000 pyiono-0.1.0/LICENSE
+-rw-rw-r--   0 greg      (1000) greg      (1000)    14942 2023-07-25 14:35:42.255078 pyiono-0.1.0/PKG-INFO
+-rw-rw-r--   0 greg      (1000) greg      (1000)     1331 2023-07-25 14:19:17.000000 pyiono-0.1.0/README.md
+-rw-rw-r--   0 greg      (1000) greg      (1000)     1657 2023-07-25 14:32:01.000000 pyiono-0.1.0/pyproject.toml
+-rw-rw-r--   0 greg      (1000) greg      (1000)       38 2023-07-25 14:35:42.255078 pyiono-0.1.0/setup.cfg
+-rw-rw-r--   0 greg      (1000) greg      (1000)       50 2023-07-25 12:36:35.000000 pyiono-0.1.0/setup.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 14:35:42.251078 pyiono-0.1.0/src/
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 14:35:42.251078 pyiono-0.1.0/src/pyiono/
+-rw-rw-r--   0 greg      (1000) greg      (1000)      124 2023-07-25 14:19:26.000000 pyiono-0.1.0/src/pyiono/__init__.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)      873 2023-07-25 14:19:20.000000 pyiono-0.1.0/src/pyiono/__main__.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 14:35:42.255078 pyiono-0.1.0/src/pyiono/cli/
+-rw-rw-r--   0 greg      (1000) greg      (1000)     3716 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/cli/GIMs_Helpers.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)     7336 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/cli/GTMs.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)     9776 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/cli/IPP.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    24364 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/cli/cli.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    23772 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/cli/download_madrigal.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    41247 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/cli/g_gnss.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    55996 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/cli/v_analysis.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    22671 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/cli/v_data.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    19082 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/cli/v_download.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    45639 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/cli/v_lsq.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    15387 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/cli/v_rps_results.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)     5234 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/cli/v_vgos.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)      118 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/imports.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)      698 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/math.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)      456 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/time.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)      543 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/transform.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 14:35:42.255078 pyiono-0.1.0/src/pyiono/vgos/
+-rw-rw-r--   0 greg      (1000) greg      (1000)     5509 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/vgos/cli.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    23775 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/vgos/download_madrigal.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    26207 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/vgos/madrigalDownload.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    14615 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/vgos/v_download.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)   117252 2023-07-25 12:36:35.000000 pyiono-0.1.0/src/pyiono/vgos/v_test.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 14:35:42.255078 pyiono-0.1.0/src/pyiono.egg-info/
+-rw-rw-r--   0 greg      (1000) greg      (1000)    14942 2023-07-25 14:35:42.000000 pyiono-0.1.0/src/pyiono.egg-info/PKG-INFO
+-rw-rw-r--   0 greg      (1000) greg      (1000)      871 2023-07-25 14:35:42.000000 pyiono-0.1.0/src/pyiono.egg-info/SOURCES.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)        1 2023-07-25 14:35:42.000000 pyiono-0.1.0/src/pyiono.egg-info/dependency_links.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)       48 2023-07-25 14:35:42.000000 pyiono-0.1.0/src/pyiono.egg-info/entry_points.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)      286 2023-07-25 14:35:42.000000 pyiono-0.1.0/src/pyiono.egg-info/requires.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)        7 2023-07-25 14:35:42.000000 pyiono-0.1.0/src/pyiono.egg-info/top_level.txt
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 14:35:42.255078 pyiono-0.1.0/tests/
+-rw-rw-r--   0 greg      (1000) greg      (1000)      181 2023-07-25 12:36:35.000000 pyiono-0.1.0/tests/test_math.py
```

### Comparing `pyiono-0.0.10/LICENSE` & `pyiono-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/PKG-INFO` & `pyiono-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiono
-Version: 0.0.10
+Version: 0.1.0
 Summary: Ionosphere-related processing based on the input from space-geodetic data
 Author-email: Grzegorz Kłopotek <klpotek@ethz.ch>, Mudathir Awadaljeed <mudathir.awadaljeed@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -233,18 +233,24 @@
     python3 -m pip install pyiono
 
 PyIono is supported on Python 3.9 and above.
 
 ## How to use
 
 
-PyIono is a command line application, named `pyiono`. To see a list of the arguments, call the program without any arguments:
+PyIono is a command line application, named `pyiono`. To see a list of the arguments, call help:
 
 ```bash
-$ pyiono
+$ pyiono --help
+```
+
+or 
+
+```bash
+$ pyiono -h
 ```
 
 You can also call PyIono in your own Python code, by importing from the `pyiono` package:
 
 ```python
  from pyiono.math import square
  square(2)
```

### Comparing `pyiono-0.0.10/README.md` & `pyiono-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,18 +15,24 @@
     python3 -m pip install pyiono
 
 PyIono is supported on Python 3.9 and above.
 
 ## How to use
 
 
-PyIono is a command line application, named `pyiono`. To see a list of the arguments, call the program without any arguments:
+PyIono is a command line application, named `pyiono`. To see a list of the arguments, call help:
 
 ```bash
-$ pyiono
+$ pyiono --help
+```
+
+or 
+
+```bash
+$ pyiono -h
 ```
 
 You can also call PyIono in your own Python code, by importing from the `pyiono` package:
 
 ```python
  from pyiono.math import square
  square(2)
```

### Comparing `pyiono-0.0.10/pyproject.toml` & `pyiono-0.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyiono"
-version = "0.0.10"
+version = "0.1.0"
 description = "Ionosphere-related processing based on the input from space-geodetic data"
 readme = "README.md"
 authors = [{ name = "Grzegorz Kłopotek", email = "klpotek@ethz.ch" },{ name = "Mudathir Awadaljeed", email = "mudathir.awadaljeed@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
 "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
@@ -35,21 +35,23 @@
 [project.optional-dependencies]
 dev = [ "bumpver", "pip-tools", "pytest","tox", "pytest-cov", "pytest-asyncio", "coverage", "sphinx", "sphinx-rtd-theme","sphinx-autoapi", "m2r2"]
 
 [project.urls]
 Homepage = "https://gitlab.ethz.ch/space-geodesy-open/pyiono"
 
 [project.scripts]
+pyiono = "pyiono.__main__:main"
 
 [tool.bumpver]
-current_version = "0.0.10"
+current_version = "0.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"src/pyiono/__init__.py" = ["{version}"]
+"src/pyiono/__init__.py" = ["{version}"]
+"src/pyiono/__main__.py" = ["- pyiono v{version}"]
```

### Comparing `pyiono-0.0.10/src/pyiono/cli/GIMs_Helpers.py` & `pyiono-0.1.0/src/pyiono/cli/GIMs_Helpers.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/cli/GTMs.py` & `pyiono-0.1.0/src/pyiono/cli/GTMs.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/cli/IPP.py` & `pyiono-0.1.0/src/pyiono/cli/IPP.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/cli/cli.py` & `pyiono-0.1.0/src/pyiono/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/cli/download_madrigal.py` & `pyiono-0.1.0/src/pyiono/cli/download_madrigal.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/cli/g_gnss.py` & `pyiono-0.1.0/src/pyiono/cli/g_gnss.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/cli/v_analysis.py` & `pyiono-0.1.0/src/pyiono/cli/v_analysis.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/cli/v_data.py` & `pyiono-0.1.0/src/pyiono/cli/v_data.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/cli/v_download.py` & `pyiono-0.1.0/src/pyiono/cli/v_download.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/cli/v_lsq.py` & `pyiono-0.1.0/src/pyiono/cli/v_lsq.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/cli/v_rps_results.py` & `pyiono-0.1.0/src/pyiono/cli/v_rps_results.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/cli/v_vgos.py` & `pyiono-0.1.0/src/pyiono/cli/v_vgos.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/math.py` & `pyiono-0.1.0/src/pyiono/math.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/transform.py` & `pyiono-0.1.0/src/pyiono/transform.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/vgos/cli.py` & `pyiono-0.1.0/src/pyiono/vgos/cli.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/vgos/download_madrigal.py` & `pyiono-0.1.0/src/pyiono/vgos/download_madrigal.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/vgos/madrigalDownload.py` & `pyiono-0.1.0/src/pyiono/vgos/madrigalDownload.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/vgos/v_download.py` & `pyiono-0.1.0/src/pyiono/vgos/v_download.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono/vgos/v_test.py` & `pyiono-0.1.0/src/pyiono/vgos/v_test.py`

 * *Files identical despite different names*

### Comparing `pyiono-0.0.10/src/pyiono.egg-info/PKG-INFO` & `pyiono-0.1.0/src/pyiono.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiono
-Version: 0.0.10
+Version: 0.1.0
 Summary: Ionosphere-related processing based on the input from space-geodetic data
 Author-email: Grzegorz Kłopotek <klpotek@ethz.ch>, Mudathir Awadaljeed <mudathir.awadaljeed@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -233,18 +233,24 @@
     python3 -m pip install pyiono
 
 PyIono is supported on Python 3.9 and above.
 
 ## How to use
 
 
-PyIono is a command line application, named `pyiono`. To see a list of the arguments, call the program without any arguments:
+PyIono is a command line application, named `pyiono`. To see a list of the arguments, call help:
 
 ```bash
-$ pyiono
+$ pyiono --help
+```
+
+or 
+
+```bash
+$ pyiono -h
 ```
 
 You can also call PyIono in your own Python code, by importing from the `pyiono` package:
 
 ```python
  from pyiono.math import square
  square(2)
```

### Comparing `pyiono-0.0.10/src/pyiono.egg-info/SOURCES.txt` & `pyiono-0.1.0/src/pyiono.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/pyiono/__init__.py
+src/pyiono/__main__.py
 src/pyiono/imports.py
-src/pyiono/main.py
 src/pyiono/math.py
 src/pyiono/time.py
 src/pyiono/transform.py
 src/pyiono.egg-info/PKG-INFO
 src/pyiono.egg-info/SOURCES.txt
 src/pyiono.egg-info/dependency_links.txt
+src/pyiono.egg-info/entry_points.txt
 src/pyiono.egg-info/requires.txt
 src/pyiono.egg-info/top_level.txt
 src/pyiono/cli/GIMs_Helpers.py
 src/pyiono/cli/GTMs.py
 src/pyiono/cli/IPP.py
 src/pyiono/cli/cli.py
 src/pyiono/cli/download_madrigal.py
```

