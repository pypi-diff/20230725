# Comparing `tmp/easypheno-0.0.4.tar.gz` & `tmp/easypheno-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypheno-0.0.4.tar", last modified: Tue Mar  7 09:14:31 2023, max compression
+gzip compressed data, was "easypheno-0.0.5.tar", last modified: Tue Jul 25 06:00:04 2023, max compression
```

## Comparing `easypheno-0.0.4.tar` & `easypheno-0.0.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-03-07 09:14:31.553306 easypheno-0.0.4/
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    35149 2023-03-06 09:43:32.000000 easypheno-0.0.4/LICENSE
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2869 2023-03-07 09:14:31.553306 easypheno-0.0.4/PKG-INFO
--rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)     2092 2023-03-06 09:51:08.000000 easypheno-0.0.4/README.md
-drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-03-07 09:14:31.549306 easypheno-0.0.4/easypheno/
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)      633 2023-03-07 09:13:54.000000 easypheno-0.0.4/easypheno/__init__.py
-drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-03-07 09:14:31.549306 easypheno-0.0.4/easypheno/evaluation/
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)       44 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/evaluation/__init__.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1914 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/evaluation/eval_metrics.py
-drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-03-07 09:14:31.549306 easypheno-0.0.4/easypheno/model/
--rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)      376 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/__init__.py
--rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)    10322 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/_base_model.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2368 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/_bayesfromR.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2656 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/_bayesian_linreg.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     6138 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/_model_functions.py
--rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)     2696 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/_param_free_base_model.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1463 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/_sklearn_model.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2248 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/_template_sklearn_model.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2769 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/_template_tensorflow_model.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2689 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/_template_torch_model.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     8379 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/_tensorflow_model.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    11194 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/_torch_model.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)      403 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/bayesAfromR.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)      403 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/bayesBfromR.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)      403 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/bayesCfromR.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1846 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/bayes_ridge.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2992 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/blup.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     5569 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/cnn.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2376 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/elasticnet.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2349 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/linearregression.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     5098 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/localcnn.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     4299 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/mlp.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2107 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/randomforest.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2212 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/svm.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2915 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/model/xgboost.py
--rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)     8402 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/optim_pipeline.py
-drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-03-07 09:14:31.549306 easypheno-0.0.4/easypheno/optimization/
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)       65 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/optimization/__init__.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    31889 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/optimization/optuna_optim.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    10373 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/optimization/paramfree_fitting.py
-drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-03-07 09:14:31.553306 easypheno-0.0.4/easypheno/postprocess/
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)       82 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/postprocess/__init__.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     7334 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/postprocess/feat_importance.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    19042 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/postprocess/model_reuse.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     8508 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/postprocess/rerun_inference.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    14013 2023-03-07 07:10:48.000000 easypheno-0.0.4/easypheno/postprocess/results_analysis.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1991 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/postprocess/run_inference.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1186 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/postprocess/run_plot_results.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1007 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/postprocess/run_post_generate_feat_impo.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     3759 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/postprocess/run_retrain_on_new_data.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1106 2023-03-06 10:21:10.000000 easypheno-0.0.4/easypheno/postprocess/run_summarize_results.py
-drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-03-07 09:14:31.553306 easypheno-0.0.4/easypheno/preprocess/
--rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)       89 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/preprocess/__init__.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    15512 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/preprocess/base_dataset.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     6205 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/preprocess/encoding_functions.py
--rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)    52617 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/preprocess/raw_data_functions.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     6149 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/run.py
-drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-03-07 09:14:31.553306 easypheno-0.0.4/easypheno/simulate/
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)       86 2023-03-06 11:50:05.000000 easypheno-0.0.4/easypheno/simulate/__init__.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    18465 2023-03-07 09:01:26.000000 easypheno-0.0.4/easypheno/simulate/results_analysis_synthetic_data.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1195 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/simulate/run_results_analysis_synthetic_data.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     4688 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/simulate/run_synthetic_phenotypes.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    17398 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/simulate/synthetic_phenotypes.py
-drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-03-07 09:14:31.553306 easypheno-0.0.4/easypheno/utils/
--rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)       86 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/utils/__init__.py
--rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)     7404 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/utils/check_functions.py
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     8701 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/utils/helper_functions.py
--rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)     2236 2023-03-06 09:43:32.000000 easypheno-0.0.4/easypheno/utils/print_functions.py
-drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-03-07 09:14:31.549306 easypheno-0.0.4/easypheno.egg-info/
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2869 2023-03-07 09:14:31.000000 easypheno-0.0.4/easypheno.egg-info/PKG-INFO
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2248 2023-03-07 09:14:31.000000 easypheno-0.0.4/easypheno.egg-info/SOURCES.txt
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)        1 2023-03-07 09:14:31.000000 easypheno-0.0.4/easypheno.egg-info/dependency_links.txt
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)        1 2023-03-07 09:14:31.000000 easypheno-0.0.4/easypheno.egg-info/not-zip-safe
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)      206 2023-03-07 09:14:31.000000 easypheno-0.0.4/easypheno.egg-info/requires.txt
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)       10 2023-03-07 09:14:31.000000 easypheno-0.0.4/easypheno.egg-info/top_level.txt
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)       89 2023-03-06 09:43:32.000000 easypheno-0.0.4/pyproject.toml
--rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1903 2023-03-07 09:14:31.553306 easypheno-0.0.4/setup.cfg
+drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-07-25 06:00:04.235335 easypheno-0.0.5/
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    35149 2023-03-06 09:43:32.000000 easypheno-0.0.5/LICENSE
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     3268 2023-07-25 06:00:04.235335 easypheno-0.0.5/PKG-INFO
+-rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)     2491 2023-07-25 05:53:25.000000 easypheno-0.0.5/README.md
+drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-07-25 06:00:04.223335 easypheno-0.0.5/easypheno/
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)      633 2023-07-25 05:58:04.000000 easypheno-0.0.5/easypheno/__init__.py
+drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-07-25 06:00:04.227335 easypheno-0.0.5/easypheno/evaluation/
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)       44 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/evaluation/__init__.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1914 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/evaluation/eval_metrics.py
+drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-07-25 06:00:04.231335 easypheno-0.0.5/easypheno/model/
+-rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)      376 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/__init__.py
+-rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)    10322 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/_base_model.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2368 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/_bayesfromR.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2656 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/_bayesian_linreg.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     6138 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/_model_functions.py
+-rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)     2696 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/_param_free_base_model.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1463 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/_sklearn_model.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2248 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/_template_sklearn_model.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2769 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/_template_tensorflow_model.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2689 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/_template_torch_model.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     8379 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/_tensorflow_model.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    11194 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/_torch_model.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)      403 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/bayesAfromR.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)      403 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/bayesBfromR.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)      403 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/bayesCfromR.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1846 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/bayes_ridge.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2992 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/blup.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     5569 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/cnn.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2376 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/elasticnet.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2349 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/linearregression.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     5098 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/localcnn.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     4299 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/mlp.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2107 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/randomforest.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2212 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/svm.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2915 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/model/xgboost.py
+-rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)     8402 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/optim_pipeline.py
+drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-07-25 06:00:04.231335 easypheno-0.0.5/easypheno/optimization/
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)       65 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/optimization/__init__.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    31889 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/optimization/optuna_optim.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    10373 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/optimization/paramfree_fitting.py
+drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-07-25 06:00:04.235335 easypheno-0.0.5/easypheno/postprocess/
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)       82 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/postprocess/__init__.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     7334 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/postprocess/feat_importance.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    19042 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/postprocess/model_reuse.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     8508 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/postprocess/rerun_inference.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    14013 2023-03-07 07:10:48.000000 easypheno-0.0.5/easypheno/postprocess/results_analysis.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1991 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/postprocess/run_inference.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1186 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/postprocess/run_plot_results.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1007 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/postprocess/run_post_generate_feat_impo.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     3759 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/postprocess/run_retrain_on_new_data.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1106 2023-03-06 10:21:10.000000 easypheno-0.0.5/easypheno/postprocess/run_summarize_results.py
+drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-07-25 06:00:04.235335 easypheno-0.0.5/easypheno/preprocess/
+-rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)       89 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/preprocess/__init__.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    15512 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/preprocess/base_dataset.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     6205 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/preprocess/encoding_functions.py
+-rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)    52617 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/preprocess/raw_data_functions.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     6149 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/run.py
+drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-07-25 06:00:04.235335 easypheno-0.0.5/easypheno/simulate/
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)       86 2023-03-06 11:50:05.000000 easypheno-0.0.5/easypheno/simulate/__init__.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    18465 2023-03-07 09:01:26.000000 easypheno-0.0.5/easypheno/simulate/results_analysis_synthetic_data.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1195 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/simulate/run_results_analysis_synthetic_data.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     4688 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/simulate/run_synthetic_phenotypes.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)    17398 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/simulate/synthetic_phenotypes.py
+drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-07-25 06:00:04.235335 easypheno-0.0.5/easypheno/utils/
+-rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)       86 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/utils/__init__.py
+-rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)     7404 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/utils/check_functions.py
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     8701 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/utils/helper_functions.py
+-rwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)     2236 2023-03-06 09:43:32.000000 easypheno-0.0.5/easypheno/utils/print_functions.py
+drwxrwxr-x   0 fhaselbeck  (1000) fhaselbeck  (1000)        0 2023-07-25 06:00:04.227335 easypheno-0.0.5/easypheno.egg-info/
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     3268 2023-07-25 06:00:04.000000 easypheno-0.0.5/easypheno.egg-info/PKG-INFO
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     2248 2023-07-25 06:00:04.000000 easypheno-0.0.5/easypheno.egg-info/SOURCES.txt
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)        1 2023-07-25 06:00:04.000000 easypheno-0.0.5/easypheno.egg-info/dependency_links.txt
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)        1 2023-03-07 09:14:31.000000 easypheno-0.0.5/easypheno.egg-info/not-zip-safe
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)      206 2023-07-25 06:00:04.000000 easypheno-0.0.5/easypheno.egg-info/requires.txt
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)       10 2023-07-25 06:00:04.000000 easypheno-0.0.5/easypheno.egg-info/top_level.txt
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)       89 2023-03-06 09:43:32.000000 easypheno-0.0.5/pyproject.toml
+-rw-rw-r--   0 fhaselbeck  (1000) fhaselbeck  (1000)     1903 2023-07-25 06:00:04.235335 easypheno-0.0.5/setup.cfg
```

### Comparing `easypheno-0.0.4/LICENSE` & `easypheno-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/PKG-INFO` & `easypheno-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypheno
-Version: 0.0.4
+Version: 0.0.5
 Summary: state-of-the-art and easy-to-use plant phenotype prediction
 Home-page: https://github.com/grimmlab/easyPheno
 Author: Florian Haselbeck, Maura John, Dominik G. Grimm
 License: GPLv3
 Project-URL: Documentation, https://easypheno.readthedocs.io/
 Project-URL: Source, https://github.com/grimmlab/easyPheno
 Classifier: Development Status :: 4 - Beta
@@ -31,17 +31,22 @@
 In addition, our framework is designed to allow an easy and straightforward integration of further prediction models.
 
 ## Documentation
 For more information, installation guides, tutorials and much more, see our documentation: https://easypheno.readthedocs.io/
 
 ## Case Study
 In the folder `case_study`, you can find all data that we used for the case study included as supplementary for our publication.  
-For more information on this case study, see our publication and its supplementary given below.  
+For more information on this case study, see our publication and its supplementary given below ([doi: 10.1093/bioadv/vbad035](https://doi.org/10.1093/bioadv/vbad035)).
 For general information, see our documentation given above. 
 
 ## Contributors
 This pipeline is developed and maintained by members of the [Bioinformatics lab](https://bit.cs.tum.de) lead by [Prof. Dr. Dominik Grimm](https://bit.cs.tum.de/team/dominik-grimm/):
 - [Florian Haselbeck, M.Sc.](https://bit.cs.tum.de/team/florian-haselbeck/)
 - [Maura John, M.Sc.](https://bit.cs.tum.de/team/maura-john/)
 
 ## Citation
-A manuscript for publishing easyPheno as a scientific paper is currently under preparation.
+When using easyPheno, please cite our publication:  
+
+**easyPheno: An easy-to-use and easy-to-extend Python framework for phenotype prediction using Bayesian optimization.**  
+Florian Haselbeck*, Maura John* and Dominik G Grimm.    
+*Bioinformatics Advances, 2023.* [doi: 10.1093/bioadv/vbad035](https://doi.org/10.1093/bioadv/vbad035)  
+**These authors have contributed equally to this work and share first authorship.*
```

### Comparing `easypheno-0.0.4/README.md` & `easypheno-0.0.5/easypheno.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: easypheno
+Version: 0.0.5
+Summary: state-of-the-art and easy-to-use plant phenotype prediction
+Home-page: https://github.com/grimmlab/easyPheno
+Author: Florian Haselbeck, Maura John, Dominik G. Grimm
+License: GPLv3
+Project-URL: Documentation, https://easypheno.readthedocs.io/
+Project-URL: Source, https://github.com/grimmlab/easyPheno
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="left"><img src="https://raw.githubusercontent.com/grimmlab/easyPheno/main/docs/image/Logo_easyPheno_Text.png" height="80"/></div>
 
 # easyPheno: A state-of-the-art and easy-to-use Python framework for plant phenotype prediction
 
 [![Python 3.8](https://img.shields.io/badge/Python-3.8-3776AB)](https://www.python.org/downloads/release/python-388/)
 
 easyPheno is a Python framework that enables the rigorous training, comparison and analysis of phenotype predictions for a variety of different models.
@@ -12,17 +31,22 @@
 In addition, our framework is designed to allow an easy and straightforward integration of further prediction models.
 
 ## Documentation
 For more information, installation guides, tutorials and much more, see our documentation: https://easypheno.readthedocs.io/
 
 ## Case Study
 In the folder `case_study`, you can find all data that we used for the case study included as supplementary for our publication.  
-For more information on this case study, see our publication and its supplementary given below.  
+For more information on this case study, see our publication and its supplementary given below ([doi: 10.1093/bioadv/vbad035](https://doi.org/10.1093/bioadv/vbad035)).
 For general information, see our documentation given above. 
 
 ## Contributors
 This pipeline is developed and maintained by members of the [Bioinformatics lab](https://bit.cs.tum.de) lead by [Prof. Dr. Dominik Grimm](https://bit.cs.tum.de/team/dominik-grimm/):
 - [Florian Haselbeck, M.Sc.](https://bit.cs.tum.de/team/florian-haselbeck/)
 - [Maura John, M.Sc.](https://bit.cs.tum.de/team/maura-john/)
 
 ## Citation
-A manuscript for publishing easyPheno as a scientific paper is currently under preparation.
+When using easyPheno, please cite our publication:  
+
+**easyPheno: An easy-to-use and easy-to-extend Python framework for phenotype prediction using Bayesian optimization.**  
+Florian Haselbeck*, Maura John* and Dominik G Grimm.    
+*Bioinformatics Advances, 2023.* [doi: 10.1093/bioadv/vbad035](https://doi.org/10.1093/bioadv/vbad035)  
+**These authors have contributed equally to this work and share first authorship.*
```

### Comparing `easypheno-0.0.4/easypheno/__init__.py` & `easypheno-0.0.5/easypheno/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,10 +10,10 @@
     import easypheno.optimization as optimization
     import easypheno.preprocess as preprocess
     import easypheno.postprocess as postprocess
     import easypheno.simulate as simulate
 
     from . import optim_pipeline
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 __author__ = 'Florian Haselbeck, Maura John, Dominik G. Grimm'
 __credits__ = 'GrimmLab @ TUM Campus Straubing (https://bit.cs.tum.de/)'
```

### Comparing `easypheno-0.0.4/easypheno/evaluation/eval_metrics.py` & `easypheno-0.0.5/easypheno/evaluation/eval_metrics.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/_base_model.py` & `easypheno-0.0.5/easypheno/model/_base_model.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/_bayesfromR.py` & `easypheno-0.0.5/easypheno/model/_bayesfromR.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/_bayesian_linreg.py` & `easypheno-0.0.5/easypheno/model/_bayesian_linreg.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/_model_functions.py` & `easypheno-0.0.5/easypheno/model/_model_functions.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/_param_free_base_model.py` & `easypheno-0.0.5/easypheno/model/_param_free_base_model.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/_sklearn_model.py` & `easypheno-0.0.5/easypheno/model/_sklearn_model.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/_template_sklearn_model.py` & `easypheno-0.0.5/easypheno/model/_template_sklearn_model.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/_template_tensorflow_model.py` & `easypheno-0.0.5/easypheno/model/_template_tensorflow_model.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/_template_torch_model.py` & `easypheno-0.0.5/easypheno/model/_template_torch_model.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/_tensorflow_model.py` & `easypheno-0.0.5/easypheno/model/_tensorflow_model.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/_torch_model.py` & `easypheno-0.0.5/easypheno/model/_torch_model.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/bayes_ridge.py` & `easypheno-0.0.5/easypheno/model/bayes_ridge.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/blup.py` & `easypheno-0.0.5/easypheno/model/blup.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/cnn.py` & `easypheno-0.0.5/easypheno/model/cnn.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/elasticnet.py` & `easypheno-0.0.5/easypheno/model/elasticnet.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/linearregression.py` & `easypheno-0.0.5/easypheno/model/linearregression.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/localcnn.py` & `easypheno-0.0.5/easypheno/model/localcnn.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/mlp.py` & `easypheno-0.0.5/easypheno/model/mlp.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/randomforest.py` & `easypheno-0.0.5/easypheno/model/randomforest.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/svm.py` & `easypheno-0.0.5/easypheno/model/svm.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/model/xgboost.py` & `easypheno-0.0.5/easypheno/model/xgboost.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/optim_pipeline.py` & `easypheno-0.0.5/easypheno/optim_pipeline.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/optimization/optuna_optim.py` & `easypheno-0.0.5/easypheno/optimization/optuna_optim.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/optimization/paramfree_fitting.py` & `easypheno-0.0.5/easypheno/optimization/paramfree_fitting.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/postprocess/feat_importance.py` & `easypheno-0.0.5/easypheno/postprocess/feat_importance.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/postprocess/model_reuse.py` & `easypheno-0.0.5/easypheno/postprocess/model_reuse.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/postprocess/rerun_inference.py` & `easypheno-0.0.5/easypheno/postprocess/rerun_inference.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/postprocess/results_analysis.py` & `easypheno-0.0.5/easypheno/postprocess/results_analysis.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/postprocess/run_inference.py` & `easypheno-0.0.5/easypheno/postprocess/run_inference.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/postprocess/run_plot_results.py` & `easypheno-0.0.5/easypheno/postprocess/run_plot_results.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/postprocess/run_post_generate_feat_impo.py` & `easypheno-0.0.5/easypheno/postprocess/run_post_generate_feat_impo.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/postprocess/run_retrain_on_new_data.py` & `easypheno-0.0.5/easypheno/postprocess/run_retrain_on_new_data.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/postprocess/run_summarize_results.py` & `easypheno-0.0.5/easypheno/postprocess/run_summarize_results.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/preprocess/base_dataset.py` & `easypheno-0.0.5/easypheno/preprocess/base_dataset.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/preprocess/encoding_functions.py` & `easypheno-0.0.5/easypheno/preprocess/encoding_functions.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/preprocess/raw_data_functions.py` & `easypheno-0.0.5/easypheno/preprocess/raw_data_functions.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/run.py` & `easypheno-0.0.5/easypheno/run.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/simulate/results_analysis_synthetic_data.py` & `easypheno-0.0.5/easypheno/simulate/results_analysis_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/simulate/run_results_analysis_synthetic_data.py` & `easypheno-0.0.5/easypheno/simulate/run_results_analysis_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/simulate/run_synthetic_phenotypes.py` & `easypheno-0.0.5/easypheno/simulate/run_synthetic_phenotypes.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/simulate/synthetic_phenotypes.py` & `easypheno-0.0.5/easypheno/simulate/synthetic_phenotypes.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/utils/check_functions.py` & `easypheno-0.0.5/easypheno/utils/check_functions.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/utils/helper_functions.py` & `easypheno-0.0.5/easypheno/utils/helper_functions.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno/utils/print_functions.py` & `easypheno-0.0.5/easypheno/utils/print_functions.py`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/easypheno.egg-info/PKG-INFO` & `easypheno-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: easypheno
-Version: 0.0.4
-Summary: state-of-the-art and easy-to-use plant phenotype prediction
-Home-page: https://github.com/grimmlab/easyPheno
-Author: Florian Haselbeck, Maura John, Dominik G. Grimm
-License: GPLv3
-Project-URL: Documentation, https://easypheno.readthedocs.io/
-Project-URL: Source, https://github.com/grimmlab/easyPheno
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="left"><img src="https://raw.githubusercontent.com/grimmlab/easyPheno/main/docs/image/Logo_easyPheno_Text.png" height="80"/></div>
 
 # easyPheno: A state-of-the-art and easy-to-use Python framework for plant phenotype prediction
 
 [![Python 3.8](https://img.shields.io/badge/Python-3.8-3776AB)](https://www.python.org/downloads/release/python-388/)
 
 easyPheno is a Python framework that enables the rigorous training, comparison and analysis of phenotype predictions for a variety of different models.
@@ -31,17 +12,22 @@
 In addition, our framework is designed to allow an easy and straightforward integration of further prediction models.
 
 ## Documentation
 For more information, installation guides, tutorials and much more, see our documentation: https://easypheno.readthedocs.io/
 
 ## Case Study
 In the folder `case_study`, you can find all data that we used for the case study included as supplementary for our publication.  
-For more information on this case study, see our publication and its supplementary given below.  
+For more information on this case study, see our publication and its supplementary given below ([doi: 10.1093/bioadv/vbad035](https://doi.org/10.1093/bioadv/vbad035)).
 For general information, see our documentation given above. 
 
 ## Contributors
 This pipeline is developed and maintained by members of the [Bioinformatics lab](https://bit.cs.tum.de) lead by [Prof. Dr. Dominik Grimm](https://bit.cs.tum.de/team/dominik-grimm/):
 - [Florian Haselbeck, M.Sc.](https://bit.cs.tum.de/team/florian-haselbeck/)
 - [Maura John, M.Sc.](https://bit.cs.tum.de/team/maura-john/)
 
 ## Citation
-A manuscript for publishing easyPheno as a scientific paper is currently under preparation.
+When using easyPheno, please cite our publication:  
+
+**easyPheno: An easy-to-use and easy-to-extend Python framework for phenotype prediction using Bayesian optimization.**  
+Florian Haselbeck*, Maura John* and Dominik G Grimm.    
+*Bioinformatics Advances, 2023.* [doi: 10.1093/bioadv/vbad035](https://doi.org/10.1093/bioadv/vbad035)  
+**These authors have contributed equally to this work and share first authorship.*
```

### Comparing `easypheno-0.0.4/easypheno.egg-info/SOURCES.txt` & `easypheno-0.0.5/easypheno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easypheno-0.0.4/setup.cfg` & `easypheno-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easypheno
-version = 0.0.4
+version = 0.0.5
 description = state-of-the-art and easy-to-use plant phenotype prediction
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GPLv3
 author = Florian Haselbeck, Maura John, Dominik G. Grimm
 url = https://github.com/grimmlab/easyPheno
 project_urls =
```

