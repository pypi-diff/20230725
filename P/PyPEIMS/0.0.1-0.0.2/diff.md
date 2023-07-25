# Comparing `tmp/pypeims-0.0.1.tar.gz` & `tmp/pypeims-0.0.2.tar.gz`

## Comparing `pypeims-0.0.1.tar` & `pypeims-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypeims-0.0.1/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypeims-0.0.1/requirements.txt
--rw-r--r--   0        0        0    84075 2020-02-02 00:00:00.000000 pypeims-0.0.1/src/data/Special Education Funding Gap/SPED data request_SY2021_3.6.2023_ORIGINAL.xlsx
--rw-r--r--   0        0        0   190464 2020-02-02 00:00:00.000000 pypeims-0.0.1/src/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_ORIGINAL.xls
--rw-r--r--   0        0        0    72044 2020-02-02 00:00:00.000000 pypeims-0.0.1/src/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_PROCESSED.xlsx
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 pypeims-0.0.1/src/instruments/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypeims-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 pypeims-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pypeims-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pypeims-0.0.1/README.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypeims-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pypeims-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypeims-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0    84075 2020-02-02 00:00:00.000000 pypeims-0.0.2/src/data/Special Education Funding Gap/SPED data request_SY2021_3.6.2023_ORIGINAL.xlsx
+-rw-r--r--   0        0        0   190464 2020-02-02 00:00:00.000000 pypeims-0.0.2/src/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_ORIGINAL.xls
+-rw-r--r--   0        0        0    72044 2020-02-02 00:00:00.000000 pypeims-0.0.2/src/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_PROCESSED.xlsx
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypeims-0.0.2/src/instruments/__init__.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 pypeims-0.0.2/src/instruments/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypeims-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 pypeims-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pypeims-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pypeims-0.0.2/README.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pypeims-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 pypeims-0.0.2/PKG-INFO
```

### Comparing `pypeims-0.0.1/src/data/Special Education Funding Gap/SPED data request_SY2021_3.6.2023_ORIGINAL.xlsx` & `pypeims-0.0.2/src/data/Special Education Funding Gap/SPED data request_SY2021_3.6.2023_ORIGINAL.xlsx`

 * *Files identical despite different names*

### Comparing `pypeims-0.0.1/src/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_ORIGINAL.xls` & `pypeims-0.0.2/src/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_ORIGINAL.xls`

 * *Files identical despite different names*

### Comparing `pypeims-0.0.1/src/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_PROCESSED.xlsx` & `pypeims-0.0.2/src/data/Special Education Funding Gap/SPED data request_SY2022_3.14.2023_PROCESSED.xlsx`

 * *Files identical despite different names*

### Comparing `pypeims-0.0.1/src/instruments/utils.py` & `pypeims-0.0.2/src/instruments/utils.py`

 * *Files identical despite different names*

### Comparing `pypeims-0.0.1/.gitignore` & `pypeims-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pypeims-0.0.1/LICENSE.txt` & `pypeims-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypeims-0.0.1/pyproject.toml` & `pypeims-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,32 @@
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
 [project]
 name = "PyPEIMS"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Alejandro Peña", email="adpena@gmail.com" },
 ]
 description = "Defining classes and functions for accessing and manipulating Texas PEIMS data (including data in TAPR and statistics typically accessed through Snapshot) programmatically."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-[project.urls]
-"Homepage" = "https://github.com/adpena/PyPEIMS"
+dependencies = [
+    "pandas",
+    "csv",
+]
 
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+[project.urls]
+"Source" = "https://github.com/adpena/PyPEIMS"
 
-[tool]
+[tool.hatch.build.targets.sdist]
+include = [
+  "/src",
+  "/tests",
+]
```

### Comparing `pypeims-0.0.1/PKG-INFO` & `pypeims-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: PyPEIMS
-Version: 0.0.1
+Version: 0.0.2
 Summary: Defining classes and functions for accessing and manipulating Texas PEIMS data (including data in TAPR and statistics typically accessed through Snapshot) programmatically.
-Project-URL: Homepage, https://github.com/adpena/PyPEIMS
+Project-URL: Source, https://github.com/adpena/PyPEIMS
 Author-email: Alejandro Peña <adpena@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: csv
+Requires-Dist: pandas
 Description-Content-Type: text/markdown
 
 ### PyPEIMS README
 
 07/25/2023 - adpena@gmail.com
```

