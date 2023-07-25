# Comparing `tmp/pheno-utils-0.3.6.tar.gz` & `tmp/pheno-utils-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.3.6.tar", last modified: Tue Jul 18 11:25:53 2023, max compression
+gzip compressed data, was "pheno-utils-0.3.7.tar", last modified: Tue Jul 25 10:13:43 2023, max compression
```

## Comparing `pheno-utils-0.3.6.tar` & `pheno-utils-0.3.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:25:53.637899 pheno-utils-0.3.6/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1409 2023-07-18 11:25:53.636137 pheno-utils-0.3.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-13 10:31:33.000000 pheno-utils-0.3.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:25:53.586105 pheno-utils-0.3.6/pheno_utils/
--rw-r--r--   0 root         (0) root         (0)      342 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17749 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/_modidx.py
--rw-r--r--   0 root         (0) root         (0)    16402 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/age_reference_plots.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/basic_analysis.py
--rw-r--r--   0 root         (0) root         (0)     2870 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/basic_plots.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/cgm_plots.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/cohort_selector.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/config.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/dates_plots.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/ecg_analysis.py
--rw-r--r--   0 root         (0) root         (0)     7781 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/meta_loader.py
--rw-r--r--   0 root         (0) root         (0)    19976 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/pheno_loader.py
--rw-r--r--   0 root         (0) root         (0)    13188 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:25:53.624369 pheno-utils-0.3.6/pheno_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1409 2023-07-18 11:25:53.000000 pheno-utils-0.3.6/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-18 11:25:53.000000 pheno-utils-0.3.6/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 11:25:53.000000 pheno-utils-0.3.6/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-18 11:25:53.000000 pheno-utils-0.3.6/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.6/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-18 11:25:53.000000 pheno-utils-0.3.6/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-18 11:25:53.000000 pheno-utils-0.3.6/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      942 2023-07-18 11:24:00.000000 pheno-utils-0.3.6/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 11:25:53.638702 pheno-utils-0.3.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2560 2023-06-21 16:13:16.000000 pheno-utils-0.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:13:43.872794 pheno-utils-0.3.7/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-07-25 10:13:43.871063 pheno-utils-0.3.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-13 10:31:33.000000 pheno-utils-0.3.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:13:43.800420 pheno-utils-0.3.7/pheno_utils/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-07-25 10:13:02.000000 pheno-utils-0.3.7/pheno_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18932 2023-07-25 10:13:02.000000 pheno-utils-0.3.7/pheno_utils/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)    16402 2023-07-25 10:13:02.000000 pheno-utils-0.3.7/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-07-25 10:13:02.000000 pheno-utils-0.3.7/pheno_utils/basic_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    11559 2023-07-25 10:13:02.000000 pheno-utils-0.3.7/pheno_utils/basic_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-25 10:13:02.000000 pheno-utils-0.3.7/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-25 10:13:02.000000 pheno-utils-0.3.7/pheno_utils/cgm_plots.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-25 10:13:02.000000 pheno-utils-0.3.7/pheno_utils/cohort_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-07-25 10:13:02.000000 pheno-utils-0.3.7/pheno_utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-25 10:13:02.000000 pheno-utils-0.3.7/pheno_utils/dates_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-25 10:13:02.000000 pheno-utils-0.3.7/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     7781 2023-07-25 10:13:02.000000 pheno-utils-0.3.7/pheno_utils/meta_loader.py
+-rw-r--r--   0 root         (0) root         (0)    20116 2023-07-25 10:13:02.000000 pheno-utils-0.3.7/pheno_utils/pheno_loader.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2023-07-25 10:13:02.000000 pheno-utils-0.3.7/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:13:43.865232 pheno-utils-0.3.7/pheno_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-07-25 10:13:43.000000 pheno-utils-0.3.7/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-25 10:13:43.000000 pheno-utils-0.3.7/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 10:13:43.000000 pheno-utils-0.3.7/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-25 10:13:43.000000 pheno-utils-0.3.7/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.7/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-25 10:13:43.000000 pheno-utils-0.3.7/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-25 10:13:43.000000 pheno-utils-0.3.7/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      942 2023-07-25 09:59:28.000000 pheno-utils-0.3.7/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 10:13:43.873614 pheno-utils-0.3.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3106 2023-07-25 09:08:28.000000 pheno-utils-0.3.7/setup.py
```

### Comparing `pheno-utils-0.3.6/LICENSE` & `pheno-utils-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.6/PKG-INFO` & `pheno-utils-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.6
+Version: 0.3.7
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.6/README.md` & `pheno-utils-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.6/pheno_utils/_modidx.py` & `pheno-utils-0.3.7/pheno_utils/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,26 @@
                                                                                                             'pheno_utils/age_reference_plots.py'),
                                                  'pheno_utils.age_reference_plots.get_gam_expectiles': ( 'age_reference_plots.html#get_gam_expectiles',
                                                                                                          'pheno_utils/age_reference_plots.py')},
             'pheno_utils.basic_analysis': { 'pheno_utils.basic_analysis.assign_nearest_research_stage': ( 'basic_analysis.html#assign_nearest_research_stage',
                                                                                                           'pheno_utils/basic_analysis.py'),
                                             'pheno_utils.basic_analysis.custom_describe': ( 'basic_analysis.html#custom_describe',
                                                                                             'pheno_utils/basic_analysis.py')},
-            'pheno_utils.basic_plots': { 'pheno_utils.basic_plots.hist_ecdf_plots': ( 'basic_plots.html#hist_ecdf_plots',
+            'pheno_utils.basic_plots': { 'pheno_utils.basic_plots.data_ecdfplot': ( 'basic_plots.html#data_ecdfplot',
+                                                                                    'pheno_utils/basic_plots.py'),
+                                         'pheno_utils.basic_plots.data_histplot': ( 'basic_plots.html#data_histplot',
+                                                                                    'pheno_utils/basic_plots.py'),
+                                         'pheno_utils.basic_plots.hist_ecdf_plots': ( 'basic_plots.html#hist_ecdf_plots',
                                                                                       'pheno_utils/basic_plots.py'),
+                                         'pheno_utils.basic_plots.plot_data_collection': ( 'basic_plots.html#plot_data_collection',
+                                                                                           'pheno_utils/basic_plots.py'),
+                                         'pheno_utils.basic_plots.plot_hist_stats': ( 'basic_plots.html#plot_hist_stats',
+                                                                                      'pheno_utils/basic_plots.py'),
+                                         'pheno_utils.basic_plots.plot_stats': ( 'basic_plots.html#plot_stats',
+                                                                                 'pheno_utils/basic_plots.py'),
                                          'pheno_utils.basic_plots.show_fundus': ( 'basic_plots.html#show_fundus',
                                                                                   'pheno_utils/basic_plots.py')},
             'pheno_utils.blandaltman_plots': { 'pheno_utils.blandaltman_plots.bland_altman_triple_plot': ( 'blandaltman_plots.html#bland_altman_triple_plot',
                                                                                                            'pheno_utils/blandaltman_plots.py')},
             'pheno_utils.cgm_plots': { 'pheno_utils.cgm_plots.AGP': ('cgm_plots.html#agp', 'pheno_utils/cgm_plots.py'),
                                        'pheno_utils.cgm_plots.AGP.__init__': ('cgm_plots.html#agp.__init__', 'pheno_utils/cgm_plots.py'),
                                        'pheno_utils.cgm_plots.AGP.plot': ('cgm_plots.html#agp.plot', 'pheno_utils/cgm_plots.py'),
```

### Comparing `pheno-utils-0.3.6/pheno_utils/age_reference_plots.py` & `pheno-utils-0.3.7/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.6/pheno_utils/basic_analysis.py` & `pheno-utils-0.3.7/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.6/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.3.7/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.6/pheno_utils/cgm_plots.py` & `pheno-utils-0.3.7/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.6/pheno_utils/cohort_selector.py` & `pheno-utils-0.3.7/pheno_utils/cohort_selector.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.6/pheno_utils/config.py` & `pheno-utils-0.3.7/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.6/pheno_utils/dates_plots.py` & `pheno-utils-0.3.7/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.6/pheno_utils/ecg_analysis.py` & `pheno-utils-0.3.7/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.6/pheno_utils/meta_loader.py` & `pheno-utils-0.3.7/pheno_utils/meta_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.6/pheno_utils/pheno_loader.py` & `pheno-utils-0.3.7/pheno_utils/pheno_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         age_sex_dataset: str = EVENTS_DATASET,
         skip_dfs: List[str] = [],
         unique_index: bool = False,
         valid_dates: bool = False,
         valid_stage: bool = False,
         flexible_field_search: bool = False,
         errors: str = ERROR_ACTION,
+        read_parquet_kwargs: Dict[str, Any] = {}
     ) -> None:
         self.dataset = dataset
         self.cohort = cohort
         self.base_path = base_path
         self.dataset_path = self.__get_dataset_path__(self.dataset)
         if self.dataset not in [age_sex_dataset, 'population']:
             self.age_sex_dataset = age_sex_dataset
@@ -88,14 +89,15 @@
             self.age_sex_dataset = None
         self.skip_dfs = skip_dfs
         self.unique_index = unique_index
         self.valid_dates = valid_dates
         self.valid_stage = valid_stage
         self.flexible_field_search = flexible_field_search
         self.errors = errors
+        self.read_parquet_kwargs = read_parquet_kwargs
 
         self.__load_dictionary__()
         self.__load_dataframes__()
         if self.age_sex_dataset is not None:
             self.__load_age_sex__()
 
     def load_sample_data(
@@ -112,15 +114,15 @@
         Load time series or bulk data for sample(s).
 
         Args:
             field_name (str): The name of the field to load.
             participant_id (str or list): The participant ID or IDs to load data for.
             research_stage (str or list, optional): The research stage or stages to load data for.
             array_index (int or list, optional): The array index or indices to load data for.
-            load_func (callable, optional): The function to use to load the data. Defaults to pd.read
+            load_func (callable, optional): The function to use to load the data. Defaults to pd.read_parquet
             concat (bool, optional): Whether to concatenate the data into a single DataFrame. Automatically ignored if data is not a DataFrame. Defaults to True.
             pivot (str, optional): The name of the field to pivot the data on (if DataFrame). Defaults to None.
         """
         query_str = 'participant_id in @participant_id'
         if not isinstance(participant_id, list):
             participant_id = [participant_id]
         if research_stage is not None:
@@ -396,15 +398,15 @@
         Returns:
             pd.DataFrame: the loaded dataframe
         """
     
         df_path = os.path.join(self.dataset_path, relative_location)
         
         try:
-            data =  pd.read_parquet(df_path)
+            data =  pd.read_parquet(df_path, **self.read_parquet_kwargs)
         except Exception as err:
             if self.errors == 'raise':
                 warnings.warn(f'Error loading {df_path}:\n{err}')
                 raise err
             if self.errors == 'warn':
                 warnings.warn(f'Error loading {df_path}:\n{err}')
             return None
```

### Comparing `pheno-utils-0.3.6/pheno_utils/sleep_plots.py` & `pheno-utils-0.3.7/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.6/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.3.7/pheno_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.6
+Version: 0.3.7
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.6/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.3.7/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.6/settings.ini` & `pheno-utils-0.3.7/settings.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pheno-utils
 lib_name = pheno-utils
-version = 0.3.6
+version = 0.3.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pheno_utils
 nbs_path = nbs
 recursive = True
```

