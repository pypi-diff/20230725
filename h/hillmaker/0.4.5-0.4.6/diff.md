# Comparing `tmp/hillmaker-0.4.5.tar.gz` & `tmp/hillmaker-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hillmaker-0.4.5.tar", last modified: Sun Nov 20 22:50:37 2022, max compression
+gzip compressed data, was "hillmaker-0.4.6.tar", last modified: Tue Jul 25 14:29:35 2023, max compression
```

## Comparing `hillmaker-0.4.5.tar` & `hillmaker-0.4.6.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-20 22:50:37.711868 hillmaker-0.4.5/
--rw-rw-r--   0 mark      (1000) mark      (1000)       86 2022-07-22 22:06:28.000000 hillmaker-0.4.5/AUTHORS
--rw-rw-r--   0 mark      (1000) mark      (1000)     1093 2022-07-22 22:06:28.000000 hillmaker-0.4.5/LICENSE
--rw-rw-r--   0 mark      (1000) mark      (1000)     4259 2022-11-20 22:50:37.711868 hillmaker-0.4.5/PKG-INFO
--rwxrwxr-x   0 mark      (1000) mark      (1000)     3302 2022-11-20 22:49:12.000000 hillmaker-0.4.5/README.md
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2022-11-20 22:50:37.711868 hillmaker-0.4.5/setup.cfg
--rwxrwxr-x   0 mark      (1000) mark      (1000)     1544 2022-11-20 22:35:44.000000 hillmaker-0.4.5/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-20 22:50:37.707868 hillmaker-0.4.5/src/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-20 22:50:37.711868 hillmaker-0.4.5/src/hillmaker/
--rwxrwxr-x   0 mark      (1000) mark      (1000)       39 2022-11-17 14:23:03.000000 hillmaker-0.4.5/src/hillmaker/__init__.py
--rwxrwxr-x   0 mark      (1000) mark      (1000)    20726 2022-11-20 17:27:18.000000 hillmaker-0.4.5/src/hillmaker/bydatetime.py
--rwxrwxr-x   0 mark      (1000) mark      (1000)    21675 2022-11-20 17:27:18.000000 hillmaker-0.4.5/src/hillmaker/hills.py
--rwxrwxr-x   0 mark      (1000) mark      (1000)     7110 2022-11-17 14:23:03.000000 hillmaker-0.4.5/src/hillmaker/hmlib.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4713 2022-11-17 14:23:03.000000 hillmaker-0.4.5/src/hillmaker/plotting.py
--rwxrwxr-x   0 mark      (1000) mark      (1000)     7654 2022-11-20 17:27:18.000000 hillmaker-0.4.5/src/hillmaker/summarize.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-20 22:50:37.711868 hillmaker-0.4.5/src/hillmaker.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)     4259 2022-11-20 22:50:37.000000 hillmaker-0.4.5/src/hillmaker.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      411 2022-11-20 22:50:37.000000 hillmaker-0.4.5/src/hillmaker.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2022-11-20 22:50:37.000000 hillmaker-0.4.5/src/hillmaker.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       51 2022-11-20 22:50:37.000000 hillmaker-0.4.5/src/hillmaker.egg-info/entry_points.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       26 2022-11-20 22:50:37.000000 hillmaker-0.4.5/src/hillmaker.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       10 2022-11-20 22:50:37.000000 hillmaker-0.4.5/src/hillmaker.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1001) mark      (1001)        0 2023-07-25 14:29:35.871400 hillmaker-0.4.6/
+-rw-rw-r--   0 mark      (1001) mark      (1001)       86 2023-07-24 15:48:50.000000 hillmaker-0.4.6/AUTHORS
+-rw-rw-r--   0 mark      (1001) mark      (1001)     1093 2023-07-24 15:48:50.000000 hillmaker-0.4.6/LICENSE
+-rw-rw-r--   0 mark      (1001) mark      (1001)     4461 2023-07-25 14:29:35.871400 hillmaker-0.4.6/PKG-INFO
+-rwxrwxr-x   0 mark      (1001) mark      (1001)     3504 2023-07-25 14:15:43.000000 hillmaker-0.4.6/README.md
+-rw-rw-r--   0 mark      (1001) mark      (1001)       38 2023-07-25 14:29:35.871400 hillmaker-0.4.6/setup.cfg
+-rwxrwxr-x   0 mark      (1001) mark      (1001)     1547 2023-07-25 14:16:43.000000 hillmaker-0.4.6/setup.py
+drwxrwxr-x   0 mark      (1001) mark      (1001)        0 2023-07-25 14:29:35.867400 hillmaker-0.4.6/src/
+drwxrwxr-x   0 mark      (1001) mark      (1001)        0 2023-07-25 14:29:35.867400 hillmaker-0.4.6/src/hillmaker/
+-rwxrwxrwx   0 mark      (1001) mark      (1001)       39 2022-11-17 14:23:03.000000 hillmaker-0.4.6/src/hillmaker/__init__.py
+-rwxrwxr-x   0 mark      (1001) mark      (1001)    20692 2023-07-25 14:15:43.000000 hillmaker-0.4.6/src/hillmaker/bydatetime.py
+-rwxrwxrwx   0 mark      (1001) mark      (1001)    21675 2022-11-20 17:27:18.000000 hillmaker-0.4.6/src/hillmaker/hills.py
+-rwxrwxrwx   0 mark      (1001) mark      (1001)     7110 2022-11-17 14:23:03.000000 hillmaker-0.4.6/src/hillmaker/hmlib.py
+-rw-rw-r--   0 mark      (1001) mark      (1001)     4713 2023-07-24 15:48:50.000000 hillmaker-0.4.6/src/hillmaker/plotting.py
+-rwxrwxrwx   0 mark      (1001) mark      (1001)     7654 2022-11-20 17:27:18.000000 hillmaker-0.4.6/src/hillmaker/summarize.py
+drwxrwxr-x   0 mark      (1001) mark      (1001)        0 2023-07-25 14:29:35.871400 hillmaker-0.4.6/src/hillmaker.egg-info/
+-rwxrwxrwx   0 mark      (1001) mark      (1001)     4461 2023-07-25 14:29:35.000000 hillmaker-0.4.6/src/hillmaker.egg-info/PKG-INFO
+-rwxrwxrwx   0 mark      (1001) mark      (1001)      489 2023-07-25 14:29:35.000000 hillmaker-0.4.6/src/hillmaker.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mark      (1001) mark      (1001)        1 2023-07-25 14:29:35.000000 hillmaker-0.4.6/src/hillmaker.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mark      (1001) mark      (1001)       51 2023-07-25 14:29:35.000000 hillmaker-0.4.6/src/hillmaker.egg-info/entry_points.txt
+-rwxrwxrwx   0 mark      (1001) mark      (1001)       26 2023-07-25 14:29:35.000000 hillmaker-0.4.6/src/hillmaker.egg-info/requires.txt
+-rwxrwxrwx   0 mark      (1001) mark      (1001)       10 2023-07-25 14:29:35.000000 hillmaker-0.4.6/src/hillmaker.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1001) mark      (1001)        0 2023-07-25 14:29:35.871400 hillmaker-0.4.6/tests/
+-rwxrwxrwx   0 mark      (1001) mark      (1001)     1256 2022-11-20 22:35:44.000000 hillmaker-0.4.6/tests/test_obsim_log.py
+-rwxrwxr-x   0 mark      (1001) mark      (1001)      660 2023-07-25 14:15:43.000000 hillmaker-0.4.6/tests/test_shortstay.py
+-rwxrwxr-x   0 mark      (1001) mark      (1001)      643 2023-07-25 14:15:43.000000 hillmaker-0.4.6/tests/test_shortstay_nocat.py
```

### Comparing `hillmaker-0.4.5/LICENSE` & `hillmaker-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hillmaker-0.4.5/PKG-INFO` & `hillmaker-0.4.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hillmaker
-Version: 0.4.5
+Version: 0.4.6
 Summary: Occupancy analysis tool for systems having time of day and day of week effects
 Home-page: http://github.com/misken/hillmaker/
 Author: Mark Isken
 Author-email: isken@oakland.edu
 Project-URL: Source, http://github.com/misken/hillmaker
 Project-URL: Examples, https://github.com/misken/hillmaker-examples
 Platform: any
@@ -57,33 +57,32 @@
 * Binary and source on PyPI: https://pypi.python.org/pypi/hillmaker
 * Documentation: Coming soon
 
 Quick Start
 -----------
 
 A companion repo, https://github.com/misken/hillmaker-examples/ contains
-Jupyter notebooks and Python scripts illustrating the use of hillmaker.
-
-You can see the most recent one at https://github.com/misken/hillmaker-examples/blob/main/notebooks/basic_usage_shortstay_unit_044.ipynb.
+Jupyter notebooks and Python scripts illustrating the use of hillmaker. You can
+also find example notebooks within this main hillmaker repo. You can see the most recent one at https://github.com/misken/hillmaker-examples/blob/main/notebooks/basic_usage_shortstay_unit_046.ipynb.
 
 The source and a binary wheel are available from PyPi. You can install using pip. 
 
     pip install tomli  # Not necessary if using Python >= 3.11
     pip install hillmaker
 
 
 Learn more about hillmaker
 --------------------------
 Hillmaker has been around in various forms for over 30 years. A few
 blog posts describing how it works are available though many things
 about the API as well as the computational guts of hillmaker have
 changed with this recent version.
 
-* [Computing occupancy statistics with Python - 1 of 3](https://misken.github.io/blog/hillpy_bydate_demo/)
-* [Computing occupancy statistics with Python - 1 of 3](https://misken.github.io/blog/hillpy_occstats_demo/)
-* [Plotting occupancy statistics with Python - 3 of 3](https://misken.github.io/blog/hillpy_plotting_matplotlib_basic_recipe/)
-* [Analyzing bike share usage](https://misken.github.io/blog/basic_usage_cycleshare/)
-* [Using hillmaker from R with reticulate](https://misken.github.io/blog/hillmaker_r_sfcs/)
-* [Numpy speeds up hillmaker dramatically](https://misken.github.io/blog/hillmaker_030_released/)
+* [Computing occupancy statistics with Python - 1 of 3](https://bitsofanalytics.org/posts/hillmaker-bydate-demo/hillpy_bydate_demo.html)
+* [Computing occupancy statistics with Python - 2 of 3](https://bitsofanalytics.org/posts/hillmaker-occstats-demo/hillpy_occstats_demo.html)
+* [Plotting occupancy statistics with Python - 3 of 3](https://bitsofanalytics.org/posts/hillmaker-plotting-recipe/hillpy_plotting_recipe.html)
+* [Analyzing bike share usage](https://bitsofanalytics.org/posts/basic-usage-cycleshare/basic_usage_cycleshare.html)
+* [Using hillmaker from R with reticulate](https://bitsofanalytics.org/posts/hillmaker-r-sfcs/hillmaker_r_sfcs.html)
+* [Numpy speeds up hillmaker dramatically](https://bitsofanalytics.org/posts/hillmaker-speedup/)
 
 I published [a paper a long time ago regarding the use of hillmaker in practice](https://www.researchgate.net/publication/7322712_Hillmaker_An_open_source_occupancy_analysis_tool).
 It describes an ancient version of hillmaker but does describe typical use cases.
```

### Comparing `hillmaker-0.4.5/README.md` & `hillmaker-0.4.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -32,33 +32,32 @@
 * Binary and source on PyPI: https://pypi.python.org/pypi/hillmaker
 * Documentation: Coming soon
 
 Quick Start
 -----------
 
 A companion repo, https://github.com/misken/hillmaker-examples/ contains
-Jupyter notebooks and Python scripts illustrating the use of hillmaker.
-
-You can see the most recent one at https://github.com/misken/hillmaker-examples/blob/main/notebooks/basic_usage_shortstay_unit_044.ipynb.
+Jupyter notebooks and Python scripts illustrating the use of hillmaker. You can
+also find example notebooks within this main hillmaker repo. You can see the most recent one at https://github.com/misken/hillmaker-examples/blob/main/notebooks/basic_usage_shortstay_unit_046.ipynb.
 
 The source and a binary wheel are available from PyPi. You can install using pip. 
 
     pip install tomli  # Not necessary if using Python >= 3.11
     pip install hillmaker
 
 
 Learn more about hillmaker
 --------------------------
 Hillmaker has been around in various forms for over 30 years. A few
 blog posts describing how it works are available though many things
 about the API as well as the computational guts of hillmaker have
 changed with this recent version.
 
-* [Computing occupancy statistics with Python - 1 of 3](https://misken.github.io/blog/hillpy_bydate_demo/)
-* [Computing occupancy statistics with Python - 1 of 3](https://misken.github.io/blog/hillpy_occstats_demo/)
-* [Plotting occupancy statistics with Python - 3 of 3](https://misken.github.io/blog/hillpy_plotting_matplotlib_basic_recipe/)
-* [Analyzing bike share usage](https://misken.github.io/blog/basic_usage_cycleshare/)
-* [Using hillmaker from R with reticulate](https://misken.github.io/blog/hillmaker_r_sfcs/)
-* [Numpy speeds up hillmaker dramatically](https://misken.github.io/blog/hillmaker_030_released/)
+* [Computing occupancy statistics with Python - 1 of 3](https://bitsofanalytics.org/posts/hillmaker-bydate-demo/hillpy_bydate_demo.html)
+* [Computing occupancy statistics with Python - 2 of 3](https://bitsofanalytics.org/posts/hillmaker-occstats-demo/hillpy_occstats_demo.html)
+* [Plotting occupancy statistics with Python - 3 of 3](https://bitsofanalytics.org/posts/hillmaker-plotting-recipe/hillpy_plotting_recipe.html)
+* [Analyzing bike share usage](https://bitsofanalytics.org/posts/basic-usage-cycleshare/basic_usage_cycleshare.html)
+* [Using hillmaker from R with reticulate](https://bitsofanalytics.org/posts/hillmaker-r-sfcs/hillmaker_r_sfcs.html)
+* [Numpy speeds up hillmaker dramatically](https://bitsofanalytics.org/posts/hillmaker-speedup/)
 
 I published [a paper a long time ago regarding the use of hillmaker in practice](https://www.researchgate.net/publication/7322712_Hillmaker_An_open_source_occupancy_analysis_tool).
 It describes an ancient version of hillmaker but does describe typical use cases.
```

### Comparing `hillmaker-0.4.5/setup.py` & `hillmaker-0.4.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Copyright 2022 Mark Isken
+# Copyright 2022-23 Mark Isken
 #
 
 from setuptools import find_packages, setup
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='hillmaker',
-      version='0.4.5',
+      version='0.4.6',
       description='Occupancy analysis tool for systems having time of day and day of week effects',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Mark Isken',
       author_email='isken@oakland.edu',
       url='http://github.com/misken/hillmaker/',
       packages=find_packages("src"),
```

### Comparing `hillmaker-0.4.5/src/hillmaker/bydatetime.py` & `hillmaker-0.4.6/src/hillmaker/bydatetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 OCC_TOLERANCE = 0.02
 EARLY_START_ANALYSIS_TOLERANCE = 48.0
 LATE_END_ANALYSIS_TOLERANCE = 48.0
 
 # This should inherit level from root logger
 logger = logging.getLogger(__name__)
 
+
 def make_bydatetime(stops_df, infield, outfield,
                     start_analysis_np, end_analysis_np, catfield=None,
                     bin_size_minutes=60,
                     cat_to_exclude=None,
                     totals=1,
                     occ_weight_field=None,
                     edge_bins=1,
@@ -118,28 +119,28 @@
         occ_weight_df = DataFrame({CONST_FAKE_OCCWEIGHT_FIELDNAME: occ_weight_vec})
         stops_df = pd.concat([stops_df, occ_weight_df], axis=1)
         occ_weight_field = CONST_FAKE_OCCWEIGHT_FIELDNAME
 
     # Handle cases of no catfield, or a single fieldname, (no longer supporting a list of fieldnames)
     # If no category, add a temporary dummy column populated with a totals str
 
-    do_totals = True
+    #do_totals = True
     if catfield is not None:
         # If catfield a string, convert to list
         # Keeping catfield as a list in case I change mind about multiple category fields
         if isinstance(catfield, str):
             catfield = [catfield]
     else:
         # No category field, create fake category field containing a single value
         totlist = [TOTAL_STR] * len(stops_df)
         totseries = Series(totlist, dtype=str, name=CONST_FAKE_CATFIELD_NAME)
         totfield_df = DataFrame({CONST_FAKE_CATFIELD_NAME: totseries})
         stops_df = pd.concat([stops_df, totfield_df], axis=1)
         catfield = [CONST_FAKE_CATFIELD_NAME]
-        do_totals = False
+        #do_totals = False
 
     # Get the unique category values and exclude any specified to exclude
     categories = []
     if isinstance(cat_to_exclude, str):
         cat_to_exclude = [cat_to_exclude]
 
     if cat_to_exclude is not None and len(cat_to_exclude) > 0:
@@ -248,25 +249,25 @@
     bydt_df_cat = arrays_to_df(results, start_analysis_np, end_analysis_np, bin_size_minutes, catfield)
 
     # Store main results bydatetime DataFrame
     bydt_dfs = {}
     totals_key = '_'.join(bydt_df_cat.index.names)
     bydt_dfs[totals_key] = bydt_df_cat.copy()
 
-    # Do totals if there was at least one category field
-    if do_totals:
-        results_totals = {}
-        totals_key = 'datetime'
-        total_occ_arr_dep = np.zeros((num_bins, 3), dtype=np.float64)
-        for cat, oad_array in results.items():
-            total_occ_arr_dep += oad_array
-
-        results_totals[totals_key] = total_occ_arr_dep
-        bydt_df_total = arrays_to_df(results_totals, start_analysis_np, end_analysis_np, bin_size_minutes)
-        bydt_dfs[totals_key] = bydt_df_total
+    # Compute totals - doing this even if only a fake category field
+    results_totals = {}
+    totals_key = 'datetime'
+
+    total_occ_arr_dep = np.zeros((num_bins, 3), dtype=np.float64)
+    for cat, oad_array in results.items():
+        total_occ_arr_dep += oad_array
+
+    results_totals[totals_key] = total_occ_arr_dep
+    bydt_df_total = arrays_to_df(results_totals, start_analysis_np, end_analysis_np, bin_size_minutes)
+    bydt_dfs[totals_key] = bydt_df_total
 
     return bydt_dfs
 
 def check_date_ranges(start_analysis, end_analysis, min_in_date, max_out_date):
     """
 
     Parameters
```

### Comparing `hillmaker-0.4.5/src/hillmaker/hills.py` & `hillmaker-0.4.6/src/hillmaker/hills.py`

 * *Files identical despite different names*

### Comparing `hillmaker-0.4.5/src/hillmaker/hmlib.py` & `hillmaker-0.4.6/src/hillmaker/hmlib.py`

 * *Files identical despite different names*

### Comparing `hillmaker-0.4.5/src/hillmaker/plotting.py` & `hillmaker-0.4.6/src/hillmaker/plotting.py`

 * *Files identical despite different names*

### Comparing `hillmaker-0.4.5/src/hillmaker/summarize.py` & `hillmaker-0.4.6/src/hillmaker/summarize.py`

 * *Files identical despite different names*

### Comparing `hillmaker-0.4.5/src/hillmaker.egg-info/PKG-INFO` & `hillmaker-0.4.6/src/hillmaker.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hillmaker
-Version: 0.4.5
+Version: 0.4.6
 Summary: Occupancy analysis tool for systems having time of day and day of week effects
 Home-page: http://github.com/misken/hillmaker/
 Author: Mark Isken
 Author-email: isken@oakland.edu
 Project-URL: Source, http://github.com/misken/hillmaker
 Project-URL: Examples, https://github.com/misken/hillmaker-examples
 Platform: any
@@ -57,33 +57,32 @@
 * Binary and source on PyPI: https://pypi.python.org/pypi/hillmaker
 * Documentation: Coming soon
 
 Quick Start
 -----------
 
 A companion repo, https://github.com/misken/hillmaker-examples/ contains
-Jupyter notebooks and Python scripts illustrating the use of hillmaker.
-
-You can see the most recent one at https://github.com/misken/hillmaker-examples/blob/main/notebooks/basic_usage_shortstay_unit_044.ipynb.
+Jupyter notebooks and Python scripts illustrating the use of hillmaker. You can
+also find example notebooks within this main hillmaker repo. You can see the most recent one at https://github.com/misken/hillmaker-examples/blob/main/notebooks/basic_usage_shortstay_unit_046.ipynb.
 
 The source and a binary wheel are available from PyPi. You can install using pip. 
 
     pip install tomli  # Not necessary if using Python >= 3.11
     pip install hillmaker
 
 
 Learn more about hillmaker
 --------------------------
 Hillmaker has been around in various forms for over 30 years. A few
 blog posts describing how it works are available though many things
 about the API as well as the computational guts of hillmaker have
 changed with this recent version.
 
-* [Computing occupancy statistics with Python - 1 of 3](https://misken.github.io/blog/hillpy_bydate_demo/)
-* [Computing occupancy statistics with Python - 1 of 3](https://misken.github.io/blog/hillpy_occstats_demo/)
-* [Plotting occupancy statistics with Python - 3 of 3](https://misken.github.io/blog/hillpy_plotting_matplotlib_basic_recipe/)
-* [Analyzing bike share usage](https://misken.github.io/blog/basic_usage_cycleshare/)
-* [Using hillmaker from R with reticulate](https://misken.github.io/blog/hillmaker_r_sfcs/)
-* [Numpy speeds up hillmaker dramatically](https://misken.github.io/blog/hillmaker_030_released/)
+* [Computing occupancy statistics with Python - 1 of 3](https://bitsofanalytics.org/posts/hillmaker-bydate-demo/hillpy_bydate_demo.html)
+* [Computing occupancy statistics with Python - 2 of 3](https://bitsofanalytics.org/posts/hillmaker-occstats-demo/hillpy_occstats_demo.html)
+* [Plotting occupancy statistics with Python - 3 of 3](https://bitsofanalytics.org/posts/hillmaker-plotting-recipe/hillpy_plotting_recipe.html)
+* [Analyzing bike share usage](https://bitsofanalytics.org/posts/basic-usage-cycleshare/basic_usage_cycleshare.html)
+* [Using hillmaker from R with reticulate](https://bitsofanalytics.org/posts/hillmaker-r-sfcs/hillmaker_r_sfcs.html)
+* [Numpy speeds up hillmaker dramatically](https://bitsofanalytics.org/posts/hillmaker-speedup/)
 
 I published [a paper a long time ago regarding the use of hillmaker in practice](https://www.researchgate.net/publication/7322712_Hillmaker_An_open_source_occupancy_analysis_tool).
 It describes an ancient version of hillmaker but does describe typical use cases.
```

