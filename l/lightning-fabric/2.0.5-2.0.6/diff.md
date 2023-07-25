# Comparing `tmp/lightning-fabric-2.0.5.tar.gz` & `tmp/lightning-fabric-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-fabric-2.0.5.tar", last modified: Mon Jul 10 16:11:25 2023, max compression
+gzip compressed data, was "lightning-fabric-2.0.6.tar", last modified: Mon Jul 24 21:38:15 2023, max compression
```

## Comparing `lightning-fabric-2.0.5.tar` & `lightning-fabric-2.0.6.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.099836 lightning-fabric-2.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.091836 lightning-fabric-2.0.5/.actions/
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-10 16:11:25.099836 lightning-fabric-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22065 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.087836 lightning-fabric-2.0.5/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.091836 lightning-fabric-2.0.5/requirements/fabric/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/requirements/fabric/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/requirements/fabric/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/requirements/fabric/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/requirements/fabric/strategies.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/requirements/fabric/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:11:25.099836 lightning-fabric-2.0.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     8000 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.091836 lightning-fabric-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.091836 lightning-fabric-2.0.5/src/lightning_fabric/
--rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/lightning_fabric/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/lightning_fabric/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/lightning_fabric/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/lightning_fabric/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/lightning_fabric/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.091836 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/mps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/accelerators/tpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    27201 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    40477 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/fabric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.091836 lightning-fabric-2.0.5/src/lightning_fabric/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/loggers/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.095836 lightning-fabric-2.0.5/src/lightning_fabric/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.095836 lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/collective.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/single_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/torch_collective.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.095836 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/cluster_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/kubeflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/torchelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.095836 lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/torch_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.095836 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/tpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/tpu_bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/lightning_fabric/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.095836 lightning-fabric-2.0.5/src/lightning_fabric/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)    37574 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/dp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15834 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.099836 lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/subprocess_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/xla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/single_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/single_tpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/strategies/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.099836 lightning-fabric-2.0.5/src/lightning_fabric/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/apply_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/device_dtype_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/device_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/lightning_fabric/version.info
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-07-10 16:11:24.000000 lightning-fabric-2.0.5/src/lightning_fabric/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:11:25.091836 lightning-fabric-2.0.5/src/lightning_fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-10 16:11:25.000000 lightning-fabric-2.0.5/src/lightning_fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-07-10 16:11:25.000000 lightning-fabric-2.0.5/src/lightning_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:11:25.000000 lightning-fabric-2.0.5/src/lightning_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:11:25.000000 lightning-fabric-2.0.5/src/lightning_fabric.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-10 16:11:25.000000 lightning-fabric-2.0.5/src/lightning_fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 16:11:25.000000 lightning-fabric-2.0.5/src/lightning_fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 16:11:11.000000 lightning-fabric-2.0.5/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.630218 lightning-fabric-2.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.622218 lightning-fabric-2.0.6/.actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-07-24 21:38:01.000000 lightning-fabric-2.0.6/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-24 21:38:01.000000 lightning-fabric-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-24 21:38:15.630218 lightning-fabric-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22065 2023-07-24 21:38:01.000000 lightning-fabric-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-07-24 21:38:01.000000 lightning-fabric-2.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.622218 lightning-fabric-2.0.6/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.622218 lightning-fabric-2.0.6/requirements/fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-24 21:38:01.000000 lightning-fabric-2.0.6/requirements/fabric/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 21:38:01.000000 lightning-fabric-2.0.6/requirements/fabric/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 21:38:01.000000 lightning-fabric-2.0.6/requirements/fabric/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-24 21:38:01.000000 lightning-fabric-2.0.6/requirements/fabric/strategies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-24 21:38:01.000000 lightning-fabric-2.0.6/requirements/fabric/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:38:15.630218 lightning-fabric-2.0.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8000 2023-07-24 21:38:01.000000 lightning-fabric-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.622218 lightning-fabric-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.622218 lightning-fabric-2.0.6/src/lightning_fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-24 21:38:02.000000 lightning-fabric-2.0.6/src/lightning_fabric/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-07-24 21:38:02.000000 lightning-fabric-2.0.6/src/lightning_fabric/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-24 21:38:02.000000 lightning-fabric-2.0.6/src/lightning_fabric/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-24 21:38:02.000000 lightning-fabric-2.0.6/src/lightning_fabric/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-24 21:38:02.000000 lightning-fabric-2.0.6/src/lightning_fabric/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.626218 lightning-fabric-2.0.6/src/lightning_fabric/accelerators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/accelerators/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/accelerators/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/accelerators/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/accelerators/mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/accelerators/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/accelerators/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27201 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40477 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/fabric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.626218 lightning-fabric-2.0.6/src/lightning_fabric/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/loggers/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.626218 lightning-fabric-2.0.6/src/lightning_fabric/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.626218 lightning-fabric-2.0.6/src/lightning_fabric/plugins/collectives/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/collectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/collectives/collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/collectives/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/collectives/torch_collective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.626218 lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/cluster_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/kubeflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/torchelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.626218 lightning-fabric-2.0.6/src/lightning_fabric/plugins/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/io/checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/io/torch_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/io/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.626218 lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/tpu_bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:02.000000 lightning-fabric-2.0.6/src/lightning_fabric/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.630218 lightning-fabric-2.0.6/src/lightning_fabric/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37574 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/dp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15834 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.630218 lightning-fabric-2.0.6/src/lightning_fabric/strategies/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/launchers/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/launchers/subprocess_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/launchers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/single_tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/strategies/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.630218 lightning-fabric-2.0.6/src/lightning_fabric/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/apply_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/device_dtype_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/device_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 21:38:02.000000 lightning-fabric-2.0.6/src/lightning_fabric/version.info
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:38:15.622218 lightning-fabric-2.0.6/src/lightning_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 21:38:15.000000 lightning-fabric-2.0.6/src/lightning_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 21:38:02.000000 lightning-fabric-2.0.6/src/version.info
```

### Comparing `lightning-fabric-2.0.5/.actions/assistant.py` & `lightning-fabric-2.0.6/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/LICENSE` & `lightning-fabric-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/PKG-INFO` & `lightning-fabric-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-fabric
-Version: 2.0.5
+Version: 2.0.6
 Summary: UNKNOWN
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
```

### Comparing `lightning-fabric-2.0.5/README.md` & `lightning-fabric-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/pyproject.toml` & `lightning-fabric-2.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/setup.py` & `lightning-fabric-2.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/CHANGELOG.md` & `lightning-fabric-2.0.6/src/lightning_fabric/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
 
+## [2.0.6] - 2023-07-20
+
+#### Fixed
+
+- Fixed `TensorBoardLogger.log_graph` not unwrapping the `_FabricModule` ([#17844](https://github.com/Lightning-AI/lightning/pull/17844))
+
+
 ## [2.0.5] - 2023-07-07
 
 ### Added
 
 - Added validation against misconfigured device selection when using the DeepSpeed strategy ([#17952](https://github.com/Lightning-AI/lightning/pull/17952))
 
 ### Changed
@@ -28,14 +35,17 @@
 
 ### Fixed
 
 - Fixed validation of parameters of `plugins.precision.MixedPrecision` ([#17687](https://github.com/Lightning-AI/lightning/pull/17687))
 - Fixed an issue with hpu imports leading to performance degradation  ([#17788](https://github.com/Lightning-AI/lightning/pull/17788))
 
 
+- Fixed computing the next version folder in `CSVLogger` ([#17139](https://github.com/Lightning-AI/lightning/pull/17139), [#17139](https://github.com/Lightning-AI/lightning/pull/17986))
+
+
 ## [2.0.3] - 2023-06-07
 
 - Added support for `Callback` registration through entry points ([#17756](https://github.com/Lightning-AI/lightning/pull/17756))
 - Add Fabric internal hooks ([#17759](https://github.com/Lightning-AI/lightning/pull/17759))
 
 ### Changed
```

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/README.md` & `lightning-fabric-2.0.6/src/lightning_fabric/README.md`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/__init__.py` & `lightning-fabric-2.0.6/src/lightning_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/__setup__.py` & `lightning-fabric-2.0.6/src/lightning_fabric/__setup__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/accelerators/__init__.py` & `lightning-fabric-2.0.6/src/lightning_fabric/accelerators/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/accelerators/accelerator.py` & `lightning-fabric-2.0.6/src/lightning_fabric/accelerators/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/accelerators/cpu.py` & `lightning-fabric-2.0.6/src/lightning_fabric/accelerators/cpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/accelerators/cuda.py` & `lightning-fabric-2.0.6/src/lightning_fabric/accelerators/cuda.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/accelerators/mps.py` & `lightning-fabric-2.0.6/src/lightning_fabric/accelerators/mps.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/accelerators/registry.py` & `lightning-fabric-2.0.6/src/lightning_fabric/accelerators/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/accelerators/tpu.py` & `lightning-fabric-2.0.6/src/lightning_fabric/accelerators/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/cli.py` & `lightning-fabric-2.0.6/src/lightning_fabric/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/connector.py` & `lightning-fabric-2.0.6/src/lightning_fabric/connector.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/fabric.py` & `lightning-fabric-2.0.6/src/lightning_fabric/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/loggers/__init__.py` & `lightning-fabric-2.0.6/src/lightning_fabric/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/loggers/csv_logs.py` & `lightning-fabric-2.0.6/src/lightning_fabric/loggers/csv_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,30 +101,30 @@
         """The log directory for this run.
 
         By default, it is named ``'version_${self.version}'`` but it can be overridden by passing a string value for the
         constructor's version parameter instead of ``None`` or an int.
         """
         # create a pseudo standard path
         version = self.version if isinstance(self.version, str) else f"version_{self.version}"
-        return os.path.join(self.root_dir, self.name, version)
+        return os.path.join(self._root_dir, self.name, version)
 
     @property
     @rank_zero_experiment
     def experiment(self) -> "_ExperimentWriter":
         """Actual ExperimentWriter object. To use ExperimentWriter features anywhere in your code, do the
         following.
 
         Example::
 
             self.logger.experiment.some_experiment_writer_function()
         """
         if self._experiment is not None:
             return self._experiment
 
-        os.makedirs(self.root_dir, exist_ok=True)
+        os.makedirs(self._root_dir, exist_ok=True)
         self._experiment = _ExperimentWriter(log_dir=self.log_dir)
         return self._experiment
 
     @rank_zero_only
     def log_hyperparams(self, params: Union[Dict[str, Any], Namespace]) -> None:  # type: ignore[override]
         raise NotImplementedError("The `CSVLogger` does not yet support logging hyperparameters.")
 
@@ -149,22 +149,22 @@
         if self._experiment is None:
             # When using multiprocessing, finalize() should be a no-op on the main process, as no experiment has been
             # initialized there
             return
         self.save()
 
     def _get_next_version(self) -> int:
-        root_dir = self.root_dir
+        versions_root = os.path.join(self._root_dir, self.name)
 
-        if not self._fs.isdir(root_dir):
-            log.warning("Missing logger folder: %s", root_dir)
+        if not self._fs.isdir(versions_root):
+            log.warning("Missing logger folder: %s", versions_root)
             return 0
 
         existing_versions = []
-        for d in self._fs.listdir(root_dir):
+        for d in self._fs.listdir(versions_root):
             full_path = d["name"]
             name = os.path.basename(full_path)
             if self._fs.isdir(full_path) and name.startswith("version_"):
                 existing_versions.append(int(name.split("_")[1]))
 
         if len(existing_versions) == 0:
             return 0
```

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/loggers/logger.py` & `lightning-fabric-2.0.6/src/lightning_fabric/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/loggers/tensorboard.py` & `lightning-fabric-2.0.6/src/lightning_fabric/loggers/tensorboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from lightning_fabric.loggers.logger import Logger, rank_zero_experiment
 from lightning_fabric.utilities.cloud_io import get_filesystem
 from lightning_fabric.utilities.logger import _add_prefix, _convert_params, _flatten_dict
 from lightning_fabric.utilities.logger import _sanitize_params as _utils_sanitize_params
 from lightning_fabric.utilities.rank_zero import rank_zero_only, rank_zero_warn
 from lightning_fabric.utilities.types import _PATH
+from lightning_fabric.wrappers import _unwrap_objects
 
 log = logging.getLogger(__name__)
 
 _TENSORBOARD_AVAILABLE = RequirementCache("tensorboard")
 _TENSORBOARDX_AVAILABLE = RequirementCache("tensorboardX")
 if TYPE_CHECKING:
     # assumes at least one will be installed when type checking
@@ -243,14 +244,15 @@
             writer.add_summary(ssi)
             writer.add_summary(sei)
 
     @rank_zero_only
     def log_graph(self, model: Module, input_array: Optional[Tensor] = None) -> None:
         model_example_input = getattr(model, "example_input_array", None)
         input_array = model_example_input if input_array is None else input_array
+        model = _unwrap_objects(model)
 
         if input_array is None:
             rank_zero_warn(
                 "Could not log computational graph to TensorBoard: The `model.example_input_array` attribute"
                 " is not set or `input_array` was not given."
             )
         elif not isinstance(input_array, (Tensor, tuple)):
@@ -259,16 +261,18 @@
                 f" has type {type(input_array)} which can't be traced by TensorBoard. Make the input array a tuple"
                 f" representing the positional arguments to the model's `forward()` implementation."
             )
         elif callable(getattr(model, "_on_before_batch_transfer", None)) and callable(
             getattr(model, "_apply_batch_transfer_handler", None)
         ):
             # this is probably is a LightningModule
-            input_array = model._on_before_batch_transfer(input_array)  # type: ignore[operator]
-            input_array = model._apply_batch_transfer_handler(input_array)  # type: ignore[operator]
+            input_array = model._on_before_batch_transfer(input_array)
+            input_array = model._apply_batch_transfer_handler(input_array)
+            self.experiment.add_graph(model, input_array)
+        else:
             self.experiment.add_graph(model, input_array)
 
     @rank_zero_only
     def save(self) -> None:
         self.experiment.flush()
 
     @rank_zero_only
```

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/__init__.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/collective.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/collectives/collective.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/single_device.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/collectives/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/collectives/torch_collective.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/collectives/torch_collective.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/__init__.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/cluster_environment.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/cluster_environment.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/kubeflow.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/kubeflow.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/lightning.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/lightning.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/lsf.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/lsf.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/mpi.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/mpi.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/slurm.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/slurm.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/torchelastic.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/torchelastic.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/environments/xla.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/environments/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/__init__.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/io/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/checkpoint_io.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/io/checkpoint_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/torch_io.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/io/torch_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/io/xla.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/io/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/__init__.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/amp.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/amp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/deepspeed.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/double.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/double.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/fsdp.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/precision.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/tpu.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/tpu_bf16.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/tpu_bf16.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/plugins/precision/utils.py` & `lightning-fabric-2.0.6/src/lightning_fabric/plugins/precision/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/__init__.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/ddp.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/ddp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/deepspeed.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/dp.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/dp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/fsdp.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/__init__.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/base.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/launchers/base.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/launcher.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/multiprocessing.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/launchers/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/subprocess_script.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/launchers/subprocess_script.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/launchers/xla.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/launchers/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/parallel.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/registry.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/single_device.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/single_tpu.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/single_tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/strategy.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/strategies/xla.py` & `lightning-fabric-2.0.6/src/lightning_fabric/strategies/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/__init__.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/apply_func.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/apply_func.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/cloud_io.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/cloud_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/data.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/data.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/device_dtype_mixin.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/device_dtype_mixin.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/device_parser.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/device_parser.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/distributed.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/enums.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/exceptions.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/imports.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/logger.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/optimizer.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/optimizer.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/rank_zero.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/rank_zero.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/registry.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/seed.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/seed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/types.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/utilities/warnings.py` & `lightning-fabric-2.0.6/src/lightning_fabric/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric/wrappers.py` & `lightning-fabric-2.0.6/src/lightning_fabric/wrappers.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric.egg-info/PKG-INFO` & `lightning-fabric-2.0.6/src/lightning_fabric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-fabric
-Version: 2.0.5
+Version: 2.0.6
 Summary: UNKNOWN
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
```

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric.egg-info/SOURCES.txt` & `lightning-fabric-2.0.6/src/lightning_fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.5/src/lightning_fabric.egg-info/requires.txt` & `lightning-fabric-2.0.6/src/lightning_fabric.egg-info/requires.txt`

 * *Files identical despite different names*

