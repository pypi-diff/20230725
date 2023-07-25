# Comparing `tmp/fedot-0.7.1.tar.gz` & `tmp/fedot-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedot-0.7.1.tar", last modified: Thu Jun  8 08:47:24 2023, max compression
+gzip compressed data, was "fedot-0.7.2.tar", last modified: Tue Jul 25 13:17:26 2023, max compression
```

## Comparing `fedot-0.7.1.tar` & `fedot-0.7.2.tar`

### file list

```diff
@@ -1,340 +1,342 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-08 08:47:17.000000 fedot-0.7.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-08 08:47:17.000000 fedot-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-06-08 08:47:24.587392 fedot-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21646 2023-06-08 08:47:17.000000 fedot-0.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.547392 fedot-0.7.1/cases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/dataset_preparation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/kc2_sourcecode_defects_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/metocean_forecasting_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/multi_target_levels_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/multi_ts_level_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/multivariate_ts_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/spam_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/time_series_gapfilling_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.551392 fedot-0.7.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.551392 fedot-0.7.1/examples/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/additional_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.551392 fedot-0.7.1/examples/advanced/automl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/automl/h2o_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/automl/pipeline_from_automl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/automl/tpot_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/automl/tpot_vs_fedot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.555392 fedot-0.7.1/examples/advanced/decompose/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/decompose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/decompose/classification_refinement_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/decompose/refinement_forecast_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/decompose/regression_refinement_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.555392 fedot-0.7.1/examples/advanced/fedot_based_solutions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/fedot_based_solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/fedot_based_solutions/external_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/gpu_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/multi_modal_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/multimodal_text_num_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/multiobj_optimisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/multitask_classification_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/parallelization_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/pipeline_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/profiler_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.555392 fedot-0.7.1/examples/advanced/remote_execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/remote_execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/remote_execution/remote_fit_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/remote_execution/ts_composer_with_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.555392 fedot-0.7.1/examples/advanced/sensitivity_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/case_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/complex_analysis_with_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/dataset_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/mta_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/pipeline_export_with_sa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/pipelines_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/run_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/surrogate_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.555392 fedot-0.7.1/examples/advanced/time_series_forecasting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/composing_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/custom_model_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/exogenous.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/multi_ts_arctic_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/multistep.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/nemo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/nemo_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/sparse_lagged_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/project_import_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.559392 fedot-0.7.1/examples/simple/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.563392 fedot-0.7.1/examples/simple/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/classification/api_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/classification/classification_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/classification/classification_with_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/classification/image_classification_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/classification/multiclass_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/classification/resample_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.563392 fedot-0.7.1/examples/simple/cli_application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/cli_application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/cli_application/cli_call_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.563392 fedot-0.7.1/examples/simple/interpretable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/interpretable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/interpretable/api_explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/interpretable/pipeline_explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/multitask_classification_regression_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/pipeline_and_history_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/pipeline_import_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/pipeline_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/pipeline_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/pipeline_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.563392 fedot-0.7.1/examples/simple/regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/regression/api_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/regression/regression_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/regression/regression_with_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.563392 fedot-0.7.1/examples/simple/time_series_forecasting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/time_series_forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/time_series_forecasting/api_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/time_series_forecasting/cgru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/time_series_forecasting/fitted_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/time_series_forecasting/gapfilling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/time_series_forecasting/ts_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/time_series_forecasting/tuning_pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.563392 fedot-0.7.1/fedot/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.567392 fedot-0.7.1/fedot/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.567392 fedot-0.7.1/fedot/api/api_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/api_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/api_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/api_params_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.567392 fedot-0.7.1/fedot/api/api_utils/assumptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/assumptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/assumptions/assumptions_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/assumptions/assumptions_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/assumptions/operations_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/assumptions/preprocessing_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/assumptions/task_assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/data_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/input_analyser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/predefined_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/fedot_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    31298 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.567392 fedot-0.7.1/fedot/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.571392 fedot-0.7.1/fedot/core/caching/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/caching/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/caching/base_cache_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/caching/pipelines_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/caching/pipelines_cache_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/caching/preprocessing_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/caching/preprocessing_cache_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.571392 fedot-0.7.1/fedot/core/composer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/composer_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.571392 fedot-0.7.1/fedot/core/composer/gp_composer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/gp_composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/gp_composer/gp_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/gp_composer/specific_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/meta_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/random_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.571392 fedot-0.7.1/fedot/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/array_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    28271 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/data_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/data_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/data_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/load_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.571392 fedot-0.7.1/fedot/core/data/merge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/merge/data_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/merge/supplementary_data_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/supplementary_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.575392 fedot-0.7.1/fedot/core/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/atomized_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/atomized_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/automl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/data_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.575392 fedot-0.7.1/fedot/core/operations/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/automl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/common_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/evaluation_interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.575392 fedot-0.7.1/fedot/core/operations/evaluation/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/gpu/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/gpu/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/gpu/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/gpu/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.575392 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.575392 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/decompose.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_imbalanced_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/text_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/text_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)    35322 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/ts_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/implementation_interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.579392 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/discriminant_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/svc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.579392 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/arima.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/cgru.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/statsmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/hyperparameters_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/operation_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/operation_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.579392 fedot-0.7.1/fedot/core/optimisers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/optimisers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.579392 fedot-0.7.1/fedot/core/optimisers/objective/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/optimisers/objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/optimisers/objective/data_objective_advisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/optimisers/objective/data_objective_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/optimisers/objective/data_source_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/optimisers/objective/metrics_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/optimisers/objective/objective_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.579392 fedot-0.7.1/fedot/core/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/automl_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14837 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    17807 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/pipeline_advisor.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/pipeline_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/pipeline_composer_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/pipeline_graph_generation_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/pipeline_node_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/random_pipeline_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    18702 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/ts_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.583392 fedot-0.7.1/fedot/core/pipelines/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/tuning/hyperparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/tuning/search_space.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/tuning/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/tuning/tuner_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/verification.py
--rw-r--r--   0 runner    (1001) docker     (123)    16905 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/verification_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.583392 fedot-0.7.1/fedot/core/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.583392 fedot-0.7.1/fedot/core/repository/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/data/automl_repository.json
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/data/data_operation_repository.json
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/data/default_operation_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/data/gpu_models_repository.json
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/data/model_repository.json
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/dataset_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/default_params_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/graph_operation_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/json_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/operation_types_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/pipeline_operation_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/quality_metrics_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.583392 fedot-0.7.1/fedot/core/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/validation/split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.583392 fedot-0.7.1/fedot/core/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/visualisation/pipeline_specific_visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.583392 fedot-0.7.1/fedot/explainability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/explainability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/explainability/explainer_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/explainability/explainers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/explainability/surrogate_explainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.583392 fedot-0.7.1/fedot/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/base_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/data_type_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    29084 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/dummy_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23886 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/fedot/remote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/fedot/remote/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/fedot/remote/infrastructure/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/infrastructure/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/infrastructure/clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/infrastructure/clients/datamall_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/infrastructure/clients/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/pipeline_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/remote_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/run_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/fedot/sensitivity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/fedot/sensitivity/deletion_methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/deletion_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/deletion_methods/multi_times_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    14594 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/node_sa_approaches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/nodes_sensitivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/multi_operations_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/one_operation_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/sa_and_sample_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/pipeline_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/pipeline_sensitivity_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/sa_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/fedot/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/define_metric_by_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/golem_imports_transition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/pattern_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/project_import_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/synth_dataset_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19330 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/ts_gapfilling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.567392 fedot-0.7.1/fedot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-06-08 08:47:24.000000 fedot-0.7.1/fedot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-06-08 08:47:24.000000 fedot-0.7.1/fedot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:47:24.000000 fedot-0.7.1/fedot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-08 08:47:24.000000 fedot-0.7.1/fedot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 08:47:24.000000 fedot-0.7.1/fedot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 08:47:24.587392 fedot-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-08 08:47:17.000000 fedot-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-08 08:47:17.000000 fedot-0.7.1/test/test_gpu_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.135538 fedot-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-25 13:17:20.000000 fedot-0.7.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-25 13:17:20.000000 fedot-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17599 2023-07-25 13:17:26.135538 fedot-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21665 2023-07-25 13:17:20.000000 fedot-0.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.099538 fedot-0.7.2/cases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-25 13:17:20.000000 fedot-0.7.2/cases/dataset_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-25 13:17:20.000000 fedot-0.7.2/cases/kc2_sourcecode_defects_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-25 13:17:20.000000 fedot-0.7.2/cases/metocean_forecasting_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-25 13:17:20.000000 fedot-0.7.2/cases/multi_target_levels_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-25 13:17:20.000000 fedot-0.7.2/cases/multi_ts_level_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-07-25 13:17:20.000000 fedot-0.7.2/cases/multivariate_ts_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-25 13:17:20.000000 fedot-0.7.2/cases/spam_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-25 13:17:20.000000 fedot-0.7.2/cases/time_series_gapfilling_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.099538 fedot-0.7.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.103538 fedot-0.7.2/examples/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/additional_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.103538 fedot-0.7.2/examples/advanced/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/automl/h2o_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/automl/pipeline_from_automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/automl/tpot_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/automl/tpot_vs_fedot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.103538 fedot-0.7.2/examples/advanced/decompose/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/decompose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/decompose/classification_refinement_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/decompose/refinement_forecast_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/decompose/regression_refinement_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.103538 fedot-0.7.2/examples/advanced/fedot_based_solutions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/fedot_based_solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/fedot_based_solutions/external_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/gpu_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/multi_modal_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/multimodal_text_num_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/multiobj_optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/multitask_classification_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/parallelization_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/pipeline_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/profiler_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.103538 fedot-0.7.2/examples/advanced/remote_execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/remote_execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/remote_execution/remote_fit_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/remote_execution/ts_composer_with_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.103538 fedot-0.7.2/examples/advanced/sensitivity_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/sensitivity_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/sensitivity_analysis/case_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/sensitivity_analysis/complex_analysis_with_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/sensitivity_analysis/dataset_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/sensitivity_analysis/mta_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/sensitivity_analysis/pipeline_export_with_sa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/sensitivity_analysis/pipelines_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/sensitivity_analysis/run_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/surrogate_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.107538 fedot-0.7.2/examples/advanced/time_series_forecasting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/time_series_forecasting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/time_series_forecasting/composing_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/time_series_forecasting/custom_model_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/time_series_forecasting/exogenous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/time_series_forecasting/multi_ts_arctic_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/time_series_forecasting/multistep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/time_series_forecasting/nemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/time_series_forecasting/nemo_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/advanced/time_series_forecasting/sparse_lagged_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/project_import_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.107538 fedot-0.7.2/examples/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.107538 fedot-0.7.2/examples/simple/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/classification/api_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/classification/classification_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/classification/classification_with_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/classification/image_classification_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/classification/multiclass_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/classification/resample_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.107538 fedot-0.7.2/examples/simple/cli_application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/cli_application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/cli_application/cli_call_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.107538 fedot-0.7.2/examples/simple/interpretable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/interpretable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/interpretable/api_explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/interpretable/pipeline_explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/multitask_classification_regression_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/pipeline_and_history_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/pipeline_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/pipeline_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/pipeline_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/pipeline_tuning_with_iopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/pipeline_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.107538 fedot-0.7.2/examples/simple/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/regression/api_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/regression/regression_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/regression/regression_with_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.111538 fedot-0.7.2/examples/simple/time_series_forecasting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/time_series_forecasting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/time_series_forecasting/api_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/time_series_forecasting/cgru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/time_series_forecasting/fitted_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/time_series_forecasting/gapfilling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/time_series_forecasting/ts_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-25 13:17:20.000000 fedot-0.7.2/examples/simple/time_series_forecasting/tuning_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.111538 fedot-0.7.2/fedot/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.111538 fedot-0.7.2/fedot/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.111538 fedot-0.7.2/fedot/api/api_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/api_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/api_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/api_params_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.115538 fedot-0.7.2/fedot/api/api_utils/assumptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/assumptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/assumptions/assumptions_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/assumptions/assumptions_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/assumptions/operations_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/assumptions/preprocessing_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/assumptions/task_assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/data_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/input_analyser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/predefined_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/api_utils/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/fedot_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31298 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/api/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.115538 fedot-0.7.2/fedot/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.115538 fedot-0.7.2/fedot/core/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/caching/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/caching/base_cache_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/caching/pipelines_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/caching/pipelines_cache_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/caching/preprocessing_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/caching/preprocessing_cache_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.115538 fedot-0.7.2/fedot/core/composer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/composer/composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/composer/composer_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.115538 fedot-0.7.2/fedot/core/composer/gp_composer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/composer/gp_composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/composer/gp_composer/gp_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/composer/gp_composer/specific_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/composer/meta_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/composer/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/composer/random_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.115538 fedot-0.7.2/fedot/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/data/array_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28287 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/data/data_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/data/data_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/data/data_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/data/load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.119538 fedot-0.7.2/fedot/core/data/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/data/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/data/merge/data_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/data/merge/supplementary_data_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/data/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/data/supplementary_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/data/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.119538 fedot-0.7.2/fedot/core/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/atomized_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/atomized_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/data_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.119538 fedot-0.7.2/fedot/core/operations/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/common_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/evaluation_interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.119538 fedot-0.7.2/fedot/core/operations/evaluation/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/gpu/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/gpu/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/gpu/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/gpu/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.119538 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.123538 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/decompose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_imbalanced_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/text_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/text_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35322 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/ts_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/implementation_interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.123538 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/discriminant_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/svc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.123538 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/arima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/cgru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/statsmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/evaluation/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/hyperparameters_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/operation_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/operations/operation_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.123538 fedot-0.7.2/fedot/core/optimisers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/optimisers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.123538 fedot-0.7.2/fedot/core/optimisers/objective/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/optimisers/objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/optimisers/objective/data_objective_advisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/optimisers/objective/data_objective_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/optimisers/objective/data_source_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/optimisers/objective/metrics_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/optimisers/objective/objective_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.127538 fedot-0.7.2/fedot/core/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/automl_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14837 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17807 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/pipeline_advisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/pipeline_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/pipeline_composer_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/pipeline_graph_generation_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/pipeline_node_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/random_pipeline_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18702 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/ts_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.127538 fedot-0.7.2/fedot/core/pipelines/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/tuning/hyperparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30255 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/tuning/search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/tuning/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/tuning/tuner_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16905 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/pipelines/verification_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.127538 fedot-0.7.2/fedot/core/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/repository/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.131538 fedot-0.7.2/fedot/core/repository/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/repository/data/automl_repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/repository/data/data_operation_repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/repository/data/default_operation_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/repository/data/gpu_models_repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/repository/data/model_repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/repository/dataset_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/repository/default_params_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/repository/graph_operation_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/repository/json_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/repository/operation_types_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/repository/pipeline_operation_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/repository/quality_metrics_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/repository/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.131538 fedot-0.7.2/fedot/core/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/validation/split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.131538 fedot-0.7.2/fedot/core/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/core/visualisation/pipeline_specific_visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.131538 fedot-0.7.2/fedot/explainability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/explainability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/explainability/explainer_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/explainability/explainers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/explainability/surrogate_explainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.131538 fedot-0.7.2/fedot/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/preprocessing/base_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/preprocessing/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/preprocessing/data_type_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29084 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/preprocessing/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/preprocessing/dummy_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23886 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/preprocessing/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/preprocessing/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.131538 fedot-0.7.2/fedot/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.131538 fedot-0.7.2/fedot/remote/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/remote/infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.131538 fedot-0.7.2/fedot/remote/infrastructure/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/remote/infrastructure/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/remote/infrastructure/clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/remote/infrastructure/clients/datamall_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/remote/infrastructure/clients/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/remote/pipeline_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/remote/remote_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/remote/run_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.131538 fedot-0.7.2/fedot/sensitivity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/sensitivity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.135538 fedot-0.7.2/fedot/sensitivity/deletion_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/sensitivity/deletion_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/sensitivity/deletion_methods/multi_times_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14594 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/sensitivity/node_sa_approaches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/sensitivity/nodes_sensitivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.135538 fedot-0.7.2/fedot/sensitivity/operations_hp_sensitivity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/sensitivity/operations_hp_sensitivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/sensitivity/operations_hp_sensitivity/multi_operations_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/sensitivity/operations_hp_sensitivity/one_operation_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/sensitivity/operations_hp_sensitivity/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/sensitivity/operations_hp_sensitivity/sa_and_sample_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/sensitivity/pipeline_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/sensitivity/pipeline_sensitivity_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/sensitivity/sa_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.135538 fedot-0.7.2/fedot/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/utilities/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/utilities/define_metric_by_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/utilities/golem_imports_transition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/utilities/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/utilities/pattern_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/utilities/project_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/utilities/synth_dataset_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19330 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/utilities/ts_gapfilling.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 13:17:20.000000 fedot-0.7.2/fedot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.111538 fedot-0.7.2/fedot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17599 2023-07-25 13:17:26.000000 fedot-0.7.2/fedot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-07-25 13:17:26.000000 fedot-0.7.2/fedot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:17:26.000000 fedot-0.7.2/fedot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-25 13:17:26.000000 fedot-0.7.2/fedot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 13:17:26.000000 fedot-0.7.2/fedot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 13:17:26.135538 fedot-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-25 13:17:20.000000 fedot-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:17:26.135538 fedot-0.7.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-25 13:17:20.000000 fedot-0.7.2/test/test_gpu_strategy.py
```

### Comparing `fedot-0.7.1/LICENSE.md` & `fedot-0.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/PKG-INFO` & `fedot-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedot
-Version: 0.7.1
+Version: 0.7.2
 Summary: Automated machine learning framework for composite pipelines
 Home-page: https://github.com/aimclub/FEDOT
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
@@ -196,22 +196,17 @@
 
 Current R&D and future plans
 ============================
 
 Currently, we are working on new features and trying to improve the performance and the user experience of FEDOT.
 The major ongoing tasks and plans:
 
-* Effective and ready-to-use pipeline templates for certain tasks and data types;
-* Integration with GPU via Rapids framework;
-* Alternative optimization methods of fixed-shaped pipelines;
-* Integration with MLFlow for import and export of the pipelines;
-* Improvement of the high-level API.
-
-
-Also, we are doing several research tasks related to AutoML time-series benchmarking and multi-modal modeling.
+* Implementation of meta-learning based at GNN and RL (see `MetaFEDOT <https://github.com/ITMO-NSS-team/MetaFEDOT>`__)
+* Improvement of the optimisation-related algorithms implemented in `GOLEM <https://github.com/aimclub/GOLEM/>`__.
+* Support for more complicated pipeline design patters, especially for time series forecasting.
 
 Any contribution is welcome. Our R&D team is open for cooperation with other scientific teams as well as with industrial partners.
 
 Documentation
 =============
 
 Also, a detailed FEDOT API description is available in `Read the Docs <https://fedot.readthedocs.io/en/latest/>`__.
@@ -224,16 +219,17 @@
 Acknowledgments
 ===============
 
 We acknowledge the contributors for their important impact and the participants of numerous scientific conferences and workshops for their valuable advice and suggestions.
 
 Side Projects
 =============
+- The optimisation core implemented in `GOLEM <https://github.com/aimclub/GOLEM/>`__ repository.
 - The prototype of the web-GUI for FEDOT is available in the `FEDOT.WEB <https://github.com/aimclub/FEDOT.Web>`__ repository.
-
+- The prototype of FEDOT-based meta-AutoML in the `MetaFEDOT <https://github.com/ITMO-NSS-team/MetaFEDOT>`__ repository.
 
 Contacts
 ========
 - `Telegram channel for solving problems and answering questions about FEDOT <https://t.me/FEDOT_helpdesk>`_
 - `Natural System Simulation Team <https://itmo-nss-team.github.io/>`_
 - `Anna Kalyuzhnaya <https://scholar.google.com/citations?user=bjiILqcAAAAJ&hl=ru>`_, Team leader (anna.kalyuzhnaya@itmo.ru)
 - `Newsfeed <https://t.me/NSS_group>`_
```

### Comparing `fedot-0.7.1/README.rst` & `fedot-0.7.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -29,20 +29,20 @@
      - | |gitlab|
    * - funding
      - | |ITMO| |NCCR|
 .. end-badges
 
 **FEDOT** - это open-source фреймворк для решения задач из области автоматизированного моделирования и машинного обучения (AutoML). Фреймворк распространяется под лицензией 3-Clause BSD.
 
-FEDOT предоставляет возможность использовать генеративный дизайн для проектирования пайплайнов машинного обучения для различных реальных задач. Ядро фреймворка основано на эволюционном подходе и поддерживает классификацию (бинарную и мультиклассовую), регрессию, кластеризацию и задачи прогнозирования временных рядов.
+FEDOT предоставляет возможность использовать генеративный дизайн для проектирования пайплайнов машинного обучения для различных реальных задач. Ядро фреймворка основано на эволюционном подходе и поддерживает классификацию (бинарную и мультиклассовую), регрессию, и задачи прогнозирования временных рядов.
 
 .. image:: docs/fedot-workflow.png
    :alt: Реализация процесса автоматического машинного обучения в FEDOT
 
-Ключевой особенностью фреймворка является управление сложными взаимодействиями между различными частями пайплайнов. Они представлены в виде графика, который определяет связи между предварительной обработкой данных и блоками модели.
+Ключевой особенностью фреймворка является управление сложными взаимодействиями между различными частями пайплайнов. Они представлены в виде графа, который определяет связи между предварительной обработкой данных и блоками модели.
 
 Проект поддерживается исследовательской группой Natural Systems Simulation Lab, которая является частью `Национального центра когнитивных разработок Университета ИТМО <https://actcognitive.org/>`__.
 
 Более подробная информация о FEDOT доступна в следующем видео:
 
 
 .. image:: https://res.cloudinary.com/marcomontalbano/image/upload/v1606396758/video_to_markdown/images/youtube--RjbuV6i6de4-c05b58ac6eb4c4700831b2b3070cd403.jpg
@@ -175,19 +175,17 @@
 
 Текущие исследования/разработки и планы на будущее
 ==================================================
 
 В настоящее время мы работаем над новыми функциями и пытаемся улучшить производительность и удобство использования FEDOT.
 Основные текущие задачи и планы:
 
-* Эффективные и готовые к использованию шаблоны пайплайнов для определенных задач и типов данных;
-* Интеграция с GPU через Rapids framework;
-* Альтернативные методы оптимизации пайплайнов с фиксированной формой;
-* Интеграция с ML Flow для импорта и экспорта пайплайнов;
-* Улучшение высокоуровневого API.
+* Реализация методов и алгоритмов мета-обучения
+* Повышение эффективности оптимизационного ядра GOLEM.
+* Поддержка более сложных вариантов пайплайнов, особенно для задач прогнозирования временных рядов.
 
 
 Кроме того, мы работаем над рядом исследовательских задач, связанных с бенчмаркингом прогнозирования временных рядов с помощью AutoML и мультимодального моделирования.
 
 Наша научно-исследовательская команда открыта для сотрудничества с другими научными коллективами, а также с партнерами из индустрии.
 
 Документация
@@ -203,15 +201,17 @@
 Благодарности
 =============
 
 Мы благодарны контрибьютерам за их важный вклад, а участникам многочисленных конференций и семинаров - за их ценные советы и предложения.
 
 Дополнительные проекты
 ======================
-- Прототип web-GUI для FEDOT доступен в репозитории `FEDOT.WEB <https://github.com/aimclub/FEDOT.Web>`__.
+- Оптимизационное ядро, вынесенное в библиотеку `GOLEM <https://github.com/aimclub/GOLEM/>`__.
+- Прототип реализации Meta-AutoML - `MetaFEDOT <https://github.com/ITMO-NSS-team/MetaFEDOT>`__.
+- Прототип web-GUI для FEDOT - `FEDOT.WEB <https://github.com/aimclub/FEDOT.Web>`__.
 
 
 Контакты
 ========
 - `Telegram-канал <https://t.me/FEDOT_helpdesk>`_  для решения проблем и ответов на вопросы о FEDOT
 - Команда `Natural System Simulation <https://itmo-nss-team.github.io/>`_
 - `Анна Калюжная <https://scholar.google.com/citations?user=bjiILqcAAAAJ&hl=ru>`_, руководитель (anna.kalyuzhnaya@itmo.ru)
```

### Comparing `fedot-0.7.1/cases/dataset_preparation.py` & `fedot-0.7.2/cases/dataset_preparation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/cases/kc2_sourcecode_defects_classification.py` & `fedot-0.7.2/cases/kc2_sourcecode_defects_classification.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/cases/metocean_forecasting_problem.py` & `fedot-0.7.2/cases/metocean_forecasting_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         'ws': ws_history,  # additional variable
         'ssh': ssh_history,  # target variable
     }
 
     fedot = Fedot(problem='ts_forecasting',
                   task_params=TsForecastingParams(forecast_length=forecast_length),
                   timeout=timeout, logging_level=logging.DEBUG)
+    fedot.current_pipeline
 
     pipeline = fedot.fit(features=historical_data, target=ssh_history)
     fedot.forecast(historical_data)
     metric = fedot.get_metrics(target=ssh_obs)
 
     if visualization:
         pipeline.show()
```

### Comparing `fedot-0.7.1/cases/multi_target_levels_forecasting.py` & `fedot-0.7.2/cases/multi_target_levels_forecasting.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/cases/multi_ts_level_forecasting.py` & `fedot-0.7.2/cases/multi_ts_level_forecasting.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/cases/multivariate_ts_forecasting.py` & `fedot-0.7.2/cases/multivariate_ts_forecasting.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/cases/spam_detection.py` & `fedot-0.7.2/cases/spam_detection.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/cases/time_series_gapfilling_case.py` & `fedot-0.7.2/cases/time_series_gapfilling_case.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/additional_learning.py` & `fedot-0.7.2/examples/advanced/additional_learning.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/automl/h2o_example.py` & `fedot-0.7.2/examples/advanced/automl/h2o_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/automl/pipeline_from_automl.py` & `fedot-0.7.2/examples/advanced/automl/pipeline_from_automl.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/automl/tpot_example.py` & `fedot-0.7.2/examples/advanced/automl/tpot_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/automl/tpot_vs_fedot.py` & `fedot-0.7.2/examples/advanced/automl/tpot_vs_fedot.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/decompose/classification_refinement_example.py` & `fedot-0.7.2/examples/advanced/decompose/classification_refinement_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/decompose/refinement_forecast_example.py` & `fedot-0.7.2/examples/advanced/decompose/refinement_forecast_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/decompose/regression_refinement_example.py` & `fedot-0.7.2/examples/advanced/decompose/regression_refinement_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/fedot_based_solutions/external_optimizer.py` & `fedot-0.7.2/examples/advanced/fedot_based_solutions/external_optimizer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/gpu_example.py` & `fedot-0.7.2/examples/advanced/gpu_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/multi_modal_pipeline.py` & `fedot-0.7.2/examples/advanced/multi_modal_pipeline.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/multimodal_text_num_example.py` & `fedot-0.7.2/examples/advanced/multimodal_text_num_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/multiobj_optimisation.py` & `fedot-0.7.2/examples/advanced/multiobj_optimisation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/multitask_classification_regression.py` & `fedot-0.7.2/examples/advanced/multitask_classification_regression.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/parallelization_comparison.py` & `fedot-0.7.2/examples/advanced/parallelization_comparison.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/pipeline_sensitivity.py` & `fedot-0.7.2/examples/advanced/pipeline_sensitivity.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/profiler_example.py` & `fedot-0.7.2/examples/advanced/profiler_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/remote_execution/remote_fit_example.py` & `fedot-0.7.2/examples/advanced/remote_execution/remote_fit_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/remote_execution/ts_composer_with_integration.py` & `fedot-0.7.2/examples/advanced/remote_execution/ts_composer_with_integration.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/sensitivity_analysis/case_analysis.py` & `fedot-0.7.2/examples/advanced/sensitivity_analysis/case_analysis.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/sensitivity_analysis/complex_analysis_with_requirements.py` & `fedot-0.7.2/examples/advanced/sensitivity_analysis/complex_analysis_with_requirements.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/sensitivity_analysis/dataset_access.py` & `fedot-0.7.2/examples/advanced/sensitivity_analysis/dataset_access.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/sensitivity_analysis/mta_example.py` & `fedot-0.7.2/examples/advanced/sensitivity_analysis/mta_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/sensitivity_analysis/pipeline_export_with_sa.py` & `fedot-0.7.2/examples/advanced/sensitivity_analysis/pipeline_export_with_sa.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/sensitivity_analysis/pipelines_access.py` & `fedot-0.7.2/examples/advanced/sensitivity_analysis/pipelines_access.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/sensitivity_analysis/run_cases.py` & `fedot-0.7.2/examples/advanced/sensitivity_analysis/run_cases.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/surrogate_optimization.py` & `fedot-0.7.2/examples/advanced/surrogate_optimization.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/time_series_forecasting/composing_pipelines.py` & `fedot-0.7.2/examples/advanced/time_series_forecasting/composing_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/time_series_forecasting/custom_model_tuning.py` & `fedot-0.7.2/examples/advanced/time_series_forecasting/custom_model_tuning.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,24 +90,31 @@
                                                                  data_type=DataTypesEnum.ts))
 
     if pipeline_type == 'with_fit':
         pipeline = get_fitting_custom_pipeline()
         # Setting custom search space for tuner (necessary)
         # model and output_type should be wrapped into hyperopt
         custom_search_space = {'custom': {
-            'alpha': (hp.uniform, [0.01, 10]),
-            'model_predict': (hp.choice, [[custom_ml_model_imitation_predict]]),
-            'model_fit': (hp.choice, [[custom_ml_model_imitation_fit]])}}
+            'alpha': {
+                'hyperopt-dist': hp.uniform,
+                'sampling-scope': [0.01, 10],
+                'type': 'continuous'}}}
     elif pipeline_type == 'without_fit':
         pipeline = get_domain_pipeline()
         # Setting custom search space for tuner (necessary)
         # model and output_type should be wrapped into hyperopt
-        custom_search_space = {'custom': {'a': (hp.uniform, [-100, 100]),
-                                          'b': (hp.uniform, [0, 1000]),
-                                          'model_predict': (hp.choice, [[domain_model_imitation_predict]])}}
+        custom_search_space = {'custom': {
+            'a': {
+                'hyperopt-dist': hp.uniform,
+                'sampling-scope': [-100, 100],
+                'type': 'continuous'},
+            'b': {
+                'hyperopt-dist': hp.uniform,
+                'sampling-scope': [0, 1000],
+                'type': 'continuous'}}}
     pipeline.fit_from_scratch(train_input)
     pipeline.print_structure()
     # Get prediction with initial approximation
     predicted_before_tuning = pipeline.predict(predict_input).predict
 
     replace_default_search_space = True
     cv_folds = 3
```

### Comparing `fedot-0.7.1/examples/advanced/time_series_forecasting/exogenous.py` & `fedot-0.7.2/examples/advanced/time_series_forecasting/exogenous.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/time_series_forecasting/multi_ts_arctic_forecasting.py` & `fedot-0.7.2/examples/advanced/time_series_forecasting/multi_ts_arctic_forecasting.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/time_series_forecasting/multistep.py` & `fedot-0.7.2/examples/advanced/time_series_forecasting/multistep.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/time_series_forecasting/nemo.py` & `fedot-0.7.2/examples/advanced/time_series_forecasting/nemo.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/time_series_forecasting/nemo_multiple.py` & `fedot-0.7.2/examples/advanced/time_series_forecasting/nemo_multiple.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/advanced/time_series_forecasting/sparse_lagged_tuning.py` & `fedot-0.7.2/examples/advanced/time_series_forecasting/sparse_lagged_tuning.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/project_import_export.py` & `fedot-0.7.2/examples/project_import_export.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/classification/api_classification.py` & `fedot-0.7.2/examples/simple/classification/api_classification.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/classification/classification_pipelines.py` & `fedot-0.7.2/examples/simple/classification/classification_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/classification/classification_with_tuning.py` & `fedot-0.7.2/examples/simple/classification/classification_with_tuning.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/classification/image_classification_problem.py` & `fedot-0.7.2/examples/simple/classification/image_classification_problem.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 from golem.utilities.requirements_notificator import warn_requirement
 
 try:
     import tensorflow as tf
 except ModuleNotFoundError:
-    warn_requirement('tensorflow')
+    warn_requirement('tensorflow', 'fedot[extra]')
 
 from sklearn.metrics import roc_auc_score as roc_auc
 
 from examples.simple.classification.classification_pipelines import cnn_composite_pipeline
 from fedot.core.data.data import InputData, OutputData
 from fedot.core.repository.tasks import Task, TaskTypesEnum
```

### Comparing `fedot-0.7.1/examples/simple/classification/multiclass_prediction.py` & `fedot-0.7.2/examples/simple/classification/multiclass_prediction.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/classification/resample_example.py` & `fedot-0.7.2/examples/simple/classification/resample_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/cli_application/cli_call_example.py` & `fedot-0.7.2/examples/simple/cli_application/cli_call_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/interpretable/api_explain.py` & `fedot-0.7.2/examples/simple/interpretable/api_explain.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/interpretable/pipeline_explain.py` & `fedot-0.7.2/examples/simple/interpretable/pipeline_explain.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/multitask_classification_regression_api.py` & `fedot-0.7.2/examples/simple/multitask_classification_regression_api.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/pipeline_and_history_visualization.py` & `fedot-0.7.2/examples/simple/pipeline_and_history_visualization.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/pipeline_import_export.py` & `fedot-0.7.2/examples/simple/pipeline_import_export.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/pipeline_log.py` & `fedot-0.7.2/examples/simple/pipeline_log.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/pipeline_tune.py` & `fedot-0.7.2/examples/simple/pipeline_tune.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/pipeline_visualization.py` & `fedot-0.7.2/examples/simple/pipeline_visualization.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/regression/api_regression.py` & `fedot-0.7.2/examples/simple/regression/api_regression.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/regression/regression_pipelines.py` & `fedot-0.7.2/examples/simple/regression/regression_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/regression/regression_with_tuning.py` & `fedot-0.7.2/examples/simple/regression/regression_with_tuning.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/time_series_forecasting/api_forecasting.py` & `fedot-0.7.2/examples/simple/time_series_forecasting/api_forecasting.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/time_series_forecasting/cgru.py` & `fedot-0.7.2/examples/simple/time_series_forecasting/cgru.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/time_series_forecasting/fitted_values.py` & `fedot-0.7.2/examples/simple/time_series_forecasting/fitted_values.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/time_series_forecasting/gapfilling.py` & `fedot-0.7.2/examples/simple/time_series_forecasting/gapfilling.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/time_series_forecasting/ts_pipelines.py` & `fedot-0.7.2/examples/simple/time_series_forecasting/ts_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/examples/simple/time_series_forecasting/tuning_pipelines.py` & `fedot-0.7.2/examples/simple/time_series_forecasting/tuning_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/api_utils/api_composer.py` & `fedot-0.7.2/fedot/api/api_utils/api_composer.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,21 +142,21 @@
         best_pipeline = best_pipelines[0] if isinstance(best_pipelines, Sequence) else best_pipelines
         return best_pipeline, best_pipeline_candidates, gp_composer
 
     def tune_final_pipeline(self, train_data: InputData, pipeline_gp_composed: Pipeline) -> Pipeline:
         """ Launch tuning procedure for obtained pipeline by composer """
         timeout_for_tuning = abs(self.timer.determine_resources_for_tuning()) / 60
         tuner = (TunerBuilder(self.params.task)
-            .with_tuner(SimultaneousTuner)
-            .with_metric(self.metrics.metric_functions)
-            .with_iterations(DEFAULT_TUNING_ITERATIONS_NUMBER)
-            .with_timeout(datetime.timedelta(minutes=timeout_for_tuning))
-            .with_eval_time_constraint(self.params.composer_requirements.max_graph_fit_time)
-            .with_requirements(self.params.composer_requirements)
-            .build(train_data))
+                 .with_tuner(SimultaneousTuner)
+                 .with_metric(self.metrics.metric_functions)
+                 .with_iterations(DEFAULT_TUNING_ITERATIONS_NUMBER)
+                 .with_timeout(datetime.timedelta(minutes=timeout_for_tuning))
+                 .with_eval_time_constraint(self.params.composer_requirements.max_graph_fit_time)
+                 .with_requirements(self.params.composer_requirements)
+                 .build(train_data))
 
         if self.timer.have_time_for_tuning():
             # Tune all nodes in the pipeline
             with self.timer.launch_tuning():
                 self.was_tuned = False
                 self.log.message(f'Hyperparameters tuning started with {round(timeout_for_tuning)} min. timeout')
                 tuned_pipeline = tuner.tune(pipeline_gp_composed)
```

### Comparing `fedot-0.7.1/fedot/api/api_utils/api_data.py` & `fedot-0.7.2/fedot/api/api_utils/api_data.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/api_utils/api_params_repository.py` & `fedot-0.7.2/fedot/api/api_utils/api_params_repository.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/api_utils/assumptions/assumptions_builder.py` & `fedot-0.7.2/fedot/api/api_utils/assumptions/assumptions_builder.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/api_utils/assumptions/assumptions_handler.py` & `fedot-0.7.2/fedot/api/api_utils/assumptions/assumptions_handler.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/api_utils/assumptions/operations_filter.py` & `fedot-0.7.2/fedot/api/api_utils/assumptions/operations_filter.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/api_utils/assumptions/preprocessing_builder.py` & `fedot-0.7.2/fedot/api/api_utils/assumptions/preprocessing_builder.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/api_utils/assumptions/task_assumptions.py` & `fedot-0.7.2/fedot/api/api_utils/assumptions/task_assumptions.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/api_utils/data_definition.py` & `fedot-0.7.2/fedot/api/api_utils/data_definition.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/api_utils/input_analyser.py` & `fedot-0.7.2/fedot/api/api_utils/input_analyser.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/api_utils/metrics.py` & `fedot-0.7.2/fedot/api/api_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/api_utils/params.py` & `fedot-0.7.2/fedot/api/api_utils/params.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/api_utils/predefined_model.py` & `fedot-0.7.2/fedot/api/api_utils/predefined_model.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/api_utils/presets.py` & `fedot-0.7.2/fedot/api/api_utils/presets.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/fedot_cli.py` & `fedot-0.7.2/fedot/api/fedot_cli.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/help.py` & `fedot-0.7.2/fedot/api/help.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     repository = OperationTypesRepository(operation_type='model')
 
     # Filter operations
     repository_operations_list = _filter_operations_by_type(repository, task)
     search_space = PipelineSearchSpace()
     for model in repository_operations_list:
         if model.id != 'custom':
-            hyperparameters = search_space.get_operation_parameter_range(str(model.id))
+            hyperparameters = search_space.get_parameters_for_operation(str(model.id))
             implementation_info = model.current_strategy(task)(model.id).implementation_info
             info_lst = [
                 f"Model name - '{model.id}'",
                 f"Available hyperparameters to optimize with tuner - {hyperparameters}",
                 f"Strategy implementation - {model.current_strategy(task)}",
                 f"Model implementation - {implementation_info}\n"
             ]
@@ -37,15 +37,15 @@
 
     task = _get_task_by_name(task_name)
 
     repository = OperationTypesRepository(operation_type='data_operation')
     repository_operations_list = _filter_operations_by_type(repository, task)
     search_space = PipelineSearchSpace()
     for operation in repository_operations_list:
-        hyperparameters = search_space.get_operation_parameter_range(str(operation.id))
+        hyperparameters = search_space.get_parameters_for_operation(str(operation.id))
         implementation_info = operation.current_strategy(task)(operation.id).implementation_info
         info_lst = [
             f"Data operation name - '{operation.id}'",
             f"Available hyperparameters to optimize with tuner - {hyperparameters}",
             f"Strategy implementation - {operation.current_strategy(task)}",
             f"Operation implementation - {implementation_info}\n"
         ]
```

### Comparing `fedot-0.7.1/fedot/api/main.py` & `fedot-0.7.2/fedot/api/main.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/api/time.py` & `fedot-0.7.2/fedot/api/time.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/caching/base_cache.py` & `fedot-0.7.2/fedot/core/caching/base_cache.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/caching/base_cache_db.py` & `fedot-0.7.2/fedot/core/caching/base_cache_db.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/caching/pipelines_cache.py` & `fedot-0.7.2/fedot/core/caching/pipelines_cache.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/caching/pipelines_cache_db.py` & `fedot-0.7.2/fedot/core/caching/pipelines_cache_db.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/caching/preprocessing_cache.py` & `fedot-0.7.2/fedot/core/caching/preprocessing_cache.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/caching/preprocessing_cache_db.py` & `fedot-0.7.2/fedot/core/caching/preprocessing_cache_db.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/composer/composer.py` & `fedot-0.7.2/fedot/core/composer/composer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/composer/composer_builder.py` & `fedot-0.7.2/fedot/core/composer/composer_builder.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/composer/gp_composer/gp_composer.py` & `fedot-0.7.2/fedot/core/composer/gp_composer/gp_composer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/composer/gp_composer/specific_operators.py` & `fedot-0.7.2/fedot/core/composer/gp_composer/specific_operators.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/composer/meta_rules.py` & `fedot-0.7.2/fedot/core/composer/meta_rules.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/composer/metrics.py` & `fedot-0.7.2/fedot/core/composer/metrics.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/composer/random_composer.py` & `fedot-0.7.2/fedot/core/composer/random_composer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/constants.py` & `fedot-0.7.2/fedot/core/constants.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/data/array_utilities.py` & `fedot-0.7.2/fedot/core/data/array_utilities.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/data/data.py` & `fedot-0.7.2/fedot/core/data/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import pandas as pd
 from golem.core.log import default_log
 from golem.utilities.requirements_notificator import warn_requirement
 
 try:
     import cv2
 except ModuleNotFoundError:
-    warn_requirement('opencv-python')
+    warn_requirement('opencv-python', 'fedot[extra]')
     cv2 = None
 
 from fedot.core.data.array_utilities import atleast_2d
 from fedot.core.data.load_data import JSONBatchLoader, TextBatchLoader
 from fedot.core.data.supplementary_data import SupplementaryData
 from fedot.core.repository.dataset_types import DataTypesEnum
 from fedot.core.repository.tasks import Task, TaskTypesEnum
```

### Comparing `fedot-0.7.1/fedot/core/data/data_detection.py` & `fedot-0.7.2/fedot/core/data/data_detection.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/data/data_preprocessing.py` & `fedot-0.7.2/fedot/core/data/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/data/data_split.py` & `fedot-0.7.2/fedot/core/data/data_split.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/data/load_data.py` & `fedot-0.7.2/fedot/core/data/load_data.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/data/merge/data_merger.py` & `fedot-0.7.2/fedot/core/data/merge/data_merger.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/data/merge/supplementary_data_merger.py` & `fedot-0.7.2/fedot/core/data/merge/supplementary_data_merger.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/data/multi_modal.py` & `fedot-0.7.2/fedot/core/data/multi_modal.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/data/supplementary_data.py` & `fedot-0.7.2/fedot/core/data/supplementary_data.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/data/visualisation.py` & `fedot-0.7.2/fedot/core/data/visualisation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/atomized_model.py` & `fedot-0.7.2/fedot/core/operations/atomized_model.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/atomized_template.py` & `fedot-0.7.2/fedot/core/operations/atomized_template.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/data_operation.py` & `fedot-0.7.2/fedot/core/operations/data_operation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/automl.py` & `fedot-0.7.2/fedot/core/operations/evaluation/automl.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/classification.py` & `fedot-0.7.2/fedot/core/operations/evaluation/classification.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/clustering.py` & `fedot-0.7.2/fedot/core/operations/evaluation/clustering.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/common_preprocessing.py` & `fedot-0.7.2/fedot/core/operations/evaluation/common_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/custom.py` & `fedot-0.7.2/fedot/core/operations/evaluation/custom.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/data_source.py` & `fedot-0.7.2/fedot/core/operations/evaluation/data_source.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/evaluation_interfaces.py` & `fedot-0.7.2/fedot/core/operations/evaluation/evaluation_interfaces.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/gpu/classification.py` & `fedot-0.7.2/fedot/core/operations/evaluation/gpu/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import warnings
 
 from golem.utilities.requirements_notificator import warn_requirement
 
 try:
     import cudf
 except ModuleNotFoundError:
-    warn_requirement('cudf')
+    warn_requirement('cudf', 'cudf')
     cudf = None
 
 from fedot.core.data.data import InputData, OutputData
 from fedot.core.operations.evaluation.gpu.common import CuMLEvaluationStrategy
 
 warnings.filterwarnings("ignore", category=UserWarning)
```

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/gpu/clustering.py` & `fedot-0.7.2/fedot/core/operations/evaluation/gpu/clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from fedot.core.operations.operation_parameters import OperationParameters
 
 try:
     from cuml import KMeans
     import cudf
 except ModuleNotFoundError:
-    warn_requirement('cudf / cuml')
+    warn_requirement('cudf / cuml', 'cudf / cuml')
     cudf = None
     KMeans = None
 
 from typing import Optional
 
 from fedot.core.data.data import InputData, OutputData
```

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/gpu/common.py` & `fedot-0.7.2/fedot/core/operations/evaluation/gpu/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     from cuml.ensemble import RandomForestClassifier, RandomForestRegressor
     from cuml.svm import SVC
     from cuml.neighbors import KNeighborsClassifier as CuMlknnClassifier, \
         KNeighborsRegressor as CuMlknnRegressor
     from cuml import LinearRegression as CuMlLinReg, SGD as CuMlSGD, \
         MultinomialNB as CuMlMultinomialNB
 except ModuleNotFoundError:
-    warn_requirement('cudf / cuml')
+    warn_requirement('cudf / cuml', 'cudf / cuml')
     cudf = None
     cuml = None
 
 from fedot.core.data.data import InputData, OutputData
 from fedot.core.operations.evaluation.evaluation_interfaces import SkLearnEvaluationStrategy
 from fedot.core.repository.operation_types_repository import OperationTypesRepository
 from fedot.core.repository.tasks import TaskTypesEnum
```

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/gpu/regression.py` & `fedot-0.7.2/fedot/core/operations/evaluation/gpu/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from golem.utilities.requirements_notificator import warn_requirement
 
 try:
     import cudf
 except ModuleNotFoundError:
-    warn_requirement('cudf')
+    warn_requirement('cudf', 'cudf / cuml')
     cudf = None
 
 from fedot.core.data.data import InputData, OutputData
 from fedot.core.operations.evaluation.gpu.common import CuMLEvaluationStrategy
 
 
 class CuMLRegressionStrategy(CuMLEvaluationStrategy):
```

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/categorical_encoders.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/decompose.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/decompose.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_filters.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_filters.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_imbalanced_class.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_imbalanced_class.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_selectors.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_selectors.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_transformations.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_transformations.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/text_preprocessing.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/text_preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from fedot.core.data.data import InputData, OutputData
 from fedot.core.operations.operation_parameters import OperationParameters
 
 try:
     import nltk
 except ModuleNotFoundError:
-    warn_requirement('nltk')
+    warn_requirement('nltk', 'fedot[extra]')
     nltk = None
 
 from fedot.core.operations.evaluation.operation_implementations.implementation_interfaces import (
     DataOperationImplementation
 )
 from fedot.core.repository.dataset_types import DataTypesEnum
```

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/text_pretrained.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/text_pretrained.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from fedot.core.operations.operation_parameters import OperationParameters
 from fedot.core.repository.dataset_types import DataTypesEnum
 
 try:
     import gensim.downloader as api
     from gensim.models import KeyedVectors
 except ModuleNotFoundError:
-    warn_requirement('gensim')
+    warn_requirement('gensim', 'fedot[extra]')
     api = None
     KeyedVectors = None
 
 
 class PretrainedEmbeddingsImplementation(DataOperationImplementation):
     """ Class for text vectorization by pretrained embeddings
     model_name can be selected from https://github.com/RaRe-Technologies/gensim-data"""
```

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/ts_transformations.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/data_operations/ts_transformations.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/implementation_interfaces.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/implementation_interfaces.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/custom_model.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/discriminant_analysis.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/discriminant_analysis.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/keras.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/keras.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from golem.utilities.requirements_notificator import warn_requirement
 
 from fedot.core.operations.operation_parameters import OperationParameters
 
 try:
     import tensorflow as tf
 except ModuleNotFoundError:
-    warn_requirement('tensorflow')
+    warn_requirement('tensorflow', 'fedot[extra]')
     tf = None
 
 from fedot.core.data.data import InputData, OutputData
 from golem.core.log import LoggerAdapter, default_log
 from fedot.core.operations.evaluation.operation_implementations.implementation_interfaces import ModelImplementation
 from sklearn import preprocessing
```

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/knn.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/knn.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/svc.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/svc.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/arima.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/arima.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/cgru.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/cgru.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 try:
     import torch
     import torch.nn as nn
 
     from torch.optim.lr_scheduler import MultiStepLR
     from torch.utils.data import DataLoader, TensorDataset
 except ModuleNotFoundError:
-    warn_requirement('torch')
+    warn_requirement('torch', 'fedot[extra]')
     torch = object()
     nn = TorchMock
 
 
 class CGRUImplementation(ModelImplementation):
     def __init__(self, params: OperationParameters):
         super().__init__(params)
```

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/naive.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/naive.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/poly.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/poly.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/statsmodels.py` & `fedot-0.7.2/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/statsmodels.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/regression.py` & `fedot-0.7.2/fedot/core/operations/evaluation/regression.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/text.py` & `fedot-0.7.2/fedot/core/operations/evaluation/text.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/evaluation/time_series.py` & `fedot-0.7.2/fedot/core/operations/evaluation/time_series.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/factory.py` & `fedot-0.7.2/fedot/core/operations/factory.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/hyperparameters_preprocessing.py` & `fedot-0.7.2/fedot/core/operations/hyperparameters_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/model.py` & `fedot-0.7.2/fedot/core/operations/model.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/operation.py` & `fedot-0.7.2/fedot/core/operations/operation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/operation_parameters.py` & `fedot-0.7.2/fedot/core/operations/operation_parameters.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/operations/operation_template.py` & `fedot-0.7.2/fedot/core/operations/operation_template.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/optimisers/objective/data_objective_advisor.py` & `fedot-0.7.2/fedot/core/optimisers/objective/data_objective_advisor.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/optimisers/objective/data_objective_eval.py` & `fedot-0.7.2/fedot/core/optimisers/objective/data_objective_eval.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/optimisers/objective/data_source_splitter.py` & `fedot-0.7.2/fedot/core/optimisers/objective/data_source_splitter.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/optimisers/objective/metrics_objective.py` & `fedot-0.7.2/fedot/core/optimisers/objective/metrics_objective.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/optimisers/objective/objective_serialization.py` & `fedot-0.7.2/fedot/core/optimisers/objective/objective_serialization.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/pipelines/adapters.py` & `fedot-0.7.2/fedot/core/pipelines/adapters.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/pipelines/automl_wrappers.py` & `fedot-0.7.2/fedot/core/pipelines/automl_wrappers.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/pipelines/node.py` & `fedot-0.7.2/fedot/core/pipelines/node.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/pipelines/pipeline.py` & `fedot-0.7.2/fedot/core/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/pipelines/pipeline_advisor.py` & `fedot-0.7.2/fedot/core/pipelines/pipeline_advisor.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/pipelines/pipeline_composer_requirements.py` & `fedot-0.7.2/fedot/core/pipelines/pipeline_composer_requirements.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/pipelines/pipeline_graph_generation_params.py` & `fedot-0.7.2/fedot/core/pipelines/pipeline_graph_generation_params.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/pipelines/pipeline_node_factory.py` & `fedot-0.7.2/fedot/core/pipelines/pipeline_node_factory.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/pipelines/random_pipeline_factory.py` & `fedot-0.7.2/fedot/core/pipelines/random_pipeline_factory.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/pipelines/template.py` & `fedot-0.7.2/fedot/core/pipelines/template.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/pipelines/ts_wrappers.py` & `fedot-0.7.2/fedot/core/pipelines/ts_wrappers.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/pipelines/tuning/hyperparams.py` & `fedot-0.7.2/fedot/core/pipelines/tuning/hyperparams.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import random
 
 from golem.core.log import default_log
+from golem.core.tuning.hyperopt_tuner import get_parameter_hyperopt_space
 from hyperopt.pyll.stochastic import sample as hp_sample
 
 from fedot.core.pipelines.tuning.search_space import PipelineSearchSpace
 
 
 class ParametersChanger:
     """
@@ -19,17 +20,17 @@
         self.current_params = current_params
         self.logger = default_log(prefix='ParametersChangerLog')
 
     def get_new_operation_params(self):
         """ Function return a dictionary with new parameters values """
 
         # Get available parameters for operation
-        params_list = PipelineSearchSpace().get_operation_parameter_range(self.operation_name)
+        params_list = PipelineSearchSpace().get_parameters_for_operation(self.operation_name)
 
-        if params_list is None:
+        if not params_list:
             params_dict = None
         else:
             # Get new values for all parameters
             params_dict = self.new_params_dict(params_list)
 
         return params_dict
 
@@ -62,35 +63,30 @@
 
             param_value = func(parameter_name, **parameters)
             params_dict.update(param_value)
 
         return params_dict
 
     def _get_current_parameter_value(self, parameter_name):
-
-        if isinstance(self.current_params, str):
-            # TODO 'default_params' - need to process
+        try:
+            current_value = self.current_params.get(parameter_name)
+        except Exception as exec:
+            self.logger.warning(f'The following error occurred during the hyperparameter configuration.{exec}')
             current_value = None
-        else:
-            # Dictionary with parameters
-            try:
-                current_value = self.current_params.get(parameter_name)
-            except Exception as exec:
-                self.logger.warning(f'The following error occurred during the hyperparameter configuration.{exec}')
-                current_value = None
 
         return current_value
 
     @staticmethod
     def _random_change(parameter_name, **kwargs):
         """ Randomly selects a parameter value from a specified range """
 
-        space = PipelineSearchSpace().get_operation_parameter_range(operation_name=kwargs['operation_name'],
-                                                                    parameter_name=parameter_name,
-                                                                    label=parameter_name)
+        space = get_parameter_hyperopt_space(PipelineSearchSpace(),
+                                             operation_name=kwargs['operation_name'],
+                                             parameter_name=parameter_name,
+                                             label=parameter_name)
         # Randomly choose new value
         new_value = hp_sample(space)
         return {parameter_name: new_value}
 
     @staticmethod
     def _incremental_change(parameter_name, **kwargs):
         """ Next to the current value, the normally distributed new value is set aside """
```

### Comparing `fedot-0.7.1/fedot/core/pipelines/tuning/tuner_builder.py` & `fedot-0.7.2/fedot/core/pipelines/tuning/tuner_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from datetime import timedelta
-from typing import Callable, Type, Union
+from typing import Type, Union
 
 from golem.core.tuning.simultaneous import SimultaneousTuner
-from golem.core.tuning.tuner_interface import HyperoptTuner
-from hyperopt import tpe
+from golem.core.tuning.tuner_interface import BaseTuner
 
 from fedot.core.constants import DEFAULT_TUNING_ITERATIONS_NUMBER
 from fedot.core.data.data import InputData
 from fedot.core.optimisers.objective import PipelineObjectiveEvaluate
 from fedot.core.optimisers.objective.data_source_splitter import DataSourceSplitter
 from fedot.core.optimisers.objective.metrics_objective import MetricsObjective
 from fedot.core.pipelines.adapters import PipelineAdapter
@@ -25,19 +24,19 @@
         self.validation_blocks = None
         self.n_jobs = -1
         self.metric: MetricsEnum = MetricByTask.get_default_quality_metrics(task.task_type)[0]
         self.iterations = DEFAULT_TUNING_ITERATIONS_NUMBER
         self.early_stopping_rounds = None
         self.timeout = timedelta(minutes=5)
         self.search_space = PipelineSearchSpace()
-        self.algo = tpe.suggest
         self.eval_time_constraint = None
+        self.additional_params = {}
         self.adapter = PipelineAdapter()
 
-    def with_tuner(self, tuner: Type[HyperoptTuner]):
+    def with_tuner(self, tuner: Type[BaseTuner]):
         self.tuner_class = tuner
         return self
 
     def with_requirements(self, requirements: PipelineComposerRequirements):
         self.cv_folds = requirements.cv_folds
         self.validation_blocks = requirements.validation_blocks
         self.n_jobs = requirements.n_jobs
@@ -81,31 +80,31 @@
         self.eval_time_constraint = eval_time_constraint
         return self
 
     def with_search_space(self, search_space: PipelineSearchSpace):
         self.search_space = search_space
         return self
 
-    def with_algo(self, algo: Callable):
-        self.algo = algo
-        return self
-
     def with_adapter(self, adapter):
         self.adapter = adapter
         return self
 
-    def build(self, data: InputData) -> HyperoptTuner:
+    def with_additional_params(self, **parameters):
+        self.additional_params = parameters
+        return self
+
+    def build(self, data: InputData) -> BaseTuner:
         objective = MetricsObjective(self.metric)
         data_producer = DataSourceSplitter(self.cv_folds, self.validation_blocks).build(data)
         objective_evaluate = PipelineObjectiveEvaluate(objective, data_producer,
                                                        validation_blocks=self.validation_blocks,
                                                        time_constraint=self.eval_time_constraint,
                                                        eval_n_jobs=self.n_jobs)  # because tuners are not parallelized
         tuner = self.tuner_class(objective_evaluate=objective_evaluate,
                                  adapter=self.adapter,
                                  iterations=self.iterations,
                                  early_stopping_rounds=self.early_stopping_rounds,
                                  timeout=self.timeout,
                                  search_space=self.search_space,
-                                 algo=self.algo,
-                                 n_jobs=self.n_jobs)
+                                 n_jobs=self.n_jobs,
+                                 **self.additional_params)
         return tuner
```

### Comparing `fedot-0.7.1/fedot/core/pipelines/verification.py` & `fedot-0.7.2/fedot/core/pipelines/verification.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/pipelines/verification_rules.py` & `fedot-0.7.2/fedot/core/pipelines/verification_rules.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/repository/data/automl_repository.json` & `fedot-0.7.2/fedot/core/repository/data/automl_repository.json`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/repository/data/data_operation_repository.json` & `fedot-0.7.2/fedot/core/repository/data/data_operation_repository.json`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/repository/data/default_operation_params.json` & `fedot-0.7.2/fedot/core/repository/data/default_operation_params.json`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/repository/data/gpu_models_repository.json` & `fedot-0.7.2/fedot/core/repository/data/gpu_models_repository.json`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/repository/data/model_repository.json` & `fedot-0.7.2/fedot/core/repository/data/model_repository.json`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/repository/dataset_types.py` & `fedot-0.7.2/fedot/core/repository/dataset_types.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/repository/default_params_repository.py` & `fedot-0.7.2/fedot/core/repository/default_params_repository.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/repository/json_evaluation.py` & `fedot-0.7.2/fedot/core/repository/json_evaluation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/repository/operation_types_repository.py` & `fedot-0.7.2/fedot/core/repository/operation_types_repository.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/repository/pipeline_operation_repository.py` & `fedot-0.7.2/fedot/core/repository/pipeline_operation_repository.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/repository/quality_metrics_repository.py` & `fedot-0.7.2/fedot/core/repository/quality_metrics_repository.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/repository/tasks.py` & `fedot-0.7.2/fedot/core/repository/tasks.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/validation/split.py` & `fedot-0.7.2/fedot/core/validation/split.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/core/visualisation/pipeline_specific_visuals.py` & `fedot-0.7.2/fedot/core/visualisation/pipeline_specific_visuals.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/explainability/explainers.py` & `fedot-0.7.2/fedot/explainability/explainers.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/explainability/surrogate_explainer.py` & `fedot-0.7.2/fedot/explainability/surrogate_explainer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/preprocessing/base_preprocessing.py` & `fedot-0.7.2/fedot/preprocessing/base_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/preprocessing/categorical.py` & `fedot-0.7.2/fedot/preprocessing/categorical.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/preprocessing/data_type_check.py` & `fedot-0.7.2/fedot/preprocessing/data_type_check.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/preprocessing/data_types.py` & `fedot-0.7.2/fedot/preprocessing/data_types.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/preprocessing/dummy_preprocessing.py` & `fedot-0.7.2/fedot/preprocessing/dummy_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/preprocessing/preprocessing.py` & `fedot-0.7.2/fedot/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/preprocessing/structure.py` & `fedot-0.7.2/fedot/preprocessing/structure.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/remote/infrastructure/clients/client.py` & `fedot-0.7.2/fedot/remote/infrastructure/clients/client.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/remote/infrastructure/clients/datamall_client.py` & `fedot-0.7.2/fedot/remote/infrastructure/clients/datamall_client.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/remote/infrastructure/clients/test_client.py` & `fedot-0.7.2/fedot/remote/infrastructure/clients/test_client.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/remote/pipeline_run_config.py` & `fedot-0.7.2/fedot/remote/pipeline_run_config.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/remote/remote_evaluator.py` & `fedot-0.7.2/fedot/remote/remote_evaluator.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/remote/run_pipeline.py` & `fedot-0.7.2/fedot/remote/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/sensitivity/deletion_methods/multi_times_analysis.py` & `fedot-0.7.2/fedot/sensitivity/deletion_methods/multi_times_analysis.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/sensitivity/node_sa_approaches.py` & `fedot-0.7.2/fedot/sensitivity/node_sa_approaches.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/sensitivity/nodes_sensitivity.py` & `fedot-0.7.2/fedot/sensitivity/nodes_sensitivity.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/multi_operations_sensitivity.py` & `fedot-0.7.2/fedot/sensitivity/operations_hp_sensitivity/multi_operations_sensitivity.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/one_operation_sensitivity.py` & `fedot-0.7.2/fedot/sensitivity/operations_hp_sensitivity/one_operation_sensitivity.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/problem.py` & `fedot-0.7.2/fedot/sensitivity/operations_hp_sensitivity/problem.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/sa_and_sample_methods.py` & `fedot-0.7.2/fedot/sensitivity/operations_hp_sensitivity/sa_and_sample_methods.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/sensitivity/pipeline_sensitivity.py` & `fedot-0.7.2/fedot/sensitivity/pipeline_sensitivity.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/sensitivity/pipeline_sensitivity_facade.py` & `fedot-0.7.2/fedot/sensitivity/pipeline_sensitivity_facade.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/sensitivity/sa_requirements.py` & `fedot-0.7.2/fedot/sensitivity/sa_requirements.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/utilities/debug.py` & `fedot-0.7.2/fedot/utilities/debug.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/utilities/define_metric_by_task.py` & `fedot-0.7.2/fedot/utilities/define_metric_by_task.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/utilities/golem_imports_transition.py` & `fedot-0.7.2/fedot/utilities/golem_imports_transition.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/utilities/memory.py` & `fedot-0.7.2/fedot/utilities/memory.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/utilities/project_import_export.py` & `fedot-0.7.2/fedot/utilities/project_import_export.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/utilities/synth_dataset_generator.py` & `fedot-0.7.2/fedot/utilities/synth_dataset_generator.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot/utilities/ts_gapfilling.py` & `fedot-0.7.2/fedot/utilities/ts_gapfilling.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.1/fedot.egg-info/PKG-INFO` & `fedot-0.7.2/fedot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedot
-Version: 0.7.1
+Version: 0.7.2
 Summary: Automated machine learning framework for composite pipelines
 Home-page: https://github.com/aimclub/FEDOT
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
@@ -196,22 +196,17 @@
 
 Current R&D and future plans
 ============================
 
 Currently, we are working on new features and trying to improve the performance and the user experience of FEDOT.
 The major ongoing tasks and plans:
 
-* Effective and ready-to-use pipeline templates for certain tasks and data types;
-* Integration with GPU via Rapids framework;
-* Alternative optimization methods of fixed-shaped pipelines;
-* Integration with MLFlow for import and export of the pipelines;
-* Improvement of the high-level API.
-
-
-Also, we are doing several research tasks related to AutoML time-series benchmarking and multi-modal modeling.
+* Implementation of meta-learning based at GNN and RL (see `MetaFEDOT <https://github.com/ITMO-NSS-team/MetaFEDOT>`__)
+* Improvement of the optimisation-related algorithms implemented in `GOLEM <https://github.com/aimclub/GOLEM/>`__.
+* Support for more complicated pipeline design patters, especially for time series forecasting.
 
 Any contribution is welcome. Our R&D team is open for cooperation with other scientific teams as well as with industrial partners.
 
 Documentation
 =============
 
 Also, a detailed FEDOT API description is available in `Read the Docs <https://fedot.readthedocs.io/en/latest/>`__.
@@ -224,16 +219,17 @@
 Acknowledgments
 ===============
 
 We acknowledge the contributors for their important impact and the participants of numerous scientific conferences and workshops for their valuable advice and suggestions.
 
 Side Projects
 =============
+- The optimisation core implemented in `GOLEM <https://github.com/aimclub/GOLEM/>`__ repository.
 - The prototype of the web-GUI for FEDOT is available in the `FEDOT.WEB <https://github.com/aimclub/FEDOT.Web>`__ repository.
-
+- The prototype of FEDOT-based meta-AutoML in the `MetaFEDOT <https://github.com/ITMO-NSS-team/MetaFEDOT>`__ repository.
 
 Contacts
 ========
 - `Telegram channel for solving problems and answering questions about FEDOT <https://t.me/FEDOT_helpdesk>`_
 - `Natural System Simulation Team <https://itmo-nss-team.github.io/>`_
 - `Anna Kalyuzhnaya <https://scholar.google.com/citations?user=bjiILqcAAAAJ&hl=ru>`_, Team leader (anna.kalyuzhnaya@itmo.ru)
 - `Newsfeed <https://t.me/NSS_group>`_
```

### Comparing `fedot-0.7.1/fedot.egg-info/SOURCES.txt` & `fedot-0.7.2/fedot.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 examples/advanced/time_series_forecasting/sparse_lagged_tuning.py
 examples/simple/__init__.py
 examples/simple/multitask_classification_regression_api.py
 examples/simple/pipeline_and_history_visualization.py
 examples/simple/pipeline_import_export.py
 examples/simple/pipeline_log.py
 examples/simple/pipeline_tune.py
+examples/simple/pipeline_tuning_with_iopt.py
 examples/simple/pipeline_visualization.py
 examples/simple/classification/__init__.py
 examples/simple/classification/api_classification.py
 examples/simple/classification/classification_pipelines.py
 examples/simple/classification/classification_with_tuning.py
 examples/simple/classification/image_classification_problem.py
 examples/simple/classification/multiclass_prediction.py
@@ -82,14 +83,15 @@
 examples/simple/time_series_forecasting/api_forecasting.py
 examples/simple/time_series_forecasting/cgru.py
 examples/simple/time_series_forecasting/fitted_values.py
 examples/simple/time_series_forecasting/gapfilling.py
 examples/simple/time_series_forecasting/ts_pipelines.py
 examples/simple/time_series_forecasting/tuning_pipelines.py
 fedot/__init__.py
+fedot/version.py
 fedot.egg-info/PKG-INFO
 fedot.egg-info/SOURCES.txt
 fedot.egg-info/dependency_links.txt
 fedot.egg-info/requires.txt
 fedot.egg-info/top_level.txt
 fedot/api/__init__.py
 fedot/api/fedot_cli.py
```

### Comparing `fedot-0.7.1/fedot.egg-info/requires.txt` & `fedot-0.7.2/fedot.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-thegolem==0.3.1
+thegolem==0.3.2
 numpy!=1.24.0,>=1.16.0
 anytree>=2.8.0
 catboost>=0.25.0
 lightgbm>=3.0.0
 xgboost>=1.4.0
 statsmodels>=0.12.0
 ete3>=3.1.0
@@ -36,15 +36,14 @@
 [examples]
 tpot==0.11.7
 h2o==3.28.1.2
 openpyxl==3.0.7
 
 [extra]
 torch>=1.9.0
-imageio<=2.10,>=2.8
 opencv-python>=4.5.5.64
 Pillow>=8.2.0
 gensim>=4.1.2
 nltk>=3.5
 protobuf~=3.19.0
 
 [extra:python_version >= "3.8"]
```

### Comparing `fedot-0.7.1/setup.py` & `fedot-0.7.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 import setuptools
 
 # The directory containing this file
 HERE = Path(__file__).parent.resolve()
 
 # The text of the README file
 NAME = 'fedot'
-VERSION = '0.7.1'
+
+version_info = {}
+with open('./fedot/version.py') as fp:
+    exec(fp.read(), version_info)
+VERSION = version_info['__version__']
+
 AUTHOR = 'NSS Lab'
 SHORT_DESCRIPTION = 'Automated machine learning framework for composite pipelines'
 README = Path(HERE, 'README_en.rst').read_text(encoding='utf-8')
 URL = 'https://github.com/aimclub/FEDOT'
 REQUIRES_PYTHON = '>=3.8'
 LICENSE = 'BSD 3-Clause'
```

### Comparing `fedot-0.7.1/test/test_gpu_strategy.py` & `fedot-0.7.2/test/test_gpu_strategy.py`

 * *Files identical despite different names*

