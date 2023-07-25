# Comparing `tmp/imat-3.2.1.tar.gz` & `tmp/imat-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imat-3.2.1.tar", last modified: Sun Jul 23 17:09:40 2023, max compression
+gzip compressed data, was "imat-3.2.2.tar", last modified: Tue Jul 25 17:26:47 2023, max compression
```

## Comparing `imat-3.2.1.tar` & `imat-3.2.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:40.551676 imat-3.2.1/
--rw-rw-rw-   0        0        0     1096 2023-07-17 17:26:37.000000 imat-3.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0    15148 2023-07-23 17:09:40.544638 imat-3.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    13939 2023-07-23 17:06:33.000000 imat-3.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:40.201021 imat-3.2.1/iMaT/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/__init__.py
--rw-rw-rw-   0        0        0     2430 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:40.212754 imat-3.2.1/iMaT/src/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:40.250100 imat-3.2.1/iMaT/src/analysis/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/analysis/__init__.py
--rw-rw-rw-   0        0        0    58077 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/analysis/functions.py
--rw-rw-rw-   0        0        0     5213 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/analysis/main.py
--rw-rw-rw-   0        0        0     3630 2023-07-23 16:40:24.000000 imat-3.2.1/iMaT/src/analysis/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:40.275519 imat-3.2.1/iMaT/src/cli/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/cli/__init__.py
--rw-rw-rw-   0        0        0    31663 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/cli/menu_constructors.py
--rw-rw-rw-   0        0        0    23891 2023-07-23 17:04:10.000000 imat-3.2.1/iMaT/src/cli/menu_entries.py
--rw-rw-rw-   0        0        0     7837 2023-07-23 17:08:29.000000 imat-3.2.1/iMaT/src/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:40.282823 imat-3.2.1/iMaT/src/conversion/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/conversion/__init__.py
--rw-rw-rw-   0        0        0     5090 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/conversion/main.py
--rw-rw-rw-   0        0        0    12992 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/conversion/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:40.286563 imat-3.2.1/iMaT/src/m21_environment/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/m21_environment/__init__.py
--rw-rw-rw-   0        0        0    10243 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/m21_environment/main.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:40.309113 imat-3.2.1/iMaT/src/pattern_search/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/pattern_search/__init__.py
--rw-rw-rw-   0        0        0    15880 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/pattern_search/functions.py
--rw-rw-rw-   0        0        0    10903 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/pattern_search/main.py
--rw-rw-rw-   0        0        0    10307 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/pattern_search/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:40.344593 imat-3.2.1/iMaT/src/score_selection/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/score_selection/__init__.py
--rw-rw-rw-   0        0        0    17704 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/score_selection/main.py
--rw-rw-rw-   0        0        0    14028 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/score_selection/name_parts.py
--rw-rw-rw-   0        0        0    12218 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/score_selection/select_parts_and_measures.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:40.362097 imat-3.2.1/iMaT/src/tokenization/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/tokenization/__init__.py
--rw-rw-rw-   0        0        0    19526 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/tokenization/main.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:40.407520 imat-3.2.1/iMaT/src/tokenization/refine_results/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/tokenization/refine_results/__init__.py
--rw-rw-rw-   0        0        0     6837 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/tokenization/refine_results/absolute_duration.py
--rw-rw-rw-   0        0        0     7020 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/tokenization/refine_results/calculate_pitch_intervals.py
--rw-rw-rw-   0        0        0     4966 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/tokenization/refine_results/remove_prefixes.py
--rw-rw-rw-   0        0        0     5447 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/tokenization/refine_results/tokens_to_txt.py
--rw-rw-rw-   0        0        0    15349 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/tokenization/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:40.433567 imat-3.2.1/iMaT/src/utils/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/utils/__init__.py
--rw-rw-rw-   0        0        0     3982 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/utils/error_handling.py
--rw-rw-rw-   0        0        0     6787 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/utils/misc.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:40.496357 imat-3.2.1/iMaT/src/visualizations/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/visualizations/__init__.py
--rw-rw-rw-   0        0        0    19214 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/visualizations/analysis_results_graphs.py
--rw-rw-rw-   0        0        0    10926 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/visualizations/m21_integrated.py
--rw-rw-rw-   0        0        0     3263 2023-07-17 17:26:37.000000 imat-3.2.1/iMaT/src/visualizations/main.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:40.523313 imat-3.2.1/imat.egg-info/
--rw-rw-rw-   0        0        0    15148 2023-07-23 17:09:38.000000 imat-3.2.1/imat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1561 2023-07-23 17:09:38.000000 imat-3.2.1/imat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 17:09:38.000000 imat-3.2.1/imat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-23 17:09:38.000000 imat-3.2.1/imat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      272 2023-07-23 17:09:38.000000 imat-3.2.1/imat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-23 17:09:38.000000 imat-3.2.1/imat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 17:09:40.552673 imat-3.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2105 2023-07-23 17:08:29.000000 imat-3.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.966630 imat-3.2.2/
+-rw-rw-rw-   0        0        0     1096 2023-07-17 17:26:37.000000 imat-3.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    15150 2023-07-25 17:26:47.964609 imat-3.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    13941 2023-07-23 17:13:18.000000 imat-3.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.645465 imat-3.2.2/iMaT/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/__init__.py
+-rw-rw-rw-   0        0        0     2430 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.652445 imat-3.2.2/iMaT/src/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.666416 imat-3.2.2/iMaT/src/analysis/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/analysis/__init__.py
+-rw-rw-rw-   0        0        0    58077 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/analysis/functions.py
+-rw-rw-rw-   0        0        0     5213 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/analysis/main.py
+-rw-rw-rw-   0        0        0     3630 2023-07-23 16:40:24.000000 imat-3.2.2/iMaT/src/analysis/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.674391 imat-3.2.2/iMaT/src/cli/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/cli/__init__.py
+-rw-rw-rw-   0        0        0    31673 2023-07-25 17:21:31.000000 imat-3.2.2/iMaT/src/cli/menu_constructors.py
+-rw-rw-rw-   0        0        0    23891 2023-07-23 17:04:10.000000 imat-3.2.2/iMaT/src/cli/menu_entries.py
+-rw-rw-rw-   0        0        0     7837 2023-07-23 17:08:29.000000 imat-3.2.2/iMaT/src/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.708294 imat-3.2.2/iMaT/src/conversion/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/conversion/__init__.py
+-rw-rw-rw-   0        0        0     5090 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/conversion/main.py
+-rw-rw-rw-   0        0        0    12992 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/conversion/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.716277 imat-3.2.2/iMaT/src/m21_environment/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/m21_environment/__init__.py
+-rw-rw-rw-   0        0        0    10243 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/m21_environment/main.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.740210 imat-3.2.2/iMaT/src/pattern_search/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/pattern_search/__init__.py
+-rw-rw-rw-   0        0        0    15880 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/pattern_search/functions.py
+-rw-rw-rw-   0        0        0    10903 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/pattern_search/main.py
+-rw-rw-rw-   0        0        0    10307 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/pattern_search/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.761154 imat-3.2.2/iMaT/src/score_selection/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/score_selection/__init__.py
+-rw-rw-rw-   0        0        0    17704 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/score_selection/main.py
+-rw-rw-rw-   0        0        0    14028 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/score_selection/name_parts.py
+-rw-rw-rw-   0        0        0    12218 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/score_selection/select_parts_and_measures.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.796060 imat-3.2.2/iMaT/src/tokenization/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/__init__.py
+-rw-rw-rw-   0        0        0    19526 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/main.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.833967 imat-3.2.2/iMaT/src/tokenization/refine_results/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/refine_results/__init__.py
+-rw-rw-rw-   0        0        0     6837 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/refine_results/absolute_duration.py
+-rw-rw-rw-   0        0        0     7020 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/refine_results/calculate_pitch_intervals.py
+-rw-rw-rw-   0        0        0     4966 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/refine_results/remove_prefixes.py
+-rw-rw-rw-   0        0        0     5447 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/refine_results/tokens_to_txt.py
+-rw-rw-rw-   0        0        0    15349 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.859889 imat-3.2.2/iMaT/src/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     3982 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/utils/error_handling.py
+-rw-rw-rw-   0        0        0     6787 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/utils/misc.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.911750 imat-3.2.2/iMaT/src/visualizations/
+-rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/visualizations/__init__.py
+-rw-rw-rw-   0        0        0    19214 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/visualizations/analysis_results_graphs.py
+-rw-rw-rw-   0        0        0    10926 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/visualizations/m21_integrated.py
+-rw-rw-rw-   0        0        0     3263 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/visualizations/main.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.961621 imat-3.2.2/imat.egg-info/
+-rw-rw-rw-   0        0        0    15150 2023-07-25 17:26:46.000000 imat-3.2.2/imat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1561 2023-07-25 17:26:46.000000 imat-3.2.2/imat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 17:26:46.000000 imat-3.2.2/imat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-25 17:26:46.000000 imat-3.2.2/imat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      272 2023-07-25 17:26:46.000000 imat-3.2.2/imat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-25 17:26:46.000000 imat-3.2.2/imat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 17:26:47.967618 imat-3.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2105 2023-07-25 17:25:27.000000 imat-3.2.2/setup.py
```

### Comparing `imat-3.2.1/LICENSE.txt` & `imat-3.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/PKG-INFO` & `imat-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imat
-Version: 3.2.1
+Version: 3.2.2
 Summary: Interactive Music Analysis Tool (I-MaT)
 Home-page: https://github.com/sebastian-eck/I-MaT
 Author: Sebastian Oliver Eck
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -80,15 +80,15 @@
 
 1. The first objective was to design an easily accessible tool with a well-structured interface, further lowering the barrier for musicology students to engage with methods from digital musicology.
 2. The second objective was to further refine and modularize I-MaT’s program code, to create a modular and flexible tool that could effortlessly be extended by either adding new functionalities offered by already integrated modules (such as music21 and MidiTok), or by incorporating new python packages related to digital musicology or other relevant fields, e.g., computational linguistics.
 
 ## I-MaT: Features and Accessibility
 
 ```
-I-MaT - Interactive Music Analysis Tool, v3.1, (2023). Project: "Computer-Assisted Music Analysis"
+I-MaT - Interactive Music Analysis Tool, v3.2.1, (2023). Project: "Computer-Assisted Music Analysis"
 
 Department of Musicology Weimar-Jena, University of Music Franz Liszt Weimar, Germany
 
 MIT License, Copyright (c) 2023 S.O. Eck.
 
 ----------------------------------------------------------------------
```

### Comparing `imat-3.2.1/README.md` & `imat-3.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 1. The first objective was to design an easily accessible tool with a well-structured interface, further lowering the barrier for musicology students to engage with methods from digital musicology.
 2. The second objective was to further refine and modularize I-MaT’s program code, to create a modular and flexible tool that could effortlessly be extended by either adding new functionalities offered by already integrated modules (such as music21 and MidiTok), or by incorporating new python packages related to digital musicology or other relevant fields, e.g., computational linguistics.
 
 ## I-MaT: Features and Accessibility
 
 ```
-I-MaT - Interactive Music Analysis Tool, v3.1, (2023). Project: "Computer-Assisted Music Analysis"
+I-MaT - Interactive Music Analysis Tool, v3.2.1, (2023). Project: "Computer-Assisted Music Analysis"
 
 Department of Musicology Weimar-Jena, University of Music Franz Liszt Weimar, Germany
 
 MIT License, Copyright (c) 2023 S.O. Eck.
 
 ----------------------------------------------------------------------
```

### Comparing `imat-3.2.1/iMaT/__main__.py` & `imat-3.2.2/iMaT/__main__.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/analysis/functions.py` & `imat-3.2.2/iMaT/src/analysis/functions.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/analysis/main.py` & `imat-3.2.2/iMaT/src/analysis/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/analysis/utils.py` & `imat-3.2.2/iMaT/src/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/cli/menu_constructors.py` & `imat-3.2.2/iMaT/src/cli/menu_constructors.py`

 * *Files 0% similar despite different names*

```diff
@@ -570,22 +570,22 @@
 
         # Add headers to col_widths calculation
         col_widths = [max(w, len(header)) for w, header in zip(col_widths, menu_columns_description)]
 
         # Print menu_columns_description in one line
         print("{:<8}".format("No."), end='  ')
         for header, width in zip(menu_columns_description, col_widths):
-            print("{:<{}}".format(header, width), end='  ')
+            print("{:<{}}".format(str(header), width), end='  ')
         print("\n")
 
         # Print menu_entries in multiple lines
         for index, item in enumerate(menu_entries, 1):
             print("{:<8}".format(index), end='  ')
             for i, (entry, width) in enumerate(zip(item, col_widths)):
-                print("{:<{}}".format(entry, width), end='  ')
+                print("{:<{}}".format(str(entry), width), end='  ')
             print()
         print("")
 
     except Exception as e:
         handle_error(e)
```

### Comparing `imat-3.2.1/iMaT/src/cli/menu_entries.py` & `imat-3.2.2/iMaT/src/cli/menu_entries.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/constants.py` & `imat-3.2.2/iMaT/src/constants.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/conversion/main.py` & `imat-3.2.2/iMaT/src/conversion/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/conversion/utils.py` & `imat-3.2.2/iMaT/src/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/m21_environment/main.py` & `imat-3.2.2/iMaT/src/m21_environment/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/pattern_search/functions.py` & `imat-3.2.2/iMaT/src/pattern_search/functions.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/pattern_search/main.py` & `imat-3.2.2/iMaT/src/pattern_search/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/pattern_search/utils.py` & `imat-3.2.2/iMaT/src/pattern_search/utils.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/score_selection/main.py` & `imat-3.2.2/iMaT/src/score_selection/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/score_selection/name_parts.py` & `imat-3.2.2/iMaT/src/score_selection/name_parts.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/score_selection/select_parts_and_measures.py` & `imat-3.2.2/iMaT/src/score_selection/select_parts_and_measures.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/tokenization/main.py` & `imat-3.2.2/iMaT/src/tokenization/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/tokenization/refine_results/absolute_duration.py` & `imat-3.2.2/iMaT/src/tokenization/refine_results/absolute_duration.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/tokenization/refine_results/calculate_pitch_intervals.py` & `imat-3.2.2/iMaT/src/tokenization/refine_results/calculate_pitch_intervals.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/tokenization/refine_results/remove_prefixes.py` & `imat-3.2.2/iMaT/src/tokenization/refine_results/remove_prefixes.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/tokenization/refine_results/tokens_to_txt.py` & `imat-3.2.2/iMaT/src/tokenization/refine_results/tokens_to_txt.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/tokenization/utils.py` & `imat-3.2.2/iMaT/src/tokenization/utils.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/utils/error_handling.py` & `imat-3.2.2/iMaT/src/utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/utils/misc.py` & `imat-3.2.2/iMaT/src/utils/misc.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/visualizations/analysis_results_graphs.py` & `imat-3.2.2/iMaT/src/visualizations/analysis_results_graphs.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/visualizations/m21_integrated.py` & `imat-3.2.2/iMaT/src/visualizations/m21_integrated.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/iMaT/src/visualizations/main.py` & `imat-3.2.2/iMaT/src/visualizations/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/imat.egg-info/PKG-INFO` & `imat-3.2.2/imat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imat
-Version: 3.2.1
+Version: 3.2.2
 Summary: Interactive Music Analysis Tool (I-MaT)
 Home-page: https://github.com/sebastian-eck/I-MaT
 Author: Sebastian Oliver Eck
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -80,15 +80,15 @@
 
 1. The first objective was to design an easily accessible tool with a well-structured interface, further lowering the barrier for musicology students to engage with methods from digital musicology.
 2. The second objective was to further refine and modularize I-MaT’s program code, to create a modular and flexible tool that could effortlessly be extended by either adding new functionalities offered by already integrated modules (such as music21 and MidiTok), or by incorporating new python packages related to digital musicology or other relevant fields, e.g., computational linguistics.
 
 ## I-MaT: Features and Accessibility
 
 ```
-I-MaT - Interactive Music Analysis Tool, v3.1, (2023). Project: "Computer-Assisted Music Analysis"
+I-MaT - Interactive Music Analysis Tool, v3.2.1, (2023). Project: "Computer-Assisted Music Analysis"
 
 Department of Musicology Weimar-Jena, University of Music Franz Liszt Weimar, Germany
 
 MIT License, Copyright (c) 2023 S.O. Eck.
 
 ----------------------------------------------------------------------
```

### Comparing `imat-3.2.1/imat.egg-info/SOURCES.txt` & `imat-3.2.2/imat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imat-3.2.1/setup.py` & `imat-3.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     include_package_data=True,
     name='imat',
-    version='3.2.1',
+    version='3.2.2',
     author='Sebastian Oliver Eck',
     url="https://github.com/sebastian-eck/I-MaT",
     description='Interactive Music Analysis Tool (I-MaT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT License",
     packages=setuptools.find_packages(),
```

