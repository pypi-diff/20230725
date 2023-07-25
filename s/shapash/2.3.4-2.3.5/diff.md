# Comparing `tmp/shapash-2.3.4.tar.gz` & `tmp/shapash-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapash-2.3.4.tar", last modified: Tue May  9 15:43:45 2023, max compression
+gzip compressed data, was "shapash-2.3.5.tar", last modified: Tue Jul 25 14:23:00 2023, max compression
```

## Comparing `shapash-2.3.4.tar` & `shapash-2.3.5.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.627162 shapash-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-09 15:40:53.000000 shapash-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-09 15:40:53.000000 shapash-2.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-05-09 15:43:45.627162 shapash-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20716 2023-05-09 15:40:53.000000 shapash-2.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-09 15:43:45.627162 shapash-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-09 15:40:53.000000 shapash-2.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.619162 shapash-2.3.4/shapash/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.619162 shapash-2.3.4/shapash/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/backend/acv_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/backend/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/backend/lime_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/backend/shap_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.619162 shapash-2.3.4/shapash/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/data/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.619162 shapash-2.3.4/shapash/decomposition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/decomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/decomposition/contributions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.623162 shapash-2.3.4/shapash/explainer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/explainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31311 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/explainer/consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/explainer/multi_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    58279 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/explainer/smart_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)   147181 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/explainer/smart_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/explainer/smart_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/explainer/smart_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.623162 shapash-2.3.4/shapash/manipulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/manipulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/manipulation/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/manipulation/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/manipulation/select_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/manipulation/summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.623162 shapash-2.3.4/shapash/report/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/base_report.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.623162 shapash-2.3.4/shapash/report/html/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/html/double_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/html/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/html/explainability.html
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/html/table_two_columns.html
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/html/univariate.html
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/project_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.619162 shapash-2.3.4/shapash/report/template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.623162 shapash-2.3.4/shapash/report/template/custom/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/template/custom/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/template/custom/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/report/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.623162 shapash-2.3.4/shapash/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/style/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/style/colors.json
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/style/style_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.627162 shapash-2.3.4/shapash/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/category_encoder_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/columntransformer_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/explanation_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/load_smartpredictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/model_synoptic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)    13696 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.627162 shapash-2.3.4/shapash/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.627162 shapash-2.3.4/shapash/webapp/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   215609 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    88144 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/main.js
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/material-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/reload.png
--rw-r--r--   0 runner    (1001) docker     (123)    29911 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)   215609 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/shapash-fond-fonce.png
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/assets/style.css
--rw-r--r--   0 runner    (1001) docker     (123)   138568 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/smart_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.627162 shapash-2.3.4/shapash/webapp/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/utils/MyGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/utils/explanations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/webapp_launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-09 15:40:53.000000 shapash-2.3.4/shapash/webapp/webapp_launch_DVF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:43:45.619162 shapash-2.3.4/shapash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-05-09 15:43:45.000000 shapash-2.3.4/shapash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-09 15:43:45.000000 shapash-2.3.4/shapash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:43:45.000000 shapash-2.3.4/shapash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:43:45.000000 shapash-2.3.4/shapash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-09 15:43:45.000000 shapash-2.3.4/shapash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 15:43:45.000000 shapash-2.3.4/shapash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.461335 shapash-2.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-25 14:19:50.000000 shapash-2.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-25 14:19:50.000000 shapash-2.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22198 2023-07-25 14:23:00.461335 shapash-2.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-07-25 14:19:50.000000 shapash-2.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-25 14:23:00.461335 shapash-2.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-25 14:19:50.000000 shapash-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.449334 shapash-2.3.5/shapash/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.449334 shapash-2.3.5/shapash/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/backend/acv_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/backend/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/backend/lime_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/backend/shap_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.449334 shapash-2.3.5/shapash/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/data/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.449334 shapash-2.3.5/shapash/decomposition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/decomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/decomposition/contributions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.453334 shapash-2.3.5/shapash/explainer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/explainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31292 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/explainer/consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/explainer/multi_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58279 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/explainer/smart_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147181 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/explainer/smart_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/explainer/smart_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/explainer/smart_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.453334 shapash-2.3.5/shapash/manipulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/manipulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/manipulation/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/manipulation/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/manipulation/select_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/manipulation/summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.453334 shapash-2.3.5/shapash/report/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/base_report.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.453334 shapash-2.3.5/shapash/report/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/html/double_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/html/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/html/explainability.html
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/html/table_two_columns.html
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/html/univariate.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21937 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/project_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.445334 shapash-2.3.5/shapash/report/template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.453334 shapash-2.3.5/shapash/report/template/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/template/custom/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/template/custom/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/report/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.453334 shapash-2.3.5/shapash/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/style/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/style/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/style/style_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.457335 shapash-2.3.5/shapash/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/utils/category_encoder_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/utils/columntransformer_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/utils/explanation_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/utils/load_smartpredictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/utils/model_synoptic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/utils/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13696 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/utils/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/utils/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.457335 shapash-2.3.5/shapash/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.461335 shapash-2.3.5/shapash/webapp/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   215609 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    88144 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/assets/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/assets/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/assets/material-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/assets/reload.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29911 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/assets/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)   215609 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/assets/shapash-fond-fonce.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/assets/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)   138568 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/smart_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.461335 shapash-2.3.5/shapash/webapp/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/utils/MyGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/utils/explanations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/webapp_launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-25 14:19:50.000000 shapash-2.3.5/shapash/webapp/webapp_launch_DVF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:23:00.449334 shapash-2.3.5/shapash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22198 2023-07-25 14:23:00.000000 shapash-2.3.5/shapash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-25 14:23:00.000000 shapash-2.3.5/shapash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:23:00.000000 shapash-2.3.5/shapash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:23:00.000000 shapash-2.3.5/shapash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-25 14:23:00.000000 shapash-2.3.5/shapash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 14:23:00.000000 shapash-2.3.5/shapash.egg-info/top_level.txt
```

### Comparing `shapash-2.3.4/LICENSE` & `shapash-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/PKG-INFO` & `shapash-2.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapash
-Version: 2.3.4
+Version: 2.3.5
 Summary: Shapash is a Python library which aims to make machine learning interpretable and understandable by everyone.
 Home-page: https://github.com/MAIF/shapash
 Author: Yann Golhen, Sebastien Bidault, Yann Lagre, Maxime Gendre
 Author-email: yann.golhen@maif.fr
 License: Apache Software License 2.0
 Keywords: shapash
 Classifier: Programming Language :: Python :: 3
@@ -56,24 +56,24 @@
 </p>
 
 ## 🎉 What's new ?
 
 
 | Version       | New Feature                                                                           | Description                                                                                                                            | Tutorial |
 |:-------------:|:-------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
-| 2.3.x         |  Additional dataset columns <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                | In Webapp: Target and error columns added to dataset and possibility to add features outside the model for more filtering options            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/add_column_icon.png" width="50" title="add_column">](https://github.com/MAIF/shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb)
-| 2.3.x         |  Identity card <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                  | In Webapp: New identity card to summarize the information of the selected sample                  |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/identity_card.png" width="50" title="identity">](https://github.com/MAIF/shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb)
-| 2.2.x         |  Picking samples <br> [Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-machine-learning-model.html)                                                                | New tab in the webapp for picking samples. The graph represents the "True Values Vs Predicted Values"            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png" width="50" title="picking">](https://github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-prediction_plot.ipynb)
+| 2.3.x         |  Additional dataset columns <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                | In Webapp: Target and error columns added to dataset and possibility to add features outside the model for more filtering options            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/add_column_icon.png" width="50" title="add_column">](https://github.com/MAIF/shapash/blob/master/tutorial/generate_webapp/tuto-webapp01-additional-data.ipynb)
+| 2.3.x         |  Identity card <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                  | In Webapp: New identity card to summarize the information of the selected sample                  |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/identity_card.png" width="50" title="identity">](https://github.com/MAIF/shapash/blob/master/tutorial/generate_webapp/tuto-webapp01-additional-data.ipynb)
+| 2.2.x         |  Picking samples <br> [Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-machine-learning-model.html)                                                                | New tab in the webapp for picking samples. The graph represents the "True Values Vs Predicted Values"            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png" width="50" title="picking">](https://github.com/MAIF/shapash/blob/master/tutorial/plots_and_charts/tuto-plot06-prediction_plot.ipynb)
 | 2.2.x         |  Dataset Filter <br>                                                              | New tab in the webapp to filter data. And several improvements in the webapp: subtitles, labels, screen adjustments                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/webapp.png" width="50" title="webapp">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
-| 2.0.x         |  Refactoring Shapash <br>                                                                   | Refactoring attributes of compile methods and init. Refactoring implementation for new backends                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/modular.png" width="50" title="modular">](https://github.com/MAIF/shapash/blob/master/tutorial/backend/tuto-backend-01.ipynb)
+| 2.0.x         |  Refactoring Shapash <br>                                                                   | Refactoring attributes of compile methods and init. Refactoring implementation for new backends                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/modular.png" width="50" title="modular">](https://github.com/MAIF/shapash/blob/master/tutorial/explainer_and_backend/tuto-expl06-Shapash-custom-backend.ipynb)
 | 1.7.x         |  Variabilize Colors <br>                                                                   | Giving possibility to have your own colour palette for outputs adapted to your design                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/variabilize-colors.png" width="50" title="variabilize-colors">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common02-colors.ipynb)
 | 1.6.x         |  Explainability Quality Metrics <br> [Article](https://towardsdatascience.com/building-confidence-on-explainability-methods-66b9ee575514)                                                                   | To help increase confidence in explainability methods, you can evaluate the relevance of your explainability using 3 metrics: **Stability**, **Consistency** and **Compacity**                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-metrics.png" width="50" title="quality-metrics">](https://github.com/MAIF/shapash/blob/master/tutorial/explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb) 
-| 1.5.x         |  ACV Backend <br>                                                                     | A new way of estimating Shapley values using ACV. [More info about ACV here](https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-cfea30509254).                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/wheel.png" width="50" title="wheel-acv-backend">](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb)    |
+| 1.5.x         |  ACV Backend <br>                                                                     | A new way of estimating Shapley values using ACV. [More info about ACV here](https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-cfea30509254).                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/wheel.png" width="50" title="wheel-acv-backend">](tutorial/explainer_and_backend/tuto-expl03-Shapash-acv-backend.ipynb)    |
 | 1.4.x         |  Groups of features <br> [Demo](https://shapash-demo2.ossbymaif.fr/)                  | You can now regroup features that share common properties together. <br>This option can be useful if your model has a lot of features. |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/groups_features.gif" width="120" title="groups-features">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common01-groups_of_features.ipynb)    | 
-| 1.3.x         |  Shapash Report <br> [Demo](https://shapash.readthedocs.io/en/latest/report.html)     | A standalone HTML report that constitutes a basis of an audit document.                                                                |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png" width="50" title="shapash-report">](https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-report01.ipynb)    | 
+| 1.3.x         |  Shapash Report <br> [Demo](https://shapash.readthedocs.io/en/latest/report.html)     | A standalone HTML report that constitutes a basis of an audit document.                                                                |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png" width="50" title="shapash-report">](https://github.com/MAIF/shapash/blob/master/tutorial/generate_report/tuto-shapash-report01.ipynb)    | 
 
 
 ## 🔍 Overview
 
 **Shapash** is a Python library which aims to make machine learning interpretable and understandable by everyone.
 It provides several types of visualization that display explicit labels that everyone can understand. 
 
@@ -247,15 +247,15 @@
     project_info_file='path/to/project_info.yml',
     x_train=Xtrain,
     y_train=ytrain,
     y_test=ytest,
     title_story="House prices report",
     title_description="""This document is a data science report of the kaggle house prices tutorial project.
         It was generated using the Shapash library.""",
-    metrics=[{‘name’: ‘MSE’, ‘path’: ‘sklearn.metrics.mean_squared_error’}]
+    metrics=[{'name': 'MSE', 'path': 'sklearn.metrics.mean_squared_error'}]
 )
 ```
 
 [Report Example](https://shapash.readthedocs.io/en/latest/report.html)
 
 - Step 5: From training to deployment : SmartPredictor Object
   > Shapash provides a SmartPredictor object to deploy the summary of local explanation for the operational needs.
@@ -274,62 +274,65 @@
 
 <details><summary><b>Overview</b> </summary>
 
 - [Launch the webapp with a concrete use case](tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
 - [Jupyter Overviews - The main outputs and methods available with the SmartExplainer object](tutorial/tutorial02-Shapash-overview-in-Jupyter.ipynb)
 - [Shapash in production: From model training to deployment (API or Batch Mode)](tutorial/tutorial03-Shapash-overview-model-in-production.ipynb)
 - [Use groups of features](tutorial/common/tuto-common01-groups_of_features.ipynb)
-- [Deploy local explainability in production with SmartPredictor](tutorial/predictor/tuto-smartpredictor-introduction-to-SmartPredictor.ipynb)
+- [Deploy local explainability in production with SmartPredictor](tutorial/predictor_to_production/tuto-smartpredictor-introduction-to-SmartPredictor.ipynb)
 
 </details>
 
 <details><summary><b>Charts and plots</b> </summary>
 
-- [**Shapash** Features Importance](tutorial/plot/tuto-plot03-features-importance.ipynb)
-- [Contribution plot to understand how one feature affects a prediction](tutorial/plot/tuto-plot02-contribution_plot.ipynb)
-- [Summarize, display and export local contribution using filter and local_plot method](tutorial/plot/tuto-plot01-local_plot-and-to_pandas.ipynb)
-- [Contributions Comparing plot to understand why predictions on several individuals are different](tutorial/plot/tuto-plot04-compare_plot.ipynb)
-- [Visualize interactions between couple of variables](tutorial/plot/tuto-plot05-interactions-plot.ipynb)
+- [**Shapash** Features Importance](tutorial/plots_and_charts/tuto-plot03-features-importance.ipynb)
+- [Contribution plot to understand how one feature affects a prediction](tutorial/plots_and_charts/tuto-plot02-contribution_plot.ipynb)
+- [Summarize, display and export local contribution using filter and local_plot method](tutorial/plots_and_charts/tuto-plot01-local_plot-and-to_pandas.ipynb)
+- [Contributions Comparing plot to understand why predictions on several individuals are different](tutorial/plots_and_charts/tuto-plot04-compare_plot.ipynb)
+- [Visualize interactions between couple of variables](tutorial/plots_and_charts/tuto-plot05-interactions-plot.ipynb)
+- [Display True Values Vs Predicted Values](tutorial/plots_and_charts/tuto-plot06-prediction_plot.ipynb)
 - [Customize colors in Webapp, plots and report](tutorial/common/tuto-common02-colors.ipynb)
 
 </details>
 
 <details><summary><b>Different ways to use Encoders and Dictionaries</b> </summary>
 
-- [Use Category_Encoder & inverse transformation](tutorial/encoder/tuto-encoder01-using-category_encoder.ipynb)
-- [Use ColumnTransformers](tutorial/encoder/tuto-encoder02-using-columntransformer.ipynb)
-- [Use Simple Python Dictionnaries](tutorial/encoder/tuto-encoder03-using-dict.ipynb)
+- [Use Category_Encoder & inverse transformation](tutorial/use_encoders/tuto-encoder01-using-category_encoder.ipynb)
+- [Use ColumnTransformers](tutorial/use_encoders/tuto-encoder02-using-columntransformer.ipynb)
+- [Use Simple Python Dictionnaries](tutorial/use_encoders/tuto-encoder03-using-dict.ipynb)
 
 </details>
 
 <details><summary><b>Displaying data with postprocessing</b> </summary>
 
 [Using postprocessing parameter in compile method](tutorial/postprocess/tuto-postprocess01.ipynb)
 
 </details>
 
 <details><summary><b>Using different backends</b> </summary>
 
-- [Compute Shapley Contributions using **Shap**](tutorial/explainer/tuto-expl01-Shapash-Viz-using-Shap-contributions.ipynb)
-- [Use **Lime** to compute local explanation, Summarize-it with **Shapash**](tutorial/explainer/tuto-expl02-Shapash-Viz-using-Lime-contributions.ipynb)
-- [Use **ACV backend** to compute Active Shapley Values and SDP global importance](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb)
-- [Compile faster Lime and consistency of contributions](tutorial/explainer/tuto-expl04-Shapash-compute-Lime-faster.ipynb)
+- [Compute Shapley Contributions using **Shap**](tutorial/explainer_and_backend/tuto-expl01-Shapash-Viz-using-Shap-contributions.ipynb)
+- [Use **Lime** to compute local explanation, Summarize-it with **Shapash**](tutorial/explainer_and_backend/tuto-expl02-Shapash-Viz-using-Lime-contributions.ipynb)
+- [Use **ACV backend** to compute Active Shapley Values and SDP global importance](tutorial/explainer_and_backend/tuto-expl03-Shapash-acv-backend.ipynb)
+- [Compile faster Lime and consistency of contributions](tutorial/explainer_and_backend/tuto-expl04-Shapash-compute-Lime-faster.ipynb)
+- [Use **FastTreeSHAP** or add contributions from another backend](tutorial/explainer_and_backend/tuto-expl05-Shapash-using-Fasttreeshap.ipynb)
+- [Use Class Shapash Backend](tutorial/explainer_and_backend/tuto-expl06-Shapash-custom-backend.ipynb)
 
 </details>
 
 <details><summary><b>Evaluating the quality of your explainability</b> </summary>
 
 - [Building confidence on explainability methods using **Stability**, **Consistency** and **Compacity** metrics](tutorial/explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb)
 
 </details>
 
 <details><summary><b>Generate a report of your project</b> </summary>
 
-- [Generate a standalone HTML report of your project with generate_report](tutorial/report/tuto-shapash-report01.ipynb)
+- [Generate a standalone HTML report of your project with generate_report](tutorial/generate_report/tuto-shapash-report01.ipynb)
 
 </details>
 
 <details><summary><b>Analysing your model via Shapash WebApp</b> </summary>
 
-- [Add features outside of the model for more exploration options](tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+- [Add features outside of the model for more exploration options](tutorial/generate_webapp/tuto-webapp01-additional-data.ipynb)
 
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shapash Version: 2.3.4 Summary: Shapash is a Python
+Metadata-Version: 2.1 Name: shapash Version: 2.3.5 Summary: Shapash is a Python
 library which aims to make machine learning interpretable and understandable by
 everyone. Home-page: https://github.com/MAIF/shapash Author: Yann Golhen,
 Sebastien Bidault, Yann Lagre, Maxime Gendre Author-email: yann.golhen@maif.fr
 License: Apache Software License 2.0 Keywords: shapash Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
@@ -20,37 +20,38 @@
 -------:| | 2.3.x | Additional dataset columns
 [New demo](https://shapash-demo.ossbymaif.fr/)
 [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-
 interpretation-40b50157c2fb) | In Webapp: Target and error columns added to
 dataset and possibility to add features outside the model for more filtering
 options | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
 add_column_icon.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
-webapp/tuto-webapp01-additional-data.ipynb) | 2.3.x | Identity card
+generate_webapp/tuto-webapp01-additional-data.ipynb) | 2.3.x | Identity card
 [New demo](https://shapash-demo.ossbymaif.fr/)
 [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-
 interpretation-40b50157c2fb) | In Webapp: New identity card to summarize the
 information of the selected sample | [[https://raw.githubusercontent.com/MAIF/
 shapash/master/docs/_static/identity_card.png]](https://github.com/MAIF/
-shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb) |
-2.2.x | Picking samples
+shapash/blob/master/tutorial/generate_webapp/tuto-webapp01-additional-
+data.ipynb) | 2.2.x | Picking samples
 [Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-
 machine-learning-model.html) | New tab in the webapp for picking samples. The
 graph represents the "True Values Vs Predicted Values" | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png]](https:
-//github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-
+//github.com/MAIF/shapash/blob/master/tutorial/plots_and_charts/tuto-plot06-
 prediction_plot.ipynb) | 2.2.x | Dataset Filter
 | New tab in the webapp to filter data. And several improvements in the webapp:
 subtitles, labels, screen adjustments | [[https://raw.githubusercontent.com/
 MAIF/shapash/master/docs/_static/webapp.png]](https://github.com/MAIF/shapash/
 blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.0.x |
 Refactoring Shapash
 | Refactoring attributes of compile methods and init. Refactoring
 implementation for new backends | [[https://raw.githubusercontent.com/MAIF/
 shapash/master/docs/_static/modular.png]](https://github.com/MAIF/shapash/blob/
-master/tutorial/backend/tuto-backend-01.ipynb) | 1.7.x | Variabilize Colors
+master/tutorial/explainer_and_backend/tuto-expl06-Shapash-custom-backend.ipynb)
+| 1.7.x | Variabilize Colors
 | Giving possibility to have your own colour palette for outputs adapted to
 your design | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
 _static/variabilize-colors.png]](https://github.com/MAIF/shapash/blob/master/
 tutorial/common/tuto-common02-colors.ipynb) | 1.6.x | Explainability Quality
 Metrics
 [Article](https://towardsdatascience.com/building-confidence-on-explainability-
 methods-66b9ee575514) | To help increase confidence in explainability methods,
@@ -59,36 +60,36 @@
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-
 metrics.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
 explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb)
 | 1.5.x | ACV Backend
 | A new way of estimating Shapley values using ACV. [More info about ACV here]
 (https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-
 cfea30509254). | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
-_static/wheel.png]](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb) |
-| 1.4.x | Groups of features
+_static/wheel.png]](tutorial/explainer_and_backend/tuto-expl03-Shapash-acv-
+backend.ipynb) | | 1.4.x | Groups of features
 [Demo](https://shapash-demo2.ossbymaif.fr/) | You can now regroup features that
 share common properties together.
 This option can be useful if your model has a lot of features. | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
 groups_features.gif]](https://github.com/MAIF/shapash/blob/master/tutorial/
 common/tuto-common01-groups_of_features.ipynb) | | 1.3.x | Shapash Report
 [Demo](https://shapash.readthedocs.io/en/latest/report.html) | A standalone
 HTML report that constitutes a basis of an audit document. | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png]]
-(https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-
-report01.ipynb) | ## ð Overview **Shapash** is a Python library which aims
-to make machine learning interpretable and understandable by everyone. It
-provides several types of visualization that display explicit labels that
-everyone can understand. Data Scientists can understand their models easily and
-share their results. End users can understand the decision proposed by a model
-using a summary of the most influential criteria. Shapash also contributes to
-data science auditing by displaying usefull information about any model and
-data in a unique report. - Readthedocs: [![documentation badge](https://
-readthedocs.org/projects/shapash/badge/?version=latest)](https://
-shapash.readthedocs.io/en/latest/) - [Presentation video for french speakers]
+(https://github.com/MAIF/shapash/blob/master/tutorial/generate_report/tuto-
+shapash-report01.ipynb) | ## ð Overview **Shapash** is a Python library
+which aims to make machine learning interpretable and understandable by
+everyone. It provides several types of visualization that display explicit
+labels that everyone can understand. Data Scientists can understand their
+models easily and share their results. End users can understand the decision
+proposed by a model using a summary of the most influential criteria. Shapash
+also contributes to data science auditing by displaying usefull information
+about any model and data in a unique report. - Readthedocs: [![documentation
+badge](https://readthedocs.org/projects/shapash/badge/?version=latest)](https:/
+/shapash.readthedocs.io/en/latest/) - [Presentation video for french speakers]
 (https://www.youtube.com/watch?v=r1R_A9B9apk) - Medium: - [Understand your
 model with Shapash - Towards AI](https://pub.towardsai.net/shapash-making-ml-
 models-understandable-by-everyone-8f96ad469eb3) - [Model auditability - Towards
 DS](https://towardsdatascience.com/shapash-1-3-2-announcing-new-features-for-
 more-auditable-ai-64a6db71c919) - [Group of features - Towards AI](https://
 pub.towardsai.net/machine-learning-6011d5d9a444) - [Building confidence on
 explainability - Towards DS](https://towardsdatascience.com/building-
@@ -186,58 +187,66 @@
 Generate the Shapash Report > This step allows to generate a standalone html
 report of your project using the different splits of your dataset and also the
 metrics you used: ``` xpl.generate_report( output_file='path/to/output/
 report.html', project_info_file='path/to/project_info.yml', x_train=Xtrain,
 y_train=ytrain, y_test=ytest, title_story="House prices report",
 title_description="""This document is a data science report of the kaggle house
 prices tutorial project. It was generated using the Shapash library.""",
-metrics=[{ânameâ: âMSEâ, âpathâ:
-âsklearn.metrics.mean_squared_errorâ}] ) ``` [Report Example](https://
-shapash.readthedocs.io/en/latest/report.html) - Step 5: From training to
-deployment : SmartPredictor Object > Shapash provides a SmartPredictor object
-to deploy the summary of local explanation for the operational needs. It is an
-object dedicated to deployment, lighter than SmartExplainer with additional
-consistency checks. SmartPredictor can be used with an API or in batch mode. It
-provides predictions, detailed or summarized local explainability using
-appropriate wording. ``` predictor = xpl.to_smartpredictor() ``` See the
-tutorial part to know how to use the SmartPredictor object ## ð Tutorials
-This github repository offers many tutorials to allow you to easily get started
-with Shapash. Overview  - [Launch the webapp with a concrete use case]
-(tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb) - [Jupyter Overviews
-- The main outputs and methods available with the SmartExplainer object]
-(tutorial/tutorial02-Shapash-overview-in-Jupyter.ipynb) - [Shapash in
-production: From model training to deployment (API or Batch Mode)](tutorial/
-tutorial03-Shapash-overview-model-in-production.ipynb) - [Use groups of
-features](tutorial/common/tuto-common01-groups_of_features.ipynb) - [Deploy
-local explainability in production with SmartPredictor](tutorial/predictor/
-tuto-smartpredictor-introduction-to-SmartPredictor.ipynb)  Charts and plots  -
-[**Shapash** Features Importance](tutorial/plot/tuto-plot03-features-
+metrics=[{'name': 'MSE', 'path': 'sklearn.metrics.mean_squared_error'}] ) ```
+[Report Example](https://shapash.readthedocs.io/en/latest/report.html) - Step
+5: From training to deployment : SmartPredictor Object > Shapash provides a
+SmartPredictor object to deploy the summary of local explanation for the
+operational needs. It is an object dedicated to deployment, lighter than
+SmartExplainer with additional consistency checks. SmartPredictor can be used
+with an API or in batch mode. It provides predictions, detailed or summarized
+local explainability using appropriate wording. ``` predictor =
+xpl.to_smartpredictor() ``` See the tutorial part to know how to use the
+SmartPredictor object ## ð Tutorials This github repository offers many
+tutorials to allow you to easily get started with Shapash. Overview  - [Launch
+the webapp with a concrete use case](tutorial/tutorial01-Shapash-Overview-
+Launch-WebApp.ipynb) - [Jupyter Overviews - The main outputs and methods
+available with the SmartExplainer object](tutorial/tutorial02-Shapash-overview-
+in-Jupyter.ipynb) - [Shapash in production: From model training to deployment
+(API or Batch Mode)](tutorial/tutorial03-Shapash-overview-model-in-
+production.ipynb) - [Use groups of features](tutorial/common/tuto-common01-
+groups_of_features.ipynb) - [Deploy local explainability in production with
+SmartPredictor](tutorial/predictor_to_production/tuto-smartpredictor-
+introduction-to-SmartPredictor.ipynb)  Charts and plots  - [**Shapash**
+Features Importance](tutorial/plots_and_charts/tuto-plot03-features-
 importance.ipynb) - [Contribution plot to understand how one feature affects a
-prediction](tutorial/plot/tuto-plot02-contribution_plot.ipynb) - [Summarize,
-display and export local contribution using filter and local_plot method]
-(tutorial/plot/tuto-plot01-local_plot-and-to_pandas.ipynb) - [Contributions
-Comparing plot to understand why predictions on several individuals are
-different](tutorial/plot/tuto-plot04-compare_plot.ipynb) - [Visualize
-interactions between couple of variables](tutorial/plot/tuto-plot05-
-interactions-plot.ipynb) - [Customize colors in Webapp, plots and report]
+prediction](tutorial/plots_and_charts/tuto-plot02-contribution_plot.ipynb) -
+[Summarize, display and export local contribution using filter and local_plot
+method](tutorial/plots_and_charts/tuto-plot01-local_plot-and-to_pandas.ipynb) -
+[Contributions Comparing plot to understand why predictions on several
+individuals are different](tutorial/plots_and_charts/tuto-plot04-
+compare_plot.ipynb) - [Visualize interactions between couple of variables]
+(tutorial/plots_and_charts/tuto-plot05-interactions-plot.ipynb) - [Display True
+Values Vs Predicted Values](tutorial/plots_and_charts/tuto-plot06-
+prediction_plot.ipynb) - [Customize colors in Webapp, plots and report]
 (tutorial/common/tuto-common02-colors.ipynb)  Different ways to use Encoders
 and Dictionaries  - [Use Category_Encoder & inverse transformation](tutorial/
-encoder/tuto-encoder01-using-category_encoder.ipynb) - [Use ColumnTransformers]
-(tutorial/encoder/tuto-encoder02-using-columntransformer.ipynb) - [Use Simple
-Python Dictionnaries](tutorial/encoder/tuto-encoder03-using-dict.ipynb)
-Displaying data with postprocessing  [Using postprocessing parameter in compile
-method](tutorial/postprocess/tuto-postprocess01.ipynb)  Using different
-backends  - [Compute Shapley Contributions using **Shap**](tutorial/explainer/
-tuto-expl01-Shapash-Viz-using-Shap-contributions.ipynb) - [Use **Lime** to
-compute local explanation, Summarize-it with **Shapash**](tutorial/explainer/
-tuto-expl02-Shapash-Viz-using-Lime-contributions.ipynb) - [Use **ACV backend**
-to compute Active Shapley Values and SDP global importance](tutorial/explainer/
-tuto-expl03-Shapash-acv-backend.ipynb) - [Compile faster Lime and consistency
-of contributions](tutorial/explainer/tuto-expl04-Shapash-compute-Lime-
-faster.ipynb)  Evaluating the quality of your explainability  - [Building
-confidence on explainability methods using **Stability**, **Consistency** and
-**Compacity** metrics](tutorial/explainability_quality/tuto-quality01-Builing-
-confidence-explainability.ipynb)  Generate a report of your project  -
-[Generate a standalone HTML report of your project with generate_report]
-(tutorial/report/tuto-shapash-report01.ipynb)  Analysing your model via Shapash
-WebApp  - [Add features outside of the model for more exploration options]
-(tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+use_encoders/tuto-encoder01-using-category_encoder.ipynb) - [Use
+ColumnTransformers](tutorial/use_encoders/tuto-encoder02-using-
+columntransformer.ipynb) - [Use Simple Python Dictionnaries](tutorial/
+use_encoders/tuto-encoder03-using-dict.ipynb)  Displaying data with
+postprocessing  [Using postprocessing parameter in compile method](tutorial/
+postprocess/tuto-postprocess01.ipynb)  Using different backends  - [Compute
+Shapley Contributions using **Shap**](tutorial/explainer_and_backend/tuto-
+expl01-Shapash-Viz-using-Shap-contributions.ipynb) - [Use **Lime** to compute
+local explanation, Summarize-it with **Shapash**](tutorial/
+explainer_and_backend/tuto-expl02-Shapash-Viz-using-Lime-contributions.ipynb) -
+[Use **ACV backend** to compute Active Shapley Values and SDP global
+importance](tutorial/explainer_and_backend/tuto-expl03-Shapash-acv-
+backend.ipynb) - [Compile faster Lime and consistency of contributions]
+(tutorial/explainer_and_backend/tuto-expl04-Shapash-compute-Lime-faster.ipynb)
+- [Use **FastTreeSHAP** or add contributions from another backend](tutorial/
+explainer_and_backend/tuto-expl05-Shapash-using-Fasttreeshap.ipynb) - [Use
+Class Shapash Backend](tutorial/explainer_and_backend/tuto-expl06-Shapash-
+custom-backend.ipynb)  Evaluating the quality of your explainability  -
+[Building confidence on explainability methods using **Stability**,
+**Consistency** and **Compacity** metrics](tutorial/explainability_quality/
+tuto-quality01-Builing-confidence-explainability.ipynb)  Generate a report of
+your project  - [Generate a standalone HTML report of your project with
+generate_report](tutorial/generate_report/tuto-shapash-report01.ipynb)
+Analysing your model via Shapash WebApp  - [Add features outside of the model
+for more exploration options](tutorial/generate_webapp/tuto-webapp01-
+additional-data.ipynb)
```

### Comparing `shapash-2.3.4/README.md` & `shapash-2.3.5/shapash.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: shapash
+Version: 2.3.5
+Summary: Shapash is a Python library which aims to make machine learning interpretable and understandable by everyone.
+Home-page: https://github.com/MAIF/shapash
+Author: Yann Golhen, Sebastien Bidault, Yann Lagre, Maxime Gendre
+Author-email: yann.golhen@maif.fr
+License: Apache Software License 2.0
+Keywords: shapash
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >3.7, <3.11
+Description-Content-Type: text/markdown
+Provides-Extra: report
+Provides-Extra: xgboost
+Provides-Extra: lightgbm
+Provides-Extra: catboost
+Provides-Extra: acv
+Provides-Extra: lime
+License-File: LICENSE
+
 <p align="center">
 <img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/shapash-resize.png" width="300" title="shapash-logo">
 </p>
 
 
 <p align="center">
   <!-- Tests -->
@@ -31,24 +56,24 @@
 </p>
 
 ## 🎉 What's new ?
 
 
 | Version       | New Feature                                                                           | Description                                                                                                                            | Tutorial |
 |:-------------:|:-------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
-| 2.3.x         |  Additional dataset columns <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                | In Webapp: Target and error columns added to dataset and possibility to add features outside the model for more filtering options            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/add_column_icon.png" width="50" title="add_column">](https://github.com/MAIF/shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb)
-| 2.3.x         |  Identity card <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                  | In Webapp: New identity card to summarize the information of the selected sample                  |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/identity_card.png" width="50" title="identity">](https://github.com/MAIF/shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb)
-| 2.2.x         |  Picking samples <br> [Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-machine-learning-model.html)                                                                | New tab in the webapp for picking samples. The graph represents the "True Values Vs Predicted Values"            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png" width="50" title="picking">](https://github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-prediction_plot.ipynb)
+| 2.3.x         |  Additional dataset columns <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                | In Webapp: Target and error columns added to dataset and possibility to add features outside the model for more filtering options            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/add_column_icon.png" width="50" title="add_column">](https://github.com/MAIF/shapash/blob/master/tutorial/generate_webapp/tuto-webapp01-additional-data.ipynb)
+| 2.3.x         |  Identity card <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                  | In Webapp: New identity card to summarize the information of the selected sample                  |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/identity_card.png" width="50" title="identity">](https://github.com/MAIF/shapash/blob/master/tutorial/generate_webapp/tuto-webapp01-additional-data.ipynb)
+| 2.2.x         |  Picking samples <br> [Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-machine-learning-model.html)                                                                | New tab in the webapp for picking samples. The graph represents the "True Values Vs Predicted Values"            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png" width="50" title="picking">](https://github.com/MAIF/shapash/blob/master/tutorial/plots_and_charts/tuto-plot06-prediction_plot.ipynb)
 | 2.2.x         |  Dataset Filter <br>                                                              | New tab in the webapp to filter data. And several improvements in the webapp: subtitles, labels, screen adjustments                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/webapp.png" width="50" title="webapp">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
-| 2.0.x         |  Refactoring Shapash <br>                                                                   | Refactoring attributes of compile methods and init. Refactoring implementation for new backends                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/modular.png" width="50" title="modular">](https://github.com/MAIF/shapash/blob/master/tutorial/backend/tuto-backend-01.ipynb)
+| 2.0.x         |  Refactoring Shapash <br>                                                                   | Refactoring attributes of compile methods and init. Refactoring implementation for new backends                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/modular.png" width="50" title="modular">](https://github.com/MAIF/shapash/blob/master/tutorial/explainer_and_backend/tuto-expl06-Shapash-custom-backend.ipynb)
 | 1.7.x         |  Variabilize Colors <br>                                                                   | Giving possibility to have your own colour palette for outputs adapted to your design                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/variabilize-colors.png" width="50" title="variabilize-colors">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common02-colors.ipynb)
 | 1.6.x         |  Explainability Quality Metrics <br> [Article](https://towardsdatascience.com/building-confidence-on-explainability-methods-66b9ee575514)                                                                   | To help increase confidence in explainability methods, you can evaluate the relevance of your explainability using 3 metrics: **Stability**, **Consistency** and **Compacity**                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-metrics.png" width="50" title="quality-metrics">](https://github.com/MAIF/shapash/blob/master/tutorial/explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb) 
-| 1.5.x         |  ACV Backend <br>                                                                     | A new way of estimating Shapley values using ACV. [More info about ACV here](https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-cfea30509254).                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/wheel.png" width="50" title="wheel-acv-backend">](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb)    |
+| 1.5.x         |  ACV Backend <br>                                                                     | A new way of estimating Shapley values using ACV. [More info about ACV here](https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-cfea30509254).                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/wheel.png" width="50" title="wheel-acv-backend">](tutorial/explainer_and_backend/tuto-expl03-Shapash-acv-backend.ipynb)    |
 | 1.4.x         |  Groups of features <br> [Demo](https://shapash-demo2.ossbymaif.fr/)                  | You can now regroup features that share common properties together. <br>This option can be useful if your model has a lot of features. |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/groups_features.gif" width="120" title="groups-features">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common01-groups_of_features.ipynb)    | 
-| 1.3.x         |  Shapash Report <br> [Demo](https://shapash.readthedocs.io/en/latest/report.html)     | A standalone HTML report that constitutes a basis of an audit document.                                                                |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png" width="50" title="shapash-report">](https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-report01.ipynb)    | 
+| 1.3.x         |  Shapash Report <br> [Demo](https://shapash.readthedocs.io/en/latest/report.html)     | A standalone HTML report that constitutes a basis of an audit document.                                                                |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png" width="50" title="shapash-report">](https://github.com/MAIF/shapash/blob/master/tutorial/generate_report/tuto-shapash-report01.ipynb)    | 
 
 
 ## 🔍 Overview
 
 **Shapash** is a Python library which aims to make machine learning interpretable and understandable by everyone.
 It provides several types of visualization that display explicit labels that everyone can understand. 
 
@@ -222,15 +247,15 @@
     project_info_file='path/to/project_info.yml',
     x_train=Xtrain,
     y_train=ytrain,
     y_test=ytest,
     title_story="House prices report",
     title_description="""This document is a data science report of the kaggle house prices tutorial project.
         It was generated using the Shapash library.""",
-    metrics=[{‘name’: ‘MSE’, ‘path’: ‘sklearn.metrics.mean_squared_error’}]
+    metrics=[{'name': 'MSE', 'path': 'sklearn.metrics.mean_squared_error'}]
 )
 ```
 
 [Report Example](https://shapash.readthedocs.io/en/latest/report.html)
 
 - Step 5: From training to deployment : SmartPredictor Object
   > Shapash provides a SmartPredictor object to deploy the summary of local explanation for the operational needs.
@@ -249,62 +274,65 @@
 
 <details><summary><b>Overview</b> </summary>
 
 - [Launch the webapp with a concrete use case](tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
 - [Jupyter Overviews - The main outputs and methods available with the SmartExplainer object](tutorial/tutorial02-Shapash-overview-in-Jupyter.ipynb)
 - [Shapash in production: From model training to deployment (API or Batch Mode)](tutorial/tutorial03-Shapash-overview-model-in-production.ipynb)
 - [Use groups of features](tutorial/common/tuto-common01-groups_of_features.ipynb)
-- [Deploy local explainability in production with SmartPredictor](tutorial/predictor/tuto-smartpredictor-introduction-to-SmartPredictor.ipynb)
+- [Deploy local explainability in production with SmartPredictor](tutorial/predictor_to_production/tuto-smartpredictor-introduction-to-SmartPredictor.ipynb)
 
 </details>
 
 <details><summary><b>Charts and plots</b> </summary>
 
-- [**Shapash** Features Importance](tutorial/plot/tuto-plot03-features-importance.ipynb)
-- [Contribution plot to understand how one feature affects a prediction](tutorial/plot/tuto-plot02-contribution_plot.ipynb)
-- [Summarize, display and export local contribution using filter and local_plot method](tutorial/plot/tuto-plot01-local_plot-and-to_pandas.ipynb)
-- [Contributions Comparing plot to understand why predictions on several individuals are different](tutorial/plot/tuto-plot04-compare_plot.ipynb)
-- [Visualize interactions between couple of variables](tutorial/plot/tuto-plot05-interactions-plot.ipynb)
+- [**Shapash** Features Importance](tutorial/plots_and_charts/tuto-plot03-features-importance.ipynb)
+- [Contribution plot to understand how one feature affects a prediction](tutorial/plots_and_charts/tuto-plot02-contribution_plot.ipynb)
+- [Summarize, display and export local contribution using filter and local_plot method](tutorial/plots_and_charts/tuto-plot01-local_plot-and-to_pandas.ipynb)
+- [Contributions Comparing plot to understand why predictions on several individuals are different](tutorial/plots_and_charts/tuto-plot04-compare_plot.ipynb)
+- [Visualize interactions between couple of variables](tutorial/plots_and_charts/tuto-plot05-interactions-plot.ipynb)
+- [Display True Values Vs Predicted Values](tutorial/plots_and_charts/tuto-plot06-prediction_plot.ipynb)
 - [Customize colors in Webapp, plots and report](tutorial/common/tuto-common02-colors.ipynb)
 
 </details>
 
 <details><summary><b>Different ways to use Encoders and Dictionaries</b> </summary>
 
-- [Use Category_Encoder & inverse transformation](tutorial/encoder/tuto-encoder01-using-category_encoder.ipynb)
-- [Use ColumnTransformers](tutorial/encoder/tuto-encoder02-using-columntransformer.ipynb)
-- [Use Simple Python Dictionnaries](tutorial/encoder/tuto-encoder03-using-dict.ipynb)
+- [Use Category_Encoder & inverse transformation](tutorial/use_encoders/tuto-encoder01-using-category_encoder.ipynb)
+- [Use ColumnTransformers](tutorial/use_encoders/tuto-encoder02-using-columntransformer.ipynb)
+- [Use Simple Python Dictionnaries](tutorial/use_encoders/tuto-encoder03-using-dict.ipynb)
 
 </details>
 
 <details><summary><b>Displaying data with postprocessing</b> </summary>
 
 [Using postprocessing parameter in compile method](tutorial/postprocess/tuto-postprocess01.ipynb)
 
 </details>
 
 <details><summary><b>Using different backends</b> </summary>
 
-- [Compute Shapley Contributions using **Shap**](tutorial/explainer/tuto-expl01-Shapash-Viz-using-Shap-contributions.ipynb)
-- [Use **Lime** to compute local explanation, Summarize-it with **Shapash**](tutorial/explainer/tuto-expl02-Shapash-Viz-using-Lime-contributions.ipynb)
-- [Use **ACV backend** to compute Active Shapley Values and SDP global importance](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb)
-- [Compile faster Lime and consistency of contributions](tutorial/explainer/tuto-expl04-Shapash-compute-Lime-faster.ipynb)
+- [Compute Shapley Contributions using **Shap**](tutorial/explainer_and_backend/tuto-expl01-Shapash-Viz-using-Shap-contributions.ipynb)
+- [Use **Lime** to compute local explanation, Summarize-it with **Shapash**](tutorial/explainer_and_backend/tuto-expl02-Shapash-Viz-using-Lime-contributions.ipynb)
+- [Use **ACV backend** to compute Active Shapley Values and SDP global importance](tutorial/explainer_and_backend/tuto-expl03-Shapash-acv-backend.ipynb)
+- [Compile faster Lime and consistency of contributions](tutorial/explainer_and_backend/tuto-expl04-Shapash-compute-Lime-faster.ipynb)
+- [Use **FastTreeSHAP** or add contributions from another backend](tutorial/explainer_and_backend/tuto-expl05-Shapash-using-Fasttreeshap.ipynb)
+- [Use Class Shapash Backend](tutorial/explainer_and_backend/tuto-expl06-Shapash-custom-backend.ipynb)
 
 </details>
 
 <details><summary><b>Evaluating the quality of your explainability</b> </summary>
 
 - [Building confidence on explainability methods using **Stability**, **Consistency** and **Compacity** metrics](tutorial/explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb)
 
 </details>
 
 <details><summary><b>Generate a report of your project</b> </summary>
 
-- [Generate a standalone HTML report of your project with generate_report](tutorial/report/tuto-shapash-report01.ipynb)
+- [Generate a standalone HTML report of your project with generate_report](tutorial/generate_report/tuto-shapash-report01.ipynb)
 
 </details>
 
 <details><summary><b>Analysing your model via Shapash WebApp</b> </summary>
 
-- [Add features outside of the model for more exploration options](tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+- [Add features outside of the model for more exploration options](tutorial/generate_webapp/tuto-webapp01-additional-data.ipynb)
 
 </details>
```

#### html2text {}

```diff
@@ -1,44 +1,57 @@
+Metadata-Version: 2.1 Name: shapash Version: 2.3.5 Summary: Shapash is a Python
+library which aims to make machine learning interpretable and understandable by
+everyone. Home-page: https://github.com/MAIF/shapash Author: Yann Golhen,
+Sebastien Bidault, Yann Lagre, Maxime Gendre Author-email: yann.golhen@maif.fr
+License: Apache Software License 2.0 Keywords: shapash Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Operating System :: OS Independent Requires-
+Python: >3.7, <3.11 Description-Content-Type: text/markdown Provides-Extra:
+report Provides-Extra: xgboost Provides-Extra: lightgbm Provides-Extra:
+catboost Provides-Extra: acv Provides-Extra: lime License-File: LICENSE
  [https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/shapash-
                                   resize.png]
           [tests]  [pypi]  [downloads]  [pyversion]  [license]  [doc]
 ## ð What's new ? | Version | New Feature | Description | Tutorial | |:-----
 --------:|:--------------------------------------------------------------------
 -----------------:|:-----------------------------------------------------------
 ---------------------------------------------------------------------------:|:-
 -------:| | 2.3.x | Additional dataset columns
 [New demo](https://shapash-demo.ossbymaif.fr/)
 [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-
 interpretation-40b50157c2fb) | In Webapp: Target and error columns added to
 dataset and possibility to add features outside the model for more filtering
 options | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
 add_column_icon.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
-webapp/tuto-webapp01-additional-data.ipynb) | 2.3.x | Identity card
+generate_webapp/tuto-webapp01-additional-data.ipynb) | 2.3.x | Identity card
 [New demo](https://shapash-demo.ossbymaif.fr/)
 [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-
 interpretation-40b50157c2fb) | In Webapp: New identity card to summarize the
 information of the selected sample | [[https://raw.githubusercontent.com/MAIF/
 shapash/master/docs/_static/identity_card.png]](https://github.com/MAIF/
-shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb) |
-2.2.x | Picking samples
+shapash/blob/master/tutorial/generate_webapp/tuto-webapp01-additional-
+data.ipynb) | 2.2.x | Picking samples
 [Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-
 machine-learning-model.html) | New tab in the webapp for picking samples. The
 graph represents the "True Values Vs Predicted Values" | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png]](https:
-//github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-
+//github.com/MAIF/shapash/blob/master/tutorial/plots_and_charts/tuto-plot06-
 prediction_plot.ipynb) | 2.2.x | Dataset Filter
 | New tab in the webapp to filter data. And several improvements in the webapp:
 subtitles, labels, screen adjustments | [[https://raw.githubusercontent.com/
 MAIF/shapash/master/docs/_static/webapp.png]](https://github.com/MAIF/shapash/
 blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.0.x |
 Refactoring Shapash
 | Refactoring attributes of compile methods and init. Refactoring
 implementation for new backends | [[https://raw.githubusercontent.com/MAIF/
 shapash/master/docs/_static/modular.png]](https://github.com/MAIF/shapash/blob/
-master/tutorial/backend/tuto-backend-01.ipynb) | 1.7.x | Variabilize Colors
+master/tutorial/explainer_and_backend/tuto-expl06-Shapash-custom-backend.ipynb)
+| 1.7.x | Variabilize Colors
 | Giving possibility to have your own colour palette for outputs adapted to
 your design | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
 _static/variabilize-colors.png]](https://github.com/MAIF/shapash/blob/master/
 tutorial/common/tuto-common02-colors.ipynb) | 1.6.x | Explainability Quality
 Metrics
 [Article](https://towardsdatascience.com/building-confidence-on-explainability-
 methods-66b9ee575514) | To help increase confidence in explainability methods,
@@ -47,36 +60,36 @@
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-
 metrics.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
 explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb)
 | 1.5.x | ACV Backend
 | A new way of estimating Shapley values using ACV. [More info about ACV here]
 (https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-
 cfea30509254). | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
-_static/wheel.png]](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb) |
-| 1.4.x | Groups of features
+_static/wheel.png]](tutorial/explainer_and_backend/tuto-expl03-Shapash-acv-
+backend.ipynb) | | 1.4.x | Groups of features
 [Demo](https://shapash-demo2.ossbymaif.fr/) | You can now regroup features that
 share common properties together.
 This option can be useful if your model has a lot of features. | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
 groups_features.gif]](https://github.com/MAIF/shapash/blob/master/tutorial/
 common/tuto-common01-groups_of_features.ipynb) | | 1.3.x | Shapash Report
 [Demo](https://shapash.readthedocs.io/en/latest/report.html) | A standalone
 HTML report that constitutes a basis of an audit document. | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png]]
-(https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-
-report01.ipynb) | ## ð Overview **Shapash** is a Python library which aims
-to make machine learning interpretable and understandable by everyone. It
-provides several types of visualization that display explicit labels that
-everyone can understand. Data Scientists can understand their models easily and
-share their results. End users can understand the decision proposed by a model
-using a summary of the most influential criteria. Shapash also contributes to
-data science auditing by displaying usefull information about any model and
-data in a unique report. - Readthedocs: [![documentation badge](https://
-readthedocs.org/projects/shapash/badge/?version=latest)](https://
-shapash.readthedocs.io/en/latest/) - [Presentation video for french speakers]
+(https://github.com/MAIF/shapash/blob/master/tutorial/generate_report/tuto-
+shapash-report01.ipynb) | ## ð Overview **Shapash** is a Python library
+which aims to make machine learning interpretable and understandable by
+everyone. It provides several types of visualization that display explicit
+labels that everyone can understand. Data Scientists can understand their
+models easily and share their results. End users can understand the decision
+proposed by a model using a summary of the most influential criteria. Shapash
+also contributes to data science auditing by displaying usefull information
+about any model and data in a unique report. - Readthedocs: [![documentation
+badge](https://readthedocs.org/projects/shapash/badge/?version=latest)](https:/
+/shapash.readthedocs.io/en/latest/) - [Presentation video for french speakers]
 (https://www.youtube.com/watch?v=r1R_A9B9apk) - Medium: - [Understand your
 model with Shapash - Towards AI](https://pub.towardsai.net/shapash-making-ml-
 models-understandable-by-everyone-8f96ad469eb3) - [Model auditability - Towards
 DS](https://towardsdatascience.com/shapash-1-3-2-announcing-new-features-for-
 more-auditable-ai-64a6db71c919) - [Group of features - Towards AI](https://
 pub.towardsai.net/machine-learning-6011d5d9a444) - [Building confidence on
 explainability - Towards DS](https://towardsdatascience.com/building-
@@ -174,58 +187,66 @@
 Generate the Shapash Report > This step allows to generate a standalone html
 report of your project using the different splits of your dataset and also the
 metrics you used: ``` xpl.generate_report( output_file='path/to/output/
 report.html', project_info_file='path/to/project_info.yml', x_train=Xtrain,
 y_train=ytrain, y_test=ytest, title_story="House prices report",
 title_description="""This document is a data science report of the kaggle house
 prices tutorial project. It was generated using the Shapash library.""",
-metrics=[{ânameâ: âMSEâ, âpathâ:
-âsklearn.metrics.mean_squared_errorâ}] ) ``` [Report Example](https://
-shapash.readthedocs.io/en/latest/report.html) - Step 5: From training to
-deployment : SmartPredictor Object > Shapash provides a SmartPredictor object
-to deploy the summary of local explanation for the operational needs. It is an
-object dedicated to deployment, lighter than SmartExplainer with additional
-consistency checks. SmartPredictor can be used with an API or in batch mode. It
-provides predictions, detailed or summarized local explainability using
-appropriate wording. ``` predictor = xpl.to_smartpredictor() ``` See the
-tutorial part to know how to use the SmartPredictor object ## ð Tutorials
-This github repository offers many tutorials to allow you to easily get started
-with Shapash. Overview  - [Launch the webapp with a concrete use case]
-(tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb) - [Jupyter Overviews
-- The main outputs and methods available with the SmartExplainer object]
-(tutorial/tutorial02-Shapash-overview-in-Jupyter.ipynb) - [Shapash in
-production: From model training to deployment (API or Batch Mode)](tutorial/
-tutorial03-Shapash-overview-model-in-production.ipynb) - [Use groups of
-features](tutorial/common/tuto-common01-groups_of_features.ipynb) - [Deploy
-local explainability in production with SmartPredictor](tutorial/predictor/
-tuto-smartpredictor-introduction-to-SmartPredictor.ipynb)  Charts and plots  -
-[**Shapash** Features Importance](tutorial/plot/tuto-plot03-features-
+metrics=[{'name': 'MSE', 'path': 'sklearn.metrics.mean_squared_error'}] ) ```
+[Report Example](https://shapash.readthedocs.io/en/latest/report.html) - Step
+5: From training to deployment : SmartPredictor Object > Shapash provides a
+SmartPredictor object to deploy the summary of local explanation for the
+operational needs. It is an object dedicated to deployment, lighter than
+SmartExplainer with additional consistency checks. SmartPredictor can be used
+with an API or in batch mode. It provides predictions, detailed or summarized
+local explainability using appropriate wording. ``` predictor =
+xpl.to_smartpredictor() ``` See the tutorial part to know how to use the
+SmartPredictor object ## ð Tutorials This github repository offers many
+tutorials to allow you to easily get started with Shapash. Overview  - [Launch
+the webapp with a concrete use case](tutorial/tutorial01-Shapash-Overview-
+Launch-WebApp.ipynb) - [Jupyter Overviews - The main outputs and methods
+available with the SmartExplainer object](tutorial/tutorial02-Shapash-overview-
+in-Jupyter.ipynb) - [Shapash in production: From model training to deployment
+(API or Batch Mode)](tutorial/tutorial03-Shapash-overview-model-in-
+production.ipynb) - [Use groups of features](tutorial/common/tuto-common01-
+groups_of_features.ipynb) - [Deploy local explainability in production with
+SmartPredictor](tutorial/predictor_to_production/tuto-smartpredictor-
+introduction-to-SmartPredictor.ipynb)  Charts and plots  - [**Shapash**
+Features Importance](tutorial/plots_and_charts/tuto-plot03-features-
 importance.ipynb) - [Contribution plot to understand how one feature affects a
-prediction](tutorial/plot/tuto-plot02-contribution_plot.ipynb) - [Summarize,
-display and export local contribution using filter and local_plot method]
-(tutorial/plot/tuto-plot01-local_plot-and-to_pandas.ipynb) - [Contributions
-Comparing plot to understand why predictions on several individuals are
-different](tutorial/plot/tuto-plot04-compare_plot.ipynb) - [Visualize
-interactions between couple of variables](tutorial/plot/tuto-plot05-
-interactions-plot.ipynb) - [Customize colors in Webapp, plots and report]
+prediction](tutorial/plots_and_charts/tuto-plot02-contribution_plot.ipynb) -
+[Summarize, display and export local contribution using filter and local_plot
+method](tutorial/plots_and_charts/tuto-plot01-local_plot-and-to_pandas.ipynb) -
+[Contributions Comparing plot to understand why predictions on several
+individuals are different](tutorial/plots_and_charts/tuto-plot04-
+compare_plot.ipynb) - [Visualize interactions between couple of variables]
+(tutorial/plots_and_charts/tuto-plot05-interactions-plot.ipynb) - [Display True
+Values Vs Predicted Values](tutorial/plots_and_charts/tuto-plot06-
+prediction_plot.ipynb) - [Customize colors in Webapp, plots and report]
 (tutorial/common/tuto-common02-colors.ipynb)  Different ways to use Encoders
 and Dictionaries  - [Use Category_Encoder & inverse transformation](tutorial/
-encoder/tuto-encoder01-using-category_encoder.ipynb) - [Use ColumnTransformers]
-(tutorial/encoder/tuto-encoder02-using-columntransformer.ipynb) - [Use Simple
-Python Dictionnaries](tutorial/encoder/tuto-encoder03-using-dict.ipynb)
-Displaying data with postprocessing  [Using postprocessing parameter in compile
-method](tutorial/postprocess/tuto-postprocess01.ipynb)  Using different
-backends  - [Compute Shapley Contributions using **Shap**](tutorial/explainer/
-tuto-expl01-Shapash-Viz-using-Shap-contributions.ipynb) - [Use **Lime** to
-compute local explanation, Summarize-it with **Shapash**](tutorial/explainer/
-tuto-expl02-Shapash-Viz-using-Lime-contributions.ipynb) - [Use **ACV backend**
-to compute Active Shapley Values and SDP global importance](tutorial/explainer/
-tuto-expl03-Shapash-acv-backend.ipynb) - [Compile faster Lime and consistency
-of contributions](tutorial/explainer/tuto-expl04-Shapash-compute-Lime-
-faster.ipynb)  Evaluating the quality of your explainability  - [Building
-confidence on explainability methods using **Stability**, **Consistency** and
-**Compacity** metrics](tutorial/explainability_quality/tuto-quality01-Builing-
-confidence-explainability.ipynb)  Generate a report of your project  -
-[Generate a standalone HTML report of your project with generate_report]
-(tutorial/report/tuto-shapash-report01.ipynb)  Analysing your model via Shapash
-WebApp  - [Add features outside of the model for more exploration options]
-(tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+use_encoders/tuto-encoder01-using-category_encoder.ipynb) - [Use
+ColumnTransformers](tutorial/use_encoders/tuto-encoder02-using-
+columntransformer.ipynb) - [Use Simple Python Dictionnaries](tutorial/
+use_encoders/tuto-encoder03-using-dict.ipynb)  Displaying data with
+postprocessing  [Using postprocessing parameter in compile method](tutorial/
+postprocess/tuto-postprocess01.ipynb)  Using different backends  - [Compute
+Shapley Contributions using **Shap**](tutorial/explainer_and_backend/tuto-
+expl01-Shapash-Viz-using-Shap-contributions.ipynb) - [Use **Lime** to compute
+local explanation, Summarize-it with **Shapash**](tutorial/
+explainer_and_backend/tuto-expl02-Shapash-Viz-using-Lime-contributions.ipynb) -
+[Use **ACV backend** to compute Active Shapley Values and SDP global
+importance](tutorial/explainer_and_backend/tuto-expl03-Shapash-acv-
+backend.ipynb) - [Compile faster Lime and consistency of contributions]
+(tutorial/explainer_and_backend/tuto-expl04-Shapash-compute-Lime-faster.ipynb)
+- [Use **FastTreeSHAP** or add contributions from another backend](tutorial/
+explainer_and_backend/tuto-expl05-Shapash-using-Fasttreeshap.ipynb) - [Use
+Class Shapash Backend](tutorial/explainer_and_backend/tuto-expl06-Shapash-
+custom-backend.ipynb)  Evaluating the quality of your explainability  -
+[Building confidence on explainability methods using **Stability**,
+**Consistency** and **Compacity** metrics](tutorial/explainability_quality/
+tuto-quality01-Builing-confidence-explainability.ipynb)  Generate a report of
+your project  - [Generate a standalone HTML report of your project with
+generate_report](tutorial/generate_report/tuto-shapash-report01.ipynb)
+Analysing your model via Shapash WebApp  - [Add features outside of the model
+for more exploration options](tutorial/generate_webapp/tuto-webapp01-
+additional-data.ipynb)
```

### Comparing `shapash-2.3.4/setup.py` & `shapash-2.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 with open(os.path.join(here, 'shapash', "__version__.py")) as f:
     exec(f.read(), version_d)
 
 
 requirements = [
     'plotly>=5.0.0',
     'matplotlib>=3.2.0',
-    'numpy>1.18.0,<1.24.0',
-    'pandas>1.0.2,<2.0.0',
+    'numpy>1.18.0',
+    'pandas>1.0.2',
     'shap>=0.38.1',
     'Flask<2.3.0',
     'dash>=2.3.1',
     'dash-bootstrap-components>=1.1.0',
     'dash-core-components>=2.0.0',
     'dash-daq>=0.5.0',
     'dash-html-components>=2.0.0',
```

### Comparing `shapash-2.3.4/shapash/backend/__init__.py` & `shapash-2.3.5/shapash/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/backend/acv_backend.py` & `shapash-2.3.5/shapash/backend/acv_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/backend/base_backend.py` & `shapash-2.3.5/shapash/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/backend/lime_backend.py` & `shapash-2.3.5/shapash/backend/lime_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/backend/shap_backend.py` & `shapash-2.3.5/shapash/backend/shap_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/data/data_loader.py` & `shapash-2.3.5/shapash/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/decomposition/contributions.py` & `shapash-2.3.5/shapash/decomposition/contributions.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/explainer/consistency.py` & `shapash-2.3.5/shapash/explainer/consistency.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         Plot the main graph displaying distances between methods
 
         Parameters
         ----------
         mean_distances : DataFrame
             DataFrame storing all pairwise distances between methods
         """
-        font = {"family": "Arial", "color": '#{:02x}{:02x}{:02x}'.format(50, 50, 50)}
+        font = {"color": '#{:02x}{:02x}{:02x}'.format(50, 50, 50)}
 
         fig, ax = plt.subplots(ncols=1, figsize=(10, 6))
 
         ax.text(x=0.5, y=1.04, s="Consistency of explanations:", fontsize=24, ha="center", transform=fig.transFigure, **font)
         ax.text(x=0.5, y=0.98, s="How similar are explanations from different methods?",
                 fontsize=18, ha="center", transform=fig.transFigure, **font)
```

### Comparing `shapash-2.3.4/shapash/explainer/multi_decorator.py` & `shapash-2.3.5/shapash/explainer/multi_decorator.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/explainer/smart_explainer.py` & `shapash-2.3.5/shapash/explainer/smart_explainer.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/explainer/smart_plotter.py` & `shapash-2.3.5/shapash/explainer/smart_plotter.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/explainer/smart_predictor.py` & `shapash-2.3.5/shapash/explainer/smart_predictor.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/explainer/smart_state.py` & `shapash-2.3.5/shapash/explainer/smart_state.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/manipulation/filters.py` & `shapash-2.3.5/shapash/manipulation/filters.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/manipulation/mask.py` & `shapash-2.3.5/shapash/manipulation/mask.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/manipulation/select_lines.py` & `shapash-2.3.5/shapash/manipulation/select_lines.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/manipulation/summarize.py` & `shapash-2.3.5/shapash/manipulation/summarize.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/report/__init__.py` & `shapash-2.3.5/shapash/report/__init__.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/report/base_report.ipynb` & `shapash-2.3.5/shapash/report/base_report.ipynb`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/report/common.py` & `shapash-2.3.5/shapash/report/common.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/report/data_analysis.py` & `shapash-2.3.5/shapash/report/data_analysis.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/report/generation.py` & `shapash-2.3.5/shapash/report/generation.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/report/html/dropdown.html` & `shapash-2.3.5/shapash/report/html/dropdown.html`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/report/html/explainability.html` & `shapash-2.3.5/shapash/report/html/explainability.html`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/report/html/univariate.html` & `shapash-2.3.5/shapash/report/html/univariate.html`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/report/plots.py` & `shapash-2.3.5/shapash/report/plots.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/report/project_report.py` & `shapash-2.3.5/shapash/report/project_report.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/report/template/custom/index.html.j2` & `shapash-2.3.5/shapash/report/template/custom/index.html.j2`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/report/visualisation.py` & `shapash-2.3.5/shapash/report/visualisation.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/style/colors.json` & `shapash-2.3.5/shapash/style/colors.json`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/style/style_utils.py` & `shapash-2.3.5/shapash/style/style_utils.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/utils/category_encoder_backend.py` & `shapash-2.3.5/shapash/utils/category_encoder_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/utils/check.py` & `shapash-2.3.5/shapash/utils/check.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/utils/columntransformer_backend.py` & `shapash-2.3.5/shapash/utils/columntransformer_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/utils/explanation_metrics.py` & `shapash-2.3.5/shapash/utils/explanation_metrics.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/utils/io.py` & `shapash-2.3.5/shapash/utils/io.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/utils/load_smartpredictor.py` & `shapash-2.3.5/shapash/utils/load_smartpredictor.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/utils/model.py` & `shapash-2.3.5/shapash/utils/model.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/utils/model_synoptic.py` & `shapash-2.3.5/shapash/utils/model_synoptic.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/utils/threading.py` & `shapash-2.3.5/shapash/utils/threading.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/utils/transform.py` & `shapash-2.3.5/shapash/utils/transform.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/utils/utils.py` & `shapash-2.3.5/shapash/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/webapp/assets/favicon.ico` & `shapash-2.3.5/shapash/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/webapp/assets/jquery.js` & `shapash-2.3.5/shapash/webapp/assets/jquery.js`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/webapp/assets/material-icons.css` & `shapash-2.3.5/shapash/webapp/assets/material-icons.css`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/webapp/assets/reload.png` & `shapash-2.3.5/shapash/webapp/assets/reload.png`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/webapp/assets/settings.png` & `shapash-2.3.5/shapash/webapp/assets/settings.png`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/webapp/assets/shapash-fond-fonce.png` & `shapash-2.3.5/shapash/webapp/assets/shapash-fond-fonce.png`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/webapp/assets/style.css` & `shapash-2.3.5/shapash/webapp/assets/style.css`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/webapp/smart_app.py` & `shapash-2.3.5/shapash/webapp/smart_app.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/webapp/utils/MyGraph.py` & `shapash-2.3.5/shapash/webapp/utils/MyGraph.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/webapp/utils/explanations.py` & `shapash-2.3.5/shapash/webapp/utils/explanations.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/webapp/utils/utils.py` & `shapash-2.3.5/shapash/webapp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/webapp/webapp_launch.py` & `shapash-2.3.5/shapash/webapp/webapp_launch.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash/webapp/webapp_launch_DVF.py` & `shapash-2.3.5/shapash/webapp/webapp_launch_DVF.py`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash.egg-info/PKG-INFO` & `shapash-2.3.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: shapash
-Version: 2.3.4
-Summary: Shapash is a Python library which aims to make machine learning interpretable and understandable by everyone.
-Home-page: https://github.com/MAIF/shapash
-Author: Yann Golhen, Sebastien Bidault, Yann Lagre, Maxime Gendre
-Author-email: yann.golhen@maif.fr
-License: Apache Software License 2.0
-Keywords: shapash
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >3.7, <3.11
-Description-Content-Type: text/markdown
-Provides-Extra: report
-Provides-Extra: xgboost
-Provides-Extra: lightgbm
-Provides-Extra: catboost
-Provides-Extra: acv
-Provides-Extra: lime
-License-File: LICENSE
-
 <p align="center">
 <img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/shapash-resize.png" width="300" title="shapash-logo">
 </p>
 
 
 <p align="center">
   <!-- Tests -->
@@ -56,24 +31,24 @@
 </p>
 
 ## 🎉 What's new ?
 
 
 | Version       | New Feature                                                                           | Description                                                                                                                            | Tutorial |
 |:-------------:|:-------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
-| 2.3.x         |  Additional dataset columns <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                | In Webapp: Target and error columns added to dataset and possibility to add features outside the model for more filtering options            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/add_column_icon.png" width="50" title="add_column">](https://github.com/MAIF/shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb)
-| 2.3.x         |  Identity card <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                  | In Webapp: New identity card to summarize the information of the selected sample                  |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/identity_card.png" width="50" title="identity">](https://github.com/MAIF/shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb)
-| 2.2.x         |  Picking samples <br> [Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-machine-learning-model.html)                                                                | New tab in the webapp for picking samples. The graph represents the "True Values Vs Predicted Values"            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png" width="50" title="picking">](https://github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-prediction_plot.ipynb)
+| 2.3.x         |  Additional dataset columns <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                | In Webapp: Target and error columns added to dataset and possibility to add features outside the model for more filtering options            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/add_column_icon.png" width="50" title="add_column">](https://github.com/MAIF/shapash/blob/master/tutorial/generate_webapp/tuto-webapp01-additional-data.ipynb)
+| 2.3.x         |  Identity card <br> [New demo](https://shapash-demo.ossbymaif.fr/) <br> [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-interpretation-40b50157c2fb)                                                                  | In Webapp: New identity card to summarize the information of the selected sample                  |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/identity_card.png" width="50" title="identity">](https://github.com/MAIF/shapash/blob/master/tutorial/generate_webapp/tuto-webapp01-additional-data.ipynb)
+| 2.2.x         |  Picking samples <br> [Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-machine-learning-model.html)                                                                | New tab in the webapp for picking samples. The graph represents the "True Values Vs Predicted Values"            |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png" width="50" title="picking">](https://github.com/MAIF/shapash/blob/master/tutorial/plots_and_charts/tuto-plot06-prediction_plot.ipynb)
 | 2.2.x         |  Dataset Filter <br>                                                              | New tab in the webapp to filter data. And several improvements in the webapp: subtitles, labels, screen adjustments                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/webapp.png" width="50" title="webapp">](https://github.com/MAIF/shapash/blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
-| 2.0.x         |  Refactoring Shapash <br>                                                                   | Refactoring attributes of compile methods and init. Refactoring implementation for new backends                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/modular.png" width="50" title="modular">](https://github.com/MAIF/shapash/blob/master/tutorial/backend/tuto-backend-01.ipynb)
+| 2.0.x         |  Refactoring Shapash <br>                                                                   | Refactoring attributes of compile methods and init. Refactoring implementation for new backends                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/modular.png" width="50" title="modular">](https://github.com/MAIF/shapash/blob/master/tutorial/explainer_and_backend/tuto-expl06-Shapash-custom-backend.ipynb)
 | 1.7.x         |  Variabilize Colors <br>                                                                   | Giving possibility to have your own colour palette for outputs adapted to your design                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/variabilize-colors.png" width="50" title="variabilize-colors">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common02-colors.ipynb)
 | 1.6.x         |  Explainability Quality Metrics <br> [Article](https://towardsdatascience.com/building-confidence-on-explainability-methods-66b9ee575514)                                                                   | To help increase confidence in explainability methods, you can evaluate the relevance of your explainability using 3 metrics: **Stability**, **Consistency** and **Compacity**                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-metrics.png" width="50" title="quality-metrics">](https://github.com/MAIF/shapash/blob/master/tutorial/explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb) 
-| 1.5.x         |  ACV Backend <br>                                                                     | A new way of estimating Shapley values using ACV. [More info about ACV here](https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-cfea30509254).                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/wheel.png" width="50" title="wheel-acv-backend">](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb)    |
+| 1.5.x         |  ACV Backend <br>                                                                     | A new way of estimating Shapley values using ACV. [More info about ACV here](https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-cfea30509254).                   |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/wheel.png" width="50" title="wheel-acv-backend">](tutorial/explainer_and_backend/tuto-expl03-Shapash-acv-backend.ipynb)    |
 | 1.4.x         |  Groups of features <br> [Demo](https://shapash-demo2.ossbymaif.fr/)                  | You can now regroup features that share common properties together. <br>This option can be useful if your model has a lot of features. |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/groups_features.gif" width="120" title="groups-features">](https://github.com/MAIF/shapash/blob/master/tutorial/common/tuto-common01-groups_of_features.ipynb)    | 
-| 1.3.x         |  Shapash Report <br> [Demo](https://shapash.readthedocs.io/en/latest/report.html)     | A standalone HTML report that constitutes a basis of an audit document.                                                                |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png" width="50" title="shapash-report">](https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-report01.ipynb)    | 
+| 1.3.x         |  Shapash Report <br> [Demo](https://shapash.readthedocs.io/en/latest/report.html)     | A standalone HTML report that constitutes a basis of an audit document.                                                                |  [<img src="https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png" width="50" title="shapash-report">](https://github.com/MAIF/shapash/blob/master/tutorial/generate_report/tuto-shapash-report01.ipynb)    | 
 
 
 ## 🔍 Overview
 
 **Shapash** is a Python library which aims to make machine learning interpretable and understandable by everyone.
 It provides several types of visualization that display explicit labels that everyone can understand. 
 
@@ -247,15 +222,15 @@
     project_info_file='path/to/project_info.yml',
     x_train=Xtrain,
     y_train=ytrain,
     y_test=ytest,
     title_story="House prices report",
     title_description="""This document is a data science report of the kaggle house prices tutorial project.
         It was generated using the Shapash library.""",
-    metrics=[{‘name’: ‘MSE’, ‘path’: ‘sklearn.metrics.mean_squared_error’}]
+    metrics=[{'name': 'MSE', 'path': 'sklearn.metrics.mean_squared_error'}]
 )
 ```
 
 [Report Example](https://shapash.readthedocs.io/en/latest/report.html)
 
 - Step 5: From training to deployment : SmartPredictor Object
   > Shapash provides a SmartPredictor object to deploy the summary of local explanation for the operational needs.
@@ -274,62 +249,65 @@
 
 <details><summary><b>Overview</b> </summary>
 
 - [Launch the webapp with a concrete use case](tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb)
 - [Jupyter Overviews - The main outputs and methods available with the SmartExplainer object](tutorial/tutorial02-Shapash-overview-in-Jupyter.ipynb)
 - [Shapash in production: From model training to deployment (API or Batch Mode)](tutorial/tutorial03-Shapash-overview-model-in-production.ipynb)
 - [Use groups of features](tutorial/common/tuto-common01-groups_of_features.ipynb)
-- [Deploy local explainability in production with SmartPredictor](tutorial/predictor/tuto-smartpredictor-introduction-to-SmartPredictor.ipynb)
+- [Deploy local explainability in production with SmartPredictor](tutorial/predictor_to_production/tuto-smartpredictor-introduction-to-SmartPredictor.ipynb)
 
 </details>
 
 <details><summary><b>Charts and plots</b> </summary>
 
-- [**Shapash** Features Importance](tutorial/plot/tuto-plot03-features-importance.ipynb)
-- [Contribution plot to understand how one feature affects a prediction](tutorial/plot/tuto-plot02-contribution_plot.ipynb)
-- [Summarize, display and export local contribution using filter and local_plot method](tutorial/plot/tuto-plot01-local_plot-and-to_pandas.ipynb)
-- [Contributions Comparing plot to understand why predictions on several individuals are different](tutorial/plot/tuto-plot04-compare_plot.ipynb)
-- [Visualize interactions between couple of variables](tutorial/plot/tuto-plot05-interactions-plot.ipynb)
+- [**Shapash** Features Importance](tutorial/plots_and_charts/tuto-plot03-features-importance.ipynb)
+- [Contribution plot to understand how one feature affects a prediction](tutorial/plots_and_charts/tuto-plot02-contribution_plot.ipynb)
+- [Summarize, display and export local contribution using filter and local_plot method](tutorial/plots_and_charts/tuto-plot01-local_plot-and-to_pandas.ipynb)
+- [Contributions Comparing plot to understand why predictions on several individuals are different](tutorial/plots_and_charts/tuto-plot04-compare_plot.ipynb)
+- [Visualize interactions between couple of variables](tutorial/plots_and_charts/tuto-plot05-interactions-plot.ipynb)
+- [Display True Values Vs Predicted Values](tutorial/plots_and_charts/tuto-plot06-prediction_plot.ipynb)
 - [Customize colors in Webapp, plots and report](tutorial/common/tuto-common02-colors.ipynb)
 
 </details>
 
 <details><summary><b>Different ways to use Encoders and Dictionaries</b> </summary>
 
-- [Use Category_Encoder & inverse transformation](tutorial/encoder/tuto-encoder01-using-category_encoder.ipynb)
-- [Use ColumnTransformers](tutorial/encoder/tuto-encoder02-using-columntransformer.ipynb)
-- [Use Simple Python Dictionnaries](tutorial/encoder/tuto-encoder03-using-dict.ipynb)
+- [Use Category_Encoder & inverse transformation](tutorial/use_encoders/tuto-encoder01-using-category_encoder.ipynb)
+- [Use ColumnTransformers](tutorial/use_encoders/tuto-encoder02-using-columntransformer.ipynb)
+- [Use Simple Python Dictionnaries](tutorial/use_encoders/tuto-encoder03-using-dict.ipynb)
 
 </details>
 
 <details><summary><b>Displaying data with postprocessing</b> </summary>
 
 [Using postprocessing parameter in compile method](tutorial/postprocess/tuto-postprocess01.ipynb)
 
 </details>
 
 <details><summary><b>Using different backends</b> </summary>
 
-- [Compute Shapley Contributions using **Shap**](tutorial/explainer/tuto-expl01-Shapash-Viz-using-Shap-contributions.ipynb)
-- [Use **Lime** to compute local explanation, Summarize-it with **Shapash**](tutorial/explainer/tuto-expl02-Shapash-Viz-using-Lime-contributions.ipynb)
-- [Use **ACV backend** to compute Active Shapley Values and SDP global importance](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb)
-- [Compile faster Lime and consistency of contributions](tutorial/explainer/tuto-expl04-Shapash-compute-Lime-faster.ipynb)
+- [Compute Shapley Contributions using **Shap**](tutorial/explainer_and_backend/tuto-expl01-Shapash-Viz-using-Shap-contributions.ipynb)
+- [Use **Lime** to compute local explanation, Summarize-it with **Shapash**](tutorial/explainer_and_backend/tuto-expl02-Shapash-Viz-using-Lime-contributions.ipynb)
+- [Use **ACV backend** to compute Active Shapley Values and SDP global importance](tutorial/explainer_and_backend/tuto-expl03-Shapash-acv-backend.ipynb)
+- [Compile faster Lime and consistency of contributions](tutorial/explainer_and_backend/tuto-expl04-Shapash-compute-Lime-faster.ipynb)
+- [Use **FastTreeSHAP** or add contributions from another backend](tutorial/explainer_and_backend/tuto-expl05-Shapash-using-Fasttreeshap.ipynb)
+- [Use Class Shapash Backend](tutorial/explainer_and_backend/tuto-expl06-Shapash-custom-backend.ipynb)
 
 </details>
 
 <details><summary><b>Evaluating the quality of your explainability</b> </summary>
 
 - [Building confidence on explainability methods using **Stability**, **Consistency** and **Compacity** metrics](tutorial/explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb)
 
 </details>
 
 <details><summary><b>Generate a report of your project</b> </summary>
 
-- [Generate a standalone HTML report of your project with generate_report](tutorial/report/tuto-shapash-report01.ipynb)
+- [Generate a standalone HTML report of your project with generate_report](tutorial/generate_report/tuto-shapash-report01.ipynb)
 
 </details>
 
 <details><summary><b>Analysing your model via Shapash WebApp</b> </summary>
 
-- [Add features outside of the model for more exploration options](tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+- [Add features outside of the model for more exploration options](tutorial/generate_webapp/tuto-webapp01-additional-data.ipynb)
 
 </details>
```

#### html2text {}

```diff
@@ -1,56 +1,45 @@
-Metadata-Version: 2.1 Name: shapash Version: 2.3.4 Summary: Shapash is a Python
-library which aims to make machine learning interpretable and understandable by
-everyone. Home-page: https://github.com/MAIF/shapash Author: Yann Golhen,
-Sebastien Bidault, Yann Lagre, Maxime Gendre Author-email: yann.golhen@maif.fr
-License: Apache Software License 2.0 Keywords: shapash Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Operating System :: OS Independent Requires-
-Python: >3.7, <3.11 Description-Content-Type: text/markdown Provides-Extra:
-report Provides-Extra: xgboost Provides-Extra: lightgbm Provides-Extra:
-catboost Provides-Extra: acv Provides-Extra: lime License-File: LICENSE
  [https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/shapash-
                                   resize.png]
           [tests]  [pypi]  [downloads]  [pyversion]  [license]  [doc]
 ## ð What's new ? | Version | New Feature | Description | Tutorial | |:-----
 --------:|:--------------------------------------------------------------------
 -----------------:|:-----------------------------------------------------------
 ---------------------------------------------------------------------------:|:-
 -------:| | 2.3.x | Additional dataset columns
 [New demo](https://shapash-demo.ossbymaif.fr/)
 [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-
 interpretation-40b50157c2fb) | In Webapp: Target and error columns added to
 dataset and possibility to add features outside the model for more filtering
 options | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
 add_column_icon.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
-webapp/tuto-webapp01-additional-data.ipynb) | 2.3.x | Identity card
+generate_webapp/tuto-webapp01-additional-data.ipynb) | 2.3.x | Identity card
 [New demo](https://shapash-demo.ossbymaif.fr/)
 [Article](https://pub.towardsai.net/shapash-2-3-0-comprehensive-model-
 interpretation-40b50157c2fb) | In Webapp: New identity card to summarize the
 information of the selected sample | [[https://raw.githubusercontent.com/MAIF/
 shapash/master/docs/_static/identity_card.png]](https://github.com/MAIF/
-shapash/blob/master/tutorial/webapp/tuto-webapp01-additional-data.ipynb) |
-2.2.x | Picking samples
+shapash/blob/master/tutorial/generate_webapp/tuto-webapp01-additional-
+data.ipynb) | 2.2.x | Picking samples
 [Article](https://www.kdnuggets.com/2022/11/picking-examples-understand-
 machine-learning-model.html) | New tab in the webapp for picking samples. The
 graph represents the "True Values Vs Predicted Values" | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/picking.png]](https:
-//github.com/MAIF/shapash/blob/master/tutorial/plot/tuto-plot06-
+//github.com/MAIF/shapash/blob/master/tutorial/plots_and_charts/tuto-plot06-
 prediction_plot.ipynb) | 2.2.x | Dataset Filter
 | New tab in the webapp to filter data. And several improvements in the webapp:
 subtitles, labels, screen adjustments | [[https://raw.githubusercontent.com/
 MAIF/shapash/master/docs/_static/webapp.png]](https://github.com/MAIF/shapash/
 blob/master/tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb) | 2.0.x |
 Refactoring Shapash
 | Refactoring attributes of compile methods and init. Refactoring
 implementation for new backends | [[https://raw.githubusercontent.com/MAIF/
 shapash/master/docs/_static/modular.png]](https://github.com/MAIF/shapash/blob/
-master/tutorial/backend/tuto-backend-01.ipynb) | 1.7.x | Variabilize Colors
+master/tutorial/explainer_and_backend/tuto-expl06-Shapash-custom-backend.ipynb)
+| 1.7.x | Variabilize Colors
 | Giving possibility to have your own colour palette for outputs adapted to
 your design | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
 _static/variabilize-colors.png]](https://github.com/MAIF/shapash/blob/master/
 tutorial/common/tuto-common02-colors.ipynb) | 1.6.x | Explainability Quality
 Metrics
 [Article](https://towardsdatascience.com/building-confidence-on-explainability-
 methods-66b9ee575514) | To help increase confidence in explainability methods,
@@ -59,36 +48,36 @@
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/quality-
 metrics.png]](https://github.com/MAIF/shapash/blob/master/tutorial/
 explainability_quality/tuto-quality01-Builing-confidence-explainability.ipynb)
 | 1.5.x | ACV Backend
 | A new way of estimating Shapley values using ACV. [More info about ACV here]
 (https://towardsdatascience.com/the-right-way-to-compute-your-shapley-values-
 cfea30509254). | [[https://raw.githubusercontent.com/MAIF/shapash/master/docs/
-_static/wheel.png]](tutorial/explainer/tuto-expl03-Shapash-acv-backend.ipynb) |
-| 1.4.x | Groups of features
+_static/wheel.png]](tutorial/explainer_and_backend/tuto-expl03-Shapash-acv-
+backend.ipynb) | | 1.4.x | Groups of features
 [Demo](https://shapash-demo2.ossbymaif.fr/) | You can now regroup features that
 share common properties together.
 This option can be useful if your model has a lot of features. | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/
 groups_features.gif]](https://github.com/MAIF/shapash/blob/master/tutorial/
 common/tuto-common01-groups_of_features.ipynb) | | 1.3.x | Shapash Report
 [Demo](https://shapash.readthedocs.io/en/latest/report.html) | A standalone
 HTML report that constitutes a basis of an audit document. | [[https://
 raw.githubusercontent.com/MAIF/shapash/master/docs/_static/report-icon.png]]
-(https://github.com/MAIF/shapash/blob/master/tutorial/report/tuto-shapash-
-report01.ipynb) | ## ð Overview **Shapash** is a Python library which aims
-to make machine learning interpretable and understandable by everyone. It
-provides several types of visualization that display explicit labels that
-everyone can understand. Data Scientists can understand their models easily and
-share their results. End users can understand the decision proposed by a model
-using a summary of the most influential criteria. Shapash also contributes to
-data science auditing by displaying usefull information about any model and
-data in a unique report. - Readthedocs: [![documentation badge](https://
-readthedocs.org/projects/shapash/badge/?version=latest)](https://
-shapash.readthedocs.io/en/latest/) - [Presentation video for french speakers]
+(https://github.com/MAIF/shapash/blob/master/tutorial/generate_report/tuto-
+shapash-report01.ipynb) | ## ð Overview **Shapash** is a Python library
+which aims to make machine learning interpretable and understandable by
+everyone. It provides several types of visualization that display explicit
+labels that everyone can understand. Data Scientists can understand their
+models easily and share their results. End users can understand the decision
+proposed by a model using a summary of the most influential criteria. Shapash
+also contributes to data science auditing by displaying usefull information
+about any model and data in a unique report. - Readthedocs: [![documentation
+badge](https://readthedocs.org/projects/shapash/badge/?version=latest)](https:/
+/shapash.readthedocs.io/en/latest/) - [Presentation video for french speakers]
 (https://www.youtube.com/watch?v=r1R_A9B9apk) - Medium: - [Understand your
 model with Shapash - Towards AI](https://pub.towardsai.net/shapash-making-ml-
 models-understandable-by-everyone-8f96ad469eb3) - [Model auditability - Towards
 DS](https://towardsdatascience.com/shapash-1-3-2-announcing-new-features-for-
 more-auditable-ai-64a6db71c919) - [Group of features - Towards AI](https://
 pub.towardsai.net/machine-learning-6011d5d9a444) - [Building confidence on
 explainability - Towards DS](https://towardsdatascience.com/building-
@@ -186,58 +175,66 @@
 Generate the Shapash Report > This step allows to generate a standalone html
 report of your project using the different splits of your dataset and also the
 metrics you used: ``` xpl.generate_report( output_file='path/to/output/
 report.html', project_info_file='path/to/project_info.yml', x_train=Xtrain,
 y_train=ytrain, y_test=ytest, title_story="House prices report",
 title_description="""This document is a data science report of the kaggle house
 prices tutorial project. It was generated using the Shapash library.""",
-metrics=[{ânameâ: âMSEâ, âpathâ:
-âsklearn.metrics.mean_squared_errorâ}] ) ``` [Report Example](https://
-shapash.readthedocs.io/en/latest/report.html) - Step 5: From training to
-deployment : SmartPredictor Object > Shapash provides a SmartPredictor object
-to deploy the summary of local explanation for the operational needs. It is an
-object dedicated to deployment, lighter than SmartExplainer with additional
-consistency checks. SmartPredictor can be used with an API or in batch mode. It
-provides predictions, detailed or summarized local explainability using
-appropriate wording. ``` predictor = xpl.to_smartpredictor() ``` See the
-tutorial part to know how to use the SmartPredictor object ## ð Tutorials
-This github repository offers many tutorials to allow you to easily get started
-with Shapash. Overview  - [Launch the webapp with a concrete use case]
-(tutorial/tutorial01-Shapash-Overview-Launch-WebApp.ipynb) - [Jupyter Overviews
-- The main outputs and methods available with the SmartExplainer object]
-(tutorial/tutorial02-Shapash-overview-in-Jupyter.ipynb) - [Shapash in
-production: From model training to deployment (API or Batch Mode)](tutorial/
-tutorial03-Shapash-overview-model-in-production.ipynb) - [Use groups of
-features](tutorial/common/tuto-common01-groups_of_features.ipynb) - [Deploy
-local explainability in production with SmartPredictor](tutorial/predictor/
-tuto-smartpredictor-introduction-to-SmartPredictor.ipynb)  Charts and plots  -
-[**Shapash** Features Importance](tutorial/plot/tuto-plot03-features-
+metrics=[{'name': 'MSE', 'path': 'sklearn.metrics.mean_squared_error'}] ) ```
+[Report Example](https://shapash.readthedocs.io/en/latest/report.html) - Step
+5: From training to deployment : SmartPredictor Object > Shapash provides a
+SmartPredictor object to deploy the summary of local explanation for the
+operational needs. It is an object dedicated to deployment, lighter than
+SmartExplainer with additional consistency checks. SmartPredictor can be used
+with an API or in batch mode. It provides predictions, detailed or summarized
+local explainability using appropriate wording. ``` predictor =
+xpl.to_smartpredictor() ``` See the tutorial part to know how to use the
+SmartPredictor object ## ð Tutorials This github repository offers many
+tutorials to allow you to easily get started with Shapash. Overview  - [Launch
+the webapp with a concrete use case](tutorial/tutorial01-Shapash-Overview-
+Launch-WebApp.ipynb) - [Jupyter Overviews - The main outputs and methods
+available with the SmartExplainer object](tutorial/tutorial02-Shapash-overview-
+in-Jupyter.ipynb) - [Shapash in production: From model training to deployment
+(API or Batch Mode)](tutorial/tutorial03-Shapash-overview-model-in-
+production.ipynb) - [Use groups of features](tutorial/common/tuto-common01-
+groups_of_features.ipynb) - [Deploy local explainability in production with
+SmartPredictor](tutorial/predictor_to_production/tuto-smartpredictor-
+introduction-to-SmartPredictor.ipynb)  Charts and plots  - [**Shapash**
+Features Importance](tutorial/plots_and_charts/tuto-plot03-features-
 importance.ipynb) - [Contribution plot to understand how one feature affects a
-prediction](tutorial/plot/tuto-plot02-contribution_plot.ipynb) - [Summarize,
-display and export local contribution using filter and local_plot method]
-(tutorial/plot/tuto-plot01-local_plot-and-to_pandas.ipynb) - [Contributions
-Comparing plot to understand why predictions on several individuals are
-different](tutorial/plot/tuto-plot04-compare_plot.ipynb) - [Visualize
-interactions between couple of variables](tutorial/plot/tuto-plot05-
-interactions-plot.ipynb) - [Customize colors in Webapp, plots and report]
+prediction](tutorial/plots_and_charts/tuto-plot02-contribution_plot.ipynb) -
+[Summarize, display and export local contribution using filter and local_plot
+method](tutorial/plots_and_charts/tuto-plot01-local_plot-and-to_pandas.ipynb) -
+[Contributions Comparing plot to understand why predictions on several
+individuals are different](tutorial/plots_and_charts/tuto-plot04-
+compare_plot.ipynb) - [Visualize interactions between couple of variables]
+(tutorial/plots_and_charts/tuto-plot05-interactions-plot.ipynb) - [Display True
+Values Vs Predicted Values](tutorial/plots_and_charts/tuto-plot06-
+prediction_plot.ipynb) - [Customize colors in Webapp, plots and report]
 (tutorial/common/tuto-common02-colors.ipynb)  Different ways to use Encoders
 and Dictionaries  - [Use Category_Encoder & inverse transformation](tutorial/
-encoder/tuto-encoder01-using-category_encoder.ipynb) - [Use ColumnTransformers]
-(tutorial/encoder/tuto-encoder02-using-columntransformer.ipynb) - [Use Simple
-Python Dictionnaries](tutorial/encoder/tuto-encoder03-using-dict.ipynb)
-Displaying data with postprocessing  [Using postprocessing parameter in compile
-method](tutorial/postprocess/tuto-postprocess01.ipynb)  Using different
-backends  - [Compute Shapley Contributions using **Shap**](tutorial/explainer/
-tuto-expl01-Shapash-Viz-using-Shap-contributions.ipynb) - [Use **Lime** to
-compute local explanation, Summarize-it with **Shapash**](tutorial/explainer/
-tuto-expl02-Shapash-Viz-using-Lime-contributions.ipynb) - [Use **ACV backend**
-to compute Active Shapley Values and SDP global importance](tutorial/explainer/
-tuto-expl03-Shapash-acv-backend.ipynb) - [Compile faster Lime and consistency
-of contributions](tutorial/explainer/tuto-expl04-Shapash-compute-Lime-
-faster.ipynb)  Evaluating the quality of your explainability  - [Building
-confidence on explainability methods using **Stability**, **Consistency** and
-**Compacity** metrics](tutorial/explainability_quality/tuto-quality01-Builing-
-confidence-explainability.ipynb)  Generate a report of your project  -
-[Generate a standalone HTML report of your project with generate_report]
-(tutorial/report/tuto-shapash-report01.ipynb)  Analysing your model via Shapash
-WebApp  - [Add features outside of the model for more exploration options]
-(tutorial/webapp/tuto-webapp01-additional-data.ipynb)
+use_encoders/tuto-encoder01-using-category_encoder.ipynb) - [Use
+ColumnTransformers](tutorial/use_encoders/tuto-encoder02-using-
+columntransformer.ipynb) - [Use Simple Python Dictionnaries](tutorial/
+use_encoders/tuto-encoder03-using-dict.ipynb)  Displaying data with
+postprocessing  [Using postprocessing parameter in compile method](tutorial/
+postprocess/tuto-postprocess01.ipynb)  Using different backends  - [Compute
+Shapley Contributions using **Shap**](tutorial/explainer_and_backend/tuto-
+expl01-Shapash-Viz-using-Shap-contributions.ipynb) - [Use **Lime** to compute
+local explanation, Summarize-it with **Shapash**](tutorial/
+explainer_and_backend/tuto-expl02-Shapash-Viz-using-Lime-contributions.ipynb) -
+[Use **ACV backend** to compute Active Shapley Values and SDP global
+importance](tutorial/explainer_and_backend/tuto-expl03-Shapash-acv-
+backend.ipynb) - [Compile faster Lime and consistency of contributions]
+(tutorial/explainer_and_backend/tuto-expl04-Shapash-compute-Lime-faster.ipynb)
+- [Use **FastTreeSHAP** or add contributions from another backend](tutorial/
+explainer_and_backend/tuto-expl05-Shapash-using-Fasttreeshap.ipynb) - [Use
+Class Shapash Backend](tutorial/explainer_and_backend/tuto-expl06-Shapash-
+custom-backend.ipynb)  Evaluating the quality of your explainability  -
+[Building confidence on explainability methods using **Stability**,
+**Consistency** and **Compacity** metrics](tutorial/explainability_quality/
+tuto-quality01-Builing-confidence-explainability.ipynb)  Generate a report of
+your project  - [Generate a standalone HTML report of your project with
+generate_report](tutorial/generate_report/tuto-shapash-report01.ipynb)
+Analysing your model via Shapash WebApp  - [Add features outside of the model
+for more exploration options](tutorial/generate_webapp/tuto-webapp01-
+additional-data.ipynb)
```

### Comparing `shapash-2.3.4/shapash.egg-info/SOURCES.txt` & `shapash-2.3.5/shapash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shapash-2.3.4/shapash.egg-info/requires.txt` & `shapash-2.3.5/shapash.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 plotly>=5.0.0
 matplotlib>=3.2.0
-numpy<1.24.0,>1.18.0
-pandas<2.0.0,>1.0.2
+numpy>1.18.0
+pandas>1.0.2
 shap>=0.38.1
 Flask<2.3.0
 dash>=2.3.1
 dash-bootstrap-components>=1.1.0
 dash-core-components>=2.0.0
 dash-daq>=0.5.0
 dash-html-components>=2.0.0
```

