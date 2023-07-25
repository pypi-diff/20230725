# Comparing `tmp/KIF-0.3.1.tar.gz` & `tmp/KIF-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KIF-0.3.1.tar", last modified: Mon Jul 24 10:11:37 2023, max compression
+gzip compressed data, was "KIF-0.3.2.tar", last modified: Tue Jul 25 17:48:51 2023, max compression
```

## Comparing `KIF-0.3.1.tar` & `KIF-0.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 10:11:37.176185 KIF-0.3.1/
-drwxrwxrwx   0        0        0        0 2023-07-24 10:11:37.035586 KIF-0.3.1/KIF.egg-info/
--rw-rw-rw-   0        0        0      439 2023-07-24 10:11:36.000000 KIF-0.3.1/KIF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      948 2023-07-24 10:11:36.000000 KIF-0.3.1/KIF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 10:11:36.000000 KIF-0.3.1/KIF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-07-24 10:11:36.000000 KIF-0.3.1/KIF.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-24 10:11:36.000000 KIF-0.3.1/KIF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18431 2022-09-22 10:55:30.000000 KIF-0.3.1/LICENSE.md
--rw-rw-rw-   0        0        0      439 2023-07-24 10:11:37.176185 KIF-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    10944 2023-07-24 10:06:40.000000 KIF-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 10:11:37.129335 KIF-0.3.1/key_interactions_finder/
--rw-rw-rw-   0        0        0        0 2021-12-19 18:36:56.000000 KIF-0.3.1/key_interactions_finder/__init__.py
--rw-rw-rw-   0        0        0    12253 2023-07-24 10:03:14.000000 KIF-0.3.1/key_interactions_finder/contact_identification.py
--rw-rw-rw-   0        0        0    10177 2023-07-14 09:23:12.000000 KIF-0.3.1/key_interactions_finder/contact_identification_old.py
--rw-rw-rw-   0        0        0    15396 2023-04-05 11:38:25.000000 KIF-0.3.1/key_interactions_finder/data_preperation.py
--rw-rw-rw-   0        0        0    35948 2023-03-29 13:17:18.000000 KIF-0.3.1/key_interactions_finder/model_building.py
-drwxrwxrwx   0        0        0        0 2023-07-24 10:11:37.176185 KIF-0.3.1/key_interactions_finder/model_params/
--rw-rw-rw-   0        0        0      418 2022-08-15 09:07:57.000000 KIF-0.3.1/key_interactions_finder/model_params/gridsearch_custom.json
--rw-rw-rw-   0        0        0     4457 2022-08-15 08:59:17.000000 KIF-0.3.1/key_interactions_finder/model_params/gridsearch_exhaustive.json
--rw-rw-rw-   0        0        0     3003 2022-08-15 09:00:56.000000 KIF-0.3.1/key_interactions_finder/model_params/gridsearch_moderate.json
--rw-rw-rw-   0        0        0     1159 2022-03-02 11:45:57.000000 KIF-0.3.1/key_interactions_finder/model_params/gridsearch_none.json
--rw-rw-rw-   0        0        0     1471 2022-08-15 09:01:34.000000 KIF-0.3.1/key_interactions_finder/model_params/gridsearch_quick.json
--rw-rw-rw-   0        0        0    14426 2023-07-14 15:10:53.000000 KIF-0.3.1/key_interactions_finder/network_analysis.py
--rw-rw-rw-   0        0        0    36620 2023-03-29 13:17:18.000000 KIF-0.3.1/key_interactions_finder/post_proccessing.py
--rw-rw-rw-   0        0        0    17183 2023-03-29 13:17:18.000000 KIF-0.3.1/key_interactions_finder/pycontact_processing.py
--rw-rw-rw-   0        0        0    11503 2023-03-29 13:17:18.000000 KIF-0.3.1/key_interactions_finder/pymol_projections.py
--rw-rw-rw-   0        0        0    19316 2023-03-29 13:17:18.000000 KIF-0.3.1/key_interactions_finder/stat_modelling.py
--rw-rw-rw-   0        0        0     7786 2023-04-05 11:38:25.000000 KIF-0.3.1/key_interactions_finder/utils.py
--rw-rw-rw-   0        0        0       42 2023-07-24 10:11:37.176185 KIF-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      978 2023-07-24 10:07:35.000000 KIF-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:48:51.981721 KIF-0.3.2/
+drwxrwxrwx   0        0        0        0 2023-07-25 17:48:51.914095 KIF-0.3.2/KIF.egg-info/
+-rw-rw-rw-   0        0        0      439 2023-07-25 17:48:51.000000 KIF-0.3.2/KIF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      948 2023-07-25 17:48:51.000000 KIF-0.3.2/KIF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 17:48:51.000000 KIF-0.3.2/KIF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-07-25 17:48:51.000000 KIF-0.3.2/KIF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-25 17:48:51.000000 KIF-0.3.2/KIF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    18431 2022-09-22 10:55:30.000000 KIF-0.3.2/LICENSE.md
+-rw-rw-rw-   0        0        0      439 2023-07-25 17:48:51.980719 KIF-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10944 2023-07-24 10:06:40.000000 KIF-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 17:48:51.937569 KIF-0.3.2/key_interactions_finder/
+-rw-rw-rw-   0        0        0        0 2021-12-19 18:36:56.000000 KIF-0.3.2/key_interactions_finder/__init__.py
+-rw-rw-rw-   0        0        0    12253 2023-07-24 10:03:14.000000 KIF-0.3.2/key_interactions_finder/contact_identification.py
+-rw-rw-rw-   0        0        0    10177 2023-07-14 09:23:12.000000 KIF-0.3.2/key_interactions_finder/contact_identification_old.py
+-rw-rw-rw-   0        0        0    15396 2023-04-05 11:38:25.000000 KIF-0.3.2/key_interactions_finder/data_preperation.py
+-rw-rw-rw-   0        0        0    35948 2023-03-29 13:17:18.000000 KIF-0.3.2/key_interactions_finder/model_building.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:48:51.979719 KIF-0.3.2/key_interactions_finder/model_params/
+-rw-rw-rw-   0        0        0      418 2022-08-15 09:07:57.000000 KIF-0.3.2/key_interactions_finder/model_params/gridsearch_custom.json
+-rw-rw-rw-   0        0        0     4457 2022-08-15 08:59:17.000000 KIF-0.3.2/key_interactions_finder/model_params/gridsearch_exhaustive.json
+-rw-rw-rw-   0        0        0     3003 2022-08-15 09:00:56.000000 KIF-0.3.2/key_interactions_finder/model_params/gridsearch_moderate.json
+-rw-rw-rw-   0        0        0     1159 2022-03-02 11:45:57.000000 KIF-0.3.2/key_interactions_finder/model_params/gridsearch_none.json
+-rw-rw-rw-   0        0        0     1471 2022-08-15 09:01:34.000000 KIF-0.3.2/key_interactions_finder/model_params/gridsearch_quick.json
+-rw-rw-rw-   0        0        0    14505 2023-07-25 17:47:58.000000 KIF-0.3.2/key_interactions_finder/network_analysis.py
+-rw-rw-rw-   0        0        0    36620 2023-03-29 13:17:18.000000 KIF-0.3.2/key_interactions_finder/post_proccessing.py
+-rw-rw-rw-   0        0        0    17183 2023-03-29 13:17:18.000000 KIF-0.3.2/key_interactions_finder/pycontact_processing.py
+-rw-rw-rw-   0        0        0    11503 2023-03-29 13:17:18.000000 KIF-0.3.2/key_interactions_finder/pymol_projections.py
+-rw-rw-rw-   0        0        0    19316 2023-03-29 13:17:18.000000 KIF-0.3.2/key_interactions_finder/stat_modelling.py
+-rw-rw-rw-   0        0        0     7786 2023-04-05 11:38:25.000000 KIF-0.3.2/key_interactions_finder/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 17:48:51.981721 KIF-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      978 2023-07-25 17:47:58.000000 KIF-0.3.2/setup.py
```

### Comparing `KIF-0.3.1/KIF.egg-info/SOURCES.txt` & `KIF-0.3.2/KIF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/LICENSE.md` & `KIF-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/README.md` & `KIF-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/key_interactions_finder/contact_identification.py` & `KIF-0.3.2/key_interactions_finder/contact_identification.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/key_interactions_finder/contact_identification_old.py` & `KIF-0.3.2/key_interactions_finder/contact_identification_old.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/key_interactions_finder/data_preperation.py` & `KIF-0.3.2/key_interactions_finder/data_preperation.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/key_interactions_finder/model_building.py` & `KIF-0.3.2/key_interactions_finder/model_building.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/key_interactions_finder/model_params/gridsearch_exhaustive.json` & `KIF-0.3.2/key_interactions_finder/model_params/gridsearch_exhaustive.json`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/key_interactions_finder/model_params/gridsearch_moderate.json` & `KIF-0.3.2/key_interactions_finder/model_params/gridsearch_moderate.json`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/key_interactions_finder/model_params/gridsearch_none.json` & `KIF-0.3.2/key_interactions_finder/model_params/gridsearch_none.json`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/key_interactions_finder/model_params/gridsearch_quick.json` & `KIF-0.3.2/key_interactions_finder/model_params/gridsearch_quick.json`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/key_interactions_finder/network_analysis.py` & `KIF-0.3.2/key_interactions_finder/network_analysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 based analyses tools in different programs.
 
 There is only a single class in this module (CorrelationNetwork) as this module
 does not require a target variable and if you have one it does not need it.
 """
 from dataclasses import dataclass, field
 from typing import Optional
+import re
 import pandas as pd
 import numpy as np
 import MDAnalysis as mda
 from MDAnalysis.analysis import distances
 
 
 @dataclass
@@ -152,20 +153,24 @@
         extract the residue numbers for each contact. (Helper Function.)
 
         Returns
         ----------
         pd.DataFrame
             1st and 2nd residue number of each contact/feature in the dataframe.
         """
-        df_cols = pd.DataFrame(list(self.dataset.columns), columns=["Feature_Names"])
-        df_cols["Res1"] = df_cols["Feature_Names"].str.split("[a-zA-Z]+").str.get(0)
-        df_cols["Res2"] = df_cols["Feature_Names"].str.split("[a-zA-Z]+").str.get(1)
-        df_cols["Res1"] = pd.to_numeric(df_cols["Res1"])
-        df_cols["Res2"] = pd.to_numeric(df_cols["Res2"])
-        return df_cols[["Res1", "Res2"]]
+        res1_numbs, res2_numbs = [], []
+        for residue_pair in list(self.dataset.columns):
+            res1_info, res2_info, _ = residue_pair.split(" ")
+            res1_numb = int(re.findall(r"\d+", res1_info)[0])
+            res2_numb = int(re.findall(r"\d+", res2_info)[0])
+            res1_numbs.append(res1_numb)
+            res2_numbs.append(res2_numb)
+
+        res_pairs_dict = {"Res1": res1_numbs, "Res2": res2_numbs}
+        return pd.DataFrame(res_pairs_dict)
 
     def _get_last_residue(self) -> int:
         """
         Given a dataframe (self.dataset) containing only PyContact features,
         find the last residue in the sequence.
         (Helper function for generating the per residue matrices,
         so one knows when to stop).
```

### Comparing `KIF-0.3.1/key_interactions_finder/post_proccessing.py` & `KIF-0.3.2/key_interactions_finder/post_proccessing.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/key_interactions_finder/pycontact_processing.py` & `KIF-0.3.2/key_interactions_finder/pycontact_processing.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/key_interactions_finder/pymol_projections.py` & `KIF-0.3.2/key_interactions_finder/pymol_projections.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/key_interactions_finder/stat_modelling.py` & `KIF-0.3.2/key_interactions_finder/stat_modelling.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/key_interactions_finder/utils.py` & `KIF-0.3.2/key_interactions_finder/utils.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.1/setup.py` & `KIF-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.3.1"
+VERSION = "0.3.2"
 DESCRIPTION = "Python package for MD simulation analysis"
 LONG_DESCRIPTION = """
     A python package to identify the key molecular interactions that regulate any conformational change."""
 
 setup(
     name="KIF",
     version=VERSION,
```

