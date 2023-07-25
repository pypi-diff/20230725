# Comparing `tmp/substrafl-0.38.0rc1.tar.gz` & `tmp/substrafl-0.39.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrafl-0.38.0rc1.tar", last modified: Tue Jun 27 09:44:58 2023, max compression
+gzip compressed data, was "substrafl-0.39.0rc1.tar", last modified: Tue Jul 25 15:09:01 2023, max compression
```

## Comparing `substrafl-0.38.0rc1.tar` & `substrafl-0.39.0rc1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.935521 substrafl-0.38.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-27 09:44:58.935521 substrafl-0.38.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 09:44:58.935521 substrafl-0.38.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.927521 substrafl-0.38.0rc1/substrafl/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.927521 substrafl-0.38.0rc1/substrafl/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    23454 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/algorithms/pytorch/weight_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/compute_plan_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/dependency/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/dependency/path_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/dependency/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/evaluation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/index_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/index_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/index_generator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/index_generator/np_index_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    18182 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/model_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/aggregation_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/nodes/references/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/references/local_state.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/references/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/test_data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/nodes/train_data_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/remote/register/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/register/generate_wheel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/register/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/remote_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.931521 substrafl-0.38.0rc1/substrafl/remote/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/serializers/pickle_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/serializers/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/remote/substratools_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.935521 substrafl-0.38.0rc1/substrafl/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/fed_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/fed_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/newton_raphson.py
--rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/single_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-06-27 09:44:55.000000 substrafl-0.38.0rc1/substrafl/strategies/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:44:58.927521 substrafl-0.38.0rc1/substrafl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-27 09:44:58.000000 substrafl-0.38.0rc1/substrafl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-27 09:44:58.000000 substrafl-0.38.0rc1/substrafl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:44:58.000000 substrafl-0.38.0rc1/substrafl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-27 09:44:58.000000 substrafl-0.38.0rc1/substrafl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 09:44:58.000000 substrafl-0.38.0rc1/substrafl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:09:01.540048 substrafl-0.39.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-25 15:09:01.540048 substrafl-0.39.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:09:01.540048 substrafl-0.39.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:09:01.532048 substrafl-0.39.0rc1/substrafl/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:09:01.532048 substrafl-0.39.0rc1/substrafl/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/algorithms/algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:09:01.536048 substrafl-0.39.0rc1/substrafl/algorithms/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/algorithms/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18146 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23454 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/algorithms/pytorch/weight_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/compute_plan_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:09:01.536048 substrafl-0.39.0rc1/substrafl/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/dependency/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/dependency/path_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/dependency/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/evaluation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:09:01.536048 substrafl-0.39.0rc1/substrafl/index_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/index_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/index_generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/index_generator/np_index_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/model_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:09:01.536048 substrafl-0.39.0rc1/substrafl/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/nodes/aggregation_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/nodes/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:09:01.536048 substrafl-0.39.0rc1/substrafl/nodes/references/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/nodes/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/nodes/references/local_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/nodes/references/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/nodes/test_data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13180 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/nodes/train_data_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:09:01.536048 substrafl-0.39.0rc1/substrafl/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/remote/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/remote/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:09:01.536048 substrafl-0.39.0rc1/substrafl/remote/register/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/remote/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/remote/register/generate_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/remote/register/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/remote/remote_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:09:01.536048 substrafl-0.39.0rc1/substrafl/remote/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/remote/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/remote/serializers/pickle_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/remote/serializers/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/remote/substratools_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:09:01.540048 substrafl-0.39.0rc1/substrafl/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/strategies/fed_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/strategies/fed_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/strategies/newton_raphson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/strategies/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/strategies/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/strategies/single_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-07-25 15:08:50.000000 substrafl-0.39.0rc1/substrafl/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:09:01.532048 substrafl-0.39.0rc1/substrafl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-25 15:09:01.000000 substrafl-0.39.0rc1/substrafl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-25 15:09:01.000000 substrafl-0.39.0rc1/substrafl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:09:01.000000 substrafl-0.39.0rc1/substrafl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-25 15:09:01.000000 substrafl-0.39.0rc1/substrafl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 15:09:01.000000 substrafl-0.39.0rc1/substrafl.egg-info/top_level.txt
```

### Comparing `substrafl-0.38.0rc1/LICENSE` & `substrafl-0.39.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/PKG-INFO` & `substrafl-0.39.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrafl
-Version: 0.38.0rc1
+Version: 0.39.0rc1
 Summary: A high-level federated learning Python library to run      federated learning experiments at scale on a Substra network
 Home-page: https://docs.substra.org/
 Author: Owkin, Inc.
 License: Apache 2.0
 Description: readme
 Keywords: substrafl
 Platform: UNKNOWN
```

### Comparing `substrafl-0.38.0rc1/README.md` & `substrafl-0.39.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/pyproject.toml` & `substrafl-0.39.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/setup.py` & `substrafl-0.39.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     packages=find_packages(exclude=["tests*", "benchmark*"]),
     # Not compatible with substratools 0.8.0 because
     # that release is private and in the Docker container
     # it has access only to the public PyPi
     install_requires=[
         "numpy>=1.20.3, <1.24",
         "cloudpickle>=1.6.0",
-        "substra~=0.45.0",
+        "substra~=0.46.0rc1",
         "substratools~=0.20.0",
-        "pydantic>=1.9.0",
+        "pydantic>=1.9.0, <2.0",
         "pip>=21.2",
         "wheel",
         "six",
         "packaging",
     ],
     extras_require={
         "dev": [
```

### Comparing `substrafl-0.38.0rc1/substrafl/__init__.py` & `substrafl-0.39.0rc1/substrafl/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/algorithms/algo.py` & `substrafl-0.39.0rc1/substrafl/algorithms/algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/__init__.py` & `substrafl-0.39.0rc1/substrafl/algorithms/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py` & `substrafl-0.39.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             raise BatchSizeNotFoundError(
                 "No default batch size has been found to perform local prediction. "
                 "Please overwrite the _local_predict function of your algorithm."
             )
 
         self._model.eval()
 
-        predictions = torch.Tensor([])
+        predictions = torch.Tensor([]).to(self._device)
         with torch.inference_mode():
             for x in predict_loader:
                 x = x.to(self._device)
                 predictions = torch.cat((predictions, self._model(x)), 0)
 
         predictions = predictions.cpu().detach()
         self._save_predictions(predictions, predictions_path)
```

### Comparing `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py` & `substrafl-0.39.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py` & `substrafl-0.39.0rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py` & `substrafl-0.39.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
             predict_dataset (torch.utils.data.Dataset): predict_dataset build from the x returned by the opener.
         """
         dataloader_batchsize = min(self._batch_size, len(predict_dataset)) if self._batch_size else len(predict_dataset)
         predict_loader = torch.utils.data.DataLoader(predict_dataset, batch_size=dataloader_batchsize)
 
         self._model.eval()
 
-        predictions = torch.Tensor([])
+        predictions = torch.Tensor([]).to(self._device)
         with torch.inference_mode():
             for x in predict_loader:
                 x = x.to(self._device)
                 predictions = torch.cat((predictions, self._model(x)), 0)
 
         predictions = predictions.cpu().detach()
```

### Comparing `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py` & `substrafl-0.39.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py` & `substrafl-0.39.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/algorithms/pytorch/weight_manager.py` & `substrafl-0.39.0rc1/substrafl/algorithms/pytorch/weight_manager.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/compute_plan_builder.py` & `substrafl-0.39.0rc1/substrafl/compute_plan_builder.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/dependency/constants.py` & `substrafl-0.39.0rc1/substrafl/dependency/constants.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/dependency/path_management.py` & `substrafl-0.39.0rc1/substrafl/dependency/path_management.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/dependency/schemas.py` & `substrafl-0.39.0rc1/substrafl/dependency/schemas.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/evaluation_strategy.py` & `substrafl-0.39.0rc1/substrafl/evaluation_strategy.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/exceptions.py` & `substrafl-0.39.0rc1/substrafl/exceptions.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/experiment.py` & `substrafl-0.39.0rc1/substrafl/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,29 +114,29 @@
 
 def _save_experiment_summary(
     experiment_folder: Path,
     compute_plan_key: str,
     strategy: ComputePlanBuilder,
     num_rounds: int,
     operation_cache: Dict[RemoteStruct, OperationKey],
-    train_data_nodes: TrainDataNode,
+    train_data_nodes: List[TrainDataNode],
     aggregation_node: Optional[AggregationNode],
     evaluation_strategy: EvaluationStrategy,
     timestamp: str,
     additional_metadata: Optional[Dict],
 ):
     """Saves the experiment summary in `experiment_folder`, with the name format `{timestamp}_{compute_plan.key}.json`
 
     Args:
         experiment_folder (typing.Union[str, pathlib.Path]): path to the folder where the experiment summary is saved.
         compute_plan_key (str): compute plan key
         strategy (substrafl.strategies.Strategy): strategy
         num_rounds (int): num_rounds
         operation_cache (typing.Dict[RemoteStruct, OperationKey]): operation_cache
-        train_data_nodes (TrainDataNode): train_data_nodes
+        train_data_nodes (typing.List[TrainDataNode]): train_data_nodes
         aggregation_node (typing.Optional[AggregationNode]): aggregation_node
         evaluation_strategy (EvaluationStrategy): evaluation_strategy
         timestamp (str): timestamp with "%Y_%m_%d_%H_%M_%S" format
         additional_metadata (dict, Optional): Optional dictionary of metadata to be shown on the Substra WebApp.
     """
     # create the experiment folder if it doesn't exist
     experiment_folder = Path(experiment_folder)
```

### Comparing `substrafl-0.38.0rc1/substrafl/index_generator/base.py` & `substrafl-0.39.0rc1/substrafl/index_generator/base.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/index_generator/np_index_generator.py` & `substrafl-0.39.0rc1/substrafl/index_generator/np_index_generator.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/logger.py` & `substrafl-0.39.0rc1/substrafl/logger.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/model_loading.py` & `substrafl-0.39.0rc1/substrafl/model_loading.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,15 @@
                 "The instance from the given input folder requires the installation of "
                 "additional dependencies. Those can be found in "
                 f"{str(folder / 'substrafl_internal' / 'installable_library')}"
                 f"\nFull trace of the error: {e}"
             )
 
     else:
-        loaded_instance = instance.load_model(folder / metadata[MODEL_DICT_KEY])
+        loaded_instance = instance.load_shared(folder / metadata[MODEL_DICT_KEY])
 
     return loaded_instance
 
 
 def _download_task_output_files(
     *,
     client: substra.Client,
@@ -467,12 +467,12 @@
         _download_task_output_files(
             client=client,
             compute_plan_key=compute_plan_key,
             dest_folder=temp_folder,
             round_idx=round_idx,
             rank_idx=rank_idx,
             task_type=TaskType.AGGREGATE,
-            identifier=OutputIdentifiers.model,
+            identifier=OutputIdentifiers.shared,
         )
         aggregated = _load_from_files(input_folder=temp_folder, remote=True)
 
     return aggregated
```

### Comparing `substrafl-0.38.0rc1/substrafl/nodes/__init__.py` & `substrafl-0.39.0rc1/substrafl/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/nodes/aggregation_node.py` & `substrafl-0.39.0rc1/substrafl/nodes/aggregation_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             )
 
         op_id = str(uuid.uuid4())
 
         inputs = (
             [
                 substra.schemas.InputRef(
-                    identifier=InputIdentifiers.models,
+                    identifier=InputIdentifiers.shared,
                     parent_task_key=ref.key,
                     parent_task_output_identifier=OutputIdentifiers.shared,
                 )
                 for ref in operation.shared_states
             ]
             if operation.shared_states is not None
             else None
@@ -79,15 +79,15 @@
 
         task_metadata = {"round_idx": round_idx} if round_idx is not None else {}
         aggregate_task = substra.schemas.ComputePlanTaskSpec(
             function_key=str(uuid.uuid4()),  # bogus function key
             task_id=op_id,
             inputs=inputs,
             outputs={
-                OutputIdentifiers.model: substra.schemas.ComputeTaskOutputSpec(
+                OutputIdentifiers.shared: substra.schemas.ComputeTaskOutputSpec(
                     permissions=substra.schemas.Permissions(public=False, authorized_ids=list(authorized_ids)),
                     transient=clean_models,
                 )
             },
             metadata=task_metadata,
             tag=TaskType.AGGREGATE,
             worker=self.organization_id,
@@ -135,23 +135,23 @@
                     function_key = register_function(
                         client=client,
                         remote_struct=remote_struct,
                         permissions=permissions,
                         dependencies=dependencies,
                         inputs=[
                             substra.schemas.FunctionInputSpec(
-                                identifier=InputIdentifiers.models,
+                                identifier=InputIdentifiers.shared,
                                 kind=substra.schemas.AssetKind.model.value,
                                 optional=False,
                                 multiple=True,
                             )
                         ],
                         outputs=[
                             substra.schemas.FunctionOutputSpec(
-                                identifier=OutputIdentifiers.model,
+                                identifier=OutputIdentifiers.shared,
                                 kind=substra.schemas.AssetKind.model.value,
                                 multiple=False,
                             )
                         ],
                     )
                     cache[remote_struct] = function_key
                 else:
```

### Comparing `substrafl-0.38.0rc1/substrafl/nodes/node.py` & `substrafl-0.39.0rc1/substrafl/nodes/node.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,25 @@
 
 OperationKey = NewType("OperationKey", str)
 
 
 class InputIdentifiers(str, Enum):
     local = "local"
     shared = "shared"
-    model = "model"
-    models = "models"
     predictions = "predictions"
     opener = "opener"
     datasamples = "datasamples"
     rank = "rank"
     X = "X"
     y = "y"
 
 
 class OutputIdentifiers(str, Enum):
     local = "local"
     shared = "shared"
-    model = "model"
     predictions = "predictions"
 
 
 class Node:
     def __init__(self, organization_id: str):
         self.organization_id = organization_id
         self.tasks: List[Dict] = []
```

### Comparing `substrafl-0.38.0rc1/substrafl/nodes/test_data_node.py` & `substrafl-0.39.0rc1/substrafl/nodes/test_data_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/nodes/train_data_node.py` & `substrafl-0.39.0rc1/substrafl/nodes/train_data_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
             else []
         )
         if operation.shared_state is not None:
             shared_inputs = [
                 substra.schemas.InputRef(
                     identifier=InputIdentifiers.shared,
                     parent_task_key=operation.shared_state.key,
-                    parent_task_output_identifier=OutputIdentifiers.model,
+                    parent_task_output_identifier=OutputIdentifiers.shared,
                 )
             ]
 
         elif local_state is not None and not local_state.init:
             # If the parent task is an init task, no shared states have been produced.
             shared_inputs = [
                 substra.schemas.InputRef(
```

### Comparing `substrafl-0.38.0rc1/substrafl/remote/decorators.py` & `substrafl-0.39.0rc1/substrafl/remote/decorators.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/remote/operations.py` & `substrafl-0.39.0rc1/substrafl/remote/operations.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/remote/register/generate_wheel.py` & `substrafl-0.39.0rc1/substrafl/remote/register/generate_wheel.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/remote/register/register.py` & `substrafl-0.39.0rc1/substrafl/remote/register/register.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/remote/remote_struct.py` & `substrafl-0.39.0rc1/substrafl/remote/remote_struct.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/remote/serializers/pickle_serializer.py` & `substrafl-0.39.0rc1/substrafl/remote/serializers/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/remote/substratools_methods.py` & `substrafl-0.39.0rc1/substrafl/remote/substratools_methods.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import os
+from collections.abc import Iterable
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import Type
 from typing import TypedDict
+from typing import Union
 
 import substratools as tools
 
 from substrafl.nodes.node import InputIdentifiers
 from substrafl.nodes.node import OutputIdentifiers
 from substrafl.remote.serializers.pickle_serializer import PickleSerializer
 from substrafl.remote.serializers.serializer import Serializer
@@ -44,28 +47,31 @@
 
         loaded_inputs = {}
 
         instance_path = inputs.get(InputIdentifiers.local)
         if instance_path is not None:
             self.instance = self.load_instance(instance_path)
 
-        if InputIdentifiers.models in inputs:
-            models = []
-            for m_path in inputs[InputIdentifiers.models]:
-                models.append(self.load_model(m_path))
-            loaded_inputs["shared_states"] = models
+        if InputIdentifiers.shared in inputs:
+            input_shared = inputs[InputIdentifiers.shared]
+            if input_shared is None:
+                loaded_inputs["shared_state"] = None
+
+            elif isinstance(input_shared, str) or isinstance(input_shared, Path):
+                loaded_inputs["shared_state"] = self.load_shared(input_shared)
+
+            elif isinstance(input_shared, Iterable):
+                shared_states = []
+                for m_path in input_shared:
+                    shared_states.append(self.load_shared(m_path))
+                loaded_inputs["shared_states"] = shared_states
 
         if InputIdentifiers.datasamples in inputs:
             loaded_inputs["datasamples"] = inputs[InputIdentifiers.datasamples]
 
-        if InputIdentifiers.shared in inputs:
-            loaded_inputs["shared_state"] = (
-                self.load_model(inputs[InputIdentifiers.shared]) if inputs[InputIdentifiers.shared] else None
-            )
-
         if InputIdentifiers.predictions in inputs:
             loaded_inputs["predictions_path"] = inputs[InputIdentifiers.predictions]
 
         if OutputIdentifiers.predictions in outputs:
             loaded_inputs["predictions_path"] = outputs[OutputIdentifiers.predictions]
 
         return loaded_inputs
@@ -78,19 +84,16 @@
             method_output (Any): return value from the called method.
             outputs (TypedDict): dictionary containing the paths where to save the output for the method.
         """
 
         if OutputIdentifiers.local in outputs:
             self.save_instance(outputs[OutputIdentifiers.local])
 
-        if OutputIdentifiers.model in outputs:
-            self.save_model(method_output, outputs[OutputIdentifiers.model])
-
-        elif OutputIdentifiers.shared in outputs:
-            self.save_model(method_output, outputs[OutputIdentifiers.shared])
+        if OutputIdentifiers.shared in outputs:
+            self.save_shared(method_output, outputs[OutputIdentifiers.shared])
 
         else:
             for output_id in outputs:
                 # The performances are the only identifier user defined.
                 if output_id not in list(OutputIdentifiers):
                     tools.save_performance(method_output[output_id], outputs[output_id])
 
@@ -116,51 +119,51 @@
         method_output = method_to_call(
             **method_inputs,
             **self.method_parameters,
         )
 
         self.save_method_output(method_output, outputs)
 
-    def load_model(self, path: str) -> Any:
-        """Load the model from disk
+    def load_shared(self, path: Union[str, os.PathLike]) -> Any:
+        """Load the shared state from disk
 
         Args:
-            path (str): path to the saved model
+            path (Union[str, os.PathLike]): path to the saved shared state
 
         Returns:
-            Any: loaded model
+            Any: loaded shared state
         """
         return self.shared_state_serializer.load(Path(path))
 
-    def save_model(self, model, path: str) -> None:
-        """Save the model
+    def save_shared(self, shared_state, path: Union[str, os.PathLike]) -> None:
+        """Save the shared state
 
         Args:
-            model (Any): Model to save
-            path (str): Path where to save the model
+            model (Any): Shared state to save
+            path (Union[str, os.PathLike]): Path where to save the model
         """
-        self.shared_state_serializer.save(model, Path(path))
+        self.shared_state_serializer.save(shared_state, Path(path))
 
-    def load_instance(self, path: str) -> Any:
+    def load_instance(self, path: Union[str, os.PathLike]) -> Any:
         """Load the instance from disk
 
         Args:
-            path (str): path to the saved instance
+            path (Union[str, os.PathLike]): path to the saved instance
 
         Returns:
             Any: loaded instance
         """
         return self.instance.load_local_state(Path(path))
 
-    def save_instance(self, path: str) -> None:
+    def save_instance(self, path: Union[str, os.PathLike]) -> None:
         """Save the instance
 
         Args:
             model (Any): Instance to save
-            path (str): Path where to save the instance
+            path (Union[str, os.PathLike]): Path where to save the instance
         """
         self.instance.save_local_state(Path(path))
 
     def register_substratools_function(self):
         """Register the function that can be accessed and executed by substratools."""
 
         tools.register(
```

### Comparing `substrafl-0.38.0rc1/substrafl/strategies/fed_avg.py` & `substrafl-0.39.0rc1/substrafl/strategies/fed_avg.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/strategies/fed_pca.py` & `substrafl-0.39.0rc1/substrafl/strategies/fed_pca.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/strategies/newton_raphson.py` & `substrafl-0.39.0rc1/substrafl/strategies/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/strategies/scaffold.py` & `substrafl-0.39.0rc1/substrafl/strategies/scaffold.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/strategies/schemas.py` & `substrafl-0.39.0rc1/substrafl/strategies/schemas.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/strategies/single_organization.py` & `substrafl-0.39.0rc1/substrafl/strategies/single_organization.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl/strategies/strategy.py` & `substrafl-0.39.0rc1/substrafl/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.38.0rc1/substrafl.egg-info/PKG-INFO` & `substrafl-0.39.0rc1/substrafl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrafl
-Version: 0.38.0rc1
+Version: 0.39.0rc1
 Summary: A high-level federated learning Python library to run      federated learning experiments at scale on a Substra network
 Home-page: https://docs.substra.org/
 Author: Owkin, Inc.
 License: Apache 2.0
 Description: readme
 Keywords: substrafl
 Platform: UNKNOWN
```

### Comparing `substrafl-0.38.0rc1/substrafl.egg-info/SOURCES.txt` & `substrafl-0.39.0rc1/substrafl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

