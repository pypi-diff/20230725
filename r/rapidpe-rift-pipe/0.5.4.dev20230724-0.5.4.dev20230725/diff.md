# Comparing `tmp/rapidpe_rift_pipe-0.5.4.dev20230724.tar.gz` & `tmp/rapidpe_rift_pipe-0.5.4.dev20230725.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.5.4.dev20230724.tar", last modified: Mon Jul 24 05:15:51 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.5.4.dev20230725.tar", last modified: Tue Jul 25 05:17:32 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.5.4.dev20230724.tar` & `rapidpe_rift_pipe-0.5.4.dev20230725.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:15:51.016406 rapidpe_rift_pipe-0.5.4.dev20230724/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1090 2023-07-24 05:15:51.017406 rapidpe_rift_pipe-0.5.4.dev20230724/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:15:51.003405 rapidpe_rift_pipe-0.5.4.dev20230724/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:15:51.006405 rapidpe_rift_pipe-0.5.4.dev20230724/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-07-15 05:18:18.000000 rapidpe_rift_pipe-0.5.4.dev20230724/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6342 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     5579 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1419 2023-07-24 05:15:51.017406 rapidpe_rift_pipe-0.5.4.dev20230724/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:15:51.003405 rapidpe_rift_pipe-0.5.4.dev20230724/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:15:51.014406 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-10 17:53:47.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    47573 2023-07-15 05:18:18.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:15:51.015406 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 05:15:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:15:51.016406 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 05:15:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31454 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4719 2023-07-15 05:18:18.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    27677 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:15:51.016406 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 05:15:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:15:51.015406 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1090 2023-07-24 05:15:50.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-07-24 05:15:51.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:15:50.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 05:15:50.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-24 05:15:50.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-24 05:15:50.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:15:50.000000 rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.484939 rapidpe_rift_pipe-0.5.4.dev20230725/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-25 05:17:32.485939 rapidpe_rift_pipe-0.5.4.dev20230725/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.479939 rapidpe_rift_pipe-0.5.4.dev20230725/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.481939 rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     6351 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2023-07-25 05:17:32.485939 rapidpe_rift_pipe-0.5.4.dev20230725/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.480939 rapidpe_rift_pipe-0.5.4.dev20230725/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.483939 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    47573 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.484939 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.484939 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31210 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4719 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    27677 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.484939 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.484939 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-25 05:17:32.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-07-25 05:17:32.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 05:17:32.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-25 05:17:32.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-25 05:17:32.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 05:17:32.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 05:17:32.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/COPYING` & `rapidpe_rift_pipe-0.5.4.dev20230725/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/PKG-INFO` & `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rapidpe_rift_pipe
-Version: 0.5.4.dev20230724
+Name: rapidpe-rift-pipe
+Version: 0.5.4.dev20230725
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/compute_posterior.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/create_summarypage.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,15 +94,29 @@
     event_url = gracedb_url._replace(path=event_path).geturl()
     print_output(
         html_file, f'GraceDB url : <a href="{event_url}">{event_id}</a> <br>'
     )
 
 filelist = glob(output_dir + "/grid*png")
 print_output(html_file, "<h1> Grid Plots </h1>")
-for fname_full in sorted(filelist):
+distance_coordinate = config.distance_coordinates
+all_grid_fname = os.path.join(
+    output_dir, f"grid_{distance_coordinate}_all.png"
+)
+print_output(html_file, f'<img src="{os.path.basename(all_grid_fname)}">')
+distance_coordinate_filelist = glob(
+    f"{output_dir}/grid_{distance_coordinate}_iteration-*.png"
+)
+for fname_full in sorted(distance_coordinate_filelist):
+    fname = os.path.basename(fname_full)
+    print_output(html_file, f'<img src="{fname}">')
+remaining_filelist = (
+    set(filelist) - set([all_grid_fname]) - set(distance_coordinate_filelist)
+)
+for fname_full in sorted(remaining_filelist):
     fname = os.path.basename(fname_full)
     print_output(html_file, f'<img src="{fname}">')
 
 print_output(html_file, "<h1> Posterior Plots </h1>")
 
 
 filelist = glob(output_dir + "/posterior*.png")
@@ -114,62 +128,61 @@
 if filelist != []:
     print_output(html_file, "<h1> Pastro </h1>")
     for fname_full in sorted(filelist):
         fname = os.path.basename(fname_full)
         print_output(html_file, f"<br>{fname}")
         print_output(html_file, f'<img src="{fname}">')
 
-
-print_output(html_file, "<h1> Skymaps </h1>")
 filelist = glob(output_dir + "/skymap*png")
-for fname_full in sorted(filelist):
-    fname = os.path.basename(fname_full)
-    print_output(html_file, f"<br>{fname}")
-    print_output(html_file, f'<img src="{fname}">')
-
-
-print_output(html_file, """<h1> Timing </h1> """)
-
-if os.path.exists(f"{summary_plot_dir}/cprofile.html"):
-    filelist = np.sort(glob(output_dir + "/cprofile*hist*png"))
+if len(filelist) != 0:
+    print_output(html_file, "<h1> Skymaps </h1>")
     for fname_full in sorted(filelist):
         fname = os.path.basename(fname_full)
+        print_output(html_file, f"<br>{fname}")
         print_output(html_file, f'<img src="{fname}">')
 
 
-# Total job time:
-condor_submit_time = int(event_info_dict["condor_submit_time"])
-job_timing_file = os.path.join(input_dir, "job_timing.txt")
-iteration_completion_time = []
-with open(job_timing_file) as f:
-    lines = f.readlines()
-    for line_id, line in enumerate(lines):
-        line_split = line.split(" ")
-        level_complete_time = float(line_split[1])
-        iteration_completion_time.append(level_complete_time)
-        if line_id == 0:
-            print_output(
-                html_file,
-                f'<br> <font size="+2"> iteration level {line_split[0]} took '
-                f"{level_complete_time-condor_submit_time} s </font>",
-            )
-        else:
-            print_output(
-                html_file,
-                f'<br> <font size="+2"> iteration level {line_split[0]} took '
-                f"{level_complete_time-iteration_completion_time[line_id-1]} s </font>",
-            )
-
+if config.cProfile:
+    print_output(html_file, """<h1> Timing </h1> """)
 
-if os.path.exists(f"{summary_plot_dir}/cprofile.html"):
-    print_output(
-        html_file,
-        "<br><a href='cprofile.html'>Detailed cProfile info for a single ILE job</a>",
-    )
-print_output(html_file, "<h1> Config.ini </h1>")
+    if os.path.exists(f"{summary_plot_dir}/cprofile.html"):
+        filelist = np.sort(glob(output_dir + "/cprofile*hist*png"))
+        for fname_full in sorted(filelist):
+            fname = os.path.basename(fname_full)
+            print_output(html_file, f'<img src="{fname}">')
+
+    # Total job time:
+    condor_submit_time = int(event_info_dict["condor_submit_time"])
+    job_timing_file = os.path.join(input_dir, "job_timing.txt")
+    iteration_completion_time = []
+    with open(job_timing_file) as f:
+        lines = f.readlines()
+        for line_id, line in enumerate(lines):
+            line_split = line.split(" ")
+            level_complete_time = float(line_split[1])
+            iteration_completion_time.append(level_complete_time)
+            if line_id == 0:
+                print_output(
+                    html_file,
+                    f'<br> <font size="+2"> iteration level {line_split[0]} took '
+                    f"{level_complete_time-condor_submit_time} s </font>",
+                )
+            else:
+                print_output(
+                    html_file,
+                    f'<br> <font size="+2"> iteration level {line_split[0]} took '
+                    f"{level_complete_time-iteration_completion_time[line_id-1]} s </font>",
+                )
+
+    if os.path.exists(f"{summary_plot_dir}/cprofile.html"):
+        print_output(
+            html_file,
+            "<br><a href='cprofile.html'>Detailed cProfile info for a single ILE job</a>",
+        )
+    print_output(html_file, "<h1> Config.ini </h1>")
 
 with open(os.path.join(input_dir, "Config.ini")) as config_f:
     for line in config_f:
         if line[0] != "#" and len(line.strip()) > 0:
             if line[0] == "[":
                 print_output(html_file, f"<br> <b> {line} </b>")
             else:
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/setup.cfg` & `rapidpe_rift_pipe-0.5.4.dev20230725/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -49,10 +49,10 @@
 rapidpe_rift_pipe.config_files = *.ini, *.json
 
 [options.entry_points]
 console_scripts = 
 	rapidpe-rift-pipe = rapidpe_rift_pipe.cli:main
 
 [egg_info]
-tag_build = dev.20230724
+tag_build = dev.20230725
 tag_date = 0
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/cli.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -347,16 +347,14 @@
             web_dir_str = ""
             if config.web_dir:
                 web_dir_str = f"--web-dir {config.web_dir}"
             summary_plots_outfile = os.path.join(output_dir,"summary/summary_plots.out")
             if indx == (config.n_iterations_per_job-1):
                 iter_pt_str = f"#!/bin/bash\necho {str(int(indx))} `date +%s` >> {output_dir}/job_timing.txt\n"
                 iter_pt_str += f"echo 'job_complete' >> {output_dir}/JOB_COMPLETE\n"
-                iter_pt_str += f"convert_result_to_txt.py {output_dir} --ratio-to-include 0.95  &>> {summary_plots_outfile}\n"
-                iter_pt_str += f"plot_skymap.py {output_dir} --ratio-to-include 0.95  &>> {summary_plots_outfile}\n"
                 iter_pt_str += f"compute_posterior.py {output_dir} --distance-coordinates {config.distance_coordinates } &>> {summary_plots_outfile}\n"
                 if config.cProfile:
                     iter_pt_str += f"cprofile_summary.py {output_dir} &>> {summary_plots_outfile}\n"
                 iter_pt_str += f"create_summarypage.py {output_dir} {web_dir_str}  &>> {summary_plots_outfile}\n"
                 #automatically plot the posteriors when the job is done. FIXME: change 0.99 to whatever
                 #iter_pt_str += "python "+init_directory+"/plot_all_posteriors.py "+output_dir+" 0.99\n"
                 #iter_pt_str += "python "+init_directory+"/plot_all_posteriors.py "+output_dir+" 0.9\n"
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/pastro.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.5.4.dev20230725/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rapidpe-rift-pipe
-Version: 0.5.4.dev20230724
+Name: rapidpe_rift_pipe
+Version: 0.5.4.dev20230725
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230724/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

