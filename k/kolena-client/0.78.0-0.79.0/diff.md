# Comparing `tmp/kolena_client-0.78.0.tar.gz` & `tmp/kolena_client-0.79.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena_client-0.78.0.tar", max compression
+gzip compressed data, was "kolena_client-0.79.0.tar", max compression
```

## Comparing `kolena_client-0.78.0.tar` & `kolena_client-0.79.0.tar`

### file list

```diff
@@ -1,116 +1,118 @@
--rw-r--r--   0        0        0    11346 2023-07-17 22:07:07.936741 kolena_client-0.78.0/LICENSE
--rw-r--r--   0        0        0      556 2023-07-17 22:07:07.936741 kolena_client-0.78.0/LICENSE_HEADER
--rw-r--r--   0        0        0     1948 2023-07-17 22:07:07.936741 kolena_client-0.78.0/README.md
--rw-r--r--   0        0        0     1356 2023-07-17 22:14:34.547923 kolena_client-0.78.0/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1737 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     5111 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7531 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5597 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      833 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_experimental/__init__.py
--rw-r--r--   0        0        0     1117 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_experimental/object_detection/__init__.py
--rw-r--r--   0        0        0     5654 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_experimental/object_detection/evaluator.py
--rw-r--r--   0        0        0    15465 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_experimental/object_detection/evaluator_multiclass.py
--rw-r--r--   0        0        0    10294 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_experimental/object_detection/evaluator_single_class.py
--rw-r--r--   0        0        0    13260 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_experimental/object_detection/utils.py
--rw-r--r--   0        0        0     5173 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_experimental/object_detection/workflow.py
--rw-r--r--   0        0        0      579 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_extras/__init__.py
--rw-r--r--   0        0        0      676 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_extras/metrics/__init__.py
--rw-r--r--   0        0        0      783 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_extras/metrics/sklearn.py
--rw-r--r--   0        0        0      579 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_utils/__init__.py
--rw-r--r--   0        0        0     1616 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     5313 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_utils/cli.py
--rw-r--r--   0        0        0      921 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_utils/consts.py
--rw-r--r--   0        0        0      579 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3403 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1183 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2990 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     5033 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/log.py
--rw-r--r--   0        0        0     1003 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     5450 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/state.py
--rw-r--r--   0        0        0     1942 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0     1164 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1272 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1475 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3512 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3354 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    15698 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3573 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     3185 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2694 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2372 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4480 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6013 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/test_run.py
--rw-r--r--   0        0        0     3180 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1477 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1035 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5470 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8995 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    14122 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1201 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     1761 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12390 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    13804 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     5867 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5435 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/inference.py
--rw-r--r--   0        0        0     1460 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/metadata.py
--rw-r--r--   0        0        0     3210 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/model.py
--rw-r--r--   0        0        0     2387 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3199 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/test_config.py
--rw-r--r--   0        0        0     5967 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5405 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2854 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2681 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/fr/__init__.py
--rw-r--r--   0        0        0     2171 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/fr/_utils.py
--rw-r--r--   0        0        0    20960 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/fr/datatypes.py
--rw-r--r--   0        0        0    10274 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/fr/model.py
--rw-r--r--   0        0        0    14952 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12237 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/fr/test_images.py
--rw-r--r--   0        0        0    16943 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/fr/test_run.py
--rw-r--r--   0        0        0    16329 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     3880 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/initialize.py
--rw-r--r--   0        0        0     2439 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13948 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     6281 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/_validators.py
--rw-r--r--   0        0        0    10397 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     4926 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/asset.py
--rw-r--r--   0        0        0     3469 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/define_workflow.py
--rw-r--r--   0        0        0    13854 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0    11232 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     4421 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     4334 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/inference.py
--rw-r--r--   0        0        0     1150 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0     3931 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/metrics/_formula.py
--rw-r--r--   0        0        0    16014 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     8459 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/model.py
--rw-r--r--   0        0        0    10261 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/plot.py
--rw-r--r--   0        0        0    18319 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    22734 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/test_run.py
--rw-r--r--   0        0        0    10564 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    15455 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0      841 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/visualization/__init__.py
--rw-r--r--   0        0        0     6145 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/visualization/_activation_map.py
--rw-r--r--   0        0        0     1910 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/visualization/_utils.py
--rw-r--r--   0        0        0     9419 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     3037 2023-07-17 22:14:34.547923 kolena_client-0.78.0/pyproject.toml
--rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 kolena_client-0.78.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-25 21:10:33.482132 kolena_client-0.79.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-07-25 21:10:33.482132 kolena_client-0.79.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     1948 2023-07-25 21:10:33.482132 kolena_client-0.79.0/README.md
+-rw-r--r--   0        0        0     1356 2023-07-25 21:17:43.374114 kolena_client-0.79.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1737 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     5111 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7531 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5597 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      833 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_experimental/__init__.py
+-rw-r--r--   0        0        0      579 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_experimental/classification/__init__.py
+-rw-r--r--   0        0        0     4256 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_experimental/classification/utils.py
+-rw-r--r--   0        0        0     1117 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_experimental/object_detection/__init__.py
+-rw-r--r--   0        0        0     5654 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_experimental/object_detection/evaluator.py
+-rw-r--r--   0        0        0    15465 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_experimental/object_detection/evaluator_multiclass.py
+-rw-r--r--   0        0        0    10294 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_experimental/object_detection/evaluator_single_class.py
+-rw-r--r--   0        0        0    13260 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_experimental/object_detection/utils.py
+-rw-r--r--   0        0        0     5173 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_experimental/object_detection/workflow.py
+-rw-r--r--   0        0        0      579 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_extras/__init__.py
+-rw-r--r--   0        0        0      676 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_extras/metrics/__init__.py
+-rw-r--r--   0        0        0      783 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_extras/metrics/sklearn.py
+-rw-r--r--   0        0        0      579 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0     1616 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     5313 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      921 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/consts.py
+-rw-r--r--   0        0        0      579 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1183 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2990 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     5033 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0     1003 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     5450 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     1942 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0     1164 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1272 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1475 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3512 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3354 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    15698 2023-07-25 21:10:33.558138 kolena_client-0.79.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3573 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     3185 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2694 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2372 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4480 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6013 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     3180 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1477 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1035 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5470 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8995 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    14122 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1201 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     1761 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12390 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    13804 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     5867 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5435 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1460 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     3210 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2387 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3199 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     5967 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5405 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2854 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2681 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0     2171 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/fr/_utils.py
+-rw-r--r--   0        0        0    20960 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0    10274 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14952 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12237 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    16943 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    16329 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     3880 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/initialize.py
+-rw-r--r--   0        0        0     2493 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13948 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     6281 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0    10397 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     4926 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0     3469 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/define_workflow.py
+-rw-r--r--   0        0        0    13854 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0    11232 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     4421 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     4334 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0     1150 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0     3931 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/metrics/_formula.py
+-rw-r--r--   0        0        0    16014 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     8459 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    10261 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/plot.py
+-rw-r--r--   0        0        0    18319 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    23730 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0    11006 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    15455 2023-07-25 21:10:33.562138 kolena_client-0.79.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0      841 2023-07-25 21:10:33.566139 kolena_client-0.79.0/kolena/workflow/visualization/__init__.py
+-rw-r--r--   0        0        0     6145 2023-07-25 21:10:33.566139 kolena_client-0.79.0/kolena/workflow/visualization/_activation_map.py
+-rw-r--r--   0        0        0     1910 2023-07-25 21:10:33.566139 kolena_client-0.79.0/kolena/workflow/visualization/_utils.py
+-rw-r--r--   0        0        0     9419 2023-07-25 21:10:33.566139 kolena_client-0.79.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     3037 2023-07-25 21:17:43.374114 kolena_client-0.79.0/pyproject.toml
+-rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 kolena_client-0.79.0/PKG-INFO
```

### Comparing `kolena_client-0.78.0/LICENSE` & `kolena_client-0.79.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/LICENSE_HEADER` & `kolena_client-0.79.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/README.md` & `kolena_client-0.79.0/README.md`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/__init__.py` & `kolena_client-0.79.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_api/__init__.py` & `kolena_client-0.79.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_api/v1/__init__.py` & `kolena_client-0.79.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_api/v1/batched_load.py` & `kolena_client-0.79.0/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_api/v1/client_log.py` & `kolena_client-0.79.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_api/v1/core.py` & `kolena_client-0.79.0/kolena/_api/v1/core.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_api/v1/detection.py` & `kolena_client-0.79.0/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_api/v1/fr.py` & `kolena_client-0.79.0/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_api/v1/generic.py` & `kolena_client-0.79.0/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_api/v1/repository.py` & `kolena_client-0.79.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_api/v1/token.py` & `kolena_client-0.79.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_api/v1/workflow.py` & `kolena_client-0.79.0/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_experimental/__init__.py` & `kolena_client-0.79.0/kolena/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_experimental/object_detection/__init__.py` & `kolena_client-0.79.0/kolena/_experimental/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_experimental/object_detection/evaluator.py` & `kolena_client-0.79.0/kolena/_experimental/object_detection/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_experimental/object_detection/evaluator_multiclass.py` & `kolena_client-0.79.0/kolena/_experimental/object_detection/evaluator_multiclass.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_experimental/object_detection/evaluator_single_class.py` & `kolena_client-0.79.0/kolena/_experimental/object_detection/evaluator_single_class.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_experimental/object_detection/utils.py` & `kolena_client-0.79.0/kolena/_experimental/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_experimental/object_detection/workflow.py` & `kolena_client-0.79.0/kolena/_experimental/object_detection/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_extras/__init__.py` & `kolena_client-0.79.0/kolena/_experimental/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_extras/metrics/__init__.py` & `kolena_client-0.79.0/kolena/_extras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_extras/metrics/sklearn.py` & `kolena_client-0.79.0/kolena/_extras/metrics/sklearn.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/__init__.py` & `kolena_client-0.79.0/kolena/_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/asset_path_mapper.py` & `kolena_client-0.79.0/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/batched_load.py` & `kolena_client-0.79.0/kolena/_utils/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/cli.py` & `kolena_client-0.79.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/consts.py` & `kolena_client-0.79.0/kolena/_utils/consts.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/dataframes/__init__.py` & `kolena_client-0.79.0/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/dataframes/validators.py` & `kolena_client-0.79.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/datatypes.py` & `kolena_client-0.79.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/endpoints.py` & `kolena_client-0.79.0/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/frozen.py` & `kolena_client-0.79.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/geometry.py` & `kolena_client-0.79.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/inference_validators.py` & `kolena_client-0.79.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/instrumentation.py` & `kolena_client-0.79.0/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/krequests.py` & `kolena_client-0.79.0/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/log.py` & `kolena_client-0.79.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/repository.py` & `kolena_client-0.79.0/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/serde.py` & `kolena_client-0.79.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/serializable.py` & `kolena_client-0.79.0/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/state.py` & `kolena_client-0.79.0/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/uninstantiable.py` & `kolena_client-0.79.0/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/_utils/validators.py` & `kolena_client-0.79.0/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/classification/__init__.py` & `kolena_client-0.79.0/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/classification/metadata.py` & `kolena_client-0.79.0/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/classification/model.py` & `kolena_client-0.79.0/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/classification/multiclass/__init__.py` & `kolena_client-0.79.0/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/classification/multiclass/_utils.py` & `kolena_client-0.79.0/kolena/classification/multiclass/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/classification/multiclass/evaluator.py` & `kolena_client-0.79.0/kolena/classification/multiclass/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/classification/multiclass/test_run.py` & `kolena_client-0.79.0/kolena/classification/multiclass/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/classification/multiclass/workflow.py` & `kolena_client-0.79.0/kolena/classification/multiclass/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/classification/test_case.py` & `kolena_client-0.79.0/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/classification/test_config.py` & `kolena_client-0.79.0/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/classification/test_image.py` & `kolena_client-0.79.0/kolena/classification/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/classification/test_run.py` & `kolena_client-0.79.0/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/classification/test_suite.py` & `kolena_client-0.79.0/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/__init__.py` & `kolena_client-0.79.0/kolena/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/_datatypes.py` & `kolena_client-0.79.0/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/_internal/__init__.py` & `kolena_client-0.79.0/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/_internal/datatypes.py` & `kolena_client-0.79.0/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/_internal/ground_truth.py` & `kolena_client-0.79.0/kolena/detection/_internal/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/_internal/inference.py` & `kolena_client-0.79.0/kolena/detection/_internal/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/_internal/metadata.py` & `kolena_client-0.79.0/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/_internal/model.py` & `kolena_client-0.79.0/kolena/detection/_internal/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/_internal/test_case.py` & `kolena_client-0.79.0/kolena/detection/_internal/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/_internal/test_config.py` & `kolena_client-0.79.0/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/_internal/test_image.py` & `kolena_client-0.79.0/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/_internal/test_run.py` & `kolena_client-0.79.0/kolena/detection/_internal/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/_internal/test_suite.py` & `kolena_client-0.79.0/kolena/detection/_internal/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/ground_truth.py` & `kolena_client-0.79.0/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/inference.py` & `kolena_client-0.79.0/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/metadata.py` & `kolena_client-0.79.0/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/model.py` & `kolena_client-0.79.0/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/test_case.py` & `kolena_client-0.79.0/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/test_config.py` & `kolena_client-0.79.0/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/test_image.py` & `kolena_client-0.79.0/kolena/detection/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/test_run.py` & `kolena_client-0.79.0/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/detection/test_suite.py` & `kolena_client-0.79.0/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/errors.py` & `kolena_client-0.79.0/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/fr/__init__.py` & `kolena_client-0.79.0/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/fr/_utils.py` & `kolena_client-0.79.0/kolena/fr/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/fr/datatypes.py` & `kolena_client-0.79.0/kolena/fr/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/fr/model.py` & `kolena_client-0.79.0/kolena/fr/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/fr/test_case.py` & `kolena_client-0.79.0/kolena/fr/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/fr/test_images.py` & `kolena_client-0.79.0/kolena/fr/test_images.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/fr/test_run.py` & `kolena_client-0.79.0/kolena/fr/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/fr/test_suite.py` & `kolena_client-0.79.0/kolena/fr/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/initialize.py` & `kolena_client-0.79.0/kolena/initialize.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/__init__.py` & `kolena_client-0.79.0/kolena/workflow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .test_sample import ImageText
 from .test_sample import TestSample
 from .test_sample import Composite
 from .test_sample import Text
 from .test_sample import BaseVideo
 from .test_sample import Video
 from .test_sample import Document
+from .test_sample import PointCloud
 from .ground_truth import GroundTruth
 from .inference import Inference
 from .workflow import Workflow
 from .test_case import TestCase
 from .test_suite import TestSuite
 from .model import Model
 from .plot import AxisConfig
@@ -57,14 +58,15 @@
     "ImageText",
     "TestSample",
     "Composite",
     "Text",
     "BaseVideo",
     "Video",
     "Document",
+    "PointCloud",
     "GroundTruth",
     "Inference",
     "Workflow",
     "TestCase",
     "TestSuite",
     "Model",
     "AxisConfig",
```

### Comparing `kolena_client-0.78.0/kolena/workflow/_datatypes.py` & `kolena_client-0.79.0/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/_validators.py` & `kolena_client-0.79.0/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/annotation.py` & `kolena_client-0.79.0/kolena/workflow/annotation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/asset.py` & `kolena_client-0.79.0/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/define_workflow.py` & `kolena_client-0.79.0/kolena/workflow/define_workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/evaluator.py` & `kolena_client-0.79.0/kolena/workflow/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/evaluator_function.py` & `kolena_client-0.79.0/kolena/workflow/evaluator_function.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/ground_truth.py` & `kolena_client-0.79.0/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/inference.py` & `kolena_client-0.79.0/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/metrics/__init__.py` & `kolena_client-0.79.0/kolena/workflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/metrics/_formula.py` & `kolena_client-0.79.0/kolena/workflow/metrics/_formula.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/metrics/_geometry.py` & `kolena_client-0.79.0/kolena/workflow/metrics/_geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/model.py` & `kolena_client-0.79.0/kolena/workflow/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/plot.py` & `kolena_client-0.79.0/kolena/workflow/plot.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/test_case.py` & `kolena_client-0.79.0/kolena/workflow/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/test_run.py` & `kolena_client-0.79.0/kolena/workflow/test_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     def __init__(
         self,
         model: Model,
         test_suite: TestSuite,
         evaluator: Union[Evaluator, BasicEvaluatorFunction, None] = None,
         configurations: Optional[List[EvaluatorConfiguration]] = None,
         reset: bool = False,
+        dry_run: bool = False,
     ):
         if configurations is None:
             configurations = []
 
         if model.workflow != test_suite.workflow:
             raise WorkflowMismatchError(
                 f"model workflow ({model.workflow}) does not match test suite workflow ({test_suite.workflow})",
@@ -115,14 +116,15 @@
             log.info("not overwriting any existing inferences from this model (reset=False)")
 
         self.model = model
         self.test_suite = test_suite
         self.evaluator = evaluator
         self.configurations = self.evaluator.configurations if isinstance(evaluator, Evaluator) else configurations
         self.reset = reset
+        self.dry_run = dry_run
 
         evaluator_display_name = (
             None
             if evaluator is None
             else evaluator.display_name()
             if isinstance(evaluator, Evaluator)
             else evaluator.__name__
@@ -144,32 +146,34 @@
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(res)
         response = from_dict(data_class=API.CreateOrRetrieveResponse, data=res.json())
         self._id = response.test_run_id
         self._freeze()
 
-    def run(self) -> None:
+    def run(self) -> Dict[str, Any]:
         """
         Run the testing process, first extracting inferences for all test samples in the test suite then performing
         evaluation.
         """
         try:
             inferences = []
             for ts in log.progress_bar(self.iter_test_samples(), desc="performing inference"):
                 if self.model.infer is None:  # only fail when `infer` is necessary
                     raise ValueError("model must implement `infer`")
                 inferences.append((ts, self.model.infer(ts)))
 
             if len(inferences) > 0:
                 log.success(f"performed inference on {len(inferences)} test samples")
-                log.info("uploading inferences")
-                self.upload_inferences(inferences)
+                if not self.dry_run:
+                    log.info("uploading inferences")
+                    self.upload_inferences(inferences)
 
-            self.evaluate()
+            metrics = self.evaluate()
+            return dict(inferences=inferences, metrics=metrics)
         except Exception as e:
             report_crash(self._id, API.Path.MARK_CRASHED.value)
             raise e
 
     def load_test_samples(self) -> List[TestSample]:
         """
         Load the test samples in the test suite that do not yet have inferences uploaded.
@@ -232,36 +236,38 @@
         request = API.UploadInferencesRequest(uuid=init_response.uuid, test_run_id=self._id, reset=self.reset)
         res = krequests.put(
             endpoint_path=API.Path.UPLOAD_INFERENCES.value,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(res)
 
-    def evaluate(self) -> None:
+    def evaluate(self) -> Dict[str, Any]:
         """
         Perform evaluation by computing metrics for individual test samples, in aggregate across test cases, and across
         the complete test suite at each [`EvaluatorConfiguration`][kolena.workflow.EvaluatorConfiguration].
         """
-        if self.evaluator is None:
+        if self.evaluator is None and not self.dry_run:
             log.info("commencing server side metrics evaluation")
             self._start_server_side_evaluation()
-            return
+            return {}
 
         # TODO: assert that testing is complete?
         t0 = time.time()
         log.info("commencing evaluation")
         if isinstance(self.evaluator, Evaluator):
-            self._perform_evaluation(self.evaluator)
+            metrics = self._perform_evaluation(self.evaluator)
         else:
-            self._perform_streamlined_evaluation(self.evaluator)
+            metrics = self._perform_streamlined_evaluation(self.evaluator)
 
         log.success(f"completed evaluation in {time.time() - t0:0.1f} seconds")
         log.success(f"results: {get_results_url(self.model.workflow.name, self.model._id, self.test_suite._id)}")
 
-    def _perform_evaluation(self, evaluator: Evaluator) -> None:
+        return metrics
+
+    def _perform_evaluation(self, evaluator: Evaluator) -> Dict[str, Any]:
         configurations: Sequence[Optional[EvaluatorConfiguration]] = (
             cast(Sequence[Optional[EvaluatorConfiguration]], evaluator.configurations)
             if len(evaluator.configurations) > 0
             else [None]
         )
         test_case_metrics: Dict[int, Dict[Optional[EvaluatorConfiguration], MetricsTestCase]] = {}
         test_case_plots: Dict[int, Dict[Optional[EvaluatorConfiguration], Optional[List[Plot]]]] = {}
@@ -273,34 +279,36 @@
             inferences = self.model.load_inferences(test_case)
 
             for configuration in configurations:
                 configuration_description = _configuration_description(configuration)
                 log.info(f"computing test sample metrics {configuration_description}")
                 metrics_test_sample = evaluator.compute_test_sample_metrics(test_case, inferences, configuration)
 
-                log.info(f"uploading test sample metrics {configuration_description}")
-                self._upload_test_sample_metrics(test_case, metrics_test_sample, configuration)
+                if not self.dry_run:
+                    log.info(f"uploading test sample metrics {configuration_description}")
+                    self._upload_test_sample_metrics(test_case, metrics_test_sample, configuration)
 
                 log.info(f"computing test case metrics {configuration_description}")
                 # TODO: sort? order returned from evaluator may not match inferences order
                 mts = [metrics for _, metrics in metrics_test_sample]
                 metrics_test_case = evaluator.compute_test_case_metrics(test_case, inferences, mts, configuration)
                 test_case_metrics_by_config[configuration] = metrics_test_case
 
                 log.info(f"computing test case plots {configuration_description}")
                 plots_test_case = evaluator.compute_test_case_plots(test_case, inferences, mts, configuration)
                 test_case_plots_by_config[configuration] = plots_test_case
 
             test_case_metrics[test_case._id] = test_case_metrics_by_config
             test_case_plots[test_case._id] = test_case_plots_by_config
 
-        log.info("uploading test case metrics")
-        self._upload_test_case_metrics(test_case_metrics)
-        log.info("uploading test case plots")
-        self._upload_test_case_plots(test_case_plots)
+        if not self.dry_run:
+            log.info("uploading test case metrics")
+            self._upload_test_case_metrics(test_case_metrics)
+            log.info("uploading test case plots")
+            self._upload_test_case_plots(test_case_plots)
 
         log.info("computing test suite metrics")
         test_suite_metrics: Dict[Optional[EvaluatorConfiguration], Optional[MetricsTestSuite]] = {}
         for configuration in configurations:
             test_case_with_metrics = [
                 (tc, test_case_metrics[tc._id][configuration]) for tc in self.test_suite.test_cases
             ]
@@ -308,18 +316,25 @@
             metrics_test_suite = evaluator.compute_test_suite_metrics(
                 self.test_suite,
                 test_case_with_metrics,
                 configuration,
             )
             test_suite_metrics[configuration] = metrics_test_suite
 
-        log.info("uploading test suite metrics")
-        self._upload_test_suite_metrics(test_suite_metrics)
+        if not self.dry_run:
+            log.info("uploading test suite metrics")
+            self._upload_test_suite_metrics(test_suite_metrics)
+
+        return dict(
+            test_case_metrics=test_case_metrics,
+            test_case_plots=test_case_plots,
+            test_suite_metrics=test_suite_metrics,
+        )
 
-    def _perform_streamlined_evaluation(self, evaluator: BasicEvaluatorFunction) -> None:
+    def _perform_streamlined_evaluation(self, evaluator: BasicEvaluatorFunction) -> Dict[str, Any]:
         test_samples, ground_truths, inferences = [], [], []
         for sample, gt, inf in self._iter_all_inferences():
             test_samples.append(sample)
             ground_truths.append(gt)
             inferences.append(inf)
         test_case_membership: List[Tuple[TestCase, List[TestSample]]] = self.test_suite.load_test_samples()
         test_case_test_samples = _TestCases(
@@ -333,16 +348,21 @@
         test_suite_metrics: Dict[Optional[EvaluatorConfiguration], MetricsTestSuite] = dict()
 
         def process_results(results: Optional[EvaluationResults], config: Optional[EvaluatorConfiguration]) -> None:
             if results is None:
                 log.info(f"no results {_configuration_description(config)}")
                 return
 
-            log.info(f"uploading test sample metrics {_configuration_description(config)}")
-            self._upload_test_sample_metrics(test_case=None, metrics=results.metrics_test_sample, configuration=config)
+            if not self.dry_run:
+                log.info(f"uploading test sample metrics {_configuration_description(config)}")
+                self._upload_test_sample_metrics(
+                    test_case=None,
+                    metrics=results.metrics_test_sample,
+                    configuration=config,
+                )
             for test_case, metrics in results.metrics_test_case:
                 test_case_metrics[test_case._id][config] = metrics
             for test_case, plots in results.plots_test_case:
                 test_case_plots[test_case._id][config] = plots
             if results.metrics_test_suite is not None:
                 test_suite_metrics[config] = results.metrics_test_suite
 
@@ -358,20 +378,27 @@
                 )
                 process_results(evaluation_results, configuration)
         else:
             test_case_test_samples._set_configuration(None)
             evaluation_results = evaluator(test_samples, ground_truths, inferences, test_case_test_samples)
             process_results(evaluation_results, None)
 
-        log.info("uploading test case metrics")
-        self._upload_test_case_metrics(test_case_metrics)
-        log.info("uploading test case plots")
-        self._upload_test_case_plots(test_case_plots)
-        log.info("uploading test suite metrics")
-        self._upload_test_suite_metrics(test_suite_metrics)
+        if not self.dry_run:
+            log.info("uploading test case metrics")
+            self._upload_test_case_metrics(test_case_metrics)
+            log.info("uploading test case plots")
+            self._upload_test_case_plots(test_case_plots)
+            log.info("uploading test suite metrics")
+            self._upload_test_suite_metrics(test_suite_metrics)
+
+        return dict(
+            test_case_metrics=test_case_metrics,
+            test_case_plots=test_case_plots,
+            test_suite_metrics=test_suite_metrics,
+        )
 
     def _iter_test_samples_batch(
         self,
         batch_size: int = BatchSize.LOAD_SAMPLES.value,
     ) -> Iterator[TestSampleDataFrame]:
         if batch_size <= 0:
             raise InputValidationError(f"invalid batch_size '{batch_size}': expected positive integer")
@@ -474,15 +501,16 @@
 @validate_arguments(config=ValidatorConfig)
 def test(
     model: Model,
     test_suite: TestSuite,
     evaluator: Union[Evaluator, BasicEvaluatorFunction, None] = None,
     configurations: Optional[List[EvaluatorConfiguration]] = None,
     reset: bool = False,
-) -> None:
+    dry_run: bool = False,
+) -> Dict[str, Any]:
     """
     Test a [`Model`][kolena.workflow.Model] on a [`TestSuite`][kolena.workflow.TestSuite] using a specific
     [`Evaluator`][kolena.workflow.Evaluator] implementation.
 
     ```python
     from kolena.workflow import test
 
@@ -494,8 +522,8 @@
     :param evaluator: An optional evaluator implementation.
         Requires a previously configured server-side evaluator to default to if omitted.
         (Please see [`BasicEvaluatorFunction`][kolena.workflow.evaluator_function.BasicEvaluatorFunction] for type
         definition.)
     :param configurations: A list of configurations to use when running the evaluator.
     :param reset: Overwrites existing inferences if set.
     """
-    TestRun(model, test_suite, evaluator, configurations, reset).run()
+    return TestRun(model, test_suite, evaluator, configurations, reset, dry_run).run()
```

### Comparing `kolena_client-0.78.0/kolena/workflow/test_sample.py` & `kolena_client-0.79.0/kolena/workflow/test_sample.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 
 class _TestSampleType(DataType):
     IMAGE = "IMAGE"
     TEXT = "TEXT"
     VIDEO = "VIDEO"
     DOCUMENT = "DOCUMENT"
     COMPOSITE = "COMPOSITE"
+    POINT_CLOUD = "POINT_CLOUD"
     CUSTOM = "CUSTOM"
 
     @staticmethod
     def _data_category() -> str:
         return "TEST_SAMPLE"
 
 
@@ -263,15 +264,27 @@
     """URL (e.g. S3, HTTPS) of the document."""
 
     @classmethod
     def _data_type(cls) -> _TestSampleType:
         return _TestSampleType.DOCUMENT
 
 
-_TEST_SAMPLE_BASE_TYPES = [Composite, Image, Text, BaseVideo, Document]
+@dataclass(frozen=True, config=ValidatorConfig)
+class PointCloud(TestSample):
+    """A pointcloud file located in a cloud bucket or served at a URL."""
+
+    locator: str
+    """The URL of the pointcloud file, using e.g. `s3`, `gs`, or `https` scheme (`s3://my-bucket/path/to/image.pcd`)."""
+
+    @classmethod
+    def _data_type(cls) -> _TestSampleType:
+        return _TestSampleType.POINT_CLOUD
+
+
+_TEST_SAMPLE_BASE_TYPES = [Composite, Image, Text, BaseVideo, Document, PointCloud]
 
 
 def _validate_test_sample_type(test_sample_type: Type[TestSample], recurse: bool = True) -> None:
     if not issubclass(test_sample_type, TestSample):
         raise ValueError(f"Test sample must subclass {TestSample.__name__}")
 
     if (
```

### Comparing `kolena_client-0.78.0/kolena/workflow/test_suite.py` & `kolena_client-0.79.0/kolena/workflow/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/visualization/__init__.py` & `kolena_client-0.79.0/kolena/workflow/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/visualization/_activation_map.py` & `kolena_client-0.79.0/kolena/workflow/visualization/_activation_map.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/visualization/_utils.py` & `kolena_client-0.79.0/kolena/workflow/visualization/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/kolena/workflow/workflow.py` & `kolena_client-0.79.0/kolena/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.78.0/pyproject.toml` & `kolena_client-0.79.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena-client"
-version = "0.78.0"  # version is automatically set to latest git tag during release process
+version = "0.79.0"  # version is automatically set to latest git tag during release process
 description = "Client for Kolena's machine learning testing platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
```

### Comparing `kolena_client-0.78.0/PKG-INFO` & `kolena_client-0.79.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena-client
-Version: 0.78.0
+Version: 0.79.0
 Summary: Client for Kolena's machine learning testing platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
 Requires-Python: >=3.7.1,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena-client Version: 0.78.0 Summary: Client for
+Metadata-Version: 2.1 Name: kolena-client Version: 0.79.0 Summary: Client for
 Kolena's machine learning testing platform. Home-page: https://kolena.io
 License: Apache-2.0 Keywords: Kolena,ML,testing Author: Kolena Engineering
 Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.12 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

