# Comparing `tmp/mlfoundry-0.9.2.tar.gz` & `tmp/mlfoundry-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfoundry-0.9.2.tar", max compression
+gzip compressed data, was "mlfoundry-0.9.3.tar", max compression
```

## Comparing `mlfoundry-0.9.2.tar` & `mlfoundry-0.9.3.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0     3165 2023-07-05 12:46:31.848489 mlfoundry-0.9.2/README.md
--rw-r--r--   0        0        0      941 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/__init__.py
--rw-r--r--   0        0        0     1211 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/__main__.py
--rw-r--r--   0        0        0     3713 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/amplitude.py
--rw-r--r--   0        0        0        0 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/artifact/__init__.py
--rw-r--r--   0        0        0    29009 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/artifact/truefoundry_artifact_repo.py
--rw-r--r--   0        0        0        0 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/background/__init__.py
--rw-r--r--   0        0        0      287 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/background/events.py
--rw-r--r--   0        0        0     3032 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/background/interface.py
--rw-r--r--   0        0        0     4016 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/background/sender.py
--rw-r--r--   0        0        0     8756 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/background/system_metrics.py
--rw-r--r--   0        0        0     4028 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/background/utils.py
--rw-r--r--   0        0        0        0 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/cli/__init__.py
--rw-r--r--   0        0        0      918 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/cli/cli_interface.py
--rw-r--r--   0        0        0      100 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1840 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/cli/commands/download.py
--rw-r--r--   0        0        0      813 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/cli/commands/login.py
--rw-r--r--   0        0        0     2768 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/constants.py
--rw-r--r--   0        0        0     1392 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/enums.py
--rw-r--r--   0        0        0      383 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/env_vars.py
--rw-r--r--   0        0        0      365 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/exceptions.py
--rw-r--r--   0        0        0     2037 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/__init__.py
--rw-r--r--   0        0        0      301 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/base_registry.py
--rw-r--r--   0        0        0      718 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/fastai_registry.py
--rw-r--r--   0        0        0      892 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/gluon_registry.py
--rw-r--r--   0        0        0      700 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/h2o_registry.py
--rw-r--r--   0        0        0      712 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/keras_registry.py
--rw-r--r--   0        0        0      730 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/lightgbm_registry.py
--rw-r--r--   0        0        0      706 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/onnx_registry.py
--rw-r--r--   0        0        0      775 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/paddle_registry.py
--rw-r--r--   0        0        0      744 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/pytorch_registry.py
--rw-r--r--   0        0        0      724 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/sklearn_registry.py
--rw-r--r--   0        0        0      712 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/spacy_registry.py
--rw-r--r--   0        0        0      748 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/statsmodel_registry.py
--rw-r--r--   0        0        0     3077 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/tensorflow_registry.py
--rw-r--r--   0        0        0      774 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/transformers_registry.py
--rw-r--r--   0        0        0      724 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/xgboost_registry.py
--rw-r--r--   0        0        0     2349 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/git_info.py
--rw-r--r--   0        0        0        0 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/integrations/__init__.py
--rw-r--r--   0        0        0    15423 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/integrations/lightning.py
--rw-r--r--   0        0        0    22410 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/integrations/transformers.py
--rw-r--r--   0        0        0     1785 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/internal_namespace.py
--rw-r--r--   0        0        0      153 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/__init__.py
--rw-r--r--   0        0        0     8173 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/artifacts/artifact.py
--rw-r--r--   0        0        0     1019 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/artifacts/constants.py
--rw-r--r--   0        0        0     3072 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/artifacts/general_artifact.py
--rw-r--r--   0        0        0    15463 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/artifacts/model.py
--rw-r--r--   0        0        0     5952 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/artifacts/utils.py
--rw-r--r--   0        0        0       50 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/image/__init__.py
--rw-r--r--   0        0        0      255 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/image/constants.py
--rw-r--r--   0        0        0    11446 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/image/image.py
--rw-r--r--   0        0        0     2767 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/image/image_normalizer.py
--rw-r--r--   0        0        0     1566 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/image/types.py
--rw-r--r--   0        0        0      271 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/model_artifact.py
--rw-r--r--   0        0        0     7125 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/plot.py
--rw-r--r--   0        0        0     2486 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/pydantic_base.py
--rw-r--r--   0        0        0     1332 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/utils.py
--rw-r--r--   0        0        0      453 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/logger.py
--rw-r--r--   0        0        0     9286 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/login.py
--rw-r--r--   0        0        0        0 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/__init__.py
--rw-r--r--   0        0        0     1065 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v1/__init__.py
--rw-r--r--   0        0        0     2080 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v1/base_metrics.py
--rw-r--r--   0        0        0     6852 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v1/binary_classification_metrics.py
--rw-r--r--   0        0        0     6736 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v1/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     4419 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v1/regression_metrics.py
--rw-r--r--   0        0        0     3976 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v1/timeseries_metrics.py
--rw-r--r--   0        0        0     1026 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v2/__init__.py
--rw-r--r--   0        0        0     1898 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v2/base_metrics.py
--rw-r--r--   0        0        0      566 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v2/custom_metric_types.py
--rw-r--r--   0        0        0     6192 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v2/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     2718 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v2/regression_metrics.py
--rw-r--r--   0        0        0     2251 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v2/timeseries_metrics.py
--rw-r--r--   0        0        0      295 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v2/utils.py
--rw-r--r--   0        0        0    45880 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/mlfoundry_api.py
--rw-r--r--   0        0        0    47398 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/mlfoundry_run.py
--rw-r--r--   0        0        0        0 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/__init__.py
--rw-r--r--   0        0        0     1994 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/entities.py
--rw-r--r--   0        0        0       63 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/store/__init__.py
--rw-r--r--   0        0        0     6630 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/store/client.py
--rw-r--r--   0        0        0      169 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/store/constants.py
--rw-r--r--   0        0        0      336 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/store/repositories/__init__.py
--rw-r--r--   0        0        0     1351 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/store/repositories/dto.py
--rw-r--r--   0        0        0     6529 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
--rw-r--r--   0        0        0     2178 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/store/worker.py
--rw-r--r--   0        0        0     4468 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/run_utils.py
--rw-r--r--   0        0        0    10048 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/session.py
--rw-r--r--   0        0        0        0 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/tracking/__init__.py
--rw-r--r--   0        0        0     2766 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/tracking/auth_service.py
--rw-r--r--   0        0        0     2629 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/tracking/entities.py
--rw-r--r--   0        0        0     1175 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/tracking/servicefoundry_service.py
--rw-r--r--   0        0        0     4308 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/tracking/truefoundry_rest_store.py
--rw-r--r--   0        0        0        0 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/vendor/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/vendor/pynvml/__init__.py
--rw-r--r--   0        0        0    56147 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/vendor/pynvml/pynvml.py
--rw-r--r--   0        0        0      253 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/version.py
--rw-r--r--   0        0        0        0 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/webapp/__init__.py
--rw-r--r--   0        0        0       38 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/webapp/inputs.py
--rw-r--r--   0        0        0       39 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/webapp/outputs.py
--rw-r--r--   0        0        0     3304 2023-07-05 12:46:43.128831 mlfoundry-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 mlfoundry-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     3165 2023-07-25 10:01:39.305001 mlfoundry-0.9.3/README.md
+-rw-r--r--   0        0        0      941 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/__init__.py
+-rw-r--r--   0        0        0     1211 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/__main__.py
+-rw-r--r--   0        0        0     3713 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/amplitude.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/artifact/__init__.py
+-rw-r--r--   0        0        0    29009 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/artifact/truefoundry_artifact_repo.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/background/__init__.py
+-rw-r--r--   0        0        0      287 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/background/events.py
+-rw-r--r--   0        0        0     3032 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/background/interface.py
+-rw-r--r--   0        0        0     4016 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/background/sender.py
+-rw-r--r--   0        0        0     8756 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/background/system_metrics.py
+-rw-r--r--   0        0        0     4028 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/background/utils.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/cli/__init__.py
+-rw-r--r--   0        0        0      918 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/cli/cli_interface.py
+-rw-r--r--   0        0        0      100 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1840 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/cli/commands/download.py
+-rw-r--r--   0        0        0      814 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/cli/commands/login.py
+-rw-r--r--   0        0        0     2768 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/constants.py
+-rw-r--r--   0        0        0     1392 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/enums.py
+-rw-r--r--   0        0        0      384 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/env_vars.py
+-rw-r--r--   0        0        0      365 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/exceptions.py
+-rw-r--r--   0        0        0     2037 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/__init__.py
+-rw-r--r--   0        0        0      301 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/base_registry.py
+-rw-r--r--   0        0        0      718 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/fastai_registry.py
+-rw-r--r--   0        0        0      892 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/gluon_registry.py
+-rw-r--r--   0        0        0      700 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/h2o_registry.py
+-rw-r--r--   0        0        0      712 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/keras_registry.py
+-rw-r--r--   0        0        0      730 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/lightgbm_registry.py
+-rw-r--r--   0        0        0      706 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/onnx_registry.py
+-rw-r--r--   0        0        0      775 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/paddle_registry.py
+-rw-r--r--   0        0        0      744 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/pytorch_registry.py
+-rw-r--r--   0        0        0      724 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/sklearn_registry.py
+-rw-r--r--   0        0        0      712 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/spacy_registry.py
+-rw-r--r--   0        0        0      748 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/statsmodel_registry.py
+-rw-r--r--   0        0        0     3077 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/tensorflow_registry.py
+-rw-r--r--   0        0        0      774 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/transformers_registry.py
+-rw-r--r--   0        0        0      724 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/frameworks/xgboost_registry.py
+-rw-r--r--   0        0        0     2349 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/git_info.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/integrations/__init__.py
+-rw-r--r--   0        0        0    15423 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/integrations/lightning.py
+-rw-r--r--   0        0        0    22410 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/integrations/transformers.py
+-rw-r--r--   0        0        0     1785 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/internal_namespace.py
+-rw-r--r--   0        0        0      153 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/__init__.py
+-rw-r--r--   0        0        0    12820 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/artifacts/artifact.py
+-rw-r--r--   0        0        0     1019 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/artifacts/constants.py
+-rw-r--r--   0        0        0     3072 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/artifacts/general_artifact.py
+-rw-r--r--   0        0        0    20095 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/artifacts/model.py
+-rw-r--r--   0        0        0     5952 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/artifacts/utils.py
+-rw-r--r--   0        0        0       50 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/image/__init__.py
+-rw-r--r--   0        0        0      255 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/image/constants.py
+-rw-r--r--   0        0        0    11446 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/image/image.py
+-rw-r--r--   0        0        0     2767 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/image/image_normalizer.py
+-rw-r--r--   0        0        0     1566 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/image/types.py
+-rw-r--r--   0        0        0      271 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/model_artifact.py
+-rw-r--r--   0        0        0     7125 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/plot.py
+-rw-r--r--   0        0        0     2486 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/pydantic_base.py
+-rw-r--r--   0        0        0     1332 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/log_types/utils.py
+-rw-r--r--   0        0        0      453 2023-07-25 10:01:39.325003 mlfoundry-0.9.3/mlfoundry/logger.py
+-rw-r--r--   0        0        0     9289 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/login.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/__init__.py
+-rw-r--r--   0        0        0     1065 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v1/__init__.py
+-rw-r--r--   0        0        0     2080 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v1/base_metrics.py
+-rw-r--r--   0        0        0     6852 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v1/binary_classification_metrics.py
+-rw-r--r--   0        0        0     6736 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v1/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     4419 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v1/regression_metrics.py
+-rw-r--r--   0        0        0     3976 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v1/timeseries_metrics.py
+-rw-r--r--   0        0        0     1026 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v2/__init__.py
+-rw-r--r--   0        0        0     1898 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v2/base_metrics.py
+-rw-r--r--   0        0        0      566 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v2/custom_metric_types.py
+-rw-r--r--   0        0        0     6192 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v2/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     2718 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v2/regression_metrics.py
+-rw-r--r--   0        0        0     2251 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v2/timeseries_metrics.py
+-rw-r--r--   0        0        0      295 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/metrics/v2/utils.py
+-rw-r--r--   0        0        0    50297 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/mlfoundry_api.py
+-rw-r--r--   0        0        0    49336 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/mlfoundry_run.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/__init__.py
+-rw-r--r--   0        0        0     1994 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/entities.py
+-rw-r--r--   0        0        0       63 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/store/__init__.py
+-rw-r--r--   0        0        0     6630 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/store/client.py
+-rw-r--r--   0        0        0      169 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/store/constants.py
+-rw-r--r--   0        0        0      336 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/store/repositories/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/store/repositories/dto.py
+-rw-r--r--   0        0        0     6529 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
+-rw-r--r--   0        0        0     2178 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/monitoring/store/worker.py
+-rw-r--r--   0        0        0     4471 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/run_utils.py
+-rw-r--r--   0        0        0    10048 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/session.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/tracking/__init__.py
+-rw-r--r--   0        0        0     2766 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/tracking/auth_service.py
+-rw-r--r--   0        0        0     2629 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/tracking/entities.py
+-rw-r--r--   0        0        0     1175 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/tracking/servicefoundry_service.py
+-rw-r--r--   0        0        0     4308 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/tracking/truefoundry_rest_store.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/vendor/pynvml/__init__.py
+-rw-r--r--   0        0        0    56147 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/vendor/pynvml/pynvml.py
+-rw-r--r--   0        0        0      253 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/version.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/webapp/__init__.py
+-rw-r--r--   0        0        0       38 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/webapp/inputs.py
+-rw-r--r--   0        0        0       39 2023-07-25 10:01:39.329003 mlfoundry-0.9.3/mlfoundry/webapp/outputs.py
+-rw-r--r--   0        0        0     3329 2023-07-25 10:01:53.607149 mlfoundry-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     4664 1970-01-01 00:00:00.000000 mlfoundry-0.9.3/PKG-INFO
```

### Comparing `mlfoundry-0.9.2/README.md` & `mlfoundry-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/__init__.py` & `mlfoundry-0.9.3/mlfoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/__main__.py` & `mlfoundry-0.9.3/mlfoundry/__main__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/amplitude.py` & `mlfoundry-0.9.3/mlfoundry/amplitude.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/artifact/truefoundry_artifact_repo.py` & `mlfoundry-0.9.3/mlfoundry/artifact/truefoundry_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/background/interface.py` & `mlfoundry-0.9.3/mlfoundry/background/interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/background/sender.py` & `mlfoundry-0.9.3/mlfoundry/background/sender.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/background/system_metrics.py` & `mlfoundry-0.9.3/mlfoundry/background/system_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/background/utils.py` & `mlfoundry-0.9.3/mlfoundry/background/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/cli/cli_interface.py` & `mlfoundry-0.9.3/mlfoundry/cli/cli_interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/cli/commands/download.py` & `mlfoundry-0.9.3/mlfoundry/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/cli/commands/login.py` & `mlfoundry-0.9.3/mlfoundry/cli/commands/login.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 @click.command(short_help="Store API key in the local file system")
 @click.option(
     "--tracking_uri",
     "--host",
     "tracking_uri",
     type=str,
     required=True,
-    envvar=env_vars.TRACKING_HOST_GLOBAL,
+    envvar=env_vars._TRACKING_HOST_GLOBAL,
     help="Tracking server host",
 )
 @click.option(
     "--relogin",
     is_flag=True,
     show_default=True,
     default=False,
```

### Comparing `mlfoundry-0.9.2/mlfoundry/constants.py` & `mlfoundry-0.9.3/mlfoundry/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/enums.py` & `mlfoundry-0.9.3/mlfoundry/enums.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/__init__.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/fastai_registry.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/fastai_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/gluon_registry.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/gluon_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/h2o_registry.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/h2o_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/keras_registry.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/keras_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/lightgbm_registry.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/lightgbm_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/onnx_registry.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/onnx_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/paddle_registry.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/paddle_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/pytorch_registry.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/pytorch_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/sklearn_registry.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/sklearn_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/spacy_registry.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/spacy_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/statsmodel_registry.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/statsmodel_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/tensorflow_registry.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/tensorflow_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/transformers_registry.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/transformers_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/frameworks/xgboost_registry.py` & `mlfoundry-0.9.3/mlfoundry/frameworks/xgboost_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/git_info.py` & `mlfoundry-0.9.3/mlfoundry/git_info.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/integrations/lightning.py` & `mlfoundry-0.9.3/mlfoundry/integrations/lightning.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/integrations/transformers.py` & `mlfoundry-0.9.3/mlfoundry/integrations/transformers.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/internal_namespace.py` & `mlfoundry-0.9.3/mlfoundry/internal_namespace.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/log_types/artifacts/constants.py` & `mlfoundry-0.9.3/mlfoundry/log_types/artifacts/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/log_types/artifacts/general_artifact.py` & `mlfoundry-0.9.3/mlfoundry/log_types/artifacts/general_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/log_types/artifacts/model.py` & `mlfoundry-0.9.3/mlfoundry/log_types/artifacts/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -74,14 +74,32 @@
         # TODO (chiragjn): The default on `model_version.metrics` is `list` there is no way to
         #   distinguish if the API returned something or there are no metrics
         self._metrics = None
         self._set_mutable_attrs()
 
     @classmethod
     def from_fqn(cls, fqn: str):
+        """
+        Get the version of a model to download contents or load them in memory
+
+        Args:
+            fqn (str): Fully qualified name of the model version.
+
+        Returns:
+            ModelVersion: An ModelVersion instance of the Model
+
+        Examples:
+
+            ```python
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            model_version = mlfoundry.ModelVersion.from_fqn(fqn="<your-model-fqn>")
+            ```
+        """
         mlflow_client = _get_mlflow_client()
         model_version = mlflow_client.get_model_version_by_fqn(fqn=fqn)
         model = mlflow_client.get_model_by_id(model_id=model_version.model_id)
         instance = cls(model_version=model_version, model=model)
         instance._metrics = model_version.metrics or []
         return instance
 
@@ -104,88 +122,128 @@
         self._model_schema = copy.deepcopy(self._model_version.model_schema)
 
     def __repr__(self):
         return f"{self.__class__.__name__}(fqn={self.fqn!r}, model_schema={self._model_schema!r})"
 
     @property
     def name(self) -> str:
+        """Get the name of the model"""
         return self._model.name
 
     @property
     def model_fqn(self) -> str:
+        """Get fqn of the model"""
         return self._model.fqn
 
     @property
     def version(self) -> int:
+        """Get version information of the model"""
         return self._model_version.version
 
     @property
     def fqn(self) -> str:
+        """Get fqn of the current model version"""
         return self._model_version.fqn
 
     @property
     def step(self) -> int:
+        """Get the step in which model was created"""
         return self._model_version.step
 
     @property
     def description(self) -> Optional[str]:
+        """Get description of the model"""
         return self._description
 
     @description.setter
     def description(self, value: str):
+        """set the description of the model"""
         _validate_description(value)
         self._description = value
 
     @property
     def metadata(self) -> Dict[str, Any]:
+        """Get metadata for the current model"""
         return self._metadata
 
     @metadata.setter
     def metadata(self, value: Dict[str, Any]):
+        """set the metadata for current model"""
         _validate_artifact_metadata(value)
         self._metadata = value
 
     @property
     def model_schema(self) -> Optional[ModelSchema]:
+        """get the model schema for current model"""
         return self._model_schema
 
     @model_schema.setter
     def model_schema(self, value: Union[Dict[str, Any], ModelSchema]):
         if not isinstance(value, ModelSchema):
             value = ModelSchema.parse_obj(value)
         self._model_schema = value
 
     @property
     def metrics(self) -> Dict[str, Union[float, int]]:
+        """get the metrics for the current version of the model"""
         if self._metrics is None:
             self._refetch_model_version()
             metrics_as_kv = {}
             metrics: List[Metric] = sorted(
                 self._model_version.metrics or [], key=lambda m: m.timestamp
             )
             for metric in metrics:
                 metrics_as_kv[metric.key] = metric.value
             self._metrics = metrics_as_kv
         return self._metrics
 
     @property
     def created_by(self) -> str:
+        """Get the information about who created the model version"""
         return self._model_version.created_by
 
     @property
     def created_at(self) -> datetime.datetime:
+        """Get the time at which model version was created"""
         return self._model_version.created_at
 
     @property
     def updated_at(self) -> datetime.datetime:
+        """Get the information about when the model version was updated"""
         return self._model_version.updated_at
 
     def raw_download(
         self, path: Optional[Union[str, Path]], overwrite: bool = False
     ) -> str:
+        """
+        Download an model file or directory to a local directory if applicable, and return a
+        local path for it.
+
+        Args:
+            path (str): Absolute path of the local filesystem destination directory to which to
+                        download the specified models. This directory must already exist.
+                        If unspecified, the models will either be downloaded to a new
+                        uniquely-named directory on the local filesystem or will be returned
+                        directly in the case of the Local ModelRepository.
+            overwrite (bool): If True it will overwrite the file if it is already present in the download directory else
+                              it will throw an error
+
+        Returns:
+            path:  Absolute path of the local filesystem location containing the desired models.
+
+        Examples:
+
+            ```python
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            model_version = client.get_model_version_by_fqn(fqn="<your-model-fqn>")
+            model_version.raw_download(path="<your-desired-download-path>")
+            ```
+        """
         logger.info("Downloading model version contents, this might take a while ...")
         mlfa_repo = MlFoundryArtifactsRepository(
             version_id=self._model_version.id, mlflow_client=self._mlflow_client
         )
         return mlfa_repo.download_artifacts(
             artifact_path="", dst_path=path, overwrite=overwrite
         )
@@ -211,14 +269,40 @@
             model_framework=internal_metadata.framework,
         )
         return internal_metadata, download_info
 
     def download(
         self, path: Optional[Union[str, Path]], overwrite: bool = False
     ) -> ModelVersionDownloadInfo:
+        """
+        Download an model file or directory to a local directory if applicable, and return a
+        local path for it.
+
+        Args:
+            path (str): Absolute path of the local filesystem destination directory to which to
+                        download the specified models. This directory must already exist.
+                        If unspecified, the models will either be downloaded to a new
+                        uniquely-named directory on the local filesystem or will be returned
+                        directly in the case of the Local ModelRepository.
+            overwrite (bool): If True it will overwrite the file if it is already present in the download directory else
+                              it will throw an error
+
+        Returns:
+            path:  Absolute path of the local filesystem location containing the desired models.
+
+        Examples:
+
+            ```python
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            model_version = client.get_model_version_by_fqn(fqn="<your-model-fqn>")
+            model_version.download(path="<your-desired-download-path>")
+            ```
+        """
         _, download_info = self._download(path=path, overwrite=overwrite)
         return download_info
 
     def load(self, **load_model_kwargs):
         from mlfoundry.frameworks import get_model_registry
 
         internal_metadata, download_info = self._download(path=None)
@@ -232,34 +316,73 @@
                 "contents by calling `.download(path='your/path/here') and load the model manually."
             )
         return get_model_registry(internal_metadata.framework).load_model(
             download_info.model_dir, **load_model_kwargs
         )
 
     def delete(self) -> bool:
+        """
+        Deletes the current instance of the ModelVersion hence deleting the current version.
+
+        Returns:
+            True if model was deleted successfully
+
+        Examples:
+
+            ```python
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            model_version = client.get_model_version_by_fqn(fqn="<your-model-fqn>")
+            model_version.delete()
+            ```
+        """
         self._ensure_not_deleted()
         self._mlflow_client.delete_artifact_version(version_id=self._model_version.id)
         self._deleted = True
         return True
 
     def update(self):
+        """
+        Updates the current instance of the ModelVersion hence updating the current version.
+
+        Examples:
+
+            ```python
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            model_version = client.get_model_version_by_fqn(fqn="<your-model-fqn>")
+            model_version.description = 'This is the new description'
+            model_version.update()
+            ```
+        """
         self._ensure_not_deleted()
         kwargs = {}
         if self.model_schema is not None:
             kwargs["model_schema"] = self.model_schema
         self._model_version = self._mlflow_client.update_model_version(
             version_id=self._model_version.id,
             description=self.description,
             artifact_metadata=self.metadata,
             **kwargs,
         )
         self._set_mutable_attrs()
 
 
 def calculate_model_size(artifact_dir: tempfile.TemporaryDirectory):
+    """
+    Tells about the size of the model
+
+    Args:
+        model_dir (str): directory in which model is present.
+
+    Returns:
+        total size of the model
+    """
     total_size = 0
     for path, dirs, files in os.walk(artifact_dir.name):
         for f in files:
             file_path = os.path.join(path, f)
             total_size += os.stat(file_path).st_size
     return total_size
```

### Comparing `mlfoundry-0.9.2/mlfoundry/log_types/artifacts/utils.py` & `mlfoundry-0.9.3/mlfoundry/log_types/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/log_types/image/image.py` & `mlfoundry-0.9.3/mlfoundry/log_types/image/image.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/log_types/image/image_normalizer.py` & `mlfoundry-0.9.3/mlfoundry/log_types/image/image_normalizer.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/log_types/image/types.py` & `mlfoundry-0.9.3/mlfoundry/log_types/image/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/log_types/plot.py` & `mlfoundry-0.9.3/mlfoundry/log_types/plot.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/log_types/pydantic_base.py` & `mlfoundry-0.9.3/mlfoundry/log_types/pydantic_base.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/log_types/utils.py` & `mlfoundry-0.9.3/mlfoundry/log_types/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/login.py` & `mlfoundry-0.9.3/mlfoundry/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 from typing import Optional
 
 import click
 from filelock import FileLock, Timeout
 from pydantic import BaseModel, Field, constr
 
-from mlfoundry.env_vars import API_KEY_GLOBAL, TRACKING_HOST_GLOBAL
+from mlfoundry.env_vars import _TRACKING_HOST_GLOBAL, API_KEY_GLOBAL
 from mlfoundry.exceptions import MlFoundryException
 from mlfoundry.logger import logger
 from mlfoundry.run_utils import resolve_tracking_uri
 from mlfoundry.tracking.entities import Token
 from mlfoundry.tracking.servicefoundry_service import ServicefoundryService
 from mlfoundry.tracking.truefoundry_rest_store import get_rest_store
 
@@ -157,20 +157,20 @@
             If `api_key` is not passed, this function prompts for the API key.
 
     Returns:
         bool: Returns `True` if any credential was persisted.
     """
     from mlfoundry.session import EnvCredentialProvider
 
-    if API_KEY_GLOBAL in os.environ and TRACKING_HOST_GLOBAL in os.environ:
+    if API_KEY_GLOBAL in os.environ and _TRACKING_HOST_GLOBAL in os.environ:
         logger.warning(
             "Skipping login because environment variables %s and "
             "%s are set and will be used when running mlfoundry. "
             "If you want to relogin then unset these environment keys.",
-            TRACKING_HOST_GLOBAL,
+            _TRACKING_HOST_GLOBAL,
             API_KEY_GLOBAL,
         )
         return False
 
     if EnvCredentialProvider.can_provide():
         logger.warning(
             "TFY_API_KEY env var is already set. "
```

### Comparing `mlfoundry-0.9.2/mlfoundry/metrics/v1/__init__.py` & `mlfoundry-0.9.3/mlfoundry/metrics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/metrics/v1/base_metrics.py` & `mlfoundry-0.9.3/mlfoundry/metrics/v1/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/metrics/v1/binary_classification_metrics.py` & `mlfoundry-0.9.3/mlfoundry/metrics/v1/binary_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/metrics/v1/multiclass_classification_metrics.py` & `mlfoundry-0.9.3/mlfoundry/metrics/v1/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/metrics/v1/regression_metrics.py` & `mlfoundry-0.9.3/mlfoundry/metrics/v1/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/metrics/v1/timeseries_metrics.py` & `mlfoundry-0.9.3/mlfoundry/metrics/v1/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/metrics/v2/__init__.py` & `mlfoundry-0.9.3/mlfoundry/metrics/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/metrics/v2/base_metrics.py` & `mlfoundry-0.9.3/mlfoundry/metrics/v2/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/metrics/v2/custom_metric_types.py` & `mlfoundry-0.9.3/mlfoundry/metrics/v2/custom_metric_types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/metrics/v2/multiclass_classification_metrics.py` & `mlfoundry-0.9.3/mlfoundry/metrics/v2/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/metrics/v2/regression_metrics.py` & `mlfoundry-0.9.3/mlfoundry/metrics/v2/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/metrics/v2/timeseries_metrics.py` & `mlfoundry-0.9.3/mlfoundry/metrics/v2/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/mlfoundry_api.py` & `mlfoundry-0.9.3/mlfoundry/mlfoundry_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     Union,
 )
 
 import coolname
 import mlflow
 import pandas as pd
 from mlflow.entities import Artifact, ArtifactType, CustomMetric, Model, ModelSchema
-from mlflow.store.tracking import SEARCH_MAX_RESULTS_DEFAULT
+from mlflow.store.tracking import _SEARCH_MAX_RESULTS_DEFAULT
 from mlflow.tracking import MlflowClient
 
 from mlfoundry import amplitude, constants, env_vars
 from mlfoundry.enums import ModelFramework, ViewType
-from mlfoundry.env_vars import TRACKING_HOST_GLOBAL
+from mlfoundry.env_vars import _TRACKING_HOST_GLOBAL
 from mlfoundry.exceptions import MlflowException, MlFoundryException
 from mlfoundry.internal_namespace import NAMESPACE
 from mlfoundry.log_types.artifacts.artifact import ArtifactPath, ArtifactVersion
 from mlfoundry.log_types.artifacts.general_artifact import _log_artifact_version
 from mlfoundry.log_types.artifacts.model import ModelVersion, _log_model_version
 from mlfoundry.logger import logger
 from mlfoundry.mlfoundry_run import MlFoundryRun
@@ -60,28 +60,28 @@
         disable_analytics (bool, optional): To turn off usage analytics collection, pass `True`.
             By default, this is set to `False`.
 
     Returns:
         MlFoundry: Instance of `MlFoundry` class which represents a `run`.
 
     Examples:
-    ### Get client
-    ```python
-    import mlfoundry
+        ### Get client
+        ```python
+        import mlfoundry
 
-    client = mlfoundry.get_client()
-    ```
+        client = mlfoundry.get_client()
+        ```
     """
     user_id = amplitude.NO_USER
 
     session = None
 
     # NOTE: hack to run tests
-    if os.getenv(TRACKING_HOST_GLOBAL, "").startswith("file:"):
-        tracking_uri = os.getenv(TRACKING_HOST_GLOBAL)
+    if os.getenv(_TRACKING_HOST_GLOBAL, "").startswith("file:"):
+        tracking_uri = os.getenv(_TRACKING_HOST_GLOBAL)
         tracking_uri = os.path.join(tracking_uri, constants.MLRUNS_FOLDER_NAME)
         mlflow.set_tracking_uri(tracking_uri)
     else:
         session = init_session()
         user_id = session.user_info.user_id
 
     amplitude.init(user_id=user_id, disable_analytics=disable_analytics)
@@ -189,17 +189,35 @@
         return ml_repos_names
 
     def create_ml_repo(
         self,
         ml_repo: Optional[str] = None,
         storage_integration_fqn: Optional[str] = None,
     ):
+        """Creates an ML Repository.
+
+        Args:
+            ml_repo (str, optional): The name of the Repository you want to create.
+                if not given, it creates a name by itself.
+
+            storage_integration_fqn(str, optional): The storage integration FQN to use for the experiment for saving artifacts.
+
+        Examples:
+                ### Create Repository
+                ```python
+                import mlfoundry
+
+                client = mlfoundry.get_client()
+
+                ml_repo = client.create_ml_repo(ml_repo="my-repo")
+            ```
+        """
         existing_ml_repo = self.mlflow_client.get_experiment_by_name(name=ml_repo)
         if not existing_ml_repo:  # ml_repo does not exist
-            return self.mlflow_client.get_experiment(
+            self.mlflow_client.get_experiment(
                 experiment_id=self.mlflow_client.create_experiment(
                     name=ml_repo, storage_integration_fqn=storage_integration_fqn
                 )
             )
 
         if storage_integration_fqn:
             session = get_active_session()
@@ -221,16 +239,14 @@
             if existing_storage_integration["fqn"] != storage_integration_fqn:
                 raise MlFoundryException(
                     f"ML Repo with same name already exists with storage integration:"
                     f"{existing_storage_integration['fqn']}. Cannot update the storage integration to: "
                     f"{storage_integration_fqn}"
                 )
 
-        return existing_ml_repo
-
     def create_run(
         self,
         ml_repo: Optional[str] = None,
         run_name: Optional[str] = None,
         tags: Optional[Dict[str, Any]] = None,
         project_name: Optional[str] = None,
         **kwargs,
@@ -252,56 +268,56 @@
                 this run. Tags are key-value pairs.
             kwargs:
 
         Returns:
             MlFoundryRun: An instance of `MlFoundryRun` class which represents a `run`.
 
         Examples:
-        ### Create a run under current user.
-        ```python
-        import mlfoundry
+            ### Create a run under current user.
+            ```python
+            import mlfoundry
 
-        client = mlfoundry.get_client()
+            client = mlfoundry.get_client()
 
-        tags = {"model_type": "svm"}
-        run = client.create_run(
-            ml_repo="my-classification-project", run_name="svm-with-rbf-kernel", tags=tags
-        )
+            tags = {"model_type": "svm"}
+            run = client.create_run(
+                ml_repo="my-classification-project", run_name="svm-with-rbf-kernel", tags=tags
+            )
 
-        run.end()
-        ```
+            run.end()
+            ```
 
-        ### Creating a run using context manager.
-        ```python
-        import mlfoundry
+            ### Creating a run using context manager.
+            ```python
+            import mlfoundry
 
-        client = mlfoundry.get_client()
-        with client.create_run(
-            ml_repo="my-classification-project", run_name="svm-with-rbf-kernel"
-        ) as run:
-            # ...
-            # Model training code
-            ...
-        # `run` will be automatically marked as `FINISHED` or `FAILED`.
-        ```
+            client = mlfoundry.get_client()
+            with client.create_run(
+                ml_repo="my-classification-project", run_name="svm-with-rbf-kernel"
+            ) as run:
+                # ...
+                # Model training code
+                ...
+            # `run` will be automatically marked as `FINISHED` or `FAILED`.
+            ```
 
-        ### Create a run in a project owned by a different user.
-        ```python
-        import mlfoundry
+            ### Create a run in a project owned by a different user.
+            ```python
+            import mlfoundry
 
-        client = mlfoundry.get_client()
+            client = mlfoundry.get_client()
 
-        tags = {"model_type": "svm"}
-        run = client.create_run(
-            ml_repo="my-classification-project",
-            run_name="svm-with-rbf-kernel",
-            tags=tags,
-        )
-        run.end()
-        ```
+            tags = {"model_type": "svm"}
+            run = client.create_run(
+                ml_repo="my-classification-project",
+                run_name="svm-with-rbf-kernel",
+                tags=tags,
+            )
+            run.end()
+            ```
         """
         amplitude.track(amplitude.Event.CREATE_RUN)
 
         if not run_name:
             run_name = coolname.generate_slug(2)
             logger.info(
                 f"No run_name given. Using a randomly generated name {run_name}."
@@ -333,14 +349,26 @@
         """Get an existing `run` by the `run_id`.
 
         Args:
             run_id (str): run_id or fqn of an existing `run`.
 
         Returns:
             MlFoundryRun: An instance of `MlFoundryRun` class which represents a `run`.
+
+        Examples:
+
+            ### Get run by the run id
+            ```python
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+
+            run = client.get_run_by_id(run_id='a8f6dafd70aa4baf9437a33c52d7ee90')
+            ```
+
         """
         amplitude.track(amplitude.Event.GET_RUN)
         if run_id == "" or (not isinstance(run_id, str)):
             raise MlFoundryException(
                 f"run_id must be string type and not empty. "
                 f"Got {type(run_id)} type with value {run_id}"
             )
@@ -363,14 +391,25 @@
         the `fqn` will be `truefoundry/cat-classifier/svm`.
 
         Args:
             run_fqn (str): `fqn` of an existing run.
 
         Returns:
             MlFoundryRun: An instance of `MlFoundryRun` class which represents a `run`.
+
+        Examples:
+            ### get run by run fqn
+            ```python
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+
+            run = client.get_run_by_fqn(run_fqn='truefoundry/my-repo/svm')
+            ```
+
         """
         run = self.mlflow_client.get_run_by_fqn(run_fqn)
         return MlFoundryRun(
             experiment_id=run.info.experiment_id,
             run_id=run.info.run_id,
         )
 
@@ -383,14 +422,24 @@
 
         Args:
             ml_repo (str): name of an the project of which the run is part of.
             run_name (str): the name of the run required
 
         Returns:
             MlFoundryRun: An instance of `MlFoundryRun` class which represents a `run`.
+
+        Examples:
+            ### get run by run run name
+            ```python
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+
+            run = client.get_run_by_name(run_name='svm', ml_repo='my-repo')
+            ```
         """
         ml_repo = _resolve_ml_repo_name(ml_repo=ml_repo)
 
         ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
 
         run = self.mlflow_client.get_run_by_name(
             experiment_id=ml_repo_id, run_name=run_name
@@ -408,14 +457,24 @@
         """Returns all the run name and id present under a project.
 
         The user must have `READ` access to the project.
         Args:
             ml_repo (str): Name of the project.
         Returns:
             pd.DataFrame: dataframe with two columns- run_id and run_name
+
+        Examples:
+            ### get all the runs from an ml_repo
+            ```python
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+
+            run = client.get_all_runs(ml_repo='my-repo')
+            ```
         """
         amplitude.track(amplitude.Event.GET_ALL_RUNS)
         ml_repo = _resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
         ml_repo_obj = self.mlflow_client.get_experiment_by_name(ml_repo)
         if ml_repo_obj is None:
             return pd.DataFrame(
                 columns=[constants.RUN_ID_COL_NAME, constants.RUN_NAME_COL_NAME]
@@ -559,46 +618,65 @@
                     f" and tags.TFY_INTERNAL_JOB_RUN_NAME = '{job_run_name}'"
                 )
         while not done:
             all_runs = self.mlflow_client.search_runs(
                 experiment_ids=[ml_repo_id],
                 filter_string=filter_string,
                 run_view_type=run_view_type,
-                max_results=min(SEARCH_MAX_RESULTS_DEFAULT, max_results)
+                max_results=min(_SEARCH_MAX_RESULTS_DEFAULT, max_results)
                 if max_results
-                else SEARCH_MAX_RESULTS_DEFAULT,
+                else _SEARCH_MAX_RESULTS_DEFAULT,
                 order_by=order_by,
                 page_token=page_token,
             )
             page_token = all_runs.token
             for run in all_runs:
                 if max_results is not None:
                     max_results -= 1
                 yield MlFoundryRun(run.info.experiment_id, run.info.run_id)
             done = page_token is None or max_results == 0
 
     @staticmethod
     def get_tracking_uri():
-        """get_tracking_uri."""
+        """
+        Get the current tracking URI.
+
+        Returns:
+            The tracking URI.
+
+        Examples:
+
+            ```python
+            import tempfile
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            tracking_uri = client.get_tracking_uri()
+            print("Current tracking uri: {}".format(tracking_uri))
+            ```
+        """
         return mlflow.tracking.get_tracking_uri()
 
     def get_model_version(
         self,
         ml_repo: str,
-        model_name: str,
+        name: str,
         version: Union[str, int] = constants.LATEST_ARTIFACT_OR_MODEL_VERSION,
     ) -> Optional[ModelVersion]:
         """
         Get the model version to download contents or load it in memory
 
         Args:
             ml_repo (str): ML Repo to which model is logged
-            model_name (str): Model Name
+            name (str): Model Name
             version (str | int): Model Version to fetch (default is the latest version)
 
+        Returns:
+            The ModelVersion instance of the model.
+
         Examples:
 
             ```python
             import tempfile
             import mlfoundry
 
             client = mlfoundry.get_client()
@@ -616,25 +694,28 @@
         resolved_version = None
         if version != constants.LATEST_ARTIFACT_OR_MODEL_VERSION:
             resolved_version = _resolve_version(version=version)
 
         ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
         return self.mlflow_client.get_model_version(
             experiment_id=int(ml_repo_id),
-            model_name=model_name,
+            model_name=name,
             version=resolved_version,
         )
 
     def get_model_version_by_fqn(self, fqn: str) -> ModelVersion:
         """
         Get the model version to download contents or load it in memory
 
         Args:
             fqn (str): Fully qualified name of the model version.
 
+        Returns:
+            The ModelVersion instance of the model.
+
         Examples:
 
             ```python
             import tempfile
             import mlfoundry
 
             client = mlfoundry.get_client()
@@ -654,14 +735,17 @@
     def get_model(self, fqn: str) -> ModelVersion:
         """
         Get the model version to download contents or load it in memory
 
         Args:
             fqn (str): Fully qualified name of the model version.
 
+        Returns:
+            The ModelVersion instance of the model.
+
         Examples:
 
             ```python
             import tempfile
             import mlfoundry
 
             client = mlfoundry.get_client()
@@ -679,14 +763,37 @@
         warning_message = "get_model will be deprecated in a future release. Please use get_model_version instead"
         warnings.warn(
             message=warning_message, category=DeprecationWarning, stacklevel=2
         )
         return ModelVersion.from_fqn(fqn)
 
     def list_model_versions(self, ml_repo: str, name: str) -> Iterator[ModelVersion]:
+        """
+        Get all the version of a model to download contents or load them in memory
+
+        Args:
+            ml_repo (str): Repository in which the model is stored.
+            name (str): Name of the model whose version is required
+
+        Returns:
+            Iterator[ModelVersion]: An iterator that yields non deleted model versions
+                of a model under a given ml_repo  sorted reverse by the version number
+
+        Examples:
+
+            ```python
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            model_versions = client.list_mode_version(ml_repo="my-repo", name="svm")
+
+            for model_version in model_versions:
+                print(model_version)
+            ```
+        """
         ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
         models = self.mlflow_client.list_models(ml_repo_id=ml_repo_id, name=name)
         if not models or len(models) == 0:
             err_msg = f"Model Does Not Exist for ml_repo={ml_repo}, name={name}"
             raise MlFoundryException(err_msg)
         return self._list_model_versions_by_id(model=models[0])
 
@@ -756,14 +863,17 @@
 
         Args:
             ml_repo (str): ML Repo to which artifact is logged
             artifact_name (str): Artifact Name
             artifact_type (str): The type of artifact to fetch (acceptable values: "artifact", "model", "plot", "image")
             version (str | int): Artifact Version to fetch (default is the latest version)
 
+        Returns:
+            ArtifactVersion : An ArtifactVersion instance of the artifact
+
         Examples:
 
             ```python
             import tempfile
             import mlfoundry
 
             client = mlfoundry.get_client()
@@ -793,14 +903,17 @@
     def get_artifact_version_by_fqn(self, fqn: str) -> ArtifactVersion:
         """
         Get the artifact version to download contents
 
         Args:
             fqn (str): Fully qualified name of the artifact version.
 
+        Returns:
+            ArtifactVersion : An ArtifactVersion instance of the artifact
+
         Examples:
 
             ```python
             import tempfile
             import mlfoundry
 
             client = mlfoundry.get_client()
@@ -817,14 +930,17 @@
     def get_artifact(self, fqn: str) -> ArtifactVersion:
         """
         Get the artifact version to download contents
 
         Args:
             fqn (str): Fully qualified name of the artifact version.
 
+        Returns:
+            ArtifactVersion : An ArtifactVersion instance of the artifact
+
         Examples:
 
             ```python
             import tempfile
             import mlfoundry
 
             client = mlfoundry.get_client()
@@ -844,14 +960,38 @@
 
     def list_artifact_versions(
         self,
         ml_repo: str,
         name: str,
         artifact_type: Optional[ArtifactType] = ArtifactType.ARTIFACT,
     ) -> Iterator[ArtifactVersion]:
+        """
+        Get all the version of a artifact to download contents or load them in memory
+
+        Args:
+            ml_repo (str): Repository in which the model is stored.
+            name (str): Name of the artifact whose version is required
+            artifact_type (ArtifactType): Type of artifact you want for example model, image, etc.
+
+        Returns:
+            Iterator[ArtifactVersion]: An iterator that yields non deleted artifact-versions
+                of a artifact under a given ml_repo  sorted reverse by the version number
+
+        Examples:
+
+            ```python
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            artifact_versions = client.list_artifact_versions(ml_repo="my-repo", name="artifact-name")
+
+            for artifact_version in artifact_versions:
+                print(artifact_version)
+            ```
+        """
         ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
         artifacts = self.mlflow_client.list_artifacts_(
             ml_repo_id=ml_repo_id, name=name, artifact_type=artifact_type
         )
         if not artifacts or len(artifacts) == 0:
             err_msg = f"Artifact Does Not Exist for ml_repo={ml_repo}, name={name}, type={artifact_type}"
             raise MlFoundryException(err_msg)
@@ -875,16 +1015,14 @@
                 under the given artifact_fqn sorted reverse by the version number
 
         Yields:
             ArtifactVersion: An instance of `mlfoundry.ArtifactVersion`
 
         Examples:
 
-            Examples:
-
             ```python
             import mlfoundry
 
             mlfoundry.login(tracking_uri=https://your.truefoundry.site.com")
             client = mlfoundry.get_client()
             artifact_fqn = "artifact:org/user/my-project/my-artifact"
             for av in client.list_artifact_versions(artifact_fqn=artifact_fqn):
@@ -939,14 +1077,15 @@
                 the logged artifact will be added as a new version under that `name`. If no artifact exist with the given
                 `name`, the given artifact will be logged as version 1.
             artifact_paths (List[mlfoundry.ArtifactPath], optional): A list of pairs
                 of (source path, destination path) to add files and folders
                 to the artifact version contents. The first member of the pair should be a file or directory path
                 and the second member should be the path inside the artifact contents to upload to.
 
+                ```
                 E.g. >>> client.log_artifact(
                      ...     ml_repo="sample-repo",
                      ...     name="xyz",
                      ...     artifact_paths=[
                                 mlfoundry.ArtifactPath("foo.txt", "foo/bar/foo.txt"),
                                 mlfoundry.ArtifactPath("tokenizer/", "foo/tokenizer/"),
                                 mlfoundry.ArtifactPath('bar.text'),
@@ -957,42 +1096,43 @@
                 would result in
                 .
                 └── foo/
                     ├── bar/
                     │   └── foo.txt
                     └── tokenizer/
                         └── # contents of tokenizer/ directory will be uploaded here
+                ```
             description (Optional[str], optional): arbitrary text upto 1024 characters to store as description.
                 This field can be updated at any time after logging. Defaults to `None`
             metadata (Optional[Dict[str, Any]], optional): arbitrary json serializable dictionary to store metadata.
                 For example, you can use this to store metrics, params, notes.
                 This field can be updated at any time after logging. Defaults to `None`
 
         Returns:
             mlfoundry.ArtifactVersion: an instance of `ArtifactVersion` that can be used to download the files,
             or update attributes like description, metadata.
 
         Examples:
-        ```python
-        import os
-        import mlfoundry
+            ```python
+            import os
+            import mlfoundry
 
-        with open("artifact.txt", "w") as f:
-            f.write("hello-world")
+            with open("artifact.txt", "w") as f:
+                f.write("hello-world")
 
-        client = mlfoundry.get_client()
-        ml_repo = "sample-repo"
+            client = mlfoundry.get_client()
+            ml_repo = "sample-repo"
 
-        client.create_ml_repo(ml_repo=ml_repo)
-        client.log_artifact(
-            ml_repo=ml_repo,
-            name="hello-world-file",
-            artifact_paths=[mlfoundry.ArtifactPath('artifact.txt', 'a/b/')]
-        )
-        ```
+            client.create_ml_repo(ml_repo=ml_repo)
+            client.log_artifact(
+                ml_repo=ml_repo,
+                name="hello-world-file",
+                artifact_paths=[mlfoundry.ArtifactPath('artifact.txt', 'a/b/')]
+            )
+            ```
         """
         if not artifact_paths:
             raise MlFoundryException(
                 "artifact_paths cannot be empty, atleast one artifact_path must be passed"
             )
 
         ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
@@ -1047,50 +1187,53 @@
                 The model version contents are arranged like follows
                 .
                 └── model/
                     └── # model files are serialized here
                 └── # any additional files and folders can be added here.
 
                 You can also add additional files to model/ subdirectory by specifying the destination path as model/
-
+                ```
                 E.g. >>> client.log_model(
                      ...     ml_repo="sample-repo", name="xyz", model=clf, framework="sklearn",
                      ...     additional_files=[("foo.txt", "foo/bar/foo.txt"), ("tokenizer/", "foo/tokenizer/")]
                      ... )
                 would result in
                 .
                 ├── model/
                 │   └── # model files are serialized here e.g. model.joblib
                 └── foo/
                     ├── bar/
                     │   └── foo.txt
                     └── tokenizer/
                         └── # contents of tokenizer/ directory will be uploaded here
+                ```
             description (Optional[str], optional): arbitrary text upto 1024 characters to store as description.
                 This field can be updated at any time after logging. Defaults to `None`
             metadata (Optional[Dict[str, Any]], optional): arbitrary json serializable dictionary to store metadata.
                 For example, you can use this to store metrics, params, notes.
                 This field can be updated at any time after logging. Defaults to `None`
             model_schema (Optional[Union[Dict[str, Any], ModelSchema]], optional): instance of `mlfoundry.ModelSchema`.
                 This schema needs to be consistent with older versions of the model under the given `name` i.e.
                 a feature's value type and model's prediction type cannot be changed in the schema of new version.
                 Features can be removed or added between versions.
+                ```
                 E.g. if there exists a v1 with
                 schema = {"features": {"name": "feat1": "int"}, "prediction": "categorical"}, then
 
                 schema = {"features": {"name": "feat1": "string"}, "prediction": "categorical"} or
                 schema = {"features": {"name": "feat1": "int"}, "prediction": "numerical"}
                 are invalid because they change the types of existing features and prediction
 
                 while
                 schema = {"features": {"name": "feat1": "int", "feat2": "string"}, "prediction": "categorical"} or
                 schema = {"features": {"feat2": "string"}, "prediction": "categorical"}
                 are valid
 
                 This field can be updated at any time after logging. Defaults to `None`
+                ```
             custom_metrics: (Optional[Union[List[Dict[str, Any]], CustomMetric]], optional): list of instances of
                 `mlfoundry.CustomMetric`
                 The custom metrics must be added according to the prediction type of schema.
                 custom_metrics = [{
                     "name": "mean_square_error",
                     "type": "metric",
                     "value_type": "float"
@@ -1098,37 +1241,38 @@
 
         Returns:
             mlfoundry.ModelVersion: an instance of `ModelVersion` that can be used to download the files,
                 load the model, or update attributes like description, metadata, schema.
 
         Examples:
 
-        ### sklearn
-        ```python
-        import mlfoundry
-        import numpy as np
-        from sklearn.pipeline import make_pipeline
-        from sklearn.preprocessing import StandardScaler
-        from sklearn.svm import SVC
+            ### sklearn
+            ```python
+            import mlfoundry
+            import numpy as np
+            from sklearn.pipeline import make_pipeline
+            from sklearn.preprocessing import StandardScaler
+            from sklearn.svm import SVC
 
-        client = mlfoundry.get_client()
-        run = client.create_run(
-            ml_repo="my-classification-project"
-        )
-        X = np.array([[-1, -1], [-2, -1], [1, 1], [2, 1]])
-        y = np.array([1, 1, 2, 2])
-        clf = make_pipeline(StandardScaler(), SVC(gamma='auto'))
-        clf.fit(X, y)
-
-        model_version = run.log_model(
-            name="my-sklearn-model",
-            model=clf,
-            framework="sklearn"
-        )
-        print(model_version.fqn)
+            client = mlfoundry.get_client()
+            run = client.create_run(
+                ml_repo="my-classification-project"
+            )
+            X = np.array([[-1, -1], [-2, -1], [1, 1], [2, 1]])
+            y = np.array([1, 1, 2, 2])
+            clf = make_pipeline(StandardScaler(), SVC(gamma='auto'))
+            clf.fit(X, y)
+
+            model_version = run.log_model(
+                name="my-sklearn-model",
+                model=clf,
+                framework="sklearn"
+            )
+            print(model_version.fqn)
+            ```
         """
         ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
 
         model_version = _log_model_version(
             run=None,
             mlflow_client=self.mlflow_client,
             ml_repo_id=ml_repo_id,
```

### Comparing `mlfoundry-0.9.2/mlfoundry/mlfoundry_run.py` & `mlfoundry-0.9.3/mlfoundry/mlfoundry_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,21 +51,21 @@
     log_artifact_blob,
     process_params,
 )
 from mlfoundry.session import ACTIVE_RUNS
 
 
 def _ensure_not_deleted(method):
-    def check_deleted_or_not(self, *args, **kwargs):
+    def _check_deleted_or_not(self, *args, **kwargs):
         if self._deleted:
             raise MlFoundryException(f"Run was deleted, cannot access a deleted Run")
         else:
             return method(self, *args, **kwargs)
 
-    return check_deleted_or_not
+    return _check_deleted_or_not
 
 
 class MlFoundryRun:
     """MlFoundryRun."""
 
     VALID_PARAM_AND_METRIC_NAMES = re.compile(r"^[A-Za-z0-9_\-\. /]+$")
 
@@ -101,39 +101,45 @@
 
         self._run_info = self.mlflow_client.get_run(self.run_id).info
         return self._run_info
 
     @property
     @_ensure_not_deleted
     def run_id(self) -> str:
+        """Get run_id for the current `run`"""
         return self._run_id
 
     @property
     @_ensure_not_deleted
     def run_name(self) -> str:
+        """Get run_name for the current `run`"""
         return self._get_run_info().name
 
     @property
     @_ensure_not_deleted
     def fqn(self) -> str:
+        """Get fqn for the current `run`"""
         return self._get_run_info().fqn
 
     @property
     @_ensure_not_deleted
     def status(self) -> str:
+        """Get status for the current `run`"""
         return self.mlflow_client.get_run(self.run_id).info.status
 
     @property
     @_ensure_not_deleted
     def ml_repo(self) -> str:
+        """Get ml_repo name of which the current `run` is part of"""
         return self.mlflow_client.get_experiment(self._experiment_id).name
 
     @property
     @_ensure_not_deleted
     def auto_end(self) -> bool:
+        """Tells whether automatic end for `run` is True or False"""
         return self._auto_end
 
     @_ensure_not_deleted
     def __repr__(self) -> str:
         return f"<{type(self).__name__} at 0x{id(self):x}: run={self.fqn!r}>"
 
     @_ensure_not_deleted
@@ -271,14 +277,39 @@
             raise
 
     @_ensure_not_deleted
     def list_artifact_versions(
         self,
         artifact_type: Optional[List[ArtifactType]] = None,
     ) -> Iterator[ArtifactVersion]:
+        """
+        Get all the version of a artifact from a particular run to download contents or load them in memory
+
+        Args:
+            artifact_type: Type of the artifact you want
+
+        Returns:
+            Iterator[ArtifactVersion]: An iterator that yields non deleted artifact-versions
+                of a artifact under a given run  sorted reverse by the version number
+
+        Examples:
+
+            ```python
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            run = client.create_run(ml_repo="iris-learning", run_name="svm-model1")
+            artifact_versions = run.list_artifact_versions()
+
+            for artifact_version in artifact_versions:
+                print(artifact_version)
+
+            run.end()
+            ```
+        """
         page_token, done = None, False
         while not done:
             artifact_versions = self.mlflow_client.list_artifact_versions(
                 run_ids=[self.run_id],
                 artifact_types=artifact_type,
                 page_token=page_token,
             )
@@ -286,14 +317,36 @@
                 yield ArtifactVersion.from_fqn(artifact_version.artifact_fqn)
             done = page_token is None
 
     @_ensure_not_deleted
     def list_model_versions(
         self,
     ) -> Iterator[ModelVersion]:
+        """
+        Get all the version of a models from a particular run to download contents or load them in memory
+
+        Returns:
+            Iterator[ModelVersion]: An iterator that yields non deleted model-versions
+                under a given run  sorted reverse by the version number
+
+        Examples:
+
+            ```python
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            run = client.get_run(run_id="<your-run-id>")
+            model_versions = run.list_model_versions()
+
+            for model_version in model_versions:
+                print(model_version)
+
+            run.end()
+            ```
+        """
         page_token, done = 10, None, False
         while not done:
             model_versions = self.mlflow_client.list_model_versions(
                 page_token=page_token,
                 run_ids=[self.run_id],
             )
             for model_version in model_versions:
@@ -487,14 +540,15 @@
                 the logged artifact will be added as a new version under that `name`. If no artifact exist with the given
                 `name`, the given artifact will be logged as version 1.
             artifact_paths (List[mlfoundry.ArtifactPath], optional): A list of pairs
                 of (source path, destination path) to add files and folders
                 to the artifact version contents. The first member of the pair should be a file or directory path
                 and the second member should be the path inside the artifact contents to upload to.
 
+                ```
                 E.g. >>> run.log_artifact(
                      ...     name="xyz",
                      ...     artifact_paths=[
                                 mlfoundry.ArtifactPath("foo.txt", "foo/bar/foo.txt"),
                                 mlfoundry.ArtifactPath("tokenizer/", "foo/tokenizer/"),
                                 mlfoundry.ArtifactPath('bar.text'),
                                 ('bar.txt', ),
@@ -504,14 +558,15 @@
                 would result in
                 .
                 └── foo/
                     ├── bar/
                     │   └── foo.txt
                     └── tokenizer/
                         └── # contents of tokenizer/ directory will be uploaded here
+                ```
             description (Optional[str], optional): arbitrary text upto 1024 characters to store as description.
                 This field can be updated at any time after logging. Defaults to `None`
             metadata (Optional[Dict[str, Any]], optional): arbitrary json serializable dictionary to store metadata.
                 For example, you can use this to store metrics, params, notes.
                 This field can be updated at any time after logging. Defaults to `None`
             step (int): step/iteration at which the vesion is being logged, defaults to 0.
 
@@ -934,50 +989,53 @@
                 .
                 └── model/
                     └── # model files are serialized here
                 └── # any additional files and folders can be added here.
 
                 You can also add additional files to model/ subdirectory by specifying the destination path as model/
 
-
+                ```
                 E.g. >>> run.log_model(
                      ...     name="xyz", model=clf, framework="sklearn",
                      ...     additional_files=[("foo.txt", "foo/bar/foo.txt"), ("tokenizer/", "foo/tokenizer/")]
                      ... )
                 would result in
                 .
                 ├── model/
                 │   └── # model files are serialized here e.g. model.joblib
                 └── foo/
                     ├── bar/
                     │   └── foo.txt
                     └── tokenizer/
                         └── # contents of tokenizer/ directory will be uploaded here
+                ```
             description (Optional[str], optional): arbitrary text upto 1024 characters to store as description.
                 This field can be updated at any time after logging. Defaults to `None`
             metadata (Optional[Dict[str, Any]], optional): arbitrary json serializable dictionary to store metadata.
                 For example, you can use this to store metrics, params, notes.
                 This field can be updated at any time after logging. Defaults to `None`
             model_schema (Optional[Union[Dict[str, Any], ModelSchema]], optional): instance of `mlfoundry.ModelSchema`.
                 This schema needs to be consistent with older versions of the model under the given `name` i.e.
                 a feature's value type and model's prediction type cannot be changed in the schema of new version.
                 Features can be removed or added between versions.
+                ```
                 E.g. if there exists a v1 with
-                schema = {"features": {"name": "feat1": "int"}, "prediction": "categorical"}, then
+                    schema = {"features": {"name": "feat1": "int"}, "prediction": "categorical"}, then
 
-                schema = {"features": {"name": "feat1": "string"}, "prediction": "categorical"} or
-                schema = {"features": {"name": "feat1": "int"}, "prediction": "numerical"}
-                are invalid because they change the types of existing features and prediction
-
-                while
-                schema = {"features": {"name": "feat1": "int", "feat2": "string"}, "prediction": "categorical"} or
-                schema = {"features": {"feat2": "string"}, "prediction": "categorical"}
-                are valid
+                    schema = {"features": {"name": "feat1": "string"}, "prediction": "categorical"} or
+                    schema = {"features": {"name": "feat1": "int"}, "prediction": "numerical"}
+                    are invalid because they change the types of existing features and prediction
+
+                    while
+                    schema = {"features": {"name": "feat1": "int", "feat2": "string"}, "prediction": "categorical"} or
+                    schema = {"features": {"feat2": "string"}, "prediction": "categorical"}
+                    are valid
 
-                This field can be updated at any time after logging. Defaults to `None`
+                    This field can be updated at any time after logging. Defaults to None
+                ```
             custom_metrics: (Optional[Union[List[Dict[str, Any]], CustomMetric]], optional): list of instances of
                 `mlfoundry.CustomMetric`
                 The custom metrics must be added according to the prediction type of schema.
                 custom_metrics = [{
                     "name": "mean_square_error",
                     "type": "metric",
                     "value_type": "float"
```

### Comparing `mlfoundry-0.9.2/mlfoundry/monitoring/entities.py` & `mlfoundry-0.9.3/mlfoundry/monitoring/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/monitoring/store/client.py` & `mlfoundry-0.9.3/mlfoundry/monitoring/store/client.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/monitoring/store/repositories/dto.py` & `mlfoundry-0.9.3/mlfoundry/monitoring/store/repositories/dto.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py` & `mlfoundry-0.9.3/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/monitoring/store/worker.py` & `mlfoundry-0.9.3/mlfoundry/monitoring/store/worker.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/run_utils.py` & `mlfoundry-0.9.3/mlfoundry/run_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,19 +23,19 @@
     except Exception as ex:
         msg = error_message or f"Error importing module {module_name}"
         if required:
             raise MlFoundryException(msg) from ex
 
 
 def resolve_tracking_uri(tracking_uri: typing.Optional[str]):
-    if not tracking_uri and not os.getenv(env_vars.TRACKING_HOST_GLOBAL):
+    if not tracking_uri and not os.getenv(env_vars._TRACKING_HOST_GLOBAL):
         raise ValueError(
-            f"Either `host` should be provided by --host <value>, or `{env_vars.TRACKING_HOST_GLOBAL}` env must be set"
+            f"Either `host` should be provided by --host <value>, or `{env_vars._TRACKING_HOST_GLOBAL}` env must be set"
         )
-    return tracking_uri or os.getenv(env_vars.TRACKING_HOST_GLOBAL)
+    return tracking_uri or os.getenv(env_vars._TRACKING_HOST_GLOBAL)
 
 
 def append_path_to_rest_tracking_uri(tracking_uri: str):
     if urlsplit(tracking_uri).netloc.startswith("localhost"):
         return tracking_uri
     return urljoin(tracking_uri, "/api/ml")
```

### Comparing `mlfoundry-0.9.2/mlfoundry/session.py` & `mlfoundry-0.9.3/mlfoundry/session.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/tracking/auth_service.py` & `mlfoundry-0.9.3/mlfoundry/tracking/auth_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/tracking/entities.py` & `mlfoundry-0.9.3/mlfoundry/tracking/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/tracking/servicefoundry_service.py` & `mlfoundry-0.9.3/mlfoundry/tracking/servicefoundry_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/tracking/truefoundry_rest_store.py` & `mlfoundry-0.9.3/mlfoundry/tracking/truefoundry_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/mlfoundry/vendor/pynvml/pynvml.py` & `mlfoundry-0.9.3/mlfoundry/vendor/pynvml/pynvml.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.2/pyproject.toml` & `mlfoundry-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlfoundry"
-version = "0.9.2" # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.9.3" # do not change, auto-generated by poetry-dynamic-versioning
 description = "Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/truefoundry/mlfoundry"
 repository = "https://github.com/truefoundry/mlfoundry"
 readme = "README.md"
 packages = [
     { include = "mlfoundry" },
@@ -30,15 +30,16 @@
 pydantic = ">=1.8.2,<2.0.0"
 scikit-learn = ">=0.24.2,<2.0.0"
 scipy = [
     # This is split into two because poetry will select a version which has no wheel on python >= 3.10 :/
     { version = ">=1.5.4,<2.0.0", python = "<3.10" },
     { version = ">=1.8.0,<2.0.0", python = ">=3.10" },
 ]
-tfy-mlflow-client = "0.0.36"
+tfy-mlflow-client = "0.0.37"
+tqdm = ">=4.62.3,<5.0.0"
 # Check and try to eliminate libs below this comment
 importlib-metadata = ">=4.11.3,<5.0.0"
 packaging = ">=20.0,<24.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "2.21.0"
 pytest = ">=7.2.0,<7.3.0"
```

### Comparing `mlfoundry-0.9.2/PKG-INFO` & `mlfoundry-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfoundry
-Version: 0.9.2
+Version: 0.9.3
 Summary: Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library
 Home-page: https://github.com/truefoundry/mlfoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -23,15 +23,16 @@
 Requires-Dist: pandas (>=1.0.0,<2.0.0) ; python_version < "3.10"
 Requires-Dist: pandas (>=1.4.0,<2.0.0) ; python_version >= "3.10"
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: scikit-learn (>=0.24.2,<2.0.0)
 Requires-Dist: scipy (>=1.5.4,<2.0.0) ; python_version < "3.10"
 Requires-Dist: scipy (>=1.8.0,<2.0.0) ; python_version >= "3.10"
-Requires-Dist: tfy-mlflow-client (==0.0.36)
+Requires-Dist: tfy-mlflow-client (==0.0.37)
+Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Project-URL: Repository, https://github.com/truefoundry/mlfoundry
 Description-Content-Type: text/markdown
 
 # MlFoundry
 
 ![](https://github.com/MyName/my-project/workflows/Project%20Tests/badge.svg)
```

