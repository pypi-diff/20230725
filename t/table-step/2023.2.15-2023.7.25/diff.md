# Comparing `tmp/table_step-2023.2.15.tar.gz` & `tmp/table_step-2023.7.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "table_step-2023.2.15.tar", last modified: Wed Feb 15 18:01:03 2023, max compression
+gzip compressed data, was "table_step-2023.7.25.tar", last modified: Tue Jul 25 19:48:05 2023, max compression
```

## Comparing `table_step-2023.2.15.tar` & `table_step-2023.7.25.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:01:03.377525 table_step-2023.2.15/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-15 18:00:47.000000 table_step-2023.2.15/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-02-15 18:00:47.000000 table_step-2023.2.15/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-02-15 18:00:47.000000 table_step-2023.2.15/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-02-15 18:00:47.000000 table_step-2023.2.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-15 18:00:47.000000 table_step-2023.2.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-02-15 18:01:03.377525 table_step-2023.2.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-02-15 18:00:47.000000 table_step-2023.2.15/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:01:03.373525 table_step-2023.2.15/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:01:03.373525 table_step-2023.2.15/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:01:03.373525 table_step-2023.2.15/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9577 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:01:03.373525 table_step-2023.2.15/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:01:03.373525 table_step-2023.2.15/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:01:03.373525 table_step-2023.2.15/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-15 18:00:47.000000 table_step-2023.2.15/docs/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-15 18:01:03.381525 table_step-2023.2.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-02-15 18:00:47.000000 table_step-2023.2.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:01:03.381525 table_step-2023.2.15/table_step/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-02-15 18:00:47.000000 table_step-2023.2.15/table_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-15 18:01:03.381525 table_step-2023.2.15/table_step/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23436 2023-02-15 18:00:47.000000 table_step-2023.2.15/table_step/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-02-15 18:00:47.000000 table_step-2023.2.15/table_step/table_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-02-15 18:00:47.000000 table_step-2023.2.15/table_step/table_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-02-15 18:00:47.000000 table_step-2023.2.15/table_step/tk_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:01:03.377525 table_step-2023.2.15/table_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-02-15 18:01:03.000000 table_step-2023.2.15/table_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-02-15 18:01:03.000000 table_step-2023.2.15/table_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 18:01:03.000000 table_step-2023.2.15/table_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-15 18:01:03.000000 table_step-2023.2.15/table_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-15 18:01:03.000000 table_step-2023.2.15/table_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-15 18:01:03.000000 table_step-2023.2.15/table_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 18:00:49.000000 table_step-2023.2.15/table_step.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:01:03.377525 table_step-2023.2.15/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-15 18:00:47.000000 table_step-2023.2.15/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-02-15 18:00:47.000000 table_step-2023.2.15/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:01:03.377525 table_step-2023.2.15/tests/flowcharts/
--rwxr-xr-x   0 runner    (1001) docker     (123)    38744 2023-02-15 18:00:47.000000 table_step-2023.2.15/tests/flowcharts/test1.flow
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-15 18:00:47.000000 table_step-2023.2.15/tests/test_flowcharts.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-15 18:00:47.000000 table_step-2023.2.15/tests/test_table_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:05.653726 table_step-2023.7.25/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-25 19:47:40.000000 table_step-2023.7.25/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-25 19:47:40.000000 table_step-2023.7.25/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-25 19:47:40.000000 table_step-2023.7.25/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-25 19:47:40.000000 table_step-2023.7.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-25 19:47:40.000000 table_step-2023.7.25/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-25 19:48:05.653726 table_step-2023.7.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-25 19:47:40.000000 table_step-2023.7.25/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:05.649726 table_step-2023.7.25/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:05.649726 table_step-2023.7.25/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:05.649726 table_step-2023.7.25/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9577 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:05.649726 table_step-2023.7.25/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:05.653726 table_step-2023.7.25/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:05.653726 table_step-2023.7.25/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-25 19:47:40.000000 table_step-2023.7.25/docs/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-25 19:48:05.657726 table_step-2023.7.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-25 19:47:40.000000 table_step-2023.7.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:05.657726 table_step-2023.7.25/table_step/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-25 19:47:40.000000 table_step-2023.7.25/table_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-25 19:48:05.657726 table_step-2023.7.25/table_step/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24071 2023-07-25 19:47:40.000000 table_step-2023.7.25/table_step/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-25 19:47:40.000000 table_step-2023.7.25/table_step/table_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-25 19:47:40.000000 table_step-2023.7.25/table_step/table_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-07-25 19:47:40.000000 table_step-2023.7.25/table_step/tk_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:05.653726 table_step-2023.7.25/table_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-25 19:48:05.000000 table_step-2023.7.25/table_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-25 19:48:05.000000 table_step-2023.7.25/table_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:48:05.000000 table_step-2023.7.25/table_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 19:48:05.000000 table_step-2023.7.25/table_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-25 19:48:05.000000 table_step-2023.7.25/table_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 19:48:05.000000 table_step-2023.7.25/table_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:47:45.000000 table_step-2023.7.25/table_step.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:05.653726 table_step-2023.7.25/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 19:47:40.000000 table_step-2023.7.25/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-25 19:47:40.000000 table_step-2023.7.25/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:05.653726 table_step-2023.7.25/tests/flowcharts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38744 2023-07-25 19:47:40.000000 table_step-2023.7.25/tests/flowcharts/test1.flow
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-25 19:47:40.000000 table_step-2023.7.25/tests/test_flowcharts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-25 19:47:40.000000 table_step-2023.7.25/tests/test_table_step.py
```

### Comparing `table_step-2023.2.15/CONTRIBUTING.rst` & `table_step-2023.7.25/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/HISTORY.rst` & `table_step-2023.7.25/HISTORY.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+2023.7.25 -- Bug fix and Enhancements
+    * Fixed bug with reading table using a variable for the filename, but asking for the
+      type from the extension.
+    * Add ability to save tables with a frequency of other than ever call.
+      
 2023.2.15 -- Bugs fixes and documentation
     * Restructured documentation and moved to new theme
     * Fixed bug with access rows of tables with non-integer indexes as well as "current"
       index 
     * Added support for lists of tables in pulldowns in the GUI
       
 2021.12.22 -- Improved the handling of index columns, added formats.
```

### Comparing `table_step-2023.2.15/LICENSE` & `table_step-2023.7.25/LICENSE`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/PKG-INFO` & `table_step-2023.7.25/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: table_step
-Version: 2023.2.15
+Version: 2023.7.25
 Summary: A SEAMM plug-in for data tables in a flowchart.
 Home-page: https://github.com/molssi-seamm/table_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,table,data,csv
 Platform: Linux
@@ -87,14 +87,19 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.7.25 -- Bug fix and Enhancements
+    * Fixed bug with reading table using a variable for the filename, but asking for the
+      type from the extension.
+    * Add ability to save tables with a frequency of other than ever call.
+      
 2023.2.15 -- Bugs fixes and documentation
     * Restructured documentation and moved to new theme
     * Fixed bug with access rows of tables with non-integer indexes as well as "current"
       index 
     * Added support for lists of tables in pulldowns in the GUI
       
 2021.12.22 -- Improved the handling of index columns, added formats.
```

### Comparing `table_step-2023.2.15/README.rst` & `table_step-2023.7.25/README.rst`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/docs/Makefile` & `table_step-2023.7.25/docs/Makefile`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/docs/_static/SEAMM inverted.png` & `table_step-2023.7.25/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/docs/_static/SEAMM logo.png` & `table_step-2023.7.25/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/docs/_static/molssi_main_logo.png` & `table_step-2023.7.25/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/docs/_static/molssi_main_logo_inverted_white.png` & `table_step-2023.7.25/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/docs/_static/molssi_square.png` & `table_step-2023.7.25/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/docs/_static/nsf.png` & `table_step-2023.7.25/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/docs/conf.py` & `table_step-2023.7.25/docs/conf.py`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/docs/developer_guide/installation.rst` & `table_step-2023.7.25/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/docs/getting_started/index.rst` & `table_step-2023.7.25/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/docs/index.rst` & `table_step-2023.7.25/docs/index.rst`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/docs/make.bat` & `table_step-2023.7.25/docs/make.bat`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/setup.py` & `table_step-2023.7.25/setup.py`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/table_step/__init__.py` & `table_step-2023.7.25/table_step/__init__.py`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/table_step/table.py` & `table_step-2023.7.25/table_step/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         # Initialize our parent class
         super().__init__(
             flowchart=flowchart, title="Table", extension=extension, logger=logger
         )
 
         # This needs to be after initializing subclasses...
         self.parameters = table_step.TableParameters()
+        self.calls = 0
 
     @property
     def version(self):
         """The semantic version of this module."""
         return table_step.__version__
 
     @property
@@ -83,25 +84,31 @@
                         table["Default"].append(d["default"])
             for tmp in tabulate(table, headers="keys", tablefmt="grid").splitlines():
                 lines.append(8 * " " + tmp)
         elif method == "Read":
             filename = P["filename"]
             file_type = P["file type"]
             if file_type == "from extension":
-                file_type = PurePath(filename).suffix
-                if file_type not in self.parameters["file type"].enumeration:
-                    types = "', '".join(self.parameters["file type"].enumeration)
-                    raise RuntimeError(
-                        f"Cannot handle files of type '{file_type}' when reading "
-                        f"table '{tablename}'.\nKnown types: '{types}'"
+                if isinstance(filename, str) and self.is_expr(filename):
+                    lines.append(
+                        f"        File: from variable '{filename}' with type from the "
+                        "extension"
+                    )
+                else:
+                    file_type = PurePath(filename).suffix
+                    if file_type not in self.parameters["file type"].enumeration:
+                        types = "', '".join(self.parameters["file type"].enumeration)
+                        raise RuntimeError(
+                            f"Cannot handle files of type '{file_type}' when reading "
+                            f"table '{tablename}'.\nKnown types: '{types}'"
+                        )
+                    lines.append(
+                        f"         File: '{filename}' with type '{file_type}' from the "
+                        "extension."
                     )
-                lines.append(
-                    f"         File: '{filename}' with type '{file_type}' from the "
-                    "extension."
-                )
             else:
                 lines.append(f"         File: '{filename}' with type '{file_type}'")
         elif method == "Save":
             pass
         elif method == "Save as":
             filename = P["filename"]
             file_type = P["file type"]
@@ -310,70 +317,72 @@
                     "loop index": False,
                     "current index": 0,
                 },
             )
 
             self.logger.info("Successfully read table from {}".format(filename))
         elif P["method"] == "Save" or P["method"] == "Save as":
-            if not self.variable_exists(tablename):
-                raise RuntimeError(
-                    "Table save: table '{}' does not exist.".format(tablename)
-                )
-            file_type = P["file type"]
-            table_handle = self.get_variable(tablename)
-            table = table_handle["table"]
-            if P["method"] == "Save as":
-                filename = P["filename"]
-                table_handle["filename"] = filename
-            else:
-                if "filename" not in table_handle:
-                    if file_type == "from extension":
-                        file_type = ".csv"
-                    table_handle["filename"] = os.path.join(
-                        self.flowchart.root_directory, tablename + file_type
-                    )
-                filename = table_handle["filename"]
-
-            index = table_handle["index column"]
-
-            if file_type == "from extension":
-                file_type = PurePath(filename).suffix
-                if file_type not in self.parameters["file type"].enumeration:
-                    types = "', '".join(self.parameters["file type"].enumeration)
+            self.calls += 1
+            if self.calls % P["frequency"] == 0:
+                if not self.variable_exists(tablename):
                     raise RuntimeError(
-                        f"Cannot handle files of type '{file_type}' when writing "
-                        f"table '{tablename}'.\nKnown types: '{types}'"
+                        "Table save: table '{}' does not exist.".format(tablename)
                     )
-            if file_type == ".csv":
-                if index is None:
-                    table.to_csv(filename, index=False)
-                else:
-                    table.to_csv(filename, index=True, header=True)
-            elif file_type == ".json":
-                if index is None:
-                    table.to_json(filename, indent=4, orient="table", index=False)
+                file_type = P["file type"]
+                table_handle = self.get_variable(tablename)
+                table = table_handle["table"]
+                if P["method"] == "Save as":
+                    filename = P["filename"]
+                    table_handle["filename"] = filename
                 else:
-                    table.to_json(filename, indent=4, orient="table", index=True)
-            elif file_type == ".xlsx":
-                if index is None:
-                    table.to_excel(filename, index=False)
-                else:
-                    table.to_excel(filename, index=True)
-            elif file_type == ".txt":
-                with open(filename, "w") as fd:
+                    if "filename" not in table_handle:
+                        if file_type == "from extension":
+                            file_type = ".csv"
+                        table_handle["filename"] = os.path.join(
+                            self.flowchart.root_directory, tablename + file_type
+                        )
+                    filename = table_handle["filename"]
+
+                index = table_handle["index column"]
+
+                if file_type == "from extension":
+                    file_type = PurePath(filename).suffix
+                    if file_type not in self.parameters["file type"].enumeration:
+                        types = "', '".join(self.parameters["file type"].enumeration)
+                        raise RuntimeError(
+                            f"Cannot handle files of type '{file_type}' when writing "
+                            f"table '{tablename}'.\nKnown types: '{types}'"
+                        )
+                if file_type == ".csv":
                     if index is None:
-                        fd.write(table.to_string(header=True, index=False))
+                        table.to_csv(filename, index=False)
                     else:
-                        fd.write(table.to_string(header=True, index=True))
-            else:
-                types = "', '".join(self.parameters["file type"].enumeration)
-                raise RuntimeError(
-                    f"Table save: cannot handle format '{file_type}' for file "
-                    f"'{filename}'\nKnown types: '{types}'"
-                )
+                        table.to_csv(filename, index=True, header=True)
+                elif file_type == ".json":
+                    if index is None:
+                        table.to_json(filename, indent=4, orient="table", index=False)
+                    else:
+                        table.to_json(filename, indent=4, orient="table", index=True)
+                elif file_type == ".xlsx":
+                    if index is None:
+                        table.to_excel(filename, index=False)
+                    else:
+                        table.to_excel(filename, index=True)
+                elif file_type == ".txt":
+                    with open(filename, "w") as fd:
+                        if index is None:
+                            fd.write(table.to_string(header=True, index=False))
+                        else:
+                            fd.write(table.to_string(header=True, index=True))
+                else:
+                    types = "', '".join(self.parameters["file type"].enumeration)
+                    raise RuntimeError(
+                        f"Table save: cannot handle format '{file_type}' for file "
+                        f"'{filename}'\nKnown types: '{types}'"
+                    )
         elif P["method"] == "Print":
             table_handle = self.get_variable(tablename)
             table = table_handle["table"]
             index = table_handle["index column"]
             printer.job("\nTable '{}':".format(tablename))
             if index is None:
                 printer.job(table.to_string(header=True, index=False))
```

### Comparing `table_step-2023.2.15/table_step/table_parameters.py` & `table_step-2023.7.25/table_step/table_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,23 @@
                 ".xlsx",
                 ".txt",
             ),
             "format_string": "",
             "description": "File type:",
             "help_text": "The type of file to read/write.",
         },
+        "frequency": {
+            "default": 1,
+            "kind": "integer",
+            "default_units": "",
+            "enumeration": tuple(),
+            "format_string": "",
+            "description": "Frequency:",
+            "help_text": "Number of calls before saving the table.",
+        },
         "index column": {
             "default": "--none--",
             "kind": "string",
             "default_units": "",
             "enumeration": tuple("--none--"),
             "format_string": "",
             "description": "Index column:",
```

### Comparing `table_step-2023.2.15/table_step/table_step.py` & `table_step-2023.7.25/table_step/table_step.py`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/table_step/tk_table.py` & `table_step-2023.7.25/table_step/tk_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,20 +112,25 @@
             row += 1
             self["index column"].grid(row=row, column=1, columnspan=2, sticky=tk.EW)
             row += 1
             sw.align_labels([self["filename"], self["file type"], self["index column"]])
         elif method == "Save":
             self["file type"].grid(row=row, column=1, sticky=tk.EW)
             row += 1
+            self["frequency"].grid(row=row, column=1, sticky=tk.EW)
+            row += 1
+            sw.align_labels([self["filename"], self["frequency"]])
         elif method == "Save as":
             self["filename"].grid(row=row, column=1, sticky=tk.EW)
             row += 1
             self["file type"].grid(row=row, column=1, sticky=tk.EW)
             row += 1
-            sw.align_labels([self["filename"], self["file type"]])
+            self["frequency"].grid(row=row, column=1, sticky=tk.EW)
+            row += 1
+            sw.align_labels([self["filename"], self["file type"], self["frequency"]])
         elif method == "Print":
             pass
         elif method == "Print the current row of":
             pass
         elif method == "Append a row to":
             self["columns"].grid(row=row, column=0, columnspan=4, sticky=tk.NSEW)
             frame.rowconfigure(row, weight=1)
```

### Comparing `table_step-2023.2.15/table_step.egg-info/PKG-INFO` & `table_step-2023.7.25/table_step.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: table-step
-Version: 2023.2.15
+Version: 2023.7.25
 Summary: A SEAMM plug-in for data tables in a flowchart.
 Home-page: https://github.com/molssi-seamm/table_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,table,data,csv
 Platform: Linux
@@ -87,14 +87,19 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.7.25 -- Bug fix and Enhancements
+    * Fixed bug with reading table using a variable for the filename, but asking for the
+      type from the extension.
+    * Add ability to save tables with a frequency of other than ever call.
+      
 2023.2.15 -- Bugs fixes and documentation
     * Restructured documentation and moved to new theme
     * Fixed bug with access rows of tables with non-integer indexes as well as "current"
       index 
     * Added support for lists of tables in pulldowns in the GUI
       
 2021.12.22 -- Improved the handling of index columns, added formats.
```

### Comparing `table_step-2023.2.15/table_step.egg-info/SOURCES.txt` & `table_step-2023.7.25/table_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/tests/conftest.py` & `table_step-2023.7.25/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/tests/flowcharts/test1.flow` & `table_step-2023.7.25/tests/flowcharts/test1.flow`

 * *Files identical despite different names*

### Comparing `table_step-2023.2.15/tests/test_flowcharts.py` & `table_step-2023.7.25/tests/test_flowcharts.py`

 * *Files identical despite different names*

