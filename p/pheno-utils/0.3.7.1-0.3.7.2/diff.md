# Comparing `tmp/pheno-utils-0.3.7.1.tar.gz` & `tmp/pheno-utils-0.3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.3.7.1.tar", last modified: Tue Jul 25 11:36:56 2023, max compression
+gzip compressed data, was "pheno-utils-0.3.7.2.tar", last modified: Tue Jul 25 12:02:31 2023, max compression
```

## Comparing `pheno-utils-0.3.7.1.tar` & `pheno-utils-0.3.7.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:36:56.863541 pheno-utils-0.3.7.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2737 2023-07-25 11:36:56.862470 pheno-utils-0.3.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1959 2023-07-25 11:36:20.000000 pheno-utils-0.3.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:36:56.816677 pheno-utils-0.3.7.1/pheno_utils/
--rw-r--r--   0 root         (0) root         (0)      344 2023-07-25 11:36:05.000000 pheno-utils-0.3.7.1/pheno_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18932 2023-07-25 11:36:05.000000 pheno-utils-0.3.7.1/pheno_utils/_modidx.py
--rw-r--r--   0 root         (0) root         (0)    16402 2023-07-25 11:36:05.000000 pheno-utils-0.3.7.1/pheno_utils/age_reference_plots.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-07-25 11:36:05.000000 pheno-utils-0.3.7.1/pheno_utils/basic_analysis.py
--rw-r--r--   0 root         (0) root         (0)    11559 2023-07-25 11:36:05.000000 pheno-utils-0.3.7.1/pheno_utils/basic_plots.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-25 11:36:05.000000 pheno-utils-0.3.7.1/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-07-25 11:36:05.000000 pheno-utils-0.3.7.1/pheno_utils/cgm_plots.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-07-25 11:36:05.000000 pheno-utils-0.3.7.1/pheno_utils/cohort_selector.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-07-25 11:36:05.000000 pheno-utils-0.3.7.1/pheno_utils/config.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-25 11:36:05.000000 pheno-utils-0.3.7.1/pheno_utils/dates_plots.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-25 11:36:05.000000 pheno-utils-0.3.7.1/pheno_utils/ecg_analysis.py
--rw-r--r--   0 root         (0) root         (0)     7781 2023-07-25 11:36:05.000000 pheno-utils-0.3.7.1/pheno_utils/meta_loader.py
--rw-r--r--   0 root         (0) root         (0)    20116 2023-07-25 11:36:05.000000 pheno-utils-0.3.7.1/pheno_utils/pheno_loader.py
--rw-r--r--   0 root         (0) root         (0)    13188 2023-07-25 11:36:05.000000 pheno-utils-0.3.7.1/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:36:56.852462 pheno-utils-0.3.7.1/pheno_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2737 2023-07-25 11:36:56.000000 pheno-utils-0.3.7.1/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-25 11:36:56.000000 pheno-utils-0.3.7.1/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 11:36:56.000000 pheno-utils-0.3.7.1/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-25 11:36:56.000000 pheno-utils-0.3.7.1/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.7.1/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-25 11:36:56.000000 pheno-utils-0.3.7.1/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-25 11:36:56.000000 pheno-utils-0.3.7.1/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      944 2023-07-25 11:35:51.000000 pheno-utils-0.3.7.1/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 11:36:56.864315 pheno-utils-0.3.7.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3157 2023-07-25 11:35:24.000000 pheno-utils-0.3.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:02:31.627254 pheno-utils-0.3.7.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-07-25 12:02:31.626102 pheno-utils-0.3.7.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-07-25 11:36:20.000000 pheno-utils-0.3.7.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:02:31.590030 pheno-utils-0.3.7.2/pheno_utils/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-07-25 12:01:59.000000 pheno-utils-0.3.7.2/pheno_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18932 2023-07-25 12:01:59.000000 pheno-utils-0.3.7.2/pheno_utils/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)    16402 2023-07-25 12:01:59.000000 pheno-utils-0.3.7.2/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-07-25 12:01:59.000000 pheno-utils-0.3.7.2/pheno_utils/basic_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    11559 2023-07-25 12:01:59.000000 pheno-utils-0.3.7.2/pheno_utils/basic_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-25 12:01:59.000000 pheno-utils-0.3.7.2/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-25 12:01:59.000000 pheno-utils-0.3.7.2/pheno_utils/cgm_plots.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-25 12:01:59.000000 pheno-utils-0.3.7.2/pheno_utils/cohort_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-07-25 12:01:59.000000 pheno-utils-0.3.7.2/pheno_utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-25 12:01:59.000000 pheno-utils-0.3.7.2/pheno_utils/dates_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-25 12:01:59.000000 pheno-utils-0.3.7.2/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     7781 2023-07-25 12:01:59.000000 pheno-utils-0.3.7.2/pheno_utils/meta_loader.py
+-rw-r--r--   0 root         (0) root         (0)    20116 2023-07-25 12:01:59.000000 pheno-utils-0.3.7.2/pheno_utils/pheno_loader.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2023-07-25 12:01:59.000000 pheno-utils-0.3.7.2/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:02:31.622385 pheno-utils-0.3.7.2/pheno_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-07-25 12:02:31.000000 pheno-utils-0.3.7.2/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-25 12:02:31.000000 pheno-utils-0.3.7.2/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 12:02:31.000000 pheno-utils-0.3.7.2/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-25 12:02:31.000000 pheno-utils-0.3.7.2/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.7.2/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-25 12:02:31.000000 pheno-utils-0.3.7.2/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-25 12:02:31.000000 pheno-utils-0.3.7.2/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      944 2023-07-25 12:01:55.000000 pheno-utils-0.3.7.2/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 12:02:31.627754 pheno-utils-0.3.7.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3218 2023-07-25 12:01:05.000000 pheno-utils-0.3.7.2/setup.py
```

### Comparing `pheno-utils-0.3.7.1/LICENSE` & `pheno-utils-0.3.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/PKG-INFO` & `pheno-utils-0.3.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.7.1
+Version: 0.3.7.2
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.7.1/README.md` & `pheno-utils-0.3.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/pheno_utils/_modidx.py` & `pheno-utils-0.3.7.2/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/pheno_utils/age_reference_plots.py` & `pheno-utils-0.3.7.2/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/pheno_utils/basic_analysis.py` & `pheno-utils-0.3.7.2/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/pheno_utils/basic_plots.py` & `pheno-utils-0.3.7.2/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.3.7.2/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/pheno_utils/cgm_plots.py` & `pheno-utils-0.3.7.2/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/pheno_utils/cohort_selector.py` & `pheno-utils-0.3.7.2/pheno_utils/cohort_selector.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/pheno_utils/config.py` & `pheno-utils-0.3.7.2/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/pheno_utils/dates_plots.py` & `pheno-utils-0.3.7.2/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/pheno_utils/ecg_analysis.py` & `pheno-utils-0.3.7.2/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/pheno_utils/meta_loader.py` & `pheno-utils-0.3.7.2/pheno_utils/meta_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/pheno_utils/pheno_loader.py` & `pheno-utils-0.3.7.2/pheno_utils/pheno_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/pheno_utils/sleep_plots.py` & `pheno-utils-0.3.7.2/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.3.7.2/pheno_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.7.1
+Version: 0.3.7.2
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.7.1/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.3.7.2/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.1/settings.ini` & `pheno-utils-0.3.7.2/settings.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pheno-utils
 lib_name = pheno-utils
-version = 0.3.7.1
+version = 0.3.7.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pheno_utils
 nbs_path = nbs
 recursive = True
```

### Comparing `pheno-utils-0.3.7.1/setup.py` & `pheno-utils-0.3.7.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 import json, os
 import shutil
 import setuptools, shlex
 assert parse_version(setuptools.__version__)>=parse_version('36.2')
 
 
 def copy_tre_config():
-    absolute_config_path = os.path.abspath('config_setup/config_tre.json')
+    script_path = os.path.dirname(os.path.abspath(__file__))
+    absolute_config_path = os.path.join(script_path, 'config_setup/config_tre.json')
 
     with open(absolute_config_path, 'r') as openfile:
         json_object = json.load(openfile)
     datasets_full_path = json_object['DATASETS_PATH']
     
     if os.path.exists(datasets_full_path):
         # TRE MODE
         if not os.path.exists(os.path.expanduser('~/.pheno')):
             os.makedirs(os.path.expanduser('~/.pheno'))
-        shutil.copy2('config_setup/config_tre.json', os.path.expanduser('~/.pheno/config.json'))
+        shutil.copy2(absolute_config_path, os.path.expanduser('~/.pheno/config.json'))
 
         
 copy_tre_config()     
 
 # note: all settings are in settings.ini; edit there, not here
 config = ConfigParser(delimiters=['='])
 config.read('settings.ini')
```

