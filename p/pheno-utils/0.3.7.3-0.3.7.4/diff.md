# Comparing `tmp/pheno-utils-0.3.7.3.tar.gz` & `tmp/pheno-utils-0.3.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.3.7.3.tar", last modified: Tue Jul 25 12:16:46 2023, max compression
+gzip compressed data, was "pheno-utils-0.3.7.4.tar", last modified: Tue Jul 25 13:29:19 2023, max compression
```

## Comparing `pheno-utils-0.3.7.3.tar` & `pheno-utils-0.3.7.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:16:46.983403 pheno-utils-0.3.7.3/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2737 2023-07-25 12:16:46.981857 pheno-utils-0.3.7.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1959 2023-07-25 11:36:20.000000 pheno-utils-0.3.7.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:16:46.920709 pheno-utils-0.3.7.3/pheno_utils/
--rw-r--r--   0 root         (0) root         (0)      344 2023-07-25 12:16:14.000000 pheno-utils-0.3.7.3/pheno_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18932 2023-07-25 12:16:14.000000 pheno-utils-0.3.7.3/pheno_utils/_modidx.py
--rw-r--r--   0 root         (0) root         (0)    16402 2023-07-25 12:16:14.000000 pheno-utils-0.3.7.3/pheno_utils/age_reference_plots.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-07-25 12:16:14.000000 pheno-utils-0.3.7.3/pheno_utils/basic_analysis.py
--rw-r--r--   0 root         (0) root         (0)    11559 2023-07-25 12:16:14.000000 pheno-utils-0.3.7.3/pheno_utils/basic_plots.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-25 12:16:14.000000 pheno-utils-0.3.7.3/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-07-25 12:16:14.000000 pheno-utils-0.3.7.3/pheno_utils/cgm_plots.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-07-25 12:16:14.000000 pheno-utils-0.3.7.3/pheno_utils/cohort_selector.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-07-25 12:16:14.000000 pheno-utils-0.3.7.3/pheno_utils/config.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-25 12:16:14.000000 pheno-utils-0.3.7.3/pheno_utils/dates_plots.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-25 12:16:14.000000 pheno-utils-0.3.7.3/pheno_utils/ecg_analysis.py
--rw-r--r--   0 root         (0) root         (0)     7781 2023-07-25 12:16:14.000000 pheno-utils-0.3.7.3/pheno_utils/meta_loader.py
--rw-r--r--   0 root         (0) root         (0)    20116 2023-07-25 12:16:14.000000 pheno-utils-0.3.7.3/pheno_utils/pheno_loader.py
--rw-r--r--   0 root         (0) root         (0)    13188 2023-07-25 12:16:14.000000 pheno-utils-0.3.7.3/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:16:46.976121 pheno-utils-0.3.7.3/pheno_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2737 2023-07-25 12:16:46.000000 pheno-utils-0.3.7.3/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-25 12:16:46.000000 pheno-utils-0.3.7.3/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 12:16:46.000000 pheno-utils-0.3.7.3/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-25 12:16:46.000000 pheno-utils-0.3.7.3/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.7.3/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-25 12:16:46.000000 pheno-utils-0.3.7.3/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-25 12:16:46.000000 pheno-utils-0.3.7.3/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      944 2023-07-25 12:16:10.000000 pheno-utils-0.3.7.3/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 12:16:46.984268 pheno-utils-0.3.7.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3437 2023-07-25 12:14:29.000000 pheno-utils-0.3.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:29:19.720350 pheno-utils-0.3.7.4/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-07-25 13:29:19.719227 pheno-utils-0.3.7.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-07-25 11:36:20.000000 pheno-utils-0.3.7.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:29:19.653673 pheno-utils-0.3.7.4/pheno_utils/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-07-25 13:29:06.000000 pheno-utils-0.3.7.4/pheno_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18932 2023-07-25 13:29:06.000000 pheno-utils-0.3.7.4/pheno_utils/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)    16402 2023-07-25 13:29:06.000000 pheno-utils-0.3.7.4/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-07-25 13:29:06.000000 pheno-utils-0.3.7.4/pheno_utils/basic_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    11559 2023-07-25 13:29:06.000000 pheno-utils-0.3.7.4/pheno_utils/basic_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-25 13:29:06.000000 pheno-utils-0.3.7.4/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-25 13:29:06.000000 pheno-utils-0.3.7.4/pheno_utils/cgm_plots.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-25 13:29:06.000000 pheno-utils-0.3.7.4/pheno_utils/cohort_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-07-25 13:29:06.000000 pheno-utils-0.3.7.4/pheno_utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-25 13:29:06.000000 pheno-utils-0.3.7.4/pheno_utils/dates_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-25 13:29:06.000000 pheno-utils-0.3.7.4/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     7781 2023-07-25 13:29:06.000000 pheno-utils-0.3.7.4/pheno_utils/meta_loader.py
+-rw-r--r--   0 root         (0) root         (0)    20116 2023-07-25 13:29:06.000000 pheno-utils-0.3.7.4/pheno_utils/pheno_loader.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2023-07-25 13:29:06.000000 pheno-utils-0.3.7.4/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:29:19.711645 pheno-utils-0.3.7.4/pheno_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-07-25 13:29:19.000000 pheno-utils-0.3.7.4/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-25 13:29:19.000000 pheno-utils-0.3.7.4/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 13:29:19.000000 pheno-utils-0.3.7.4/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-25 13:29:19.000000 pheno-utils-0.3.7.4/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.7.4/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-25 13:29:19.000000 pheno-utils-0.3.7.4/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-25 13:29:19.000000 pheno-utils-0.3.7.4/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      944 2023-07-25 13:28:38.000000 pheno-utils-0.3.7.4/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 13:29:19.720911 pheno-utils-0.3.7.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3797 2023-07-25 13:29:02.000000 pheno-utils-0.3.7.4/setup.py
```

### Comparing `pheno-utils-0.3.7.3/LICENSE` & `pheno-utils-0.3.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/PKG-INFO` & `pheno-utils-0.3.7.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.7.3
+Version: 0.3.7.4
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.7.3/README.md` & `pheno-utils-0.3.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/pheno_utils/_modidx.py` & `pheno-utils-0.3.7.4/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/pheno_utils/age_reference_plots.py` & `pheno-utils-0.3.7.4/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/pheno_utils/basic_analysis.py` & `pheno-utils-0.3.7.4/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/pheno_utils/basic_plots.py` & `pheno-utils-0.3.7.4/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.3.7.4/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/pheno_utils/cgm_plots.py` & `pheno-utils-0.3.7.4/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/pheno_utils/cohort_selector.py` & `pheno-utils-0.3.7.4/pheno_utils/cohort_selector.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/pheno_utils/config.py` & `pheno-utils-0.3.7.4/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/pheno_utils/dates_plots.py` & `pheno-utils-0.3.7.4/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/pheno_utils/ecg_analysis.py` & `pheno-utils-0.3.7.4/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/pheno_utils/meta_loader.py` & `pheno-utils-0.3.7.4/pheno_utils/meta_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/pheno_utils/pheno_loader.py` & `pheno-utils-0.3.7.4/pheno_utils/pheno_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/pheno_utils/sleep_plots.py` & `pheno-utils-0.3.7.4/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.3.7.4/pheno_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.7.3
+Version: 0.3.7.4
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.7.3/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.3.7.4/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.3/settings.ini` & `pheno-utils-0.3.7.4/settings.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pheno-utils
 lib_name = pheno-utils
-version = 0.3.7.3
+version = 0.3.7.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pheno_utils
 nbs_path = nbs
 recursive = True
```

### Comparing `pheno-utils-0.3.7.3/setup.py` & `pheno-utils-0.3.7.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 from pkg_resources import parse_version
 from configparser import ConfigParser
-import json, os
+import json, os, sys
 import shutil
 import setuptools, shlex
 assert parse_version(setuptools.__version__)>=parse_version('36.2')
 
 
 def copy_tre_config():
     script_path = os.path.dirname(os.path.abspath(__file__))
+    sys.stderr.write('This is an error message\n')
+    sys.stderr.write(script_path)
     print(script_path)
     absolute_config_path = os.path.join(script_path, 'config_setup/config_tre.json')
     print(absolute_config_path)
+    sys.stderr.write(absolute_config_path)
     with open(absolute_config_path, 'r') as openfile:
         json_object = json.load(openfile)
         print('wow')
+        sys.stderr.write('wow')
     datasets_full_path = json_object['DATASETS_PATH']
     print(datasets_full_path)
+    sys.stderr.write(datasets_full_path)
     if os.path.exists(datasets_full_path):
         # TRE MODE
         print('TRE MODE')
+        sys.stderr.write('TRE MODE')
         if not os.path.exists(os.path.expanduser('~/.pheno')):
             print('yes', os.path.expanduser('~/.pheno'))
+            sys.stderr.write(os.path.expanduser('~/.pheno'))
             os.makedirs(os.path.expanduser('~/.pheno'))
         print(absolute_config_path)
+        sys.stderr.write(absolute_config_path)
+        
         shutil.copy2(absolute_config_path, os.path.expanduser('~/.pheno/config.json'))
 
         
 copy_tre_config()     
 
 # note: all settings are in settings.ini; edit there, not here
 config = ConfigParser(delimiters=['='])
```

