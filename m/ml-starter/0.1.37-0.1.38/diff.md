# Comparing `tmp/ml-starter-0.1.37.tar.gz` & `tmp/ml-starter-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.37.tar", last modified: Tue Jul 25 00:37:11 2023, max compression
+gzip compressed data, was "ml-starter-0.1.38.tar", last modified: Tue Jul 25 02:38:45 2023, max compression
```

## Comparing `ml-starter-0.1.37.tar` & `ml-starter-0.1.38.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.737534 ml-starter-0.1.37/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 00:36:59.000000 ml-starter-0.1.37/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-25 00:36:59.000000 ml-starter-0.1.37/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-25 00:37:11.737534 ml-starter-0.1.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-25 00:36:59.000000 ml-starter-0.1.37/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.717534 ml-starter-0.1.37/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.721534 ml-starter-0.1.37/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.721534 ml-starter-0.1.37/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/launchers/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.721534 ml-starter-0.1.37/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.721534 ml-starter-0.1.37/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.721534 ml-starter-0.1.37/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.725535 ml-starter-0.1.37/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.725535 ml-starter-0.1.37/ml/models/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/architectures/bifpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/architectures/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/codebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.725535 ml-starter-0.1.37/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.725535 ml-starter-0.1.37/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.725535 ml-starter-0.1.37/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/tasks/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/diffusion/beta_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/diffusion/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/tasks/gan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/gan/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/losses/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/losses/kl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/losses/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24822 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.733534 ml-starter-0.1.37/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.737534 ml-starter-0.1.37/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.737534 ml-starter-0.1.37/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.737534 ml-starter-0.1.37/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.737534 ml-starter-0.1.37/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-25 00:37:11.000000 ml-starter-0.1.37/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-25 00:37:11.000000 ml-starter-0.1.37/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 00:37:11.000000 ml-starter-0.1.37/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-25 00:37:11.000000 ml-starter-0.1.37/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-25 00:37:11.000000 ml-starter-0.1.37/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-25 00:36:59.000000 ml-starter-0.1.37/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-25 00:37:11.737534 ml-starter-0.1.37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-25 00:36:59.000000 ml-starter-0.1.37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.563076 ml-starter-0.1.38/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 02:38:31.000000 ml-starter-0.1.38/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-25 02:38:31.000000 ml-starter-0.1.38/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-25 02:38:45.563076 ml-starter-0.1.38/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-25 02:38:31.000000 ml-starter-0.1.38/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.527076 ml-starter-0.1.38/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.531076 ml-starter-0.1.38/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.531076 ml-starter-0.1.38/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/launchers/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.535076 ml-starter-0.1.38/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.535076 ml-starter-0.1.38/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/lr_schedulers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.535076 ml-starter-0.1.38/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.539076 ml-starter-0.1.38/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.539076 ml-starter-0.1.38/ml/models/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/architectures/bifpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/architectures/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/codebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.543076 ml-starter-0.1.38/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/optimizers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.543076 ml-starter-0.1.38/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.543076 ml-starter-0.1.38/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.543076 ml-starter-0.1.38/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.547076 ml-starter-0.1.38/ml/tasks/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/diffusion/beta_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/diffusion/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.547076 ml-starter-0.1.38/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.547076 ml-starter-0.1.38/ml/tasks/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/gan/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.547076 ml-starter-0.1.38/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/losses/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/losses/kl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/losses/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.547076 ml-starter-0.1.38/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.547076 ml-starter-0.1.38/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.551076 ml-starter-0.1.38/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24976 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.555076 ml-starter-0.1.38/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.559076 ml-starter-0.1.38/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.563076 ml-starter-0.1.38/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.563076 ml-starter-0.1.38/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-07-25 02:38:31.000000 ml-starter-0.1.38/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 02:38:45.563076 ml-starter-0.1.38/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-25 02:38:45.000000 ml-starter-0.1.38/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-25 02:38:45.000000 ml-starter-0.1.38/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 02:38:45.000000 ml-starter-0.1.38/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-25 02:38:45.000000 ml-starter-0.1.38/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-25 02:38:45.000000 ml-starter-0.1.38/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-25 02:38:31.000000 ml-starter-0.1.38/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-25 02:38:45.563076 ml-starter-0.1.38/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-25 02:38:31.000000 ml-starter-0.1.38/setup.py
```

### Comparing `ml-starter-0.1.37/LICENSE` & `ml-starter-0.1.38/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/PKG-INFO` & `ml-starter-0.1.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.37
+Version: 0.1.38
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.37/README.md` & `ml-starter-0.1.38/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/api.py` & `ml-starter-0.1.38/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/core/common_types.py` & `ml-starter-0.1.38/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/core/config.py` & `ml-starter-0.1.38/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/core/env.py` & `ml-starter-0.1.38/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/core/registry.py` & `ml-starter-0.1.38/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/core/state.py` & `ml-starter-0.1.38/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/launchers/base.py` & `ml-starter-0.1.38/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/launchers/mp.py` & `ml-starter-0.1.38/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/launchers/sagemaker.py` & `ml-starter-0.1.38/ml/launchers/sagemaker.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,70 +12,63 @@
 them in your config:
 
 - ``SAGEMAKER_DEFAULT_INSTANCE``: The default instance type (e.g., ``ml.p3.2xlarge``).
 - ``SAGEMAKER_DEFAULT_ROLE``: The default IAM role.
 - ``SAGEMAKER_DEFAULT_BUCKET``: The default S3 bucket to use for output.
 """
 
+import datetime
+import functools
 import logging
 import os
 import re
-import uuid
+import shutil
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, cast
 
 import torch
 from omegaconf import II, MISSING, DictConfig, OmegaConf
 from packaging import version
 
 from ml.core.config import conf_field
-from ml.core.env import get_stage_dir, set_data_dir, set_model_dir
+from ml.core.env import get_stage_dir, set_data_dir, set_ml_config_path, set_model_dir
 from ml.core.registry import Objects, project_dirs, register_launcher, register_trainer
 from ml.launchers.base import BaseLauncher, BaseLauncherConfig
 from ml.scripts.train import train_main
-from ml.utils.distributed import set_master_addr, set_master_port
 from ml.utils.staging import stage_environment
 from ml.utils.torch_distributed import MultiprocessConfig, launch_subprocesses
 
 logger = logging.getLogger(__name__)
 
 LAUNCH_METHOD = "forkserver"
 
 # If the PyTorch version being used is greater than this version, then this
 # version is used instead.
 MAX_FRAMEWORK_VERSION = "2.0.0"
 
 DEFAULT_PY_VERSION = "py310"
 
 
-def sagemaker_unique_id(_: str) -> str:
-    uuid_str = str(uuid.uuid4())
-    return uuid_str[:8]
-
-
-OmegaConf.register_new_resolver("ml.sagemaker_unique_id", sagemaker_unique_id, replace=True)
-
-
 @dataclass
 class SagemakerLauncherConfig(BaseLauncherConfig):
     iam_role: str = conf_field(MISSING, help="The SageMaker role to use")
     instance_count: int = conf_field(1, help="The number of instances to use")
     instance_type: str = conf_field(MISSING, help="The training instance type")
     output_bucket: str = conf_field(MISSING, help="The S3 bucket for outputs")
     output_prefix: str = conf_field(II("ml.exp_name:job"), help="The S3 prefix to use for output")
-    unique_key: str = conf_field(II("ml.sagemaker_unique_id:unique_id"), help="A unique key for the job")
     max_framework_version: str = conf_field(MAX_FRAMEWORK_VERSION, help="The maximum PyTorch version to use")
     py_version: str = conf_field(DEFAULT_PY_VERSION, help="The Python version to use")
     use_spot_instances: bool = conf_field(
         II("oc.decode:${oc.env:SAGEMAKER_DEFAULT_SPOT_INSTANCES,0}"),
         help="Whether or not to use spot instances",
     )
     max_num_seconds: int = conf_field(24 * 60 * 60, help="The maximum number of seconds to run")
     additional_requirements: list[str] = conf_field([], help="Additional requirements to install")
+    sync_fit: bool = conf_field(False, help="If set, block on fitting")
 
 
 def set_if_missing(c: Any, ck: str, key: str) -> None:  # noqa: ANN401
     if OmegaConf.is_missing(c, ck):
         if key in os.environ:
             setattr(c, ck, os.environ[key])
         else:
@@ -108,16 +101,19 @@
         if framework_version > max_version:
             framework_version = max_version
 
         # Saves the config file to the staging directory.
         config_path = staged_env / "config.yaml"
         OmegaConf.save(self.raw_config, config_path)
 
+        cur_time = datetime.datetime.now()
+        day_str = cur_time.strftime("%Y-%m-%d")
+
         # Base S3 bucket prefix.
-        s3_prefix = f"s3://{self.config.output_bucket}/{self.config.output_prefix}/{self.config.unique_key}"
+        s3_prefix = f"s3://{self.config.output_bucket}/{self.config.output_prefix}/{day_str}"
 
         # Writes all Python dependenices to a requirements.txt file.
         all_requirements: set[str] = set()
         for project_dir in project_dirs.paths:
             if (requirements_file := project_dir / "requirements.txt").is_file():
                 with open(requirements_file, "r", encoding="utf-8") as f:
                     all_requirements.update(f.read().splitlines())
@@ -134,20 +130,20 @@
         # Builds the tensorboard logging directory.
         trainer_cfg = register_trainer.build_config(self.raw_config)
         tensorboard_output_config: sagemaker.debugger.debugger.TensorBoardOutputConfig | None
         if trainer_cfg is None:
             tensorboard_output_config = None
         else:
             tensorboard_output_config = sagemaker.debugger.debugger.TensorBoardOutputConfig(
-                s3_output_path=f"{s3_prefix}/tensorboard",
+                s3_output_path=f"{s3_prefix}/{trainer_cfg.log_dir_name}/tensorboard",
                 # container_local_output_path=f"{trainer_cfg.log_dir_name}/tensorboard",
             )
 
         # Cleans up the job name to satisfy constraints.
-        job_name = f"{self.config.output_prefix}-{self.config.unique_key}"
+        job_name = self.config.output_prefix
         cleaned_job_name = re.sub(r"[^a-zA-Z0-9-]+", "-", job_name)
 
         # Change to the staging directory.
         original_dir = os.getcwd()
         os.chdir(staged_env)
 
         estimator = sagemaker.pytorch.estimator.PyTorch(
@@ -158,45 +154,46 @@
             role=self.config.iam_role,
             instance_count=self.config.instance_count,
             instance_type=self.config.instance_type,
             sagemaker_session=sagemaker_session,
             use_spot_instances=self.config.use_spot_instances,
             max_run=self.config.max_num_seconds,
             base_job_name=cleaned_job_name,
-            output_path=f"{s3_prefix}/output",
+            output_path=s3_prefix,
+            code_location=s3_prefix,
             dependencies=dependencies,
             distribution={
                 "smdistributed": {
                     "dataparallel": {
                         "enabled": self.config.instance_count > 1,
                     },
                 },
                 "mpi": {
                     "enabled": True,
                 },
             },
             tensorboard_output_config=tensorboard_output_config,
         )
 
-        estimator.fit()
+        estimator.fit(wait=self.config.sync_fit)
 
         os.chdir(original_dir)
 
 
-def sagemaker_train_proc_main() -> None:
-    raw_config = cast(DictConfig, OmegaConf.load("config.yaml"))
-    if not OmegaConf.is_dict(raw_config):
-        raise ValueError(f"Expected a dict config, got: {raw_config}")
+def sagemaker_train_proc_main(config_path: Path) -> None:
+    config = cast(DictConfig, OmegaConf.load(config_path))
+    if not OmegaConf.is_dict(config):
+        raise ValueError(f"Expected a dict config, got: {config}")
 
-    assert (trainer := register_trainer.build_entry(raw_config)) is not None
+    assert (trainer := register_trainer.build_entry(config)) is not None
     trainer.add_lock_file("running", exists_ok=True)
     trainer.remove_lock_file("scheduled", missing_ok=True)
 
-    objs = Objects(raw_config, trainer=trainer)
-    train_main(raw_config, objs)
+    objs = Objects(config, trainer=trainer)
+    train_main(config, objs)
 
 
 def sagemaker_main() -> None:
     # Adds any directories to `project_dirs`.
     for subdir in Path.cwd().iterdir():
         if subdir.is_dir():
             project_dirs.add(subdir)
@@ -213,24 +210,29 @@
     num_gpus = int(os.environ["SM_NUM_GPUS"])
     world_size = max(len(hosts) * num_gpus, 1)
 
     # Determines a master port by hashing the hosts.
     master_port = 10_000 + hash(tuple(hosts)) % 10_000
 
     # Sets environment variables from SageMaker environment variables.
-    set_model_dir(Path(os.environ["SM_MODEL_DIR"]))
-    set_data_dir(Path(os.environ["SM_INPUT_DIR"]))
-    set_master_addr(hosts[0])
-    set_master_port(master_port)
+    sm_model_dir = Path(os.environ["SM_MODEL_DIR"])
+    sm_input_dir = Path(os.environ["SM_INPUT_DIR"])
+    set_model_dir(sm_model_dir / "models")
+    set_data_dir(sm_input_dir)
+
+    # Moves the "config.yaml" file to the `sm_model_dir`.
+    shutil.move("config.yaml", (config_path := sm_model_dir / "config.yaml"))
+    set_ml_config_path(config_path)
 
     cfg = MultiprocessConfig(
         world_size=world_size,
         local_world_size=num_gpus,
         master_addr=master_addr,
         master_port=master_port,
     )
 
-    launch_subprocesses(sagemaker_train_proc_main, cfg, rank_offset=cur_host_idx * num_gpus)
+    func = functools.partial(sagemaker_train_proc_main, config_path=config_path)
+    launch_subprocesses(func, cfg, rank_offset=cur_host_idx * num_gpus)
 
 
 if __name__ == "__main__":
     sagemaker_main()
```

### Comparing `ml-starter-0.1.37/ml/launchers/slurm.py` & `ml-starter-0.1.38/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/launchers/torchrun.py` & `ml-starter-0.1.38/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/loggers/base.py` & `ml-starter-0.1.38/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/loggers/meter.py` & `ml-starter-0.1.38/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/loggers/multi.py` & `ml-starter-0.1.38/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/loggers/stdout.py` & `ml-starter-0.1.38/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/loggers/tensorboard.py` & `ml-starter-0.1.38/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/lr_schedulers/base.py` & `ml-starter-0.1.38/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/lr_schedulers/constant.py` & `ml-starter-0.1.38/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.38/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.38/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/lr_schedulers/gan.py` & `ml-starter-0.1.38/ml/lr_schedulers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/lr_schedulers/linear.py` & `ml-starter-0.1.38/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.38/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.38/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/models/activations.py` & `ml-starter-0.1.38/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/models/architectures/bifpn.py` & `ml-starter-0.1.38/ml/models/architectures/bifpn.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/models/architectures/unet.py` & `ml-starter-0.1.38/ml/models/architectures/unet.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/models/base.py` & `ml-starter-0.1.38/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/models/codebook.py` & `ml-starter-0.1.38/ml/models/codebook.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/models/embeddings.py` & `ml-starter-0.1.38/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/models/gan.py` & `ml-starter-0.1.38/ml/models/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/models/init.py` & `ml-starter-0.1.38/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/models/kmeans.py` & `ml-starter-0.1.38/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/models/lora.py` & `ml-starter-0.1.38/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/models/modules.py` & `ml-starter-0.1.38/ml/models/modules.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/models/norms.py` & `ml-starter-0.1.38/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/models/parallel.py` & `ml-starter-0.1.38/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/optimizers/adam.py` & `ml-starter-0.1.38/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/optimizers/adan.py` & `ml-starter-0.1.38/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/optimizers/base.py` & `ml-starter-0.1.38/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/optimizers/common.py` & `ml-starter-0.1.38/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/optimizers/gan.py` & `ml-starter-0.1.38/ml/optimizers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/optimizers/lion.py` & `ml-starter-0.1.38/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/optimizers/sgd.py` & `ml-starter-0.1.38/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/optimizers/shampoo.py` & `ml-starter-0.1.38/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/scripts/cli.py` & `ml-starter-0.1.38/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/scripts/stage.py` & `ml-starter-0.1.38/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/scripts/train.py` & `ml-starter-0.1.38/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/base.py` & `ml-starter-0.1.38/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.38/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.38/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/datasets/collate.py` & `ml-starter-0.1.38/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.38/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.38/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.38/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.38/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.38/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.38/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/diffusion/beta_schedule.py` & `ml-starter-0.1.38/ml/tasks/diffusion/beta_schedule.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/diffusion/gaussian.py` & `ml-starter-0.1.38/ml/tasks/diffusion/gaussian.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/environments/base.py` & `ml-starter-0.1.38/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/environments/utils.py` & `ml-starter-0.1.38/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/environments/worker.py` & `ml-starter-0.1.38/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/gan/base.py` & `ml-starter-0.1.38/ml/tasks/gan/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/losses/audio.py` & `ml-starter-0.1.38/ml/tasks/losses/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/losses/image.py` & `ml-starter-0.1.38/ml/tasks/losses/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/losses/kl.py` & `ml-starter-0.1.38/ml/tasks/losses/kl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/losses/loss.py` & `ml-starter-0.1.38/ml/tasks/losses/loss.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/rl/base.py` & `ml-starter-0.1.38/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/rl/replay.py` & `ml-starter-0.1.38/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/tasks/sl/base.py` & `ml-starter-0.1.38/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/trainers/base.py` & `ml-starter-0.1.38/ml/trainers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,33 +224,27 @@
     load_from_ckpt_path: str | None = conf_field(None, help="If set, load initial model weights from this path")
 
 
 @dataclass
 class BaseTrainerConfig(BaseConfig):
     """Defines the base config for all trainers."""
 
-    base_run_dir: str = conf_field(II("ml.abs_path:${oc.env:RUN_DIR}"), help="The base directory for all runs")
     exp_name: str = conf_field(II("ml.exp_name:null"), help="The name of the training job")
     exp_dir: str = conf_field(MISSING, help="The directory where the experiment is stored")
     log_dir_name: str = conf_field("logs", help="Name of the subdirectory which contains logs")
     use_double_weight_precision: bool = conf_field(False, help="If set, use doubles for weights instead of floats")
     checkpoint: CheckpointConfig = conf_field(CheckpointConfig())
 
     @classmethod
     def resolve(cls, config: "BaseTrainerConfig") -> None:
         if OmegaConf.is_missing(config, "exp_dir"):
-            config.exp_dir = str(get_empty_exp_dir(Path(config.base_run_dir) / config.exp_name))
-        elif (ml_config_path := get_ml_config_path()) is not None:
-            exp_dir_path = Path(config.exp_dir).resolve()
-            if exp_dir_path != ml_config_path.parent:
-                logger.warning(
-                    "The `config.yaml` file is located in a different directory than the experiment directory; "
-                    f"updating {config.exp_dir=} to {ml_config_path.parent=}."
-                )
-                config.exp_dir = str(ml_config_path.parent)
+            if "RUN_DIR" not in os.environ:
+                raise KeyError("Set the RUN_DIR environment variable")
+            base_run_dir = Path(os.environ["RUN_DIR"]).resolve()
+            config.exp_dir = str(get_empty_exp_dir(base_run_dir / config.exp_name))
         super().resolve(config)
 
 
 TrainerConfigT = TypeVar("TrainerConfigT", bound=BaseTrainerConfig)
 ModelT = TypeVar("ModelT", bound=BaseModel)
 TaskT = TypeVar("TaskT", bound=BaseTask)
 
@@ -261,21 +255,32 @@
     logger: MultiLogger
     loggers: list[BaseLogger]
 
     def __init__(self, config: TrainerConfigT) -> None:
         super().__init__(config)
 
         self.exp_name = config.exp_name
-        self.exp_dir = Path(config.exp_dir)
+        self.exp_dir = Path(config.exp_dir).resolve()
         self.log_dir = self.exp_dir / config.log_dir_name
         self.checkpoint_config = config.checkpoint
         self.loggers = []
         self.logger = MultiLogger(default_namespace="trainer")
         self.signal_handlers: dict[signal.Signals, list[Callable[[], None]]] = {}
 
+        # Ensures that we're always training in whatever directory the
+        # `config.yaml` file is in.
+        if (ml_config_path := get_ml_config_path()) is not None:
+            exp_dir_path = self.exp_dir.resolve()
+            if exp_dir_path != ml_config_path.parent:
+                logger.warning(
+                    "The `config.yaml` file is located in a different directory than the experiment directory; "
+                    f"updating {self.exp_dir=} to {ml_config_path.parent=}."
+                )
+                self.exp_dir = ml_config_path.parent
+
         logger.info("Experiment directory: %s", self.exp_dir)
 
         self._device = self._get_device()
         self._device_type = self._get_device_type()
         self._weight_precision = self._get_weight_precision()
 
         self.__last_ckpt_time = time.time()
```

### Comparing `ml-starter-0.1.37/ml/trainers/gan.py` & `ml-starter-0.1.38/ml/trainers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/trainers/learning.py` & `ml-starter-0.1.38/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/trainers/mixins/compile.py` & `ml-starter-0.1.38/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.38/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.38/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.38/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.38/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.38/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.38/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.38/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.38/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/trainers/rl.py` & `ml-starter-0.1.38/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/trainers/sl.py` & `ml-starter-0.1.38/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/amp.py` & `ml-starter-0.1.38/ml/utils/amp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/argparse.py` & `ml-starter-0.1.38/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/atomic.py` & `ml-starter-0.1.38/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/attention.py` & `ml-starter-0.1.38/ml/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/audio.py` & `ml-starter-0.1.38/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/augmentation.py` & `ml-starter-0.1.38/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/caching.py` & `ml-starter-0.1.38/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/checkpoint.py` & `ml-starter-0.1.38/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/cli.py` & `ml-starter-0.1.38/ml/utils/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 IGNORE_ARGS: set[str] = {
     "trainer.exp_name",
     "trainer.log_dir_name",
-    "trainer.base_run_dir",
     "trainer.exp_dir",
     "trainer.name",
 }
 
 
 def get_exp_name(prefix: str | None = None, args: list[str] | None = None) -> str:
     parts: list[str] = []
```

### Comparing `ml-starter-0.1.37/ml/utils/colors.py` & `ml-starter-0.1.38/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/containers.py` & `ml-starter-0.1.38/ml/utils/containers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/data.py` & `ml-starter-0.1.38/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/datetime.py` & `ml-starter-0.1.38/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/device/auto.py` & `ml-starter-0.1.38/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/device/base.py` & `ml-starter-0.1.38/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/device/cpu.py` & `ml-starter-0.1.38/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/device/gpu.py` & `ml-starter-0.1.38/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/device/metal.py` & `ml-starter-0.1.38/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/distributed.py` & `ml-starter-0.1.38/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/exceptions.py` & `ml-starter-0.1.38/ml/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/image.py` & `ml-starter-0.1.38/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/io.py` & `ml-starter-0.1.38/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/large_models.py` & `ml-starter-0.1.38/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/logging.py` & `ml-starter-0.1.38/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/meter.py` & `ml-starter-0.1.38/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/mixed_precision.py` & `ml-starter-0.1.38/ml/utils/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/networking.py` & `ml-starter-0.1.38/ml/utils/networking.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/numpy.py` & `ml-starter-0.1.38/ml/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/parallel.py` & `ml-starter-0.1.38/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/spectrogram.py` & `ml-starter-0.1.38/ml/utils/spectrogram.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/staging.py` & `ml-starter-0.1.38/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/testing.py` & `ml-starter-0.1.38/ml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/timer.py` & `ml-starter-0.1.38/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/tokens.py` & `ml-starter-0.1.38/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/torch_distributed.py` & `ml-starter-0.1.38/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/triton/kmeans.py` & `ml-starter-0.1.38/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/triton/lion.py` & `ml-starter-0.1.38/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml/utils/video.py` & `ml-starter-0.1.38/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.38/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.37
+Version: 0.1.38
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.37/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.38/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/pyproject.toml` & `ml-starter-0.1.38/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.37/setup.py` & `ml-starter-0.1.38/setup.py`

 * *Files identical despite different names*

