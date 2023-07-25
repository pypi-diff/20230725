# Comparing `tmp/ml-starter-0.1.36.tar.gz` & `tmp/ml-starter-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.36.tar", last modified: Wed Jul 19 23:36:00 2023, max compression
+gzip compressed data, was "ml-starter-0.1.37.tar", last modified: Tue Jul 25 00:37:11 2023, max compression
```

## Comparing `ml-starter-0.1.36.tar` & `ml-starter-0.1.37.tar`

### file list

```diff
@@ -1,184 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.309047 ml-starter-0.1.36/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-19 23:35:48.000000 ml-starter-0.1.36/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-19 23:35:48.000000 ml-starter-0.1.36/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-19 23:36:00.309047 ml-starter-0.1.36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-19 23:35:48.000000 ml-starter-0.1.36/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.293047 ml-starter-0.1.36/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.293047 ml-starter-0.1.36/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    26629 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.293047 ml-starter-0.1.36/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.293047 ml-starter-0.1.36/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    45793 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.293047 ml-starter-0.1.36/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/lr_schedulers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.293047 ml-starter-0.1.36/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.297047 ml-starter-0.1.36/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/models/codebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/models/diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/models/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/models/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.297047 ml-starter-0.1.36/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/optimizers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.297047 ml-starter-0.1.36/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.297047 ml-starter-0.1.36/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19338 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.301047 ml-starter-0.1.36/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.301047 ml-starter-0.1.36/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.301047 ml-starter-0.1.36/ml/tasks/gan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/gan/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.301047 ml-starter-0.1.36/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/losses/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/losses/kl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/losses/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.301047 ml-starter-0.1.36/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.301047 ml-starter-0.1.36/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.301047 ml-starter-0.1.36/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24021 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.305047 ml-starter-0.1.36/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11397 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.309047 ml-starter-0.1.36/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.309047 ml-starter-0.1.36/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.309047 ml-starter-0.1.36/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-07-19 23:35:48.000000 ml-starter-0.1.36/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:36:00.309047 ml-starter-0.1.36/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-19 23:36:00.000000 ml-starter-0.1.36/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-19 23:36:00.000000 ml-starter-0.1.36/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 23:36:00.000000 ml-starter-0.1.36/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-19 23:36:00.000000 ml-starter-0.1.36/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-19 23:36:00.000000 ml-starter-0.1.36/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-19 23:35:48.000000 ml-starter-0.1.36/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-19 23:35:48.000000 ml-starter-0.1.36/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-19 23:35:48.000000 ml-starter-0.1.36/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-19 23:35:48.000000 ml-starter-0.1.36/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-19 23:36:00.309047 ml-starter-0.1.36/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-19 23:35:48.000000 ml-starter-0.1.36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.737534 ml-starter-0.1.37/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 00:36:59.000000 ml-starter-0.1.37/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-25 00:36:59.000000 ml-starter-0.1.37/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-25 00:37:11.737534 ml-starter-0.1.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-25 00:36:59.000000 ml-starter-0.1.37/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.717534 ml-starter-0.1.37/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.721534 ml-starter-0.1.37/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.721534 ml-starter-0.1.37/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/launchers/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.721534 ml-starter-0.1.37/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.721534 ml-starter-0.1.37/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.721534 ml-starter-0.1.37/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.725535 ml-starter-0.1.37/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.725535 ml-starter-0.1.37/ml/models/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/architectures/bifpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/architectures/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/codebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.725535 ml-starter-0.1.37/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.725535 ml-starter-0.1.37/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.725535 ml-starter-0.1.37/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/tasks/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/diffusion/beta_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/diffusion/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/tasks/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/gan/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/losses/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/losses/kl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/losses/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.729534 ml-starter-0.1.37/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24822 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.733534 ml-starter-0.1.37/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.737534 ml-starter-0.1.37/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.737534 ml-starter-0.1.37/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.737534 ml-starter-0.1.37/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-07-25 00:36:59.000000 ml-starter-0.1.37/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:37:11.737534 ml-starter-0.1.37/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-25 00:37:11.000000 ml-starter-0.1.37/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-25 00:37:11.000000 ml-starter-0.1.37/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 00:37:11.000000 ml-starter-0.1.37/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-25 00:37:11.000000 ml-starter-0.1.37/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-25 00:37:11.000000 ml-starter-0.1.37/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-25 00:36:59.000000 ml-starter-0.1.37/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-25 00:37:11.737534 ml-starter-0.1.37/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-25 00:36:59.000000 ml-starter-0.1.37/setup.py
```

### Comparing `ml-starter-0.1.36/LICENSE` & `ml-starter-0.1.37/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/PKG-INFO` & `ml-starter-0.1.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.36
+Version: 0.1.37
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.36/README.md` & `ml-starter-0.1.37/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/api.py` & `ml-starter-0.1.37/ml/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,18 @@
     "BaseOptimizer",
     "BaseOptimizerConfig",
     "BaseTask",
     "BaseTaskConfig",
     "BaseTrainer",
     "BaseTrainerConfig",
     "Batch",
+    "BiFPN",
     "cached_object",
     "cast_activation_type",
+    "cast_beta_schedule",
     "cast_embedding_kind",
     "cast_init_type",
     "cast_norm_type",
     "check_md5",
     "check_sha256",
     "ChunkSampler",
     "Clamp",
@@ -193,14 +195,15 @@
     "test_environment",
     "test_task",
     "timeout",
     "Timer",
     "TokenReader",
     "TokenWriter",
     "transforms",
+    "UNet",
     "VideoFileDataset",
     "WorkerPool",
     "write_audio",
     "write_gif",
     "write_video",
 ]
 
@@ -227,16 +230,17 @@
 )
 from ml.core.state import Phase, State
 from ml.launchers.mp import MultiProcessLauncher, MultiProcessLauncherConfig
 from ml.launchers.slurm import SlurmLauncher, SlurmLauncherConfig, set_slurm_master_addr, set_slurm_rank_and_world_size
 from ml.loggers.multi import namespace_context
 from ml.lr_schedulers.base import BaseLRScheduler, BaseLRSchedulerConfig
 from ml.models.activations import ActivationType, Clamp, cast_activation_type, get_activation
+from ml.models.architectures.bifpn import BiFPN
+from ml.models.architectures.unet import UNet
 from ml.models.base import BaseModel, BaseModelConfig
-from ml.models.diffusion import DiffusionBetaSchedule, GaussianDiffusion, get_diffusion_beta_schedule
 from ml.models.embeddings import (
     LearnedPositionalEmbeddings,
     RotaryEmbeddings,
     SinusoidalEmbeddings,
     cast_embedding_kind,
     get_positional_embeddings,
 )
@@ -266,14 +270,16 @@
 from ml.tasks.datasets.async_iterable import AsyncIterableDataset
 from ml.tasks.datasets.clippify import ClippifyDataset
 from ml.tasks.datasets.collate import CollateMode, collate, collate_non_null, pad_all, pad_sequence
 from ml.tasks.datasets.multi_iter import MultiIterDataset
 from ml.tasks.datasets.samplers import ChunkSampler
 from ml.tasks.datasets.streaming import StreamingDataset, StreamingDatasetNoIndex
 from ml.tasks.datasets.video_file import VideoFileDataset
+from ml.tasks.diffusion.beta_schedule import DiffusionBetaSchedule, cast_beta_schedule, get_diffusion_beta_schedule
+from ml.tasks.diffusion.gaussian import GaussianDiffusion
 from ml.tasks.environments.base import Environment
 from ml.tasks.environments.utils import test_environment
 from ml.tasks.environments.worker import (
     AsyncEnvironmentWorker,
     AsyncWorkerPool,
     BaseEnvironmentWorker,
     SyncEnvironmentWorker,
```

### Comparing `ml-starter-0.1.36/ml/core/common_types.py` & `ml-starter-0.1.37/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/core/config.py` & `ml-starter-0.1.37/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/core/env.py` & `ml-starter-0.1.37/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/core/registry.py` & `ml-starter-0.1.37/ml/core/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,14 +303,20 @@
             reg_obj = reg_cls(reg_cfg)
             if isinstance(reg_obj, BaseObject):
                 reg_obj.set_raw_config(raw_config)
 
         return reg_obj
 
     @classmethod
+    def build_config(cls, raw_config: DictConfig) -> Config | None:
+        if cls.config_key() not in raw_config:
+            return None
+        return raw_config[cls.config_key()]
+
+    @classmethod
     def build_entry(cls, raw_config: DictConfig) -> Entry | None:
         if cls.config_key() not in raw_config:
             return None
         with Timer(f"getting {cls.config_key()} name", spinner=True):
             reg_name = get_name(cls.config_key(), raw_config[cls.config_key()])
         return cls._build_entry_from_name(reg_name, raw_config[cls.config_key()], raw_config)
```

### Comparing `ml-starter-0.1.36/ml/core/state.py` & `ml-starter-0.1.37/ml/core/state.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Defines a dataclass for keeping track of the current training state."""
 
+import time
 from dataclasses import dataclass
 from typing import Literal, TypeVar, cast, get_args
 
 from omegaconf import MISSING
 from torch import nn
 
 from ml.core.config import conf_field
@@ -35,14 +36,16 @@
     num_epochs: int = conf_field(MISSING, help="Number of epochs so far")
     num_steps: int = conf_field(MISSING, help="Number of steps so far")
     num_epoch_steps: int = conf_field(MISSING, help="Number of steps in the current epoch")
     num_samples: int = conf_field(MISSING, help="Number of sample so far")
     num_epoch_samples: int = conf_field(MISSING, help="Number of samples in the current epoch")
     num_valid_steps: int = conf_field(MISSING, help="Number of validation steps so far")
     num_test_steps: int = conf_field(MISSING, help="Number of test steps so far")
+    start_time_s: float = conf_field(MISSING, help="Start time of training")
+    elapsed_time_s: float = conf_field(MISSING, help="Total elapsed time so far")
     raw_phase: str = conf_field(MISSING, help="Current training phase")
 
     @property
     def phase(self) -> Phase:
         return cast_phase(self.raw_phase)
 
     @phase.setter
@@ -55,14 +58,16 @@
             num_epochs=0,
             num_steps=0,
             num_epoch_steps=0,
             num_samples=0,
             num_epoch_samples=0,
             num_valid_steps=0,
             num_test_steps=0,
+            start_time_s=time.time(),
+            elapsed_time_s=0.0,
             raw_phase="train",
         )
 
     @property
     def training(self) -> bool:
         return self.phase == "train"
```

### Comparing `ml-starter-0.1.36/ml/launchers/base.py` & `ml-starter-0.1.37/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/launchers/mp.py` & `ml-starter-0.1.37/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/launchers/slurm.py` & `ml-starter-0.1.37/ml/launchers/slurm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-"""Defines a Distributed Data Parallel trainer that launches Slurm jobs.
-
-This is a light-weight wrapper around the PyTorch's built-in Distributed Data
-Parallel class. Note that this only supports one GPU per task, and one task
-per GPU.
+"""Defines a launcher for Slurm jobs.
 
 Steps
 -----
 
 1. Stages the environment to a new working directory
 2. Writes an `sbatch.sh` file
 3. Schedules `sbatch.sh` file
@@ -19,15 +15,15 @@
 import re
 import signal
 import subprocess
 import sys
 from dataclasses import dataclass
 from pathlib import Path
 from types import FrameType
-from typing import TypeVar, cast
+from typing import cast
 
 from omegaconf import II, MISSING, DictConfig, OmegaConf
 
 from ml.core.config import conf_field
 from ml.core.env import get_stage_dir
 from ml.core.registry import Objects, project_dirs, register_launcher, register_trainer
 from ml.launchers.base import BaseLauncher, BaseLauncherConfig
@@ -43,17 +39,15 @@
     set_rank,
     set_world_size,
 )
 from ml.utils.logging import configure_logging
 from ml.utils.staging import stage_environment
 from ml.utils.torch_distributed import init_process_group_from_backend
 
-logger: logging.Logger = logging.getLogger(__name__)
-
-T = TypeVar("T", bound="SlurmLauncher")
+logger = logging.getLogger(__name__)
 
 OmegaConf.register_new_resolver("ml.get_random_slurm_port", get_random_port, replace=True)
 
 SBATCH_TEMPLATE: str = """
 #!/bin/bash
 #SBATCH --job-name={job_name}
 #SBATCH --partition={partition}
@@ -133,15 +127,15 @@
             subprocess.check_call(cmd)
         else:
             logger.info("SLURM_JOB_ID environment variable not found; not requeueing")
 
 
 @dataclass
 class SlurmLauncherConfig(BaseLauncherConfig):
-    partition: str = conf_field(II("oc.env:SLURM_PARTITION,none"), help="Which partition to launch")
+    partition: str = conf_field(II("oc.env:SLURM_PARTITION,missing"), help="Which partition to launch")
     time_limit: str = conf_field(II("oc.env:SLURM_TIME_LIMIT,3-00:00:00"), help="Time limit string")
     num_nodes: int = conf_field(MISSING, help="Total number of nodes to use")
     gpus_per_node: int = conf_field(II("oc.env:SLURM_GPUS_PER_NODE,8"), help="Number of GPUs per node")
     cpus_per_gpu: int = conf_field(II("oc.env:SLURM_CPUS_PER_GPU,1"), help="Number of CPUs per task")
     gpu_type: str | None = conf_field(None, help="Specific GPU type to pass to gres")
     num_jobs: int = conf_field(1, help="Number of redundant jobs to launch")
     comment: str | None = conf_field(None, help="An optional comment to add to the experiment")
@@ -260,15 +254,15 @@
             project_dirs.add(sub_dir)
 
     # Loads the raw config.
     raw_config = cast(DictConfig, OmegaConf.load(args[0]))
     if not OmegaConf.is_dict(raw_config):
         raise ValueError(f"Expected a dict config, got: {raw_config}")
 
-    # Sets environment variables from Clurm environment variables.
+    # Sets environment variables from Slurm environment variables.
     set_slurm_master_addr()
     rank, world_size = set_slurm_rank_and_world_size()
 
     # Sets the initialization method and configures per-rank logging.
     set_init_method(f"tcp://{get_master_addr()}:{get_master_port()}")
     configure_logging(rank=rank, world_size=world_size)
     init_process_group_from_backend()
```

### Comparing `ml-starter-0.1.36/ml/launchers/torchrun.py` & `ml-starter-0.1.37/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/loggers/base.py` & `ml-starter-0.1.37/ml/loggers/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 component has access to a ``MultiLogger`` which it can use to log values.
 After each step, each ``MultiLogger`` sends its values to any implemented
 loggers which have ``should_write`` return ``True``. This lets the implemented
 loggers aggregate values over multiple ``MultiLogger``s. New loggers should
 follow the implementation of one of the existing loggers.
 """
 
-import datetime
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Callable, Generic, TypeVar, Union
 
 from omegaconf import DictConfig
 from torch import Tensor
@@ -41,16 +40,15 @@
     """Defines the base logger."""
 
     log_directory: Path
 
     def __init__(self, config: LoggerConfigT) -> None:
         super().__init__(config)
 
-        self.start_time = datetime.datetime.now()
-        self.last_write_time: dict[Phase, datetime.datetime] = {}
+        self.last_write_time: dict[Phase, float] = {}
 
     def initialize(self, log_directory: Path) -> None:
         self.log_directory = log_directory
 
     def log_scalar(self, key: str, value: Callable[[], Number], state: State, namespace: str) -> None:
         """Logs a scalar value.
 
@@ -139,24 +137,21 @@
 
         Args:
             state: The state to check
 
         Returns:
             If the logger should write values for the current state
         """
-        current_time = datetime.datetime.now()
-        min_write_time_diff = datetime.timedelta(seconds=self.write_every_n_seconds(state))
-
         if state.phase not in self.last_write_time:
-            self.last_write_time[state.phase] = current_time
+            self.last_write_time[state.phase] = state.elapsed_time_s
             return True
-        elif current_time - self.last_write_time[state.phase] < min_write_time_diff:
+        elif state.elapsed_time_s - self.last_write_time[state.phase] < self.write_every_n_seconds(state):
             return False
         else:
-            self.last_write_time[state.phase] = current_time
+            self.last_write_time[state.phase] = state.elapsed_time_s
             return True
 
     @abstractmethod
     def write(self, state: State) -> None:
         """Writes the logs.
 
         Args:
```

### Comparing `ml-starter-0.1.36/ml/loggers/meter.py` & `ml-starter-0.1.37/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/loggers/multi.py` & `ml-starter-0.1.37/ml/loggers/multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,21 +45,14 @@
 
 
 def _chunk_lines(text: str, max_length: int) -> Iterator[str]:
     for i in range(0, len(text), max_length):
         yield text[i : i + max_length]
 
 
-def _get_n_samples(t: Tensor, n: int, dim: int = 0) -> Tensor:
-    if t.shape[dim] <= n:
-        return t
-    idxs = torch.linspace(0, t.shape[dim] - 1, n, device=t.device, dtype=t.dtype).round().long()
-    return torch.index_select(t, dim, idxs)
-
-
 def standardize_text(text: str, max_line_length: int | None = None, remove_non_ascii: bool = False) -> list[str]:
     """Standardizes a text string to a list of lines.
 
     Args:
         text: The text to standardize
         max_line_length: If set, truncate lines to this length
         remove_non_ascii: Remove non-ASCII characters if present
@@ -163,26 +156,41 @@
         raise ValueError(f"Invalid image shape{'' if log_key is None else f' for {log_key}'}: {image.shape}")
 
     if not keep_resolution:
         image = make_human_viewable_resolution(image)
     return image
 
 
+LabelT = TypeVar("LabelT", Sequence[str], None)
+
+
+def _get_n_samples(t: Tensor, labels: LabelT, n: int, dim: int = 0) -> tuple[Tensor, LabelT]:
+    if t.shape[dim] <= n:
+        return t, labels
+    idxs = torch.linspace(0, t.shape[dim] - 1, n, device=t.device, dtype=t.dtype).round().long()
+    t = torch.index_select(t, dim, idxs)
+    if labels is None:
+        return t, None
+    return t, [labels[i] for i in idxs.cpu().tolist()]
+
+
 def standardize_images(
     images: Tensor,
+    labels: LabelT,
     *,
     max_images: int | None = None,
     log_key: str | None = None,
     normalize: bool = True,
     keep_resolution: bool = False,
-) -> Tensor:
+) -> tuple[Tensor, LabelT]:
     """Converts an arbitrary set of images to shape (B, C, H, W).
 
     Args:
         images: The image tensor to log
+        labels: The labels for the images
         max_images: Maximum number of images to select
         log_key: An optional logging key to use in the exception message
         normalize: Normalize images to (0, 1)
         keep_resolution: If set, preserve original image resolution, otherwise
             change image resolution to human-viewable
 
     Returns:
@@ -205,19 +213,20 @@
         elif images.shape[3] in VALID_VIDEO_CHANNEL_COUNTS:
             images = images.permute(0, 3, 1, 2)
         else:
             raise ValueError(f"Invalid channel count{'' if log_key is None else f' for {log_key}'}: {images.shape}")
     else:
         raise ValueError(f"Invalid image shape{'' if log_key is None else f' for {log_key}'}: {images.shape}")
 
-    images = images if max_images is None else _get_n_samples(images, max_images, dim=0)
+    if max_images is not None:
+        images, labels = _get_n_samples(images, labels, max_images, dim=0)
 
     if not keep_resolution:
         images = torch.stack([make_human_viewable_resolution(image) for image in images.unbind(0)], 0)
-    return images
+    return images, labels
 
 
 @functools.lru_cache()
 def audio_warning_ticker() -> IntervalTicker:
     return IntervalTicker(5.0)
 
 
@@ -275,15 +284,16 @@
         elif audios.shape[2] in VALID_AUDIO_CHANNEL_COUNTS:
             audios = audios.permute(2, 1)
         else:
             raise ValueError(f"Invalid channel count{'' if log_key is None else f' for {log_key}'}: {audios.shape}")
     else:
         raise ValueError(f"Invalid audio shape{'' if log_key is None else f' for {log_key}'}: {audios.shape}")
 
-    audios = audios if max_audios is None else _get_n_samples(audios, max_audios, dim=0)
+    if max_audios is not None:
+        audios, _ = _get_n_samples(audios, None, max_audios, dim=0)
 
     max_abs = audios.abs().max()
     if max_abs > 1.0:
         if audio_warning_ticker().tick():
             logger.warning("Audio is outside the range [-1, 1]; clipping")
         audios = audios.clamp(-5e3, 5e3) / max_abs
     return audios
@@ -730,16 +740,17 @@
         """
         namespace = self.resolve_namespace(namespace)
 
         @functools.lru_cache
         def images_future() -> Tensor:
             value_concrete = value() if callable(value) else value
             assert isinstance(value_concrete, Tensor)
-            value_concrete = standardize_images(
+            value_concrete, _ = standardize_images(
                 value_concrete,
+                None,
                 max_images=max_images,
                 log_key=f"{namespace}/{key}",
                 keep_resolution=keep_resolution,
             )
             value_concrete = cast_fp32(value_concrete)
             return make_square_image_or_video(value_concrete, sep=sep)
 
@@ -760,15 +771,15 @@
         """Logs a set of images with labels.
 
         The images are tiled to be nearly-square.
 
         Args:
             key: The key being logged
             value: The images and labels being logged; images can be
-                (B, C, H, W), (B, H, W, C) or (B H, W) as an RGB (3 channel)
+                (B, C, H, W), (B, H, W, C) or (B, H, W) as an RGB (3 channel)
                 or grayscale (1 channel) image, with exactly B labels
             namespace: An optional logging namespace
             max_line_length: Labels longer than this length are wrapped around
             keep_resolution: If set, keep the image resolution the same,
                 otherwise upscale or downscale the image to a standard
                 resolution
             max_images: The maximum number of images to show; extra images
@@ -780,21 +791,22 @@
         namespace = self.resolve_namespace(namespace)
 
         @functools.lru_cache
         def labeled_images_future() -> Tensor:
             images, texts = value() if callable(value) else value
             assert isinstance(images, Tensor)
             assert images.shape[0] == len(texts)
-            num_images = len(images)
-            images = standardize_images(
+            images, texts = standardize_images(
                 images,
+                texts,
                 max_images=max_images,
                 log_key=f"{namespace}/{key}",
                 keep_resolution=keep_resolution,
             )
+            num_images = len(images)
             text_lists = [standardize_text(text, max_line_length, remove_non_ascii=True) for text in texts]
             max_num_lines = max(len(text_list) for text_list in text_lists)
             labeled_images = torch.stack(
                 [
                     image_with_text(images[i], text_lists[i], max_num_lines=max_num_lines, centered=centered)
                     for i in range(num_images)
                 ],
@@ -1039,16 +1051,17 @@
                 return 2 ** round(math.log2(ms * sample_rate / 1000))
 
             n_fft = to_frames(n_fft_ms)
             hop_length = None if hop_length_ms is None else to_frames(hop_length_ms)
             audio = audio.to(torch.float32)
             audio_spec = torch.stft(audio, n_fft, hop_length=hop_length, normalized=True, return_complex=True)
             audio_spec = torch.log10(torch.abs(audio_spec) + 1e-6)
-            audio_spec = standardize_images(
+            audio_spec, _ = standardize_images(
                 audio_spec,
+                None,
                 log_key=f"{namespace}/{key}",
                 keep_resolution=keep_resolution,
             )
             audio_spec = make_square_image_or_video(audio_spec, sep=spec_sep)
             return audio_spec
 
         self.images[namespace][key] = spec_future
```

### Comparing `ml-starter-0.1.36/ml/loggers/stdout.py` & `ml-starter-0.1.37/ml/loggers/stdout.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self.get_log_dict(state, namespace)[key] = value
 
     def write(self, state: State) -> None:
         if not (phase_log_values := self.log_values.get(state.phase)):
             return
 
         # Gets elapsed time since last write.
-        elapsed_time = datetime.datetime.now() - self.start_time
+        elapsed_time = datetime.timedelta(seconds=state.elapsed_time_s)
         elapsed_time_str = format_timedelta(elapsed_time)
 
         def get_section_string(name: str, section: dict[str, Any], level: int = 0) -> str:
             sub_sections: dict[str, dict[str, Any]] = {}
             section_keys = list(section.keys())
             for k in section_keys:
                 ks = k.split("/", maxsplit=1)
```

### Comparing `ml-starter-0.1.36/ml/loggers/tensorboard.py` & `ml-starter-0.1.37/ml/loggers/tensorboard.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,15 +110,16 @@
     header_sep_str = "|-" + "-|-" * (max_len - 1) + "-|"
     rows_str = "\n".join(["| " + " | ".join(row) + " |" for row in rows])
     return "\n".join([header_str, header_sep_str, rows_str])
 
 
 @dataclass
 class TensorboardLoggerConfig(BaseLoggerConfig):
-    flush_seconds: float = conf_field(10, help="How often to flush logs")
+    flush_seconds: float = conf_field(10.0, help="How often to flush logs")
+    wait_seconds: float = conf_field(10.0, help="Time to wait before starting Tensorboard process")
     log_id: str = conf_field(MISSING, help="Unique log ID")
     start_in_subprocess: bool = conf_field(True, help="Start TensorBoard subprocess")
 
     @classmethod
     def resolve(cls, config: "TensorboardLoggerConfig") -> None:
         if OmegaConf.is_missing(config, "log_id"):
             config.log_id = datetime.datetime.now().strftime("%H-%M-%S")
@@ -141,23 +142,26 @@
         self.run_config: DictConfig | None = None
         self.logged_run_config = False
 
         self.line_str: str | None = None
         self.last_tensorboard_write_time = time.time()
 
         self.warning_ticker = IntervalTicker(60.0)
+        self.proc: subprocess.Popen | None = None
 
     def initialize(self, log_directory: Path) -> None:
         super().initialize(log_directory)
 
         # If on master, launch TensorBoard subprocess in a separate thread.
         if is_master():
-            threading.Thread(target=self.worker_thread, daemon=False).start()
+            threading.Thread(target=self.worker_thread, daemon=True).start()
 
     def worker_thread(self) -> None:
+        time.sleep(self.config.wait_seconds)
+
         if "TENSORBOARD_PORT" in os.environ:
             port, use_localhost = int(os.environ["TENSORBOARD_PORT"]), True
         else:
             port, use_localhost = get_unused_port(default=DEFAULT_TENSORBOARD_PORT), False
 
         def make_localhost(s: str) -> str:
             if use_localhost:
@@ -166,57 +170,64 @@
 
         def parse_url(s: str) -> str:
             m = re.search(r" (http\S+?) ", s)
             if m is None:
                 return s
             return f"Tensorboard: {m.group(1)}"
 
-        if not self.config.start_in_subprocess or is_tensorboard_disabled():
-            tensorboard_command_strs = [
-                "tensorboard serve \\",
-                f"  --logdir {self.tensorboard_log_directory} \\",
-                "  --bind_all \\",
-                f"  --port {port} \\",
-                "  --reload_interval 15",
-            ]
-            logger.info("Tensorboard command:\n%s", make_localhost(make_bold(tensorboard_command_strs)))
+        command: list[str] = [
+            "tensorboard",
+            "serve",
+            "--logdir",
+            str(self.tensorboard_log_directory),
+            "--bind_all",
+            "--port",
+            str(port),
+            "--reload_interval",
+            "15",
+        ]
+        logger.info("Tensorboard command: %s", " ".join(command))
 
-        else:
-            command: list[str] = [
-                "tensorboard",
-                "serve",
-                "--logdir",
-                str(self.tensorboard_log_directory),
-                "--bind_all",
-                "--port",
-                str(port),
-                "--reload_interval",
-                "15",
-            ]
-            logger.info("Tensorboard command: %s", " ".join(command))
+        if not self.config.start_in_subprocess:
+            logger.info("Tensorboard subprocess disabled because start_in_subprocess=False")
+
+        elif is_tensorboard_disabled():
+            logger.info("Tensorboard subprocess disabled because DISABLE_TENSORBOARD=1")
 
-            proc = subprocess.Popen(  # pylint: disable=consider-using-with
+        else:
+            self.proc = subprocess.Popen(  # pylint: disable=consider-using-with
                 command,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.STDOUT,
             )
 
             # Gets the output line that shows the running address.
-            assert proc is not None and proc.stdout is not None
-            for line in proc.stdout:
+            assert self.proc is not None and self.proc.stdout is not None
+            for line in self.proc.stdout:
                 line_str = line.decode("utf-8")
                 if line_str.startswith("TensorBoard"):
                     self.line_str = parse_url(make_localhost(line_str))
                     break
 
-            if self.line_str is not None:
+            if self.line_str is None:
+                logger.warning("Failed to parse TensorBoard address")
+            else:
                 logger.info("Running TensorBoard process:\n%s", make_bold([self.line_str], "light-green", "cyan"))
 
-            # Close the process when the program terminates.
-            atexit.register(proc.kill)
+            atexit.register(self.cleanup)
+
+    def cleanup(self) -> None:
+        if self.proc is not None:
+            logger.info("Terminating TensorBoard process")
+            self.proc.terminate()
+            self.proc.wait()
+            self.proc = None
+
+    def __del__(self) -> None:
+        self.cleanup()
 
     @property
     def tensorboard_log_directory(self) -> Path:
         return self.log_directory / "tensorboard" / self.config.log_id
 
     @functools.cached_property
     def train_writer(self) -> SummaryWriter:
@@ -274,14 +285,15 @@
 
     def write(self, state: State) -> None:
         if self.line_str is not None:
             cur_time = time.time()
             if cur_time - self.last_tensorboard_write_time > WRITE_PROC_TEXT_EVERY_N_SECONDS:
                 logger.info("Running TensorBoard process:\n%s", make_bold([self.line_str], "light-green", "cyan"))
                 self.last_tensorboard_write_time = cur_time
+
         writer = self.get_writer(state.phase)
         all_keys: set[str] = set()
 
         def filter_items(items: Iterable[tuple[str, T]]) -> Iterable[tuple[str, T]]:
             duplicate_keys: set[str] = set()
             for k, v in items:
                 if k in all_keys:
@@ -289,35 +301,86 @@
                 else:
                     all_keys.add(k)
                     yield k, v
             if duplicate_keys and self.warning_ticker.tick():
                 logger.warning("Found duplicate logging key(s): %s", duplicate_keys)
 
         for scalar_key, scalar_value in filter_items(self.scalars[state.phase].items()):
-            writer.add_scalar(scalar_key, scalar_value(), global_step=state.num_steps)
+            writer.add_scalar(
+                scalar_key,
+                scalar_value(),
+                global_step=state.num_steps,
+                walltime=state.elapsed_time_s,
+            )
+
         for string_key, string_value in filter_items(self.strings[state.phase].items()):
-            writer.add_text(string_key, string_value(), global_step=state.num_steps)
+            writer.add_text(
+                string_key,
+                string_value(),
+                global_step=state.num_steps,
+                walltime=state.elapsed_time_s,
+            )
+
         for image_key, image_value in filter_items(self.images[state.phase].items()):
-            writer.add_image(image_key, image_value(), global_step=state.num_steps)
+            writer.add_image(
+                image_key,
+                image_value(),
+                global_step=state.num_steps,
+                walltime=state.elapsed_time_s,
+            )
+
         for audio_key, audio_value in filter_items(self.audio[state.phase].items()):
             audio_wav, audio_sample_rate = audio_value()
-            writer.add_audio(audio_key, audio_wav, global_step=state.num_steps, sample_rate=audio_sample_rate)
+            writer.add_audio(
+                audio_key,
+                audio_wav,
+                global_step=state.num_steps,
+                walltime=state.elapsed_time_s,
+                sample_rate=audio_sample_rate,
+            )
+
         for video_key, video_value in filter_items(self.videos[state.phase].items()):
-            writer.add_video(video_key, video_value().unsqueeze(0), global_step=state.num_steps, fps=TARGET_FPS)
+            writer.add_video(
+                video_key,
+                video_value().unsqueeze(0),
+                global_step=state.num_steps,
+                walltime=state.elapsed_time_s,
+                fps=TARGET_FPS,
+            )
+
         for hist_key, hist_value in filter_items(self.histograms[state.phase].items()):
-            writer.add_histogram(hist_key, hist_value(), global_step=state.num_steps)
+            writer.add_histogram(
+                hist_key,
+                hist_value(),
+                global_step=state.num_steps,
+                walltime=state.elapsed_time_s,
+            )
+
         for pc_key, pc_value_func in filter_items(self.point_clouds[state.phase].items()):
             pc_value = pc_value_func()
             bsz, _, _ = pc_value.shape
             colors = torch.randint(0, 255, (bsz, 1, 3), device=pc_value.device).expand_as(pc_value)
             pc_value, colors = pc_value.flatten(0, 1).unsqueeze(0), colors.flatten(0, 1).unsqueeze(0)
-            writer.add_mesh(pc_key, pc_value, colors=colors, global_step=state.num_steps)
+            writer.add_mesh(
+                pc_key,
+                pc_value,
+                colors=colors,
+                global_step=state.num_steps,
+                walltime=state.elapsed_time_s,
+            )
+
         if not self.logged_run_config and self.run_config is not None:
-            writer.add_text("config", to_markdown_table(self.run_config), global_step=state.num_steps)
+            writer.add_text(
+                "config",
+                to_markdown_table(self.run_config),
+                global_step=state.num_steps,
+                walltime=state.elapsed_time_s,
+            )
             self.logged_run_config = True
+
         self.clear(state)
 
     def clear(self, state: State) -> None:
         self.scalars[state.phase].clear()
         self.strings[state.phase].clear()
         self.images[state.phase].clear()
         self.audio[state.phase].clear()
```

### Comparing `ml-starter-0.1.36/ml/lr_schedulers/base.py` & `ml-starter-0.1.37/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/lr_schedulers/constant.py` & `ml-starter-0.1.37/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.37/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.37/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/lr_schedulers/gan.py` & `ml-starter-0.1.37/ml/lr_schedulers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/lr_schedulers/linear.py` & `ml-starter-0.1.37/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.37/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.37/ml/lr_schedulers/scripts/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="import"
 """A simple script for plotting learning rate schedules with various parameters.
 
 This script can be used as follows:
 
 .. code-block:: bash
 
     python -m ml.lr_schedulers.scripts.plot linear /path/to/save.png
@@ -14,16 +15,16 @@
 from ml.core.state import State
 from ml.utils.argparse import add_args, from_args
 
 
 def main() -> None:
     """Plots a learning rate schedule."""
     try:
-        import matplotlib.pyplot as plt  # type: ignore[import]
-    except ImportError as e:
+        import matplotlib.pyplot as plt
+    except ModuleNotFoundError as e:
         raise ImportError("Please install matplotlib to use this script: `pip install matplotlib`") from e
 
     # Gets the plotting-specific arguments.
     parser = argparse.ArgumentParser(description="Plots a learning rate schedule")
     parser.add_argument("lr_scheduler", help="Which scheduler to plot")
     parser.add_argument("save_path", help="Where to save the plot")
     parser.add_argument("-n", "--num-iters", type=int, default=100_000, help="Number of iterations")
```

### Comparing `ml-starter-0.1.36/ml/models/activations.py` & `ml-starter-0.1.37/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/models/base.py` & `ml-starter-0.1.37/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/models/codebook.py` & `ml-starter-0.1.37/ml/models/codebook.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/models/diffusion.py` & `ml-starter-0.1.37/ml/tasks/diffusion/gaussian.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Defines utility functions for Diffusion models.
+# mypy: disable-error-code="import"
+"""Defines the API for Gaussian diffusion.
 
 This module can be used to train a Gaussian diffusion model as follows.
 
 .. code-block:: python
 
     # Instantiate the beta schedule and diffusion module.
     betas = get_diffusion_beta_schedule("linear", 1000)
@@ -29,86 +30,23 @@
 - ``"quad"``: Quadratically increasing beta.
 - ``"warmup"``: Linearly increasing beta with a warmup period.
 - ``"const"``: Constant beta.
 - ``"cosine"``: Cosine annealing schedule.
 - ``"jsd"``: Jensen-Shannon divergence schedule.
 """
 
-import math
 from typing import Callable, Literal, get_args
 
 import torch
 from torch import Tensor, nn
 
-DiffusionBetaSchedule = Literal["linear", "quad", "warmup", "const", "cosine", "jsd"]
+from ml.tasks.diffusion.beta_schedule import DiffusionBetaSchedule, get_diffusion_beta_schedule
+from ml.tasks.losses.loss import loss_fn
 
-
-def _warmup_beta_schedule(
-    beta_start: float,
-    beta_end: float,
-    num_timesteps: int,
-    warmup: float,
-    dtype: torch.dtype = torch.float32,
-) -> Tensor:
-    betas = beta_end * torch.ones(num_timesteps, dtype=dtype)
-    warmup_time = int(num_timesteps * warmup)
-    betas[:warmup_time] = torch.linspace(beta_start, beta_end, warmup_time, dtype=dtype)
-    return betas
-
-
-def _cosine_beta_schedule(
-    num_timesteps: int,
-    offset: float = 0.008,
-    dtype: torch.dtype = torch.float32,
-) -> Tensor:
-    rng = torch.arange(num_timesteps, dtype=dtype)
-    f_t = torch.cos((rng / (num_timesteps - 1) + offset) / (1 + offset) * math.pi / 2) ** 2
-    bar_alpha = f_t / f_t[0]
-    beta = torch.zeros_like(bar_alpha)
-    beta[1:] = (1 - (bar_alpha[1:] / bar_alpha[:-1])).clip(0, 0.999)
-    return beta
-
-
-def get_diffusion_beta_schedule(
-    schedule: DiffusionBetaSchedule,
-    num_timesteps: int,
-    *,
-    beta_start: float = 0.0001,
-    beta_end: float = 0.02,
-    warmup: float = 0.1,
-    dtype: torch.dtype = torch.float32,
-) -> Tensor:
-    """Returns a beta schedule for the given schedule type.
-
-    Args:
-        schedule: The schedule type.
-        num_timesteps: The total number of timesteps.
-        beta_start: The initial beta value.
-        beta_end: The final beta value.
-        warmup: The fraction of timesteps to use for warmup.
-        dtype: The dtype of the returned tensor.
-
-    Returns:
-        The beta schedule, a tensor with shape ``(num_timesteps)``.
-    """
-    match schedule:
-        case "linear":
-            return torch.linspace(beta_start, beta_end, num_timesteps, dtype=dtype)
-        case "quad":
-            return torch.linspace(beta_start**0.5, beta_end**0.5, num_timesteps, dtype=dtype) ** 2
-        case "warmup":
-            return _warmup_beta_schedule(beta_start, beta_end, num_timesteps, warmup, dtype=dtype)
-        case "const":
-            return torch.full((num_timesteps,), beta_end, dtype=dtype)
-        case "cosine":
-            return _cosine_beta_schedule(num_timesteps, dtype=dtype)
-        case "jsd":
-            return torch.linspace(num_timesteps, 1, num_timesteps, dtype=dtype) ** -1.0
-        case _:
-            raise NotImplementedError(f"Unknown schedule type: {schedule}")
+DiffusionPredMode = Literal["pred_x_0", "pred_eps", "pred_v"]
 
 
 def _extract_mul(a: Tensor, t: Tensor, x: Tensor) -> Tensor:
     b, *_ = t.shape
     out = a.gather(-1, t)
     return out.view(b, *((1,) * (len(x.shape) - 1))) * x
 
@@ -117,22 +55,30 @@
     """Defines a module which provides utility functions for Gaussian diffusion.
 
     Parameters:
         betas: The beta values for each timestep, provided by the function
             :func:`get_diffusion_beta_schedule`.
     """
 
-    __constants__ = ["num_timesteps"]
+    __constants__ = ["num_timesteps", "pred_mode"]
 
-    def __init__(self, betas: Tensor, eps: float = 1e-9) -> None:
+    def __init__(
+        self,
+        betas: Tensor,
+        pred_mode: DiffusionPredMode = "pred_eps",
+        loss_type: Literal["mse", "l1"] = "mse",
+        eps: float = 1e-9,
+    ) -> None:
         super().__init__()
 
         assert betas.dim() == 1
 
         self.num_timesteps = betas.shape[0]
+        self.pred_mode = pred_mode
+        self.loss_fn = loss_fn(loss_type)
 
         alphas = 1.0 - betas
         alphas_cum = torch.cumprod(alphas, dim=0)
         alphas_cum_prev = torch.cat([torch.ones(1, dtype=betas.dtype), alphas_cum[:-1]])
         sqrt_alphas_cum = alphas_cum.sqrt()
         sqrt_one_minus_alphas_cum = (1.0 - alphas_cum).sqrt()
         log_one_minus_alpha_cum = alphas_cum.log()
@@ -198,26 +144,40 @@
         lhs = _extract_mul(self.posterior_mean_coef1, t, x_start)
         rhs = _extract_mul(self.posterior_mean_coef2, t, x_t)
         posterior_mean = lhs + rhs
         posterior_var = self.posterior_var.gather(-1, t)
         posterior_log_var_clipped = self.posterior_log_var_clipped.gather(-1, t)
         return posterior_mean, posterior_var, posterior_log_var_clipped
 
-    def q_sample(self, x_start: Tensor, t: Tensor) -> tuple[Tensor, Tensor]:
+    def get_loss(self, y: Tensor, x_start: Tensor, noise: Tensor, t: Tensor) -> Tensor:
+        match self.pred_mode:
+            case "pred_x_0":
+                return self.loss_fn(y, x_start)
+            case "pred_eps":
+                return self.loss_fn(y, noise)
+            case "pred_v":
+                return self.loss_fn(y, self.q_sample(noise, t, x_start)[0])
+            case _:
+                raise NotImplementedError(f"Unknown pred_mode: {self.pred_mode}")
+
+    def q_sample(self, x_start: Tensor, t: Tensor, noise: Tensor | None = None) -> tuple[Tensor, Tensor]:
         r"""Samples a noise tensor from the posterior :math:`q(x_t|x_0)`.
 
         Args:
             x_start: The starting point :math:`x_0`.
             t: The timestep :math:`t`.
+            noise: The noise :math:`\epsilon_t`. If ``None``, a new noise
+                tensor is sampled.
 
         Returns:
             A tuple ``(x_t, noise)`` where ``x_t`` is the sampled point
             :math:`x_t` and ``noise`` is the sampled noise :math:`\\epsilon_t`.
         """
-        noise = torch.randn_like(x_start)
+        if noise is None:
+            noise = torch.randn_like(x_start)
         lhs = _extract_mul(self.sqrt_alphas_cum, t, x_start)
         rhs = _extract_mul(self.sqrt_one_minus_alphas_cum, t, noise)
         x_noisy = lhs + rhs
         return x_noisy, noise
 
     def _predict_start_from_noise(self, x_t: Tensor, t: Tensor, noise: Tensor) -> Tensor:
         lhs = _extract_mul(self.sqrt_recip_alphas_cum, t, x_t)
@@ -261,17 +221,17 @@
 def plot_schedules(*, num_timesteps: int = 1000) -> None:
     """Plots all of the schedules together on one graph.
 
     Args:
         num_timesteps: The number of timesteps to plot
     """
     try:
-        import matplotlib.pyplot as plt  # type: ignore[import]
-    except ImportError as e:
-        raise ImportError("Please install matplotlib to use this script: `pip install matplotlib`") from e
+        import matplotlib.pyplot as plt
+    except ModuleNotFoundError as e:
+        raise ModuleNotFoundError("Please install matplotlib to use this script: `pip install matplotlib`") from e
 
     plt.figure(figsize=(8, 8))
     time = torch.arange(num_timesteps)
     for schedule in get_args(DiffusionBetaSchedule):
         plt.plot(time, get_diffusion_beta_schedule(schedule, num_timesteps=num_timesteps), label=schedule)
     plt.yscale("log")
     plt.legend()
```

### Comparing `ml-starter-0.1.36/ml/models/embeddings.py` & `ml-starter-0.1.37/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/models/gan.py` & `ml-starter-0.1.37/ml/models/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/models/init.py` & `ml-starter-0.1.37/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/models/kmeans.py` & `ml-starter-0.1.37/ml/models/kmeans.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="import"
 """Defines a distributed K-Means module.
 
 This is used to apply K-Means clusters to a tensor. This module can be used
 with cluster centers found via Scikit-Learn, Faiss, or other libraries.
 """
 
 import logging
@@ -27,16 +28,15 @@
 
 def kmeans_fn(use_triton: bool) -> Callable[[Tensor, Tensor, Tensor], Tensor]:
     if torch.cuda.is_available() and use_triton:
         try:
             from ml.utils.triton.kmeans import kmeans as triton_kmeans_fn
 
             return triton_kmeans_fn
-
-        except ImportError:
+        except ModuleNotFoundError:
             logger.warning("Triton is not installed. Using vanilla Lion update function.")
 
     return _vanilla_kmeans
 
 
 class KMeans(nn.Module):
     __constants__ = ["n_clusters", "n_features"]
```

### Comparing `ml-starter-0.1.36/ml/models/lora.py` & `ml-starter-0.1.37/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/models/modules.py` & `ml-starter-0.1.37/ml/models/modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,12 +22,12 @@
         x: Input tensor.
         scale: Scale factor.
 
     Returns:
         The identity of the input tensor in the forward pass, and the scaled
         gradient in the backward pass.
     """
-    return _InvertGrad.apply(input, scale)
+    return _InvertGrad.apply(x, scale)
 
 
 def invert_grad(x: Tensor) -> Tensor:
     return scale_grad(x, -1.0)
```

### Comparing `ml-starter-0.1.36/ml/models/norms.py` & `ml-starter-0.1.37/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/models/parallel.py` & `ml-starter-0.1.37/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/optimizers/adam.py` & `ml-starter-0.1.37/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/optimizers/adan.py` & `ml-starter-0.1.37/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/optimizers/base.py` & `ml-starter-0.1.37/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/optimizers/common.py` & `ml-starter-0.1.37/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/optimizers/gan.py` & `ml-starter-0.1.37/ml/optimizers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/optimizers/lion.py` & `ml-starter-0.1.37/ml/optimizers/lion.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,16 +78,15 @@
 
 def get_update_fn(use_triton: bool) -> Callable[[nn.Parameter, Tensor, Tensor, float, float, float, float], None]:
     if torch.cuda.is_available() and use_triton:
         try:
             from ml.utils.triton.lion import update_fn as triton_update_fn
 
             return triton_update_fn
-
-        except ImportError:
+        except ModuleNotFoundError:
             logger.warning("Triton is not installed. Using vanilla Lion update function.")
 
     return _update_fn_vanilla
 
 
 class Lion(Optimizer):
     def __init__(
```

### Comparing `ml-starter-0.1.36/ml/optimizers/sgd.py` & `ml-starter-0.1.37/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/optimizers/shampoo.py` & `ml-starter-0.1.37/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/scripts/cli.py` & `ml-starter-0.1.37/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/scripts/stage.py` & `ml-starter-0.1.37/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/scripts/train.py` & `ml-starter-0.1.37/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/base.py` & `ml-starter-0.1.37/ml/tasks/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,33 +123,43 @@
     def step(self, state: State) -> None:
         cur_time = time.time()
         self.epoch_timer.step(state.num_epochs, cur_time)
         self.step_timer.step(state.num_steps, cur_time)
         self.sample_timer.step(state.num_samples, cur_time)
         self.iter_timer.step(cur_time)
 
-    def log_dict(self) -> dict[str, int | float]:
-        logs: dict[str, int | float] = {}
+    def log_dict(self) -> dict[str, dict[str, int | float]]:
+        logs: dict[str, dict[str, int | float]] = {}
 
         # Logs epoch statistics (only if at least one epoch seen).
         if self.epoch_timer.steps > 0:
-            logs["epoch"] = self.epoch_timer.steps
-            logs["hours/epoch"] = self.epoch_timer.hours_per_step
+            logs["⏰ epoch"] = {
+                "total": self.epoch_timer.steps,
+                "hours-per": self.epoch_timer.steps_per_hour,
+            }
 
         # Logs step statistics.
-        logs["steps/total"] = self.step_timer.steps
-        logs["steps/second"] = self.step_timer.steps_per_second
-        logs["steps/hour"] = self.step_timer.steps_per_hour
+        logs["⏰ steps"] = {
+            "total": self.step_timer.steps,
+            "per-second": self.step_timer.steps_per_second,
+            "per-hour": self.step_timer.steps_per_hour,
+        }
 
         # Logs sample statistics.
-        logs["samples/total"] = self.sample_timer.steps
-        logs["samples/second"] = self.sample_timer.steps_per_second
-        logs["samples/hour"] = self.sample_timer.steps_per_hour
+        logs["⏰ samples"] = {
+            "total": self.sample_timer.steps,
+            "per-second": self.sample_timer.steps_per_second,
+            "per-hour": self.sample_timer.steps_per_hour,
+        }
+
+        # Logs full iteration statistics.
+        logs["⏰ dt"] = {
+            "iter": self.iter_timer.iter_seconds,
+        }
 
-        logs["dt/iter"] = self.iter_timer.iter_seconds
         return logs
 
 
 @dataclass
 class DataLoaderConfig:
     batch_size: int = conf_field(MISSING, help="Size of each batch")
     shuffle: bool = conf_field(MISSING, help="Should the batches be shuffled on each iteration")
@@ -199,22 +209,22 @@
 
 
 @dataclass
 class FinishTrainingConfig:
     max_epochs: int | None = conf_field(None, help="Maximum number of epochs to run")
     max_steps: int | None = conf_field(None, help="Maximum number of steps to run")
     max_samples: int | None = conf_field(None, help="Maximum number of samples to run")
+    max_seconds: float | None = conf_field(None, help="Maximum number of seconds to run")
 
 
 @dataclass
 class BaseTaskConfig(BaseConfig, DataLoaderConfigs, FinishTrainingConfig):
     """Defines the base config for all tasks."""
 
     errors: ErrorHandlingConfig = conf_field(ErrorHandlingConfig(), help="Error handling config")
-    disable_autocast_for_loss: bool = conf_field(True, help="Disable autocast for loss calculation")
 
 
 BaseTaskConfigT = TypeVar("BaseTaskConfigT", bound=BaseTaskConfig)
 ModelT = TypeVar("ModelT", bound=BaseModel)
 
 
 class BaseTask(
@@ -234,17 +244,14 @@
             "valid": self.config.valid_dl,
             "test": self.config.test_dl,
         }
 
         # This flag can be toggled to end training from anywhere in the task.
         self.__training_over_flag = False
 
-        # Used in the internals of the task.
-        self.__disable_autocast_for_loss = self.config.disable_autocast_for_loss
-
         # Timers for iterations.
         self.train_timer = StateTimer()
         self.valid_timer = StateTimer()
         self.test_timer = StateTimer()
 
         # Used to log values.
         self.logger = MultiLogger(default_namespace="task")
@@ -257,18 +264,14 @@
     def _get_device(self) -> base_device:
         return detect_device()
 
     @torch.jit.ignore
     def _get_device_type(self) -> str:
         return self._device._get_device().type
 
-    @property
-    def disable_autocast_for_loss(self) -> bool:
-        return self.__disable_autocast_for_loss
-
     @abstractmethod
     def run_model(self, model: ModelT, batch: Batch, state: State) -> Output:
         """Runs a single training step and returns the outputs.
 
         Args:
             model: The current nn.Module
             batch: The current batch
@@ -319,28 +322,28 @@
         single_loss = torch.stack(losses, dim=0)
         return single_loss, keys
 
     def log_loss_dict(self, loss: Mapping[str, int | float | Tensor], state: State) -> None:
         for k, v in loss.items():
             self.logger.log_scalar(k, v, namespace="loss")
 
-        if state.phase == "train":
-            self.train_timer.step(state)
-            for k, v in self.train_timer.log_dict().items():
-                self.logger.log_scalar(k, v, namespace="timers")
-        elif state.phase == "valid":
-            self.valid_timer.step(state)
-            for k, v in self.valid_timer.log_dict().items():
-                self.logger.log_scalar(k, v, namespace="timers")
-        elif state.phase == "test":
-            self.test_timer.step(state)
-            for k, v in self.test_timer.log_dict().items():
-                self.logger.log_scalar(k, v, namespace="timers")
-        else:
-            raise NotImplementedError(f"Unexpected phase: {state.phase}")
+        match state.phase:
+            case "train":
+                timer = self.train_timer
+            case "valid":
+                timer = self.valid_timer
+            case "test":
+                timer = self.test_timer
+            case _:
+                raise NotImplementedError(f"Unexpected phase: {state.phase}")
+
+        timer.step(state)
+        for ns, d in timer.log_dict().items():
+            for k, v in d.items():
+                self.logger.log_scalar(k, v, namespace=ns)
 
     def get_batch_size(self, batch: Batch) -> int | None:
         if isinstance(batch, (np.ndarray, Tensor)):
             return batch.shape[0]
         if is_dataclass(batch):
             for v in batch.__dict__.values():
                 if bsz := self.get_batch_size(v):
@@ -362,23 +365,25 @@
         remaining_percents: list[float] = []
         if self.config.max_epochs is not None:
             remaining_percents.append((self.config.max_epochs - state.num_epochs) / self.config.max_epochs)
         if self.config.max_steps is not None:
             remaining_percents.append((self.config.max_steps - state.num_steps) / self.config.max_steps)
         if self.config.max_samples is not None:
             remaining_percents.append((self.config.max_samples - state.num_samples) / self.config.max_samples)
+        if self.config.max_seconds is not None:
+            remaining_percents.append((self.config.max_seconds - state.elapsed_time_s) / self.config.max_seconds)
         return None if len(remaining_percents) == 0 else min(remaining_percents)
 
     def is_training_over(self, state: State) -> bool:
         if self.__training_over_flag:
             return True
         remaining_percent = self.get_remaining_percent(state)
         if remaining_percent is None:
             return False
-        self.logger.log_scalar("remaining", remaining_percent, namespace="timers")
+        self.logger.log_scalar("percent", remaining_percent, namespace="⏰ remaining")
         return remaining_percent <= 0.0
 
     def get_sampler(self, dataset: Dataset, cfg: DataLoaderConfig, phase: Phase) -> Sampler[int]:
         """Returns a dataset sampler to use instead of random sampling.
 
         The default behavior for a non-iterable dataset is to use a
         RandomSampler for all the elements from the dataset. The sampler
@@ -465,15 +470,15 @@
         )
 
     @classmethod
     def worker_init_fn(cls, worker_id: int) -> None:
         set_random_seed(offset=worker_id)
 
     @classmethod
-    def collate_fn(cls, items: list[Any], *, mode: CollateMode = "stack") -> Any | None:
+    def collate_fn(cls, items: list[Any], *, mode: CollateMode = "stack") -> Any | None:  # noqa: ANN401
         return collate(items, mode=mode)
 
     # -----
     # Hooks
     # -----
 
     def on_after_load_checkpoint(self, ckpt: dict[str, Any]) -> None:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ml-starter-0.1.36/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.37/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.37/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/datasets/collate.py` & `ml-starter-0.1.37/ml/tasks/datasets/collate.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
 
 def collate(
     items: list[Any],
     *,
     mode: CollateMode | Callable[[list[Tensor]], Tensor] = "stack",
     pad: bool | Callable[[list[Tensor]], list[Tensor]] = False,
-) -> Any | None:
+) -> Any | None:  # noqa: ANN401
     """Defines a general-purpose collating function.
 
     Args:
         items: The list of items to collate
         mode: Either `stack`, `concat`, or a custom function which is called on
             a list of tensors and returns a single tensor
         pad: If set to True, pads sequences using the default padding function.
```

### Comparing `ml-starter-0.1.36/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.37/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.37/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.37/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.37/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.37/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.37/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/environments/base.py` & `ml-starter-0.1.37/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/environments/utils.py` & `ml-starter-0.1.37/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/environments/worker.py` & `ml-starter-0.1.37/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/gan/base.py` & `ml-starter-0.1.37/ml/tasks/gan/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,16 +183,18 @@
         batch: Batch,
         state: State,
         output: tuple[GeneratorOutput, DiscriminatorOutput],
     ) -> dict[str, Tensor]:
         gen_model, dis_model = model.generator, model.discriminator
         gen_output, dis_output = output
         if self.is_generator_step(state):
-            return self.compute_generator_loss(gen_model, dis_model, batch, state, gen_output, dis_output)
-        return self.compute_discriminator_loss(gen_model, dis_model, batch, state, gen_output, dis_output)
+            losses = self.compute_generator_loss(gen_model, dis_model, batch, state, gen_output, dis_output)
+        else:
+            losses = self.compute_discriminator_loss(gen_model, dis_model, batch, state, gen_output, dis_output)
+        return losses
 
     # -----
     # Hooks
     # -----
 
     def on_after_gan_forward_step(
         self,
```

### Comparing `ml-starter-0.1.36/ml/tasks/losses/audio.py` & `ml-starter-0.1.37/ml/tasks/losses/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/losses/image.py` & `ml-starter-0.1.37/ml/tasks/losses/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/losses/kl.py` & `ml-starter-0.1.37/ml/tasks/losses/kl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/losses/loss.py` & `ml-starter-0.1.37/ml/tasks/losses/loss.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/rl/base.py` & `ml-starter-0.1.37/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/rl/replay.py` & `ml-starter-0.1.37/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/tasks/sl/base.py` & `ml-starter-0.1.37/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/trainers/base.py` & `ml-starter-0.1.37/ml/trainers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 setting up the experiment directory, saving checkpoints, and logging.
 """
 
 import enum
 import logging
 import os
 import signal
+import time
 from dataclasses import asdict, dataclass
 from pathlib import Path
 from pickle import UnpicklingError
 from typing import Any, Callable, Generic, Literal, TypeVar, cast, get_args
 
 import torch
 from omegaconf import II, MISSING, DictConfig, ListConfig, OmegaConf
@@ -47,22 +48,28 @@
 
 def cpu_count(default: int) -> int:
     if (cpu_count := os.cpu_count()) is not None:
         return cpu_count
     return default
 
 
+def date_str(_: str) -> str:
+    return time.strftime("%Y-%m-%d")
+
+
 OmegaConf.register_new_resolver("ml.abs_path", abs_path, replace=True)
 OmegaConf.register_new_resolver("ml.cpu_count", cpu_count, replace=True)
+OmegaConf.register_new_resolver("ml.date_str", date_str, replace=True)
 
 LockType = Literal["running", "scheduled", "ckpt"]
 
 
 def add_lock_file(exp_dir: Path, lock_type: LockType, *, exists_ok: bool = False) -> None:
     if is_master():
+        exp_dir.mkdir(exist_ok=True, parents=True)
         if (lock_file := exp_dir / f".lock_{lock_type}").exists():
             if not exists_ok:
                 raise RuntimeError(f"Lock file already exists at {lock_file}")
         else:
             with open(lock_file, "w", encoding="utf-8") as f:
                 f.write(f"PID: {os.getpid()}")
             logger.debug("Added %s lock file to experiment directory %s", lock_type, exp_dir)
@@ -208,14 +215,15 @@
             OmegaConf.save(raw_config, config_path)
             logger.info("Saved config to %s", config_path)
 
 
 @dataclass
 class CheckpointConfig:
     save_every_n_steps: int | None = conf_field(None, help="Save a checkpoint every N steps")
+    save_every_n_seconds: int | None = conf_field(None, help="Save a checkpoint every N seconds")
     only_save_most_recent: bool = conf_field(False, help="Only keep the most recent checkpoint")
     load_from_ckpt_path: str | None = conf_field(None, help="If set, load initial model weights from this path")
 
 
 @dataclass
 class BaseTrainerConfig(BaseConfig):
     """Defines the base config for all trainers."""
@@ -266,14 +274,16 @@
 
         logger.info("Experiment directory: %s", self.exp_dir)
 
         self._device = self._get_device()
         self._device_type = self._get_device_type()
         self._weight_precision = self._get_weight_precision()
 
+        self.__last_ckpt_time = time.time()
+
     def _get_device(self) -> base_device:
         dev = detect_device()
         self.logger.log_string("device", str(dev))
         return dev
 
     def _get_device_type(self) -> str:
         return self._device._get_device().type
@@ -316,14 +326,19 @@
     def ckpt_path(self) -> Path:
         return self.get_ckpt_path()
 
     def should_checkpoint(self, state: State) -> bool:
         if self.checkpoint_config.save_every_n_steps is not None:
             if state.num_steps % self.checkpoint_config.save_every_n_steps == 0:
                 return True
+        if self.checkpoint_config.save_every_n_seconds is not None:
+            last_time, cur_time = self.__last_ckpt_time, time.time()
+            if cur_time - last_time >= self.checkpoint_config.save_every_n_seconds:
+                self.__last_ckpt_time = cur_time
+                return True
         return False
 
     def load_checkpoint(
         self,
         ckpt: str | Path | dict,
         task: TaskT,
         model: ModelT,
@@ -526,16 +541,16 @@
         for signal_handler in self.signal_handlers.get(sig, []):
             signal_handler()
 
     def add_signal_handler(self, sig: signal.Signals, handler: Callable[[], None]) -> None:
         self.signal_handlers[sig].append(handler)
 
     def _log_prefetcher_stats(self, pf: Prefetcher) -> None:
-        self.logger.log_scalar("dt/get_batch", pf.get_batch_time, namespace="timers")
-        self.logger.log_scalar("dt/to_device", pf.to_device_time, namespace="timers")
+        self.logger.log_scalar("get_batch", pf.get_batch_time, namespace="⏰ dt")
+        self.logger.log_scalar("to_device", pf.to_device_time, namespace="⏰ dt")
 
     # -----
     # Hooks
     # -----
 
     def on_step_start(
         self,
@@ -553,34 +568,38 @@
         loss_dict: dict[str, Tensor],
         task: TaskT,
         model: ModelT,
         optim: Optimizer | dict[str, Optimizer],
         lr_sched: SchedulerAdapter | dict[str, SchedulerAdapter],
     ) -> None:
         task.on_step_end(state, loss_dict, model, optim, lr_sched)
+        state.elapsed_time_s = time.time() - state.start_time_s
 
     def on_epoch_start(
         self,
         state: State,
         task: TaskT,
         model: ModelT,
         optim: Optimizer | dict[str, Optimizer],
         lr_sched: SchedulerAdapter | dict[str, SchedulerAdapter],
     ) -> None:
         task.on_epoch_start(state, model, optim, lr_sched)
+        state.num_epoch_steps = 0
+        state.num_epoch_samples = 0
 
     def on_epoch_end(
         self,
         state: State,
         task: TaskT,
         model: ModelT,
         optim: Optimizer | dict[str, Optimizer],
         lr_sched: SchedulerAdapter | dict[str, SchedulerAdapter],
     ) -> None:
         task.on_epoch_end(state, model, optim, lr_sched)
+        state.num_epochs += 1
 
     def on_training_start(
         self,
         state: State,
         task: TaskT,
         model: ModelT,
         optim: Optimizer | dict[str, Optimizer],
```

### Comparing `ml-starter-0.1.36/ml/trainers/gan.py` & `ml-starter-0.1.37/ml/trainers/gan.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,17 +156,14 @@
                                     model=model,
                                 )
 
                 while True:
                     with self.step_context("on_epoch_start"):
                         self.on_epoch_start(state, task, model, optims, lr_scheds)
 
-                    state.num_epoch_steps = 0
-                    state.num_epoch_samples = 0
-
                     def batch_splitter() -> Iterator[Batch]:
                         num_chunks = self.get_batch_chunks(state)
                         for batch in train_pf:
                             yield from recursive_chunk(batch, num_chunks, dim=self.config.batch_dim)
 
                     train_pf_iter: Iterator = batch_splitter()
 
@@ -237,16 +234,14 @@
 
                         with self.step_context("on_step_end"):
                             self.on_step_end(state, loss_dict, task, model, optims, lr_scheds)
 
                     with self.step_context("on_epoch_end"):
                         self.on_epoch_end(state, task, model, optims, lr_scheds)
 
-                    state.num_epochs += 1
-
         except TrainingFinishedError:
             self.save_checkpoint(state, task, model, optims, lr_scheds)
             logger.info(
                 "Finished training after %d epochs, %d steps, %d samples",
                 state.num_epochs,
                 state.num_steps,
                 state.num_samples,
```

### Comparing `ml-starter-0.1.36/ml/trainers/learning.py` & `ml-starter-0.1.37/ml/trainers/learning.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,42 +76,43 @@
         with self.step_context("change_mode"):
             task_model, state.phase = set_phase(task_model, "train")
         total_bsz: int | None = None
         losses: dict[str, tuple[Tensor, int]] = {}
         with self.step_context("zero_grads"):
             optim.zero_grad(set_to_none=self.config.set_to_none)
         num_steps = 0
-        for batch in batches:
-            bsz = task.get_batch_size(batch)
-            if bsz is not None:
-                total_bsz = bsz if total_bsz is None else total_bsz + bsz
-            with self.step_context("forward"), self.autocast_context:
-                loss = task_model(batch, state)
-            with self.step_context("get_single_loss"):
-                single_loss, loss_names = task.get_single_loss(loss)
-            with self.step_context("backward"):
-                self.backward_grads(task_model, single_loss)
-            with self.step_context("log_losses"):
-                self.log_mp_scale()
-                single_loss_detached = single_loss.detach()
-                for i, name in enumerate(loss_names):
-                    new_loss = single_loss_detached[i]
-                    if name in losses:
-                        old_loss, count = losses[name]
-                        losses[name] = (old_loss + new_loss, count + 1)
-                    else:
-                        losses[name] = (new_loss, 1)
-            num_steps += 1
+        with self.autocast_context:
+            for batch in batches:
+                bsz = task.get_batch_size(batch)
+                if bsz is not None:
+                    total_bsz = bsz if total_bsz is None else total_bsz + bsz
+                with self.step_context("forward"):
+                    loss = task_model(batch, state)
+                with self.step_context("get_single_loss"):
+                    single_loss, loss_names = task.get_single_loss(loss)
+                with self.step_context("backward"):
+                    self.backward_grads(task_model, single_loss)
+                with self.step_context("log_losses"):
+                    self.log_mp_scale()
+                    single_loss_detached = single_loss.detach()
+                    for i, name in enumerate(loss_names):
+                        new_loss = single_loss_detached[i]
+                        if name in losses:
+                            old_loss, count = losses[name]
+                            losses[name] = (old_loss + new_loss, count + 1)
+                        else:
+                            losses[name] = (new_loss, 1)
+                num_steps += 1
         with self.step_context("log_losses"):
             loss_dict = {k: value / count for k, (value, count) in losses.items()}
             task.log_loss_dict(loss_dict, state)
         with self.step_context("step"):
             self.step_optimizer(model, optim, num_steps)
             lr_sched.step(state)
-            self.logger.log_scalar("lr_scale", lr_sched.lr_scale, namespace="optim")
+            self.logger.log_scalar("lr_scale", lr_sched.lr_scale, namespace="📉 optim")
         with self.step_context("write_logs"), self.autocast_context:
             self.write_logs(task, model, state)
         with self.step_context("update_state"):
             state.num_steps += 1
             state.num_epoch_steps += 1
             if total_bsz is not None:
                 state.num_samples += total_bsz
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ml-starter-0.1.36/ml/trainers/mixins/compile.py` & `ml-starter-0.1.37/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.37/ml/trainers/mixins/cpu_stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -246,17 +246,17 @@
     ) -> None:
         super().on_step_start(state, task, model, optim, lr_sched)
 
         monitor = self._cpu_stats_monitor
         stats = monitor.get_if_set() if self.config.cpu_stats_only_log_once else monitor.get()
 
         if stats is not None:
-            self.logger.log_scalar("cpu/child_procs", stats.num_child_procs, namespace="trainer")
-            self.logger.log_scalar("cpu/percent", stats.cpu_percent, namespace="trainer")
-            self.logger.log_scalar("cpu/child_percent", stats.child_cpu_percent, namespace="trainer")
-            self.logger.log_scalar("mem/percent", stats.mem_percent, namespace="trainer")
-            self.logger.log_scalar("mem/shared", stats.mem_shared, namespace="trainer")
-            self.logger.log_scalar("mem/child_percent", stats.child_mem_percent, namespace="trainer")
-            self.logger.log_scalar("mem/rss/cur", stats.mem_rss, namespace="trainer")
-            self.logger.log_scalar("mem/rss/total", stats.mem_rss_total, namespace="trainer")
-            self.logger.log_scalar("mem/vms/cur", stats.mem_vms, namespace="trainer")
-            self.logger.log_scalar("mem/vms/total", stats.mem_vms_total, namespace="trainer")
+            self.logger.log_scalar("child_procs", stats.num_child_procs, namespace="💻 cpu")
+            self.logger.log_scalar("percent", stats.cpu_percent, namespace="💻 cpu")
+            self.logger.log_scalar("child_percent", stats.child_cpu_percent, namespace="💻 cpu")
+            self.logger.log_scalar("percent", stats.mem_percent, namespace="💻 mem")
+            self.logger.log_scalar("shared", stats.mem_shared, namespace="💻 mem")
+            self.logger.log_scalar("child_percent", stats.child_mem_percent, namespace="💻 mem")
+            self.logger.log_scalar("rss/cur", stats.mem_rss, namespace="💻 mem")
+            self.logger.log_scalar("rss/total", stats.mem_rss_total, namespace="💻 mem")
+            self.logger.log_scalar("vms/cur", stats.mem_vms, namespace="💻 mem")
+            self.logger.log_scalar("vms/total", stats.mem_vms_total, namespace="💻 mem")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ml-starter-0.1.36/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.37/ml/trainers/mixins/data_parallel.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,19 +44,15 @@
         self.task = task
         self.model = model
 
     def forward(self, batch: Batch, state: State) -> Loss:
         self.task.on_before_forward_step(self.model, batch, state)
         output = self.task.run_model(self.model, batch, state)
         self.task.on_after_forward_step(self.model, batch, output, state)
-        if self.task.disable_autocast_for_loss:
-            loss = self.task.compute_loss(self.model, batch, state, output)
-        else:
-            with self.task._device.autocast_context(enabled=False):
-                loss = self.task.compute_loss(self.model, batch, state, output)
+        loss = self.task.compute_loss(self.model, batch, state, output)
         self.task.on_after_compute_loss(self.model, batch, output, loss, state)
         return loss
 
 
 @dataclass
 class ParallelConfig:
     use_fsdp: bool = conf_field(False, help="If set, use FSDP; otherwise, use DDP")
```

### Comparing `ml-starter-0.1.36/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.37/ml/trainers/mixins/gpu_stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -262,10 +262,10 @@
             return
 
         stats = monitor.get_if_set() if self.config.gpu_stats_only_log_once else monitor.get()
 
         for gpu_stat in stats.values():
             if gpu_stat is None:
                 continue
-            self.logger.log_scalar(f"gpu/{gpu_stat.index}/mem_used", gpu_stat.memory_used, namespace="trainer")
-            self.logger.log_scalar(f"gpu/{gpu_stat.index}/temp", gpu_stat.temperature, namespace="trainer")
-            self.logger.log_scalar(f"gpu/{gpu_stat.index}/gpu_util", gpu_stat.utilization, namespace="trainer")
+            self.logger.log_scalar(f"mem/{gpu_stat.index}", gpu_stat.memory_used, namespace="💻 gpu")
+            self.logger.log_scalar(f"temp/{gpu_stat.index}", gpu_stat.temperature, namespace="💻 gpu")
+            self.logger.log_scalar(f"util/{gpu_stat.index}", gpu_stat.utilization, namespace="💻 gpu")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ml-starter-0.1.36/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.37/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.37/ml/trainers/mixins/mixed_precision.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,16 +114,16 @@
                 model.parameters(),
                 max_norm=clip_norm,
                 norm_type=norm_type,
                 foreach=True,
             )
 
         # Logs weight and gradient norms.
-        self.logger.log_scalar("weight_norm", lambda: get_weight_norm(model.parameters()), namespace="optim")
-        self.logger.log_scalar("grad_norm", total_norm, namespace="optim")
+        self.logger.log_scalar("weight_norm", lambda: get_weight_norm(model.parameters()), namespace="📉 optim")
+        self.logger.log_scalar("grad_norm", total_norm, namespace="📉 optim")
 
         # Steps the optimizer.
         if self.grad_scaler is None:
             if was_clipped:
                 optim.step()
         elif was_clipped:
             self.grad_scaler.step(optim)
@@ -135,16 +135,16 @@
             if new_scale < self.config.mixed_precision.min_grad_scale:
                 raise MinGradScaleError("Minimum gradient scale reached; your loss is probably exploding")
             logger.warning("Gradient NaNs detected; reducing scale to %.2g", new_scale)
             self.grad_scaler.update(new_scale)
 
     def log_mp_scale(self) -> None:
         if (scaler := self.grad_scaler) is not None and scaler._enabled:
-            self.logger.log_scalar("fp16_scale", scaler.get_scale)
-            self.logger.log_scalar("fp16_growth", scaler._get_growth_tracker)
+            self.logger.log_scalar("scale", scaler.get_scale, namespace="⚖️ fp16")
+            self.logger.log_scalar("growth", scaler._get_growth_tracker, namespace="⚖️ fp16")
 
     def load_state_dict(self, ckpt: dict[str, Any]) -> None:
         if self.grad_scaler is not None:
             self.grad_scaler.load_state_dict(ckpt["grad_scaler"])
 
         super().load_state_dict(ckpt)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ml-starter-0.1.36/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.37/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.37/ml/trainers/mixins/profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             step_time = time.time() - start_time
             self.step_times[step] = step_time + self.step_times.get(step, 0.0)
 
         return wrapped_ctx()
 
     def write_logs(self, task: TaskT, model: ModelT, state: State) -> None:
         for step, step_time in self.step_times.items():
-            self.logger.log_scalar(f"dt/{step}", step_time, namespace="timers")
+            self.logger.log_scalar(step, step_time, namespace="⏰ dt")
 
         super().write_logs(task, model, state)
 
         # Empty step times when done, so we only log the current step times.
         self.step_times.clear()
 
     def on_profiler_trace_ready(self, prof: torch.profiler.profile) -> None:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ml-starter-0.1.36/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.37/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/trainers/rl.py` & `ml-starter-0.1.37/ml/trainers/rl.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,17 +110,14 @@
                 if profile is not None:
                     ctx.enter_context(profile)
 
                 while True:
                     with self.step_context("on_epoch_start"):
                         self.on_epoch_start(state, task, model, optim, lr_sched)
 
-                    state.num_epoch_steps = 0
-                    state.num_epoch_samples = 0
-
                     with self.step_context("collect_rl_samples"), self.autocast_context:
                         samples = task.collect_samples(
                             model=model,
                             worker_pool=worker_pool,
                             total_samples=self.config.sampling.num_epoch_samples,
                             min_trajectory_length=self.config.sampling.min_trajectory_length,
                             max_trajectory_length=self.config.sampling.max_trajectory_length,
@@ -168,16 +165,14 @@
 
                         if task.epoch_is_over(state):
                             break
 
                     with self.step_context("on_epoch_end"):
                         self.on_epoch_end(state, task, model, optim, lr_sched)
 
-                    state.num_epochs += 1
-
         except TrainingFinishedError:
             self.save_checkpoint(state, task, model, optim, lr_sched)
             logger.info(
                 "Finished training after %d epochs, %d steps, %d samples",
                 state.num_epochs,
                 state.num_steps,
                 state.num_samples,
```

### Comparing `ml-starter-0.1.36/ml/trainers/sl.py` & `ml-starter-0.1.37/ml/trainers/sl.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 from omegaconf import MISSING
 
 from ml.core.common_types import Batch
 from ml.core.config import conf_field
 from ml.core.registry import register_trainer
 from ml.core.state import State
 from ml.lr_schedulers.base import BaseLRScheduler
+from ml.models.gan import GenerativeAdversarialNetworkModel
 from ml.optimizers.base import BaseOptimizer
+from ml.tasks.gan.base import GenerativeAdversarialNetworkTask
 from ml.tasks.sl.base import SupervisedLearningTask
 from ml.trainers.base import ModelT
 from ml.trainers.learning import BaseLearningTrainer, BaseLearningTrainerConfig
 from ml.utils.containers import recursive_chunk
 from ml.utils.device.base import InfinitePrefetcher
 from ml.utils.exceptions import EpochDoneError, TrainingFinishedError
 from ml.utils.timer import Timer
@@ -120,14 +122,18 @@
             lr_scheduler: The current learning rate scheduler
 
         Raises:
             ValueError: If the task is not a supervised learning task
         """
         if not isinstance(task, SupervisedLearningTask):
             raise ValueError(f"Expected task to be a SupervisedLearningTask, got {type(task)}")
+        if isinstance(model, GenerativeAdversarialNetworkModel):
+            raise ValueError("Model is a GenerativeAdversarialNetworkModel, use `gan` trainer instead")
+        if isinstance(task, GenerativeAdversarialNetworkTask):
+            raise ValueError("Task is a GenerativeAdversarialNetworkTask, use `gan` trainer instead")
 
         self._init_environment()
 
         with Timer("compiling model", spinner=True):
             model = self._compile_model(model)
 
         with Timer("compiling training step", spinner=True):
@@ -184,17 +190,14 @@
                                 model=model,
                             )
 
                 while True:
                     with self.step_context("on_epoch_start"):
                         self.on_epoch_start(state, task, model, optim, lr_sched)
 
-                    state.num_epoch_steps = 0
-                    state.num_epoch_samples = 0
-
                     def batch_splitter() -> Iterator[Batch]:
                         num_chunks = self.get_batch_chunks(state)
                         for batch in train_pf:
                             yield from recursive_chunk(batch, num_chunks, dim=self.config.batch_dim)
 
                     train_pf_iter: Iterator = batch_splitter()
 
@@ -253,16 +256,14 @@
 
                         with self.step_context("on_step_end"):
                             self.on_step_end(state, loss_dict, task, model, optim, lr_sched)
 
                     with self.step_context("on_epoch_end"):
                         self.on_epoch_end(state, task, model, optim, lr_sched)
 
-                    state.num_epochs += 1
-
         except TrainingFinishedError:
             self.save_checkpoint(state, task, model, optim, lr_sched)
             logger.info(
                 "Finished training after %d epochs, %d steps, %d samples",
                 state.num_epochs,
                 state.num_steps,
                 state.num_samples,
```

### Comparing `ml-starter-0.1.36/ml/utils/amp.py` & `ml-starter-0.1.37/ml/utils/amp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/argparse.py` & `ml-starter-0.1.37/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/atomic.py` & `ml-starter-0.1.37/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/attention.py` & `ml-starter-0.1.37/ml/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/audio.py` & `ml-starter-0.1.37/ml/utils/audio.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,16 +59,16 @@
                 num_frames=stream.duration,
             )
 
     @classmethod
     def from_file_ffmpeg(cls, fpath: str | Path) -> "AudioProps":
         try:
             import ffmpeg
-        except ImportError as e:
-            raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
+        except ModuleNotFoundError as e:
+            raise ModuleNotFoundError("Install FFMPEG to use this function: `pip install ffmpeg-python`") from e
 
         probe = ffmpeg.probe(str(fpath))
 
         for stream in probe["streams"]:
             if stream["codec_type"] == "audio":
                 return cls(
                     sample_rate=int(stream["sample_rate"]),
@@ -131,16 +131,16 @@
     Yields:
         Audio chunks as numpy arrays, with shape (n_channels, n_samples).
     """
     props = AudioProps.from_file_ffmpeg(in_file)
 
     try:
         import ffmpeg
-    except ImportError as e:
-        raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
+    except ModuleNotFoundError as e:
+        raise ModuleNotFoundError("Install FFMPEG to use this function: `pip install ffmpeg-python`") from e
 
     stream = ffmpeg.input(str(in_file))
     stream = ffmpeg.output(stream, "pipe:", format="f32le", acodec="pcm_f32le")
     stream = ffmpeg.run_async(stream, pipe_stdout=True, quiet=True)
 
     while True:
         chunk = stream.stdout.read(chunk_size)
@@ -225,16 +225,16 @@
         sampling_rate: Sampling rate of the audio.
     """
     first_frame = _cleanup_wav_chunk(as_numpy_array(next(itr)))
     assert (channels := first_frame.shape[0]) in (1, 2), f"Expected 1 or 2 channels, got {channels}"
 
     try:
         import ffmpeg
-    except ImportError as e:
-        raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
+    except ModuleNotFoundError as e:
+        raise ModuleNotFoundError("Install FFMPEG to use this function: `pip install ffmpeg-python`") from e
 
     stream = ffmpeg.input("pipe:", format="f32le", acodec="pcm_f32le", ar=sampling_rate, ac=channels)
     stream = ffmpeg.output(stream, str(out_file))
     stream = ffmpeg.overwrite_output(stream)
     stream = ffmpeg.run_async(stream, pipe_stdin=True, quiet=True)
 
     def get_bytes(frame: np.ndarray) -> bytes:
```

### Comparing `ml-starter-0.1.36/ml/utils/augmentation.py` & `ml-starter-0.1.37/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/caching.py` & `ml-starter-0.1.37/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/checkpoint.py` & `ml-starter-0.1.37/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/cli.py` & `ml-starter-0.1.37/ml/utils/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         args: The raw command-line arguments to parse
 
     Returns:
         The raw config, loaded from the provided arguments
     """
 
     def show_help() -> None:
-        print("Usage: cmd <path/to/config.yaml> [<new_config.yaml>, ...] overrida.a=1 override.b=2", file=sys.stderr)
+        print("\nUsage: cmd <path/to/config.yaml> [<new_config.yaml>, ...] overrida.a=1 override.b=2", file=sys.stderr)
         sys.exit(1)
 
     if len(args) == 0 or "-h" in args or "--help" in args:
         show_help()
 
     # Builds the configs from the command-line arguments.
     config = DictConfig({})
```

### Comparing `ml-starter-0.1.36/ml/utils/colors.py` & `ml-starter-0.1.37/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/containers.py` & `ml-starter-0.1.37/ml/utils/containers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/data.py` & `ml-starter-0.1.37/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/datetime.py` & `ml-starter-0.1.37/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/device/auto.py` & `ml-starter-0.1.37/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/device/base.py` & `ml-starter-0.1.37/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/device/cpu.py` & `ml-starter-0.1.37/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/device/gpu.py` & `ml-starter-0.1.37/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/device/metal.py` & `ml-starter-0.1.37/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/distributed.py` & `ml-starter-0.1.37/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/exceptions.py` & `ml-starter-0.1.37/ml/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/image.py` & `ml-starter-0.1.37/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/io.py` & `ml-starter-0.1.37/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/large_models.py` & `ml-starter-0.1.37/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/logging.py` & `ml-starter-0.1.37/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/meter.py` & `ml-starter-0.1.37/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/mixed_precision.py` & `ml-starter-0.1.37/ml/utils/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/networking.py` & `ml-starter-0.1.37/ml/utils/networking.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/numpy.py` & `ml-starter-0.1.37/ml/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/parallel.py` & `ml-starter-0.1.37/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/spectrogram.py` & `ml-starter-0.1.37/ml/utils/spectrogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 logger = logging.getLogger(__name__)
 
 Array = Tensor | np.ndarray
 
 try:
     import pyworld
-except ImportError:
+except ModuleNotFoundError:
     pyworld = None
 
 
 class _Normalizer(nn.Module):
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `ml-starter-0.1.36/ml/utils/staging.py` & `ml-starter-0.1.37/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/testing.py` & `ml-starter-0.1.37/ml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/timer.py` & `ml-starter-0.1.37/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/tokens.py` & `ml-starter-0.1.37/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/torch_distributed.py` & `ml-starter-0.1.37/ml/utils/torch_distributed.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,21 +165,23 @@
     error_queue.put(None)
 
 
 def launch_subprocesses(
     func: Callable[[], None],
     cfg: MultiprocessConfig,
     setup: Callable[[], None] | None = None,
+    rank_offset: int = 0,
 ) -> None:
     """Launches a function in multiple subprocesses.
 
     Args:
         func: The function to launch.
         cfg: The configuration for the function.
         setup: A function to run before launching the subprocesses.
+        rank_offset: The offset to add to the rank of each subprocess.
 
     Raises:
         RuntimeError: If the function fails in any subprocess.
     """
     MultiprocessConfig.resolve(cfg)
 
     if cfg.world_size <= 1:
@@ -189,14 +191,15 @@
         return
 
     logger.info("Launching %d training workers", cfg.world_size)
     ctx = mp.get_context(cfg.launch_method)
     error_queues: list["mp.SimpleQueue[str | None]"] = []
     procs = []
     for rank in range(cfg.world_size):
+        rank = rank + rank_offset
         error_queue = ctx.SimpleQueue()
         cfg.rank = rank
         cfg.local_rank = rank % cfg.local_world_size
         proc = ctx.Process(
             target=_func_wrapped,
             args=(func, setup, cfg, error_queue),
             daemon=False,
```

### Comparing `ml-starter-0.1.36/ml/utils/triton/kmeans.py` & `ml-starter-0.1.37/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/triton/lion.py` & `ml-starter-0.1.37/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/ml/utils/video.py` & `ml-starter-0.1.37/ml/utils/video.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,39 +37,39 @@
 
 @functools.lru_cache()
 def ffmpeg_python_available() -> bool:
     try:
         import ffmpeg
 
         assert ffmpeg is not None  # Silence unused import warning
-    except ImportError:
+    except ModuleNotFoundError:
         return False
     else:
         return True
 
 
 @functools.lru_cache()
 def mpl_available() -> bool:
     try:
         import matplotlib
 
         assert matplotlib is not None  # Silence unused import warning
-    except ImportError:
+    except ModuleNotFoundError:
         return False
     else:
         return True
 
 
 @functools.lru_cache()
 def cv2_available() -> bool:
     try:
         import cv2
 
         assert cv2 is not None  # Silence unused import warning
-    except ImportError:
+    except ModuleNotFoundError:
         return False
     else:
         return True
 
 
 @dataclass
 class VideoProps:
@@ -90,32 +90,32 @@
             fps=Fraction(stream.average_rate),
         )
 
     @classmethod
     def from_file_opencv(cls, fpath: str | Path) -> "VideoProps":
         try:
             import cv2
-        except ImportError as e:
-            raise ImportError("Please install OpenCV to use this function: `pip install opencv-python`") from e
+        except ModuleNotFoundError as e:
+            raise ModuleNotFoundError("Install OpenCV to use this function: `pip install opencv-python`") from e
 
         cap = cv2.VideoCapture(str(fpath))
 
         return cls(
             frame_width=int(cap.get(cv2.CAP_PROP_FRAME_WIDTH)),
             frame_height=int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT)),
             frame_count=int(cap.get(cv2.CAP_PROP_FRAME_COUNT)),
             fps=Fraction(cap.get(cv2.CAP_PROP_FPS)),
         )
 
     @classmethod
     def from_file_ffmpeg(cls, fpath: str | Path) -> "VideoProps":
         try:
             import ffmpeg
-        except ImportError as e:
-            raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
+        except ModuleNotFoundError as e:
+            raise ModuleNotFoundError("Install matplotlib to use this function: `pip install ffmpeg-python`") from e
 
         probe = ffmpeg.probe(str(fpath))
 
         for stream in probe["streams"]:
             if stream["codec_type"] == "video":
                 width, height, count = stream["width"], stream["height"], int(stream["nb_frames"])
                 fps_num, fps_denom = stream["r_frame_rate"].split("/")
@@ -174,16 +174,16 @@
         channels: Number of output channels for each video frame
 
     Yields:
         Frames from the video as numpy arrays with shape (H, W, C)
     """
     try:
         import ffmpeg
-    except ImportError as e:
-        raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
+    except ModuleNotFoundError as e:
+        raise ModuleNotFoundError("Install matplotlib to use this function: `pip install ffmpeg-python`") from e
 
     props = VideoProps.from_file_ffmpeg(in_file)
 
     stream = ffmpeg.input(str(in_file))
     stream = ffmpeg.output(stream, "pipe:", format="rawvideo", pix_fmt=output_fmt, r=float(props.fps))
     stream = ffmpeg.run_async(stream, pipe_stdout=True)
 
@@ -215,16 +215,16 @@
 
     Yields:
         Frames from the video as numpy arrays with shape (H, W, C), along with
         the frame timestamps
     """
     try:
         import ffmpeg
-    except ImportError as e:
-        raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
+    except ModuleNotFoundError as e:
+        raise ModuleNotFoundError("Install matplotlib to use this function: `pip install ffmpeg-python`") from e
 
     props = VideoProps.from_file_ffmpeg(in_file)
 
     def aspect_ratio(x: int, a: int, b: int) -> int:
         return (x * a + b - 1) // b
 
     vf: list[str] = []
@@ -287,16 +287,16 @@
         in_file: The input video to read
 
     Yields:
         Frames from the video as numpy arrays with shape (H, W, C)
     """
     try:
         import cv2
-    except ImportError as e:
-        raise ImportError("Please install OpenCV to use this function: `pip install opencv-python`") from e
+    except ModuleNotFoundError as e:
+        raise ModuleNotFoundError("Install OpenCV to use this function: `pip install opencv-python`") from e
 
     cap = cv2.VideoCapture(str(in_file))
 
     while True:
         ret, buffer = cap.read()
         if not ret:
             cap.release()
@@ -321,16 +321,16 @@
             resize to a human-friendly resolution.
         fps: Frames per second for the video.
         codec: FourCC code specifying OpenCV video codec type. Examples are
             MPEG, MP4V, DIVX, AVC1, H236.
     """
     try:
         import cv2
-    except ImportError as e:
-        raise ImportError("Please install OpenCV to use this function: `pip install opencv-python`") from e
+    except ModuleNotFoundError as e:
+        raise ModuleNotFoundError("Install OpenCV to use this function: `pip install opencv-python`") from e
 
     Path(out_file).parent.mkdir(exist_ok=True, parents=True)
 
     first_img = standardize_image(next(itr), keep_resolution=keep_resolution)
     height, width, _ = first_img.shape
 
     fourcc = cv2.VideoWriter_fourcc(*codec)
@@ -416,16 +416,16 @@
         out_fps: Frames per second for the saved video.
         vcodec: The video codec to use for the output video
         input_fmt: The input image format
         output_fmt: The output image format
     """
     try:
         import ffmpeg
-    except ImportError as e:
-        raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
+    except ModuleNotFoundError as e:
+        raise ModuleNotFoundError("Install matplotlib to use this function: `pip install ffmpeg-python`") from e
 
     Path(out_file).parent.mkdir(exist_ok=True, parents=True)
 
     first_img = standardize_image(next(itr), keep_resolution=keep_resolution)
     height, width, _ = first_img.shape
 
     stream = ffmpeg.input("pipe:", format="rawvideo", pix_fmt=input_fmt, s=f"{width}x{height}", r=float(fps))
@@ -470,16 +470,16 @@
         writer: The Matplotlib video writer to use (if you use the
             default one, make sure you have `ffmpeg` installed on your
             system).
     """
     try:
         import matplotlib.animation as ani
         import matplotlib.pyplot as plt
-    except ImportError as e:
-        raise ImportError("Please install matplotlib to use this function: `pip install matplotlib`") from e
+    except ModuleNotFoundError as e:
+        raise ModuleNotFoundError("Install matplotlib to use this function: `pip install matplotlib`") from e
 
     Path(out_file).parent.mkdir(exist_ok=True, parents=True)
 
     first_img = standardize_image(next(itr), keep_resolution=keep_resolution)
     height, width, _ = first_img.shape
     fig, ax = plt.subplots(figsize=(width / dpi, height / dpi))
```

### Comparing `ml-starter-0.1.36/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.37/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.36
+Version: 0.1.37
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.36/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.37/ml_starter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-requirements-dev.txt
-requirements-docs.txt
-requirements.txt
 setup.cfg
 setup.py
 ml/__init__.py
 ml/api.py
 ml/py.typed
+ml/requirements.txt
 ml/core/__init__.py
 ml/core/common_types.py
 ml/core/config.py
 ml/core/env.py
 ml/core/registry.py
 ml/core/state.py
 ml/launchers/__init__.py
 ml/launchers/base.py
 ml/launchers/mp.py
+ml/launchers/sagemaker.py
 ml/launchers/slurm.py
 ml/launchers/torchrun.py
 ml/loggers/__init__.py
 ml/loggers/base.py
 ml/loggers/meter.py
 ml/loggers/multi.py
 ml/loggers/stdout.py
@@ -37,23 +36,25 @@
 ml/lr_schedulers/linear_no_decay.py
 ml/lr_schedulers/scripts/__init__.py
 ml/lr_schedulers/scripts/plot.py
 ml/models/__init__.py
 ml/models/activations.py
 ml/models/base.py
 ml/models/codebook.py
-ml/models/diffusion.py
 ml/models/embeddings.py
 ml/models/gan.py
 ml/models/init.py
 ml/models/kmeans.py
 ml/models/lora.py
 ml/models/modules.py
 ml/models/norms.py
 ml/models/parallel.py
+ml/models/architectures/__init__.py
+ml/models/architectures/bifpn.py
+ml/models/architectures/unet.py
 ml/optimizers/__init__.py
 ml/optimizers/adam.py
 ml/optimizers/adan.py
 ml/optimizers/base.py
 ml/optimizers/common.py
 ml/optimizers/gan.py
 ml/optimizers/lion.py
@@ -74,14 +75,17 @@
 ml/tasks/datasets/collate.py
 ml/tasks/datasets/error_handling.py
 ml/tasks/datasets/multi_iter.py
 ml/tasks/datasets/samplers.py
 ml/tasks/datasets/streaming.py
 ml/tasks/datasets/transforms.py
 ml/tasks/datasets/video_file.py
+ml/tasks/diffusion/__init__.py
+ml/tasks/diffusion/beta_schedule.py
+ml/tasks/diffusion/gaussian.py
 ml/tasks/environments/__init__.py
 ml/tasks/environments/base.py
 ml/tasks/environments/utils.py
 ml/tasks/environments/worker.py
 ml/tasks/gan/__init__.py
 ml/tasks/gan/base.py
 ml/tasks/losses/__init__.py
```

### Comparing `ml-starter-0.1.36/pyproject.toml` & `ml-starter-0.1.37/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.36/setup.py` & `ml-starter-0.1.37/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 #!/usr/bin/env python
 """Setup script for the ml-starter project."""
 
 import re
 
 from setuptools import setup
 
+REQUIREMENTS_DEV = [
+    "black",
+    "darglint",
+    "mypy",
+    "pytest",
+    "pytest-timeout",
+    "ruff",
+]
+
+REQUIREMENTS_DOCS = [
+    "myst-parser",
+    "sphinx==6.2.1",
+    "sphinxcontrib-jquery",
+    "sphinx-rtd-theme",
+    "sphinx-autodoc-typehints",
+]
+
+
 with open("README.md", "r", encoding="utf-8") as f:
     long_description: str = f.read()
 
 
-with open("requirements.txt", "r", encoding="utf-8") as f:
+with open("ml/requirements.txt", "r", encoding="utf-8") as f:
     requirements: list[str] = f.read().splitlines()
 
 
-with open("requirements-dev.txt", "r", encoding="utf-8") as f:
-    requirements_dev: list[str] = f.read().splitlines()
-
-
-with open("requirements-docs.txt", "r", encoding="utf-8") as f:
-    requirements_docs: list[str] = f.read().splitlines()
-
-
 with open("ml/__init__.py", "r", encoding="utf-8") as fh:
     version_re = re.search(r"^__version__ = \"([^\"]*)\"", fh.read(), re.MULTILINE)
 assert version_re is not None, "Could not find version in ml/__init__.py"
 version: str = version_re.group(1)
 
 
 setup(
@@ -40,11 +50,11 @@
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
     ],
     python_requires=">=3.10",
     install_requires=requirements,
-    tests_require=requirements_dev,
-    extras_require={"dev": requirements_dev, "docs": requirements_docs},
-    package_data={"ml": ["py.typed"]},
+    tests_require=REQUIREMENTS_DEV,
+    extras_require={"dev": REQUIREMENTS_DEV, "docs": REQUIREMENTS_DOCS},
+    package_data={"ml": ["py.typed", "requirements.txt"]},
 )
```

