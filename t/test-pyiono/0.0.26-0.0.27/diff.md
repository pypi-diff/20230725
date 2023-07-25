# Comparing `tmp/test-pyiono-0.0.26.tar.gz` & `tmp/test-pyiono-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-pyiono-0.0.26.tar", last modified: Tue Jul 25 13:58:13 2023, max compression
+gzip compressed data, was "test-pyiono-0.0.27.tar", last modified: Tue Jul 25 14:03:08 2023, max compression
```

## Comparing `test-pyiono-0.0.26.tar` & `test-pyiono-0.0.27.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 13:58:13.115143 test-pyiono-0.0.26/
--rw-rw-r--   0 greg      (1000) greg      (1000)    11348 2023-07-25 08:35:45.000000 test-pyiono-0.0.26/LICENSE
--rw-rw-r--   0 greg      (1000) greg      (1000)    14948 2023-07-25 13:58:13.115143 test-pyiono-0.0.26/PKG-INFO
--rw-rw-r--   0 greg      (1000) greg      (1000)     1331 2023-07-25 13:24:19.000000 test-pyiono-0.0.26/README.md
--rw-rw-r--   0 greg      (1000) greg      (1000)     1655 2023-07-25 13:57:32.000000 test-pyiono-0.0.26/pyproject.toml
--rw-rw-r--   0 greg      (1000) greg      (1000)       38 2023-07-25 13:58:13.115143 test-pyiono-0.0.26/setup.cfg
--rw-rw-r--   0 greg      (1000) greg      (1000)       50 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/setup.py
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 13:58:13.111142 test-pyiono-0.0.26/src/
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 13:58:13.111142 test-pyiono-0.0.26/src/pyiono/
--rw-rw-r--   0 greg      (1000) greg      (1000)      125 2023-07-25 13:44:07.000000 test-pyiono-0.0.26/src/pyiono/__init__.py
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 13:58:13.111142 test-pyiono-0.0.26/src/pyiono/cli/
--rw-rw-r--   0 greg      (1000) greg      (1000)     3716 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/cli/GIMs_Helpers.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     7336 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/cli/GTMs.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     9776 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/cli/IPP.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    24364 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/cli/cli.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    23772 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/cli/download_madrigal.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    41247 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/cli/g_gnss.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    55996 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/cli/v_analysis.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    22671 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/cli/v_data.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    19082 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/cli/v_download.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    45639 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/cli/v_lsq.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    15387 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/cli/v_rps_results.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     5234 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/cli/v_vgos.py
--rw-rw-r--   0 greg      (1000) greg      (1000)      118 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/imports.py
--rw-rw-r--   0 greg      (1000) greg      (1000)      596 2023-07-25 13:58:08.000000 test-pyiono-0.0.26/src/pyiono/main.py
--rw-rw-r--   0 greg      (1000) greg      (1000)      698 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/math.py
--rw-rw-r--   0 greg      (1000) greg      (1000)      456 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/time.py
--rw-rw-r--   0 greg      (1000) greg      (1000)      543 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/transform.py
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 13:58:13.115143 test-pyiono-0.0.26/src/pyiono/vgos/
--rw-rw-r--   0 greg      (1000) greg      (1000)     5509 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/vgos/cli.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    23775 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/vgos/download_madrigal.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    26207 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/vgos/madrigalDownload.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    14615 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/vgos/v_download.py
--rw-rw-r--   0 greg      (1000) greg      (1000)   117252 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/src/pyiono/vgos/v_test.py
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 13:58:13.115143 test-pyiono-0.0.26/src/test_pyiono.egg-info/
--rw-rw-r--   0 greg      (1000) greg      (1000)    14948 2023-07-25 13:58:13.000000 test-pyiono-0.0.26/src/test_pyiono.egg-info/PKG-INFO
--rw-rw-r--   0 greg      (1000) greg      (1000)      897 2023-07-25 13:58:13.000000 test-pyiono-0.0.26/src/test_pyiono.egg-info/SOURCES.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)        1 2023-07-25 13:58:13.000000 test-pyiono-0.0.26/src/test_pyiono.egg-info/dependency_links.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)       39 2023-07-25 13:58:13.000000 test-pyiono-0.0.26/src/test_pyiono.egg-info/entry_points.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)      286 2023-07-25 13:58:13.000000 test-pyiono-0.0.26/src/test_pyiono.egg-info/requires.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)        7 2023-07-25 13:58:13.000000 test-pyiono-0.0.26/src/test_pyiono.egg-info/top_level.txt
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 13:58:13.115143 test-pyiono-0.0.26/tests/
--rw-rw-r--   0 greg      (1000) greg      (1000)      181 2023-07-25 12:36:35.000000 test-pyiono-0.0.26/tests/test_math.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 14:03:08.858465 test-pyiono-0.0.27/
+-rw-rw-r--   0 greg      (1000) greg      (1000)    11348 2023-07-25 08:35:45.000000 test-pyiono-0.0.27/LICENSE
+-rw-rw-r--   0 greg      (1000) greg      (1000)    14948 2023-07-25 14:03:08.858465 test-pyiono-0.0.27/PKG-INFO
+-rw-rw-r--   0 greg      (1000) greg      (1000)     1331 2023-07-25 13:24:19.000000 test-pyiono-0.0.27/README.md
+-rw-rw-r--   0 greg      (1000) greg      (1000)     1655 2023-07-25 14:03:00.000000 test-pyiono-0.0.27/pyproject.toml
+-rw-rw-r--   0 greg      (1000) greg      (1000)       38 2023-07-25 14:03:08.858465 test-pyiono-0.0.27/setup.cfg
+-rw-rw-r--   0 greg      (1000) greg      (1000)       50 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/setup.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 14:03:08.854465 test-pyiono-0.0.27/src/
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 14:03:08.854465 test-pyiono-0.0.27/src/pyiono/
+-rw-rw-r--   0 greg      (1000) greg      (1000)      125 2023-07-25 13:44:07.000000 test-pyiono-0.0.27/src/pyiono/__init__.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 14:03:08.858465 test-pyiono-0.0.27/src/pyiono/cli/
+-rw-rw-r--   0 greg      (1000) greg      (1000)     3716 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/cli/GIMs_Helpers.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)     7336 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/cli/GTMs.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)     9776 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/cli/IPP.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    24364 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/cli/cli.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    23772 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/cli/download_madrigal.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    41247 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/cli/g_gnss.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    55996 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/cli/v_analysis.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    22671 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/cli/v_data.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    19082 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/cli/v_download.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    45639 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/cli/v_lsq.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    15387 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/cli/v_rps_results.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)     5234 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/cli/v_vgos.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)      118 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/imports.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)      617 2023-07-25 13:59:27.000000 test-pyiono-0.0.27/src/pyiono/main.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)      698 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/math.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)      456 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/time.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)      543 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/transform.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 14:03:08.858465 test-pyiono-0.0.27/src/pyiono/vgos/
+-rw-rw-r--   0 greg      (1000) greg      (1000)     5509 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/vgos/cli.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    23775 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/vgos/download_madrigal.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    26207 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/vgos/madrigalDownload.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)    14615 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/vgos/v_download.py
+-rw-rw-r--   0 greg      (1000) greg      (1000)   117252 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/src/pyiono/vgos/v_test.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 14:03:08.858465 test-pyiono-0.0.27/src/test_pyiono.egg-info/
+-rw-rw-r--   0 greg      (1000) greg      (1000)    14948 2023-07-25 14:03:08.000000 test-pyiono-0.0.27/src/test_pyiono.egg-info/PKG-INFO
+-rw-rw-r--   0 greg      (1000) greg      (1000)      897 2023-07-25 14:03:08.000000 test-pyiono-0.0.27/src/test_pyiono.egg-info/SOURCES.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)        1 2023-07-25 14:03:08.000000 test-pyiono-0.0.27/src/test_pyiono.egg-info/dependency_links.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)       39 2023-07-25 14:03:08.000000 test-pyiono-0.0.27/src/test_pyiono.egg-info/entry_points.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)      286 2023-07-25 14:03:08.000000 test-pyiono-0.0.27/src/test_pyiono.egg-info/requires.txt
+-rw-rw-r--   0 greg      (1000) greg      (1000)        7 2023-07-25 14:03:08.000000 test-pyiono-0.0.27/src/test_pyiono.egg-info/top_level.txt
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-07-25 14:03:08.858465 test-pyiono-0.0.27/tests/
+-rw-rw-r--   0 greg      (1000) greg      (1000)      181 2023-07-25 12:36:35.000000 test-pyiono-0.0.27/tests/test_math.py
```

### Comparing `test-pyiono-0.0.26/LICENSE` & `test-pyiono-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/PKG-INFO` & `test-pyiono-0.0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-pyiono
-Version: 0.0.26
+Version: 0.0.27
 Summary: Ionosphere-related processing based on the input from space-geodetic data
 Author-email: Grzegorz Kłopotek <klpotek@ethz.ch>, Mudathir Awadaljeed <mudathir.awadaljeed@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `test-pyiono-0.0.26/README.md` & `test-pyiono-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/pyproject.toml` & `test-pyiono-0.0.27/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "test-pyiono"
-version = "0.0.26"
+version = "0.0.27"
 description = "Ionosphere-related processing based on the input from space-geodetic data"
 readme = "README.md"
 authors = [{ name = "Grzegorz Kłopotek", email = "klpotek@ethz.ch" },{ name = "Mudathir Awadaljeed", email = "mudathir.awadaljeed@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
 "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
@@ -35,15 +35,15 @@
 [project.optional-dependencies]
 dev = [ "bumpver", "pip-tools", "pytest","tox", "pytest-cov", "pytest-asyncio", "coverage", "sphinx", "sphinx-rtd-theme","sphinx-autoapi", "m2r2"]
 
 [project.urls]
 Homepage = "https://gitlab.ethz.ch/space-geodesy-open/pyiono"
 
 [project.scripts]
-pyiono = "pyiono:main"
+pyiono = "pyiono.main"
 
 [tool.bumpver]
 current_version = "0.0.10"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
```

### Comparing `test-pyiono-0.0.26/src/pyiono/cli/GIMs_Helpers.py` & `test-pyiono-0.0.27/src/pyiono/cli/GIMs_Helpers.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/cli/GTMs.py` & `test-pyiono-0.0.27/src/pyiono/cli/GTMs.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/cli/IPP.py` & `test-pyiono-0.0.27/src/pyiono/cli/IPP.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/cli/cli.py` & `test-pyiono-0.0.27/src/pyiono/cli/cli.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/cli/download_madrigal.py` & `test-pyiono-0.0.27/src/pyiono/cli/download_madrigal.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/cli/g_gnss.py` & `test-pyiono-0.0.27/src/pyiono/cli/g_gnss.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/cli/v_analysis.py` & `test-pyiono-0.0.27/src/pyiono/cli/v_analysis.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/cli/v_data.py` & `test-pyiono-0.0.27/src/pyiono/cli/v_data.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/cli/v_download.py` & `test-pyiono-0.0.27/src/pyiono/cli/v_download.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/cli/v_lsq.py` & `test-pyiono-0.0.27/src/pyiono/cli/v_lsq.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/cli/v_rps_results.py` & `test-pyiono-0.0.27/src/pyiono/cli/v_rps_results.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/cli/v_vgos.py` & `test-pyiono-0.0.27/src/pyiono/cli/v_vgos.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/math.py` & `test-pyiono-0.0.27/src/pyiono/math.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/transform.py` & `test-pyiono-0.0.27/src/pyiono/transform.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/vgos/cli.py` & `test-pyiono-0.0.27/src/pyiono/vgos/cli.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/vgos/download_madrigal.py` & `test-pyiono-0.0.27/src/pyiono/vgos/download_madrigal.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/vgos/madrigalDownload.py` & `test-pyiono-0.0.27/src/pyiono/vgos/madrigalDownload.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/vgos/v_download.py` & `test-pyiono-0.0.27/src/pyiono/vgos/v_download.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/pyiono/vgos/v_test.py` & `test-pyiono-0.0.27/src/pyiono/vgos/v_test.py`

 * *Files identical despite different names*

### Comparing `test-pyiono-0.0.26/src/test_pyiono.egg-info/PKG-INFO` & `test-pyiono-0.0.27/src/test_pyiono.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-pyiono
-Version: 0.0.26
+Version: 0.0.27
 Summary: Ionosphere-related processing based on the input from space-geodetic data
 Author-email: Grzegorz Kłopotek <klpotek@ethz.ch>, Mudathir Awadaljeed <mudathir.awadaljeed@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `test-pyiono-0.0.26/src/test_pyiono.egg-info/SOURCES.txt` & `test-pyiono-0.0.27/src/test_pyiono.egg-info/SOURCES.txt`

 * *Files identical despite different names*

