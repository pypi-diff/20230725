# Comparing `tmp/parsl-2023.7.24.tar.gz` & `tmp/parsl-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsl-2023.7.24.tar", last modified: Mon Jul 24 22:42:59 2023, max compression
+gzip compressed data, was "parsl-2023.7.3.tar", last modified: Mon Jul  3 22:43:00 2023, max compression
```

## Comparing `parsl-2023.7.24.tar` & `parsl-2023.7.3.tar`

### file list

```diff
@@ -1,481 +1,473 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.187392 parsl-2023.7.24/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 22:42:51.000000 parsl-2023.7.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-24 22:42:51.000000 parsl-2023.7.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-24 22:42:59.187392 parsl-2023.7.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-24 22:42:51.000000 parsl-2023.7.24/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.147390 parsl-2023.7.24/parsl/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.147390 parsl-2023.7.24/parsl/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/app/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/app/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/app/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/app/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.147390 parsl-2023.7.24/parsl/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/benchmark/perf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.147390 parsl-2023.7.24/parsl/channels/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/channels/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/channels/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.147390 parsl-2023.7.24/parsl/channels/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/channels/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/channels/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.147390 parsl-2023.7.24/parsl/channels/oauth_ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/channels/oauth_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/channels/oauth_ssh/oauth_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.147390 parsl-2023.7.24/parsl/channels/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/channels/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/channels/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.147390 parsl-2023.7.24/parsl/channels/ssh_il/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/channels/ssh_il/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/channels/ssh_il/ssh_il.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.147390 parsl-2023.7.24/parsl/concurrent/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/concurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.151390 parsl-2023.7.24/parsl/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/ASPIRE1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/Azure.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/ad_hoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/cooley.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/illinoiscluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/osg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/polaris.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/stampede2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/toss3_llnl.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/configs/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.151390 parsl-2023.7.24/parsl/data_provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/data_provider/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/data_provider/file_noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/data_provider/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/data_provider/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/data_provider/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/data_provider/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/data_provider/rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/data_provider/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.151390 parsl-2023.7.24/parsl/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62820 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/dataflow/dflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/dataflow/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/dataflow/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/dataflow/memoization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/dataflow/rundirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/dataflow/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/dataflow/taskrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.155390 parsl-2023.7.24/parsl/executors/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.155390 parsl-2023.7.24/parsl/executors/flux/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/flux/execute_parsl_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/flux/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/flux/flux_instance_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.155390 parsl-2023.7.24/parsl/executors/high_throughput/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/high_throughput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/high_throughput/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    33394 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/high_throughput/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28361 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/high_throughput/interchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/high_throughput/manager_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/high_throughput/monitoring_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/high_throughput/probe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32997 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/high_throughput/process_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/status_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.155390 parsl-2023.7.24/parsl/executors/taskvine/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/taskvine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/taskvine/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/taskvine/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    50232 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/taskvine/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/taskvine/factory_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/taskvine/manager_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/taskvine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.155390 parsl-2023.7.24/parsl/executors/workqueue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/workqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/workqueue/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/workqueue/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    48106 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/workqueue/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/workqueue/parsl_coprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/executors/workqueue/parsl_coprocess_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.155390 parsl-2023.7.24/parsl/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/jobs/job_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/jobs/job_status_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/jobs/states.py
--rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/jobs/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.155390 parsl-2023.7.24/parsl/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/launchers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/launchers/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.159391 parsl-2023.7.24/parsl/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/db_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    23367 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.159391 parsl-2023.7.24/parsl/monitoring/queries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/queries/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/radios.py
--rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.159391 parsl-2023.7.24/parsl/monitoring/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.159391 parsl-2023.7.24/parsl/monitoring/visualization/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.159391 parsl-2023.7.24/parsl/monitoring/visualization/plots/default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/plots/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/plots/default/task_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/plots/default/workflow_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.159391 parsl-2023.7.24/parsl/monitoring/visualization/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/static/parsl-logo-white.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/static/parsl-monitor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.159391 parsl-2023.7.24/parsl/monitoring/visualization/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/templates/app.html
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/templates/dag.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/templates/resource_usage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/templates/task.html
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/templates/workflow.html
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/templates/workflows_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/monitoring/visualization/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/process_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.159391 parsl-2023.7.24/parsl/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.159391 parsl-2023.7.24/parsl/providers/ad_hoc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/ad_hoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/ad_hoc/ad_hoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.159391 parsl-2023.7.24/parsl/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29009 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/aws/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/aws/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.163391 parsl-2023.7.24/parsl/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18396 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/azure/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/azure/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/cluster_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.163391 parsl-2023.7.24/parsl/providers/cobalt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/cobalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/cobalt/cobalt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/cobalt/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.163391 parsl-2023.7.24/parsl/providers/condor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/condor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/condor/condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/condor/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.163391 parsl-2023.7.24/parsl/providers/googlecloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/googlecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/googlecloud/googlecloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.163391 parsl-2023.7.24/parsl/providers/grid_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/grid_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/grid_engine/grid_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/grid_engine/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.163391 parsl-2023.7.24/parsl/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/kubernetes/kube.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/kubernetes/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.163391 parsl-2023.7.24/parsl/providers/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.163391 parsl-2023.7.24/parsl/providers/lsf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/lsf/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/lsf/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.163391 parsl-2023.7.24/parsl/providers/pbspro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/pbspro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/pbspro/pbspro.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/pbspro/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.163391 parsl-2023.7.24/parsl/providers/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/slurm/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/slurm/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.163391 parsl-2023.7.24/parsl/providers/torque/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/torque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/torque/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/providers/torque/torque.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.163391 parsl-2023.7.24/parsl/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/serialize/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/serialize/concretes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/serialize/facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.167391 parsl-2023.7.24/parsl/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/callables_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.171391 parsl-2023.7.24/parsl/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/ad_hoc_cluster_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/azure_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/cooley_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/ec2_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/ec2_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/htex_ad_hoc_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/htex_local_alternate.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/htex_local_intask_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/htex_local_rsync_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/local_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/local_threads_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/local_threads_checkpoint_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/local_threads_checkpoint_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/local_threads_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/local_threads_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/local_threads_http_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/local_threads_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/local_threads_no_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/nscc_singapore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/osg_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/petrelkube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/swan_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/taskvine_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/user_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/configs/workqueue_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.171391 parsl-2023.7.24/parsl/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/latency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.171391 parsl-2023.7.24/parsl/tests/integration/test_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/test_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.171391 parsl-2023.7.24/parsl/tests/integration/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/test_channels/test_local_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/test_channels/test_scp_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/test_channels/test_ssh_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/test_channels/test_ssh_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/test_channels/test_ssh_file_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/test_channels/test_ssh_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/test_parsl_load_default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.171391 parsl-2023.7.24/parsl/tests/integration/test_stress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/test_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/test_stress/test_python_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/integration/test_stress/test_python_threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.171391 parsl-2023.7.24/parsl/tests/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/manual_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/manual_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/manual_tests/test_ad_hoc_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/manual_tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/manual_tests/test_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/manual_tests/test_memory_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/manual_tests/test_oauth_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/manual_tests/test_regression_220.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/manual_tests/test_udp_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/manual_tests/test_worker_count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.171391 parsl-2023.7.24/parsl/tests/scaling_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/scaling_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/scaling_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/scaling_tests/local_threads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3751 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/scaling_tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/scaling_tests/vineex_condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/scaling_tests/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/scaling_tests/wqex_condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/scaling_tests/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.171391 parsl-2023.7.24/parsl/tests/site_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/site_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/site_tests/site_config_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/site_tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/site_tests/test_site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.175392 parsl-2023.7.24/parsl/tests/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/sites/test_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/sites/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/sites/test_dynamic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/sites/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/sites/test_launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/sites/test_local_adhoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.175392 parsl-2023.7.24/parsl/tests/sites/test_mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/sites/test_mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/sites/test_start_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/sites/test_worker_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_aalst_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.175392 parsl-2023.7.24/parsl/tests/test_bash_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_bash_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_bash_apps/test_apptimeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_bash_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_bash_apps/test_error_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_bash_apps/test_keyword_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_bash_apps/test_kwarg_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_bash_apps/test_memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_bash_apps/test_multiline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_bash_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_bash_apps/test_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_callables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.175392 parsl-2023.7.24/parsl/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_channels/test_large_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.175392 parsl-2023.7.24/parsl/tests/test_checkpointing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_checkpointing/test_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_checkpointing/test_regression_232.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_checkpointing/test_regression_233.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_checkpointing/test_regression_239.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_checkpointing/test_task_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.175392 parsl-2023.7.24/parsl/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_data/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_data/test_file_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_data/test_file_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_data/test_output_chain_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.179392 parsl-2023.7.24/parsl/tests/test_docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_docs/test_from_slides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_docs/test_tutorial_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_docs/test_workflow1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_docs/test_workflow2.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_docs/test_workflow3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_docs/test_workflow4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.179392 parsl-2023.7.24/parsl/tests/test_error_handling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_error_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_error_handling/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_error_handling/test_htex_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_error_handling/test_htex_missing_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_error_handling/test_htex_worker_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_error_handling/test_python_walltime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_error_handling/test_rand_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_error_handling/test_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_error_handling/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_error_handling/test_retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_error_handling/test_retry_handler_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_error_handling/test_serialization_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_error_handling/test_wrap_with_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.179392 parsl-2023.7.24/parsl/tests/test_flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_flowcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.179392 parsl-2023.7.24/parsl/tests/test_htex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_htex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_htex/test_htex_zmq_binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.179392 parsl-2023.7.24/parsl/tests/test_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_monitoring/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_monitoring/test_db_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_monitoring/test_fuzz_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_monitoring/test_memoization_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_monitoring/test_viz_colouring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.179392 parsl-2023.7.24/parsl/tests/test_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_providers/test_local_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.183392 parsl-2023.7.24/parsl/tests/test_python_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_arg_input_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_dep_standard_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_depfail_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_fibonacci_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_fibonacci_recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_garbage_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_import_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_join.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_mapred.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_memoize_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_memoize_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_memoize_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_memoize_joinapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_python_apps/test_type5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.183392 parsl-2023.7.24/parsl/tests/test_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_regression/test_1480.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_regression/test_1653.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_regression/test_221.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_regression/test_226.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_regression/test_2652.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_regression/test_69a.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_regression/test_854.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_regression/test_97_parallelism_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_regression/test_98.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.183392 parsl-2023.7.24/parsl/tests/test_scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_scaling/test_regression_1621.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_scaling/test_scale_down.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.183392 parsl-2023.7.24/parsl/tests/test_serialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_serialization/test_2555_caching_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_serialization/test_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.183392 parsl-2023.7.24/parsl/tests/test_staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_staging/staging_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_staging/test_1316.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_staging/test_docs_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_staging/test_docs_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_staging/test_elaborate_noop_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_staging/test_staging_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_staging/test_staging_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_staging/test_staging_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_staging/test_staging_https.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_staging/test_staging_https_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_thread_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.187392 parsl-2023.7.24/parsl/tests/test_threads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_threads/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/test_threads/test_lazy_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.187392 parsl-2023.7.24/parsl/usage_tracking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/usage_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/usage_tracking/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-07-24 22:42:51.000000 parsl-2023.7.24/parsl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-24 22:42:56.000000 parsl-2023.7.24/parsl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:42:59.147390 parsl-2023.7.24/parsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-24 22:42:59.000000 parsl-2023.7.24/parsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15751 2023-07-24 22:42:59.000000 parsl-2023.7.24/parsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:42:59.000000 parsl-2023.7.24/parsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-24 22:42:59.000000 parsl-2023.7.24/parsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-24 22:42:59.000000 parsl-2023.7.24/parsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 22:42:59.000000 parsl-2023.7.24/parsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 22:42:51.000000 parsl-2023.7.24/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 22:42:59.187392 parsl-2023.7.24/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2626 2023-07-24 22:42:51.000000 parsl-2023.7.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.767384 parsl-2023.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:42:55.000000 parsl-2023.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-03 22:42:55.000000 parsl-2023.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 22:43:00.767384 parsl-2023.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-03 22:42:55.000000 parsl-2023.7.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.695383 parsl-2023.7.3/parsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.695383 parsl-2023.7.3/parsl/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.695383 parsl-2023.7.3/parsl/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/benchmark/perf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/oauth_ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/oauth_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/oauth_ssh/oauth_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/ssh_il/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/ssh_il/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/ssh_il/ssh_il.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/concurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.703384 parsl-2023.7.3/parsl/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/ASPIRE1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/Azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/ad_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/cooley.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/illinoiscluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/osg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/polaris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/stampede2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/toss3_llnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.703384 parsl-2023.7.3/parsl/data_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/file_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.707383 parsl-2023.7.3/parsl/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62269 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/dflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/executor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/job_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/job_status_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/rundirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/taskrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.707383 parsl-2023.7.3/parsl/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.707383 parsl-2023.7.3/parsl/executors/flux/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/flux/execute_parsl_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/flux/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/flux/flux_instance_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.711384 parsl-2023.7.3/parsl/executors/high_throughput/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33191 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/interchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/manager_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/monitoring_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/probe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33011 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/process_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/status_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.711384 parsl-2023.7.3/parsl/executors/taskvine/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/taskvine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/taskvine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/taskvine/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48948 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/taskvine/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.711384 parsl-2023.7.3/parsl/executors/workqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48130 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/parsl_coprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/parsl_coprocess_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.715384 parsl-2023.7.3/parsl/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/launchers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/launchers/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.715384 parsl-2023.7.3/parsl/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.715384 parsl-2023.7.3/parsl/monitoring/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/queries/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/radios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.715384 parsl-2023.7.3/parsl/monitoring/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/monitoring/visualization/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/task_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/workflow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/monitoring/visualization/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/static/parsl-logo-white.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/static/parsl-monitor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/monitoring/visualization/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/dag.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/resource_usage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/task.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/workflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/workflows_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/process_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/providers/ad_hoc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/ad_hoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/ad_hoc/ad_hoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28980 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/aws/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/aws/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/azure/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/azure/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/cluster_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/cobalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/cobalt/cobalt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/cobalt/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/condor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/condor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/condor/condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/condor/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/googlecloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/googlecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/googlecloud/googlecloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/grid_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/grid_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/grid_engine/grid_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/grid_engine/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/kubernetes/kube.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/kubernetes/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/providers/lsf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/lsf/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/lsf/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/providers/pbspro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/pbspro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/pbspro/pbspro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/pbspro/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/providers/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/slurm/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/slurm/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/providers/torque/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/torque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/torque/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/torque/torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/serialize/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/serialize/concretes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/serialize/facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.731384 parsl-2023.7.3/parsl/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/callables_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.735384 parsl-2023.7.3/parsl/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/ad_hoc_cluster_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/azure_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/cooley_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/ec2_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/ec2_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_ad_hoc_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_local_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_local_intask_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_local_rsync_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_checkpoint_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_checkpoint_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_http_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_no_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/nscc_singapore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/osg_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/petrelkube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/swan_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/taskvine_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/user_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/workqueue_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.735384 parsl-2023.7.3/parsl/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/latency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.735384 parsl-2023.7.3/parsl/tests/integration/test_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.739384 parsl-2023.7.3/parsl/tests/integration/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_local_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_scp_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_file_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_parsl_load_default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.739384 parsl-2023.7.3/parsl/tests/integration/test_stress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_stress/test_python_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_stress/test_python_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_ad_hoc_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_memory_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_oauth_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_regression_220.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_udp_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_worker_count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/scaling_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/local_threads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3751 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/vineex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/wqex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/site_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/site_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/site_tests/site_config_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/site_tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/site_tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_dynamic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_local_adhoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/sites/test_mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_start_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_worker_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_aalst_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.747384 parsl-2023.7.3/parsl/tests/test_bash_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_apptimeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_keyword_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_kwarg_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_callables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.747384 parsl-2023.7.3/parsl/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_channels/test_large_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.747384 parsl-2023.7.3/parsl/tests/test_checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_232.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_233.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_239.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_task_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.751384 parsl-2023.7.3/parsl/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/test_file_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/test_file_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/test_output_chain_filenames.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.751384 parsl-2023.7.3/parsl/tests/test_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_from_slides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_tutorial_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_workflow1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_workflow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_workflow3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_workflow4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.755384 parsl-2023.7.3/parsl/tests/test_error_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_missing_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_worker_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_python_walltime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_rand_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_retry_handler_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_serialization_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_wrap_with_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.755384 parsl-2023.7.3/parsl/tests/test_flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_flowcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.755384 parsl-2023.7.3/parsl/tests/test_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_db_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_fuzz_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_memoization_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_viz_colouring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.755384 parsl-2023.7.3/parsl/tests/test_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_providers/test_local_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.759384 parsl-2023.7.3/parsl/tests/test_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_arg_input_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_dep_standard_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_depfail_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_fibonacci_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_fibonacci_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_garbage_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_import_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_mapred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_joinapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_type5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_1480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_1653.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_221.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_226.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_2652.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_69a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_69b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_854.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_97_parallelism_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_98.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_scaling/test_regression_1621.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_scaling/test_scale_down.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_serialization/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/staging_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_1316.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_docs_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_docs_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_elaborate_noop_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_https_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_thread_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_threads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_threads/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_threads/test_lazy_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.767384 parsl-2023.7.3/parsl/usage_tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/usage_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/usage_tracking/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-03 22:42:59.000000 parsl-2023.7.3/parsl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.695383 parsl-2023.7.3/parsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15527 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-03 22:42:55.000000 parsl-2023.7.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:43:00.767384 parsl-2023.7.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2626 2023-07-03 22:42:55.000000 parsl-2023.7.3/setup.py
```

### Comparing `parsl-2023.7.24/LICENSE` & `parsl-2023.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/PKG-INFO` & `parsl-2023.7.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2023.7.24
+Version: 2023.7.3
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2023.07.24.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2023.07.03.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2023.7.24/README.rst` & `parsl-2023.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/__init__.py` & `parsl-2023.7.3/parsl/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/addresses.py` & `parsl-2023.7.3/parsl/addresses.py`

 * *Files 15% similar despite different names*

```diff
@@ -107,47 +107,18 @@
 
     s_addresses = set()
     for interface in net_interfaces:
         try:
             s_addresses.add(address_by_interface(interface))
         except Exception:
             logger.exception("Ignoring failure to fetch address from interface {}".format(interface))
+            pass
 
     resolution_functions: List[Callable[[], str]]
     resolution_functions = [address_by_hostname, address_by_route, address_by_query]
     for f in resolution_functions:
         try:
             s_addresses.add(f())
         except Exception:
             logger.exception("Ignoring an address finder exception")
 
     return s_addresses
-
-
-def get_any_address() -> str:
-    """ Uses a combination of methods to find any address of the local machine.
-
-    Returns:
-        one address in string
-    """
-    net_interfaces = psutil.net_if_addrs()
-
-    addr = ''
-    for interface in net_interfaces:
-        try:
-            addr = address_by_interface(interface)
-            return addr
-        except Exception:
-            logger.exception("Ignoring failure to fetch address from interface {}".format(interface))
-
-    resolution_functions: List[Callable[[], str]]
-    resolution_functions = [address_by_hostname, address_by_route, address_by_query]
-    for f in resolution_functions:
-        try:
-            addr = f()
-            return addr
-        except Exception:
-            logger.exception("Ignoring an address finder exception")
-
-    if addr == '':
-        raise Exception('Cannot find address of the local machine.')
-    return addr
```

### Comparing `parsl-2023.7.24/parsl/app/app.py` & `parsl-2023.7.3/parsl/app/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/app/bash.py` & `parsl-2023.7.3/parsl/app/bash.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/app/errors.py` & `parsl-2023.7.3/parsl/app/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/app/futures.py` & `parsl-2023.7.3/parsl/app/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/app/python.py` & `parsl-2023.7.3/parsl/app/python.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/benchmark/perf.py` & `parsl-2023.7.3/parsl/benchmark/perf.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/channels/base.py` & `parsl-2023.7.3/parsl/channels/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/channels/errors.py` & `parsl-2023.7.3/parsl/channels/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/channels/local/local.py` & `parsl-2023.7.3/parsl/channels/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/channels/oauth_ssh/oauth_ssh.py` & `parsl-2023.7.3/parsl/channels/oauth_ssh/oauth_ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/channels/ssh/ssh.py` & `parsl-2023.7.3/parsl/channels/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/channels/ssh_il/ssh_il.py` & `parsl-2023.7.3/parsl/channels/ssh_il/ssh_il.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/concurrent/__init__.py` & `parsl-2023.7.3/parsl/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/config.py` & `parsl-2023.7.3/parsl/config.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/ASPIRE1.py` & `parsl-2023.7.3/parsl/configs/ASPIRE1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/Azure.py` & `parsl-2023.7.3/parsl/configs/Azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/ad_hoc.py` & `parsl-2023.7.3/parsl/configs/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/bluewaters.py` & `parsl-2023.7.3/parsl/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/bridges.py` & `parsl-2023.7.3/parsl/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/cc_in2p3.py` & `parsl-2023.7.3/parsl/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/comet.py` & `parsl-2023.7.3/parsl/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/cooley.py` & `parsl-2023.7.3/parsl/configs/cooley.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/ec2.py` & `parsl-2023.7.3/parsl/configs/ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/frontera.py` & `parsl-2023.7.3/parsl/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/illinoiscluster.py` & `parsl-2023.7.3/parsl/configs/illinoiscluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/kubernetes.py` & `parsl-2023.7.3/parsl/configs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/midway.py` & `parsl-2023.7.3/parsl/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/osg.py` & `parsl-2023.7.3/parsl/configs/osg.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/polaris.py` & `parsl-2023.7.3/parsl/configs/polaris.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/stampede2.py` & `parsl-2023.7.3/parsl/configs/stampede2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/summit.py` & `parsl-2023.7.3/parsl/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/theta.py` & `parsl-2023.7.3/parsl/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/toss3_llnl.py` & `parsl-2023.7.3/parsl/configs/toss3_llnl.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/configs/wqex_local.py` & `parsl-2023.7.3/parsl/configs/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/data_provider/data_manager.py` & `parsl-2023.7.3/parsl/data_provider/data_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/data_provider/files.py` & `parsl-2023.7.3/parsl/data_provider/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Define the File Type.
 
 The primary purpose of the File object is to track the protocol to be used
 to transfer the file as well as to give the appropriate filepath depending
 on where (client-side, remote-side, intermediary-side) the File.filepath is
 being called from.
 """
-import os
 
+import os
 import typeguard
 import logging
-from typing import Optional, Union
+from typing import Optional
 from urllib.parse import urlparse
 
 logger = logging.getLogger(__name__)
 
 
 class File:
     """The Parsl File Class.
@@ -24,26 +24,25 @@
     the path at the far end of a staging action. It is up to the user of
     the File object to track which local scope that local path actually
     refers to.
 
     """
 
     @typeguard.typechecked
-    def __init__(self, url: Union[os.PathLike, str]):
+    def __init__(self, url: str):
         """Construct a File object from a url string.
 
         Args:
-           - url (string or PathLike) : url of the file e.g.
+           - url (string) : url string of the file e.g.
               - 'input.txt'
-              - pathlib.Path('input.txt')
               - 'file:///scratch/proj101/input.txt'
               - 'globus://go#ep1/~/data/input.txt'
               - 'globus://ddb59aef-6d04-11e5-ba46-22000b92c6ec/home/johndoe/data/input.txt'
         """
-        self.url = str(url)
+        self.url = url
         parsed_url = urlparse(self.url)
         self.scheme = parsed_url.scheme if parsed_url.scheme else 'file'
         self.netloc = parsed_url.netloc
         self.path = parsed_url.path
         self.filename = os.path.basename(self.path)
         self.local_path: Optional[str] = None
```

### Comparing `parsl-2023.7.24/parsl/data_provider/ftp.py` & `parsl-2023.7.3/parsl/data_provider/ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/data_provider/globus.py` & `parsl-2023.7.3/parsl/data_provider/globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/data_provider/http.py` & `parsl-2023.7.3/parsl/data_provider/http.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/data_provider/rsync.py` & `parsl-2023.7.3/parsl/data_provider/rsync.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/data_provider/staging.py` & `parsl-2023.7.3/parsl/data_provider/staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/dataflow/dflow.py` & `parsl-2023.7.3/parsl/dataflow/dflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,28 +24,27 @@
 from parsl.app.futures import DataFuture
 from parsl.channels import Channel
 from parsl.config import Config
 from parsl.data_provider.data_manager import DataManager
 from parsl.data_provider.files import File
 from parsl.dataflow.errors import BadCheckpoint, DependencyError, JoinError
 from parsl.dataflow.futures import AppFuture
+from parsl.dataflow.job_status_poller import JobStatusPoller
 from parsl.dataflow.memoization import Memoizer
 from parsl.dataflow.rundirs import make_rundir
 from parsl.dataflow.states import States, FINAL_STATES, FINAL_FAILURE_STATES
 from parsl.dataflow.taskrecord import TaskRecord
 from parsl.errors import ConfigurationError
-from parsl.jobs.job_status_poller import JobStatusPoller
-from parsl.jobs.states import JobStatus, JobState
 from parsl.usage_tracking.usage import UsageTracker
 from parsl.executors.base import ParslExecutor
 from parsl.executors.status_handling import BlockProviderExecutor
 from parsl.executors.threads import ThreadPoolExecutor
 from parsl.monitoring import MonitoringHub
 from parsl.process_loggers import wrap_with_logs
-from parsl.providers.base import ExecutionProvider
+from parsl.providers.base import ExecutionProvider, JobStatus, JobState
 from parsl.utils import get_version, get_std_fname_mode, get_all_checkpoints, Timer
 
 from parsl.monitoring.message_type import MessageType
 
 logger = logging.getLogger(__name__)
 
 
@@ -377,20 +376,14 @@
                     # something we can't join on.
                     if isinstance(joinable, Future):
                         self.update_task_state(task_record, States.joining)
                         task_record['joins'] = joinable
                         task_record['join_lock'] = threading.Lock()
                         self._send_task_log_info(task_record)
                         joinable.add_done_callback(partial(self.handle_join_update, task_record))
-                    elif joinable == []:  # got a list, but it had no entries, and specifically, no Futures.
-                        self.update_task_state(task_record, States.joining)
-                        task_record['joins'] = joinable
-                        task_record['join_lock'] = threading.Lock()
-                        self._send_task_log_info(task_record)
-                        self.handle_join_update(task_record, None)
                     elif isinstance(joinable, list) and [j for j in joinable if not isinstance(j, Future)] == []:
                         self.update_task_state(task_record, States.joining)
                         task_record['joins'] = joinable
                         task_record['join_lock'] = threading.Lock()
                         self._send_task_log_info(task_record)
                         for inner_future in joinable:
                             inner_future.add_done_callback(partial(self.handle_join_update, task_record))
@@ -406,15 +399,15 @@
         self._log_std_streams(task_record)
 
         # it might be that in the course of the update, we've gone back to being
         # pending - in which case, we should consider ourself for relaunch
         if task_record['status'] == States.pending:
             self.launch_if_ready(task_record)
 
-    def handle_join_update(self, task_record: TaskRecord, inner_app_future: Optional[AppFuture]) -> None:
+    def handle_join_update(self, task_record: TaskRecord, inner_app_future: AppFuture) -> None:
         with task_record['join_lock']:
             # inner_app_future has completed, which is one (potentially of many)
             # futures the outer task is joining on.
 
             # If the outer task is joining on a single future, then
             # use the result of the inner_app_future as the final result of
             # the outer app future.
@@ -1196,24 +1189,23 @@
 
         logger.info("Scaling in and shutting down executors")
 
         for executor in self.executors.values():
             if not executor.bad_state_is_set:
                 if isinstance(executor, BlockProviderExecutor):
                     logger.info(f"Scaling in executor {executor.label}")
-                    if executor.provider:
-                        job_ids = executor.provider.resources.keys()
-                        block_ids = executor.scale_in(len(job_ids))
-                        if self.monitoring and block_ids:
-                            new_status = {}
-                            for bid in block_ids:
-                                new_status[bid] = JobStatus(JobState.CANCELLED)
-                            msg = executor.create_monitoring_info(new_status)
-                            logger.debug("Sending message {} to hub from DFK".format(msg))
-                            self.monitoring.send(MessageType.BLOCK_INFO, msg)
+                    job_ids = executor.provider.resources.keys()
+                    block_ids = executor.scale_in(len(job_ids))
+                    if self.monitoring and block_ids:
+                        new_status = {}
+                        for bid in block_ids:
+                            new_status[bid] = JobStatus(JobState.CANCELLED)
+                        msg = executor.create_monitoring_info(new_status)
+                        logger.debug("Sending message {} to hub from DFK".format(msg))
+                        self.monitoring.send(MessageType.BLOCK_INFO, msg)
                 logger.info(f"Shutting down executor {executor.label}")
                 executor.shutdown()
                 logger.info(f"Shut down executor {executor.label}")
             else:  # and bad_state_is_set
                 logger.warning(f"Not shutting down executor {executor.label} because it is in bad state")
 
         logger.info("Terminated executors")
```

### Comparing `parsl-2023.7.24/parsl/dataflow/errors.py` & `parsl-2023.7.3/parsl/dataflow/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/dataflow/futures.py` & `parsl-2023.7.3/parsl/dataflow/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/dataflow/memoization.py` & `parsl-2023.7.3/parsl/dataflow/memoization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 import hashlib
 from functools import lru_cache, singledispatch
 import logging
-import pickle
 from parsl.dataflow.taskrecord import TaskRecord
 
 from typing import Dict, Any, List, Optional, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from parsl import DataFlowKernel  # import loop at runtime - needed for typechecking - TODO turn into "if typing:"
 
 from concurrent.futures import Future
 
+from parsl.serialize import serialize
 import types
 
 logger = logging.getLogger(__name__)
 
 
 @singledispatch
 def id_for_memo(obj: object, output_ref: bool = False) -> bytes:
@@ -50,42 +50,42 @@
     raise ValueError("unknown type for memoization: {}".format(type(obj)))
 
 
 @id_for_memo.register(str)
 @id_for_memo.register(int)
 @id_for_memo.register(float)
 @id_for_memo.register(type(None))
-def id_for_memo_pickle(obj: object, output_ref: bool = False) -> bytes:
-    return pickle.dumps(obj)
+def id_for_memo_serialize(obj: object, output_ref: bool = False) -> bytes:
+    return serialize(obj)
 
 
 @id_for_memo.register(list)
 def id_for_memo_list(denormalized_list: list, output_ref: bool = False) -> bytes:
     if type(denormalized_list) != list:
         raise ValueError("id_for_memo_list cannot work on subclasses of list")
 
     normalized_list = []
 
     for e in denormalized_list:
         normalized_list.append(id_for_memo(e, output_ref=output_ref))
 
-    return pickle.dumps(normalized_list)
+    return serialize(normalized_list)
 
 
 @id_for_memo.register(tuple)
 def id_for_memo_tuple(denormalized_tuple: tuple, output_ref: bool = False) -> bytes:
     if type(denormalized_tuple) != tuple:
         raise ValueError("id_for_memo_tuple cannot work on subclasses of tuple")
 
     normalized_list = []
 
     for e in denormalized_tuple:
         normalized_list.append(id_for_memo(e, output_ref=output_ref))
 
-    return pickle.dumps(normalized_list)
+    return serialize(normalized_list)
 
 
 @id_for_memo.register(dict)
 def id_for_memo_dict(denormalized_dict: dict, output_ref: bool = False) -> bytes:
     """This normalises the keys and values of the supplied dictionary.
 
     When output_ref=True, the values are normalised as output refs, but
@@ -96,27 +96,27 @@
 
     keys = sorted(denormalized_dict)
 
     normalized_list = []
     for k in keys:
         normalized_list.append(id_for_memo(k))
         normalized_list.append(id_for_memo(denormalized_dict[k], output_ref=output_ref))
-    return pickle.dumps(normalized_list)
+    return serialize(normalized_list)
 
 
 # the LRU cache decorator must be applied closer to the id_for_memo_function call
 # that the .register() call, so that the cache-decorated version is registered.
 @id_for_memo.register(types.FunctionType)
 @lru_cache()
 def id_for_memo_function(f: types.FunctionType, output_ref: bool = False) -> bytes:
     """This will checkpoint a function based only on its name and module name.
     This means that changing source code (other than the function name) will
     not cause a checkpoint invalidation.
     """
-    return pickle.dumps(["types.FunctionType", f.__name__, f.__module__])
+    return serialize(["types.FunctionType", f.__name__, f.__module__])
 
 
 class Memoizer:
     """Memoizer is responsible for ensuring that identical work is not repeated.
 
     When a task is repeated, i.e., the same function is called with the same exact arguments, the
     result from a previous execution is reused. `wiki <https://en.wikipedia.org/wiki/Memoization>`_
```

### Comparing `parsl-2023.7.24/parsl/dataflow/rundirs.py` & `parsl-2023.7.3/parsl/dataflow/rundirs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/dataflow/states.py` & `parsl-2023.7.3/parsl/dataflow/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/dataflow/taskrecord.py` & `parsl-2023.7.3/parsl/dataflow/taskrecord.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,17 +76,14 @@
     ignore_for_cache: Sequence[str]
     from_memo: Optional[bool]
 
     id: int
     try_id: int
 
     resource_specification: Dict[str, Any]
-    """Dictionary containing relevant info for a task execution.
-    Includes resources to allocate and execution mode as a given
-    executor permits."""
 
     join: bool
     """Is this a join_app?"""
 
     joins: Union[None, Future, List[Future]]
     """If this is a join app and the python body has executed, then this
     contains the Future or list of Futures that the join app will join."""
```

### Comparing `parsl-2023.7.24/parsl/errors.py` & `parsl-2023.7.3/parsl/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/executors/base.py` & `parsl-2023.7.3/parsl/executors/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABCMeta, abstractmethod
 from concurrent.futures import Future
 from typing import Any, Callable, Dict, Optional, List
 from typing_extensions import Literal, Self
 
-from parsl.jobs.states import JobStatus
+from parsl.providers.base import JobStatus
 
 import parsl  # noqa F401
 
 
 class ParslExecutor(metaclass=ABCMeta):
     """Executors are abstractions that represent available compute resources
     to which you could submit arbitrary App tasks.
@@ -163,15 +163,15 @@
         should inherit from. Noop versions of methods that are related to status handling and
         running parsl tasks through workers are implemented by
         :class:parsl.executors.status_handling.NoStatusHandlingExecutor.
         """
         pass
 
     @abstractmethod
-    def handle_errors(self, error_handler: "parsl.jobs.job_error_handler.JobErrorHandler",
+    def handle_errors(self, error_handler: "parsl.dataflow.job_error_handler.JobErrorHandler",
                       status: Dict[str, JobStatus]) -> None:
         """This method is called by the error management infrastructure after a status poll. The
         executor implementing this method is then responsible for detecting abnormal conditions
         based on the status of submitted jobs. If the executor does not implement any special
         error handling, this method should return False, in which case a generic error handling
         scheme will be used.
         :param error_handler: a reference to the generic error handler calling this method
```

### Comparing `parsl-2023.7.24/parsl/executors/errors.py` & `parsl-2023.7.3/parsl/executors/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,22 +30,18 @@
 
     def __init__(self, feature, current_executor, target_executor):
         self.feature = feature
         self.current_executor = current_executor
         self.target_executor = target_executor
 
     def __str__(self):
-        if self.target_executor:
-            return "The {} feature is unsupported in {}. \
-                    Please checkout {} for this feature".format(self.feature,
-                                                                self.current_executor,
-                                                                self.target_executor)
-        else:
-            return "The {} feature is unsupported in {}.".format(self.feature,
-                                                                 self.current_executor)
+        return "The {} feature is unsupported in {}. \
+Please checkout {} for this feature".format(self.feature,
+                                            self.current_executor,
+                                            self.target_executor)
 
 
 class ScalingFailed(ExecutorError):
     """Scaling failed due to error in Execution provider."""
 
     def __str__(self):
         return f"Executor {self.executor.label} failed to scale due to: {self.reason}"
```

### Comparing `parsl-2023.7.24/parsl/executors/flux/execute_parsl_task.py` & `parsl-2023.7.3/parsl/executors/flux/execute_parsl_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/executors/flux/executor.py` & `parsl-2023.7.3/parsl/executors/flux/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/executors/flux/flux_instance_manager.py` & `parsl-2023.7.3/parsl/executors/flux/flux_instance_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/executors/high_throughput/executor.py` & `parsl-2023.7.3/parsl/executors/high_throughput/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,18 +93,17 @@
         Command line string to launch the process_worker_pool from the provider. The command line string
         will be formatted with appropriate values for the following values (debug, task_url, result_url,
         cores_per_worker, nodes_per_block, heartbeat_period ,heartbeat_threshold, logdir). For example:
         launch_cmd="process_worker_pool.py {debug} -c {cores_per_worker} --task_url={task_url} --result_url={result_url}"
 
     address : string
         An address to connect to the main Parsl process which is reachable from the network in which
-        workers will be running. This field expects an IPv4 address (xxx.xxx.xxx.xxx).
-        Most login nodes on clusters have several network interfaces available, only some of which
-        can be reached from the compute nodes. This field can be used to limit the executor to listen
-        only on a specific interface, and limiting connections to the internal network.
+        workers will be running. This can be either a hostname as returned by ``hostname`` or an
+        IP address. Most login nodes on clusters have several network interfaces available, only
+        some of which can be reached from the compute nodes.
         By default, the executor will attempt to enumerate and connect through all possible addresses.
         Setting an address here overrides the default behavior.
         default=None
 
     worker_ports : (int, int)
         Specify the ports to be used by workers to connect to Parsl. If this option is specified,
         worker_port_range will not be honored.
@@ -467,15 +466,14 @@
         """
         comm_q = Queue(maxsize=10)
         self.interchange_proc = ForkProcess(target=interchange.starter,
                                             args=(comm_q,),
                                             kwargs={"client_ports": (self.outgoing_q.port,
                                                                      self.incoming_q.port,
                                                                      self.command_client.port),
-                                                    "interchange_address": self.address,
                                                     "worker_ports": self.worker_ports,
                                                     "worker_port_range": self.worker_port_range,
                                                     "hub_address": self.hub_address,
                                                     "hub_port": self.hub_port,
                                                     "logdir": "{}/{}".format(self.run_dir, self.label),
                                                     "heartbeat_threshold": self.heartbeat_threshold,
                                                     "poll_period": self.poll_period,
@@ -557,27 +555,27 @@
 
         The outgoing_q is an external process listens on this
         queue for new work. This method behaves like a
         submit call as described here `Python docs: <https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor>`_
 
         Args:
             - func (callable) : Callable function
-            - resource_specification (dict): Dictionary containing relevant info about task that is needed by underlying executors.
             - args (list) : List of arbitrary positional arguments.
 
         Kwargs:
             - kwargs (dict) : A dictionary of arbitrary keyword args for func.
 
         Returns:
               Future
         """
         if resource_specification:
-            logger.error("Ignoring the call specification. "
-                         "Parsl call specification is not supported in HighThroughput Executor.")
-            raise UnsupportedFeatureError('resource specification', 'HighThroughput Executor', None)
+            logger.error("Ignoring the resource specification. "
+                         "Parsl resource specification is not supported in HighThroughput Executor. "
+                         "Please check WorkQueueExecutor if resource specification is needed.")
+            raise UnsupportedFeatureError('resource specification', 'HighThroughput Executor', 'WorkQueue Executor')
 
         if self.bad_state_is_set:
             raise self.executor_exception
 
         self._task_counter += 1
         task_id = self._task_counter
 
@@ -593,17 +591,18 @@
 
         try:
             fn_buf = pack_apply_message(func, args, kwargs,
                                         buffer_threshold=1024 * 1024)
         except TypeError:
             raise SerializationError(func.__name__)
 
-        msg = {"task_id": task_id, "buffer": fn_buf}
+        msg = {"task_id": task_id,
+               "buffer": fn_buf}
 
-        # Post task to the outgoing queue
+        # Post task to the the outgoing queue
         self.outgoing_q.put(msg)
 
         # Return the future
         return fut
 
     def create_monitoring_info(self, status):
         """ Create a msg for monitoring based on the poll status
```

### Comparing `parsl-2023.7.24/parsl/executors/high_throughput/interchange.py` & `parsl-2023.7.3/parsl/executors/high_throughput/interchange.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 #!/usr/bin/env python
+import argparse
 import zmq
 import os
 import sys
 import platform
 import random
 import time
 import datetime
 import pickle
 import signal
 import logging
 import queue
 import threading
 import json
 
-from typing import cast, Any, Dict, Set, Optional
+from typing import cast, Any, Dict, Set
 
 from parsl.utils import setproctitle
 from parsl.version import VERSION as PARSL_VERSION
 from parsl.serialize import serialize as serialize_object
 
 from parsl.app.errors import RemoteExceptionWrapper
 from parsl.executors.high_throughput.manager_record import ManagerRecord
 from parsl.monitoring.message_type import MessageType
 from parsl.process_loggers import wrap_with_logs
 
 
 HEARTBEAT_CODE = (2 ** 32) - 1
 PKL_HEARTBEAT_CODE = pickle.dumps((2 ** 32) - 1)
 
-LOGGER_NAME = "interchange"
-logger = logging.getLogger(LOGGER_NAME)
-
 
 class ManagerLost(Exception):
     ''' Task lost due to manager loss. Manager is considered lost when multiple heartbeats
     have been missed.
     '''
     def __init__(self, manager_id, hostname):
         self.manager_id = manager_id
         self.tstamp = time.time()
         self.hostname = hostname
 
-    def __str__(self):
+    def __repr__(self):
         return "Task failure due to loss of manager {} on host {}".format(self.manager_id.decode(), self.hostname)
 
+    def __str__(self):
+        return self.__repr__()
+
 
 class VersionMismatch(Exception):
     ''' Manager and Interchange versions do not match
     '''
     def __init__(self, interchange_version, manager_version):
         self.interchange_version = interchange_version
         self.manager_version = manager_version
 
-    def __str__(self):
+    def __repr__(self):
         return "Manager version info {} does not match interchange version info {}, causing a critical failure".format(
             self.manager_version,
             self.interchange_version)
 
+    def __str__(self):
+        return self.__repr__()
+
 
 class Interchange:
     """ Interchange is a task orchestrator for distributed systems.
 
     1. Asynchronously queue large volume of tasks (>100K)
     2. Allow for workers to join and leave the union
     3. Detect workers that have failed using heartbeats
     4. Service single and batch requests from workers
     """
     def __init__(self,
                  client_address="127.0.0.1",
-                 interchange_address: Optional[str] = None,
+                 interchange_address="127.0.0.1",
                  client_ports=(50055, 50056, 50057),
                  worker_ports=None,
                  worker_port_range=(54000, 55000),
                  hub_address=None,
                  hub_port=None,
                  heartbeat_threshold=60,
                  logdir=".",
@@ -81,17 +85,16 @@
              ) -> None:
         """
         Parameters
         ----------
         client_address : str
              The ip address at which the parsl client can be reached. Default: "127.0.0.1"
 
-        interchange_address : Optional str
-             If specified the interchange will only listen on this address for connections from workers
-             else, it binds to all addresses.
+        interchange_address : str
+             The ip address at which the workers will be able to reach the Interchange. Default: "127.0.0.1"
 
         client_ports : triple(int, int, int)
              The ports at which the client can be reached
 
         worker_ports : tuple(int, int)
              The specific two ports at which workers will connect to the Interchange. Default: None
 
@@ -124,15 +127,15 @@
         os.makedirs(self.logdir, exist_ok=True)
 
         start_file_logger("{}/interchange.log".format(self.logdir), level=logging_level)
         logger.propagate = False
         logger.debug("Initializing Interchange process")
 
         self.client_address = client_address
-        self.interchange_address: str = interchange_address or "*"
+        self.interchange_address = interchange_address
         self.poll_period = poll_period
 
         logger.info("Attempting connection to client at {} on ports: {},{},{}".format(
             client_address, client_ports[0], client_ports[1], client_ports[2]))
         self.context = zmq.Context()
         self.task_incoming = self.context.socket(zmq.DEALER)
         self.task_incoming.set_hwm(0)
@@ -159,22 +162,22 @@
         self.results_incoming = self.context.socket(zmq.ROUTER)
         self.results_incoming.set_hwm(0)
 
         if self.worker_ports:
             self.worker_task_port = self.worker_ports[0]
             self.worker_result_port = self.worker_ports[1]
 
-            self.task_outgoing.bind(f"tcp://{self.interchange_address}:{self.worker_task_port}")
-            self.results_incoming.bind(f"tcp://{self.interchange_address}:{self.worker_result_port}")
+            self.task_outgoing.bind("tcp://*:{}".format(self.worker_task_port))
+            self.results_incoming.bind("tcp://*:{}".format(self.worker_result_port))
 
         else:
-            self.worker_task_port = self.task_outgoing.bind_to_random_port(f"tcp://{self.interchange_address}",
+            self.worker_task_port = self.task_outgoing.bind_to_random_port('tcp://*',
                                                                            min_port=worker_port_range[0],
                                                                            max_port=worker_port_range[1], max_tries=100)
-            self.worker_result_port = self.results_incoming.bind_to_random_port(f"tcp://{self.interchange_address}",
+            self.worker_result_port = self.results_incoming.bind_to_random_port('tcp://*',
                                                                                 min_port=worker_port_range[0],
                                                                                 max_port=worker_port_range[1], max_tries=100)
 
         logger.info("Bound to ports {},{} for incoming worker connections".format(
             self.worker_task_port, self.worker_result_port))
 
         self._ready_managers: Dict[bytes, ManagerRecord] = {}
@@ -573,37 +576,39 @@
                     self.results_outgoing.send(pkl_package)
             logger.warning("Sent failure reports, unregistering manager")
             self._ready_managers.pop(manager_id, 'None')
             if manager_id in interesting_managers:
                 interesting_managers.remove(manager_id)
 
 
-def start_file_logger(filename, level=logging.DEBUG, format_string=None):
+def start_file_logger(filename, name='interchange', level=logging.DEBUG, format_string=None):
     """Add a stream log handler.
 
     Parameters
     ---------
 
     filename: string
         Name of the file to write logs to. Required.
+    name: string
+        Logger name. Default="parsl.executors.interchange"
     level: logging.LEVEL
         Set the logging level. Default=logging.DEBUG
         - format_string (string): Set the format string
     format_string: string
         Format string to use.
 
     Returns
     -------
         None.
     """
     if format_string is None:
         format_string = "%(asctime)s.%(msecs)03d %(name)s:%(lineno)d %(processName)s(%(process)d) %(threadName)s %(funcName)s [%(levelname)s]  %(message)s"
 
     global logger
-    logger = logging.getLogger(LOGGER_NAME)
+    logger = logging.getLogger(name)
     logger.setLevel(level)
     handler = logging.FileHandler(filename)
     handler.setLevel(level)
     formatter = logging.Formatter(format_string, datefmt='%Y-%m-%d %H:%M:%S')
     handler.setFormatter(formatter)
     logger.addHandler(handler)
 
@@ -616,7 +621,50 @@
     """
     setproctitle("parsl: HTEX interchange")
     # logger = multiprocessing.get_logger()
     ic = Interchange(*args, **kwargs)
     comm_q.put((ic.worker_task_port,
                 ic.worker_result_port))
     ic.start()
+
+
+if __name__ == '__main__':
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-c", "--client_address",
+                        help="Client address")
+    parser.add_argument("-l", "--logdir", default="parsl_worker_logs",
+                        help="Parsl worker log directory")
+    parser.add_argument("-t", "--task_url",
+                        help="REQUIRED: ZMQ url for receiving tasks")
+    parser.add_argument("-r", "--result_url",
+                        help="REQUIRED: ZMQ url for posting results")
+    parser.add_argument("-p", "--poll_period",
+                        help="REQUIRED: poll period used for main thread")
+    parser.add_argument("--worker_ports", default=None,
+                        help="OPTIONAL, pair of workers ports to listen on, eg --worker_ports=50001,50005")
+    parser.add_argument("-d", "--debug", action='store_true',
+                        help="Count of apps to launch")
+
+    args = parser.parse_args()
+
+    # Setup logging
+    global logger
+    format_string = "%(asctime)s %(name)s:%(lineno)d [%(levelname)s]  %(message)s"
+
+    logger = logging.getLogger("interchange")
+    logger.setLevel(logging.DEBUG)
+    handler = logging.StreamHandler()
+    handler.setLevel('DEBUG' if args.debug is True else 'INFO')
+    formatter = logging.Formatter(format_string, datefmt='%Y-%m-%d %H:%M:%S')
+    handler.setFormatter(formatter)
+    logger.addHandler(handler)
+
+    logger.debug("Starting Interchange")
+
+    optionals = {}
+
+    if args.worker_ports:
+        optionals['worker_ports'] = [int(i) for i in args.worker_ports.split(',')]
+
+    ic = Interchange(**optionals)
+    ic.start()
```

### Comparing `parsl-2023.7.24/parsl/executors/high_throughput/probe.py` & `parsl-2023.7.3/parsl/executors/high_throughput/probe.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/executors/high_throughput/process_worker_pool.py` & `parsl-2023.7.3/parsl/executors/high_throughput/process_worker_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,26 +366,26 @@
                     logger.debug("Result send: No items to push")
             else:
                 logger.debug(f"Result send: check condition not met - deferring {len(items)} result items")
 
         logger.critical("Exiting")
 
     @wrap_with_logs
-    def worker_watchdog(self, kill_event: threading.Event):
+    def worker_watchdog(self, kill_event):
         """Keeps workers alive.
 
         Parameters:
         -----------
         kill_event : threading.Event
               Event to let the thread know when it is time to die.
         """
 
         logger.debug("Starting worker watchdog")
 
-        while not kill_event.wait(self.heartbeat_period):
+        while not kill_event.is_set():
             for worker_id, p in self.procs.items():
                 if not p.is_alive():
                     logger.error("Worker {} has died".format(worker_id))
                     try:
                         task = self._tasks_in_progress.pop(worker_id)
                         logger.info("Worker {} was busy when it died".format(worker_id))
                         try:
@@ -405,14 +405,15 @@
                                                             self.pending_result_queue,
                                                             self.ready_worker_queue,
                                                             self._tasks_in_progress,
                                                             self.cpu_affinity),
                                        name="HTEX-Worker-{}".format(worker_id))
                     self.procs[worker_id] = p
                     logger.info("Worker {} has been restarted".format(worker_id))
+                time.sleep(self.heartbeat_period)
 
         logger.critical("Exiting")
 
     def start(self):
         """ Start the worker processes.
 
         TODO: Move task receiving to a thread
```

### Comparing `parsl-2023.7.24/parsl/executors/high_throughput/zmq_pipes.py` & `parsl-2023.7.3/parsl/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/executors/status_handling.py` & `parsl-2023.7.3/parsl/executors/status_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from abc import abstractmethod, abstractproperty
 from concurrent.futures import Future
 from typing import List, Any, Dict, Optional, Tuple, Union
 
 import parsl  # noqa F401
 from parsl.executors.base import ParslExecutor
 from parsl.executors.errors import BadStateException, ScalingFailed
-from parsl.jobs.states import JobStatus, JobState
-from parsl.providers.base import ExecutionProvider
+from parsl.providers.base import JobStatus, ExecutionProvider, JobState
 from parsl.utils import AtomicIDCounter
 
 
 logger = logging.getLogger(__name__)
 
 
 class BlockProviderExecutor(ParslExecutor):
@@ -41,15 +40,15 @@
     any init_blocks parameter. Subclasses must implement that behaviour
     themselves.
 
     BENC: TODO: block error handling: maybe I want this more user pluggable?
     I'm not sure of use cases for switchability at the moment beyond "yes or no"
     """
     def __init__(self, *,
-                 provider: Optional[ExecutionProvider],
+                 provider: ExecutionProvider,
                  block_error_handler: bool):
         super().__init__()
         self._provider = provider
         self.block_error_handler = block_error_handler
         # errors can happen during the submit call to the provider; this is used
         # to keep track of such errors so that they can be handled in one place
         # together with errors reported by status()
@@ -132,15 +131,15 @@
     def executor_exception(self):
         return self._executor_exception
 
     @property
     def error_management_enabled(self):
         return self.block_error_handler
 
-    def handle_errors(self, error_handler: "parsl.jobs.job_error_handler.JobErrorHandler",
+    def handle_errors(self, error_handler: "parsl.dataflow.job_error_handler.JobErrorHandler",
                       status: Dict[str, JobStatus]) -> None:
         if not self.block_error_handler:
             return
         init_blocks = 3
         if hasattr(self.provider, 'init_blocks'):
             init_blocks = self.provider.init_blocks
         if init_blocks < 1:
@@ -232,14 +231,14 @@
 
     def set_bad_state_and_fail_all(self, exception: Exception):
         pass
 
     def status(self):
         return {}
 
-    def handle_errors(self, error_handler: "parsl.jobs.job_error_handler.JobErrorHandler",
+    def handle_errors(self, error_handler: "parsl.dataflow.job_error_handler.JobErrorHandler",
                       status: Dict[str, JobStatus]) -> None:
         pass
 
     @property
     def provider(self):
         return self._provider
```

### Comparing `parsl-2023.7.24/parsl/executors/taskvine/exec_parsl_function.py` & `parsl-2023.7.3/parsl/executors/taskvine/exec_parsl_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 from parsl.app.errors import RemoteExceptionWrapper
 from parsl.data_provider.files import File
 from parsl.utils import get_std_fname_mode
 import traceback
 import sys
 import pickle
 
-# This scripts executes a parsl function which is pickled in 3 files:
+# This scripts executes a parsl function which is pickled in a file:
 #
 # exec_parsl_function.py map_file function_file result_file
 #
 # map_file: Contains a pickled dictionary that indicates which local_paths the
 #           parsl Files should take.
 #
-# function_file: Contains a pickle parsl function. Function might be serialized in advance.
-# See @parsl.serialize.concretes.py
+# function_file: Contains a pickle parsl function.
 #
-# result_file: A file path, whose content will contain the result of the function, including any
+# result_file: It will contain the result of the function, including any
 #              exception generated. Exceptions will be wrapped with RemoteExceptionWrapper.
 #
 # Exit codes:
 # 0: The function was evaluated to completion. The result or any exception
 #    wrapped with RemoteExceptionWrapper were written to result_file.
 # anything else: There was an error that prevented writing to the result file altogether.
 #                The exit code corresponds to whatever the python interpreter gives.
 #
 
 
-def load_pickled_file(filename: str):
-    """ Load a pickled file and return its pickled object."""
+def load_pickled_file(filename):
     with open(filename, "rb") as f_in:
         return pickle.load(f_in)
 
 
-def dump_result_to_file(result_file: str, result_package):
-    """ Dump a result to the given result file."""
+def dump_result_to_file(result_file, result_package):
     with open(result_file, "wb") as f_out:
         pickle.dump(result_package, f_out)
 
 
 def remap_location(mapping, parsl_file):
-    """ Remap files from local name (on manager) to remote name (on worker)."""
     if not isinstance(parsl_file, File):
         return
     # Below we rewrite .local_path when scheme != file only when the local_name
     # was given by the main parsl process.  This is the case when scheme !=
     # 'file' but .local_path (via filepath) is in mapping.
     if parsl_file.scheme == 'file' or parsl_file.local_path:
         master_location = parsl_file.filepath
         if master_location in mapping:
             parsl_file.local_path = mapping[master_location]
 
 
 def remap_list_of_files(mapping, maybe_files):
-    """ Remap a list of potential files."""
     for maybe_file in maybe_files:
         remap_location(mapping, maybe_file)
 
 
 def remap_all_files(mapping, fn_args, fn_kwargs):
     # remap any positional argument given to the function that looks like a
     # File
@@ -75,48 +70,70 @@
                     fn_kwargs[kwarg] = (mapping[fname], mode)
         else:
             # Treat anything else as a possible File to be remapped.
             remap_location(mapping, maybe_file)
 
 
 def unpack_function(function_info, user_namespace):
-    """ Unpack a function according to its encoding scheme."""
-    return unpack_byte_code_function(function_info, user_namespace)
+    if "source code" in function_info:
+        return unpack_source_code_function(function_info, user_namespace)
+    elif "byte code" in function_info:
+        return unpack_byte_code_function(function_info, user_namespace)
+    else:
+        raise ValueError("Function file does not have a valid function representation.")
+
+
+def unpack_source_code_function(function_info, user_namespace):
+    source_code = function_info["source code"]
+    name = function_info["name"]
+    args = function_info["args"]
+    kwargs = function_info["kwargs"]
+    return (source_code, name, args, kwargs)
 
 
 def unpack_byte_code_function(function_info, user_namespace):
-    """ Returns a function object, a default name, positional arguments, and keyword arguments
-    for a function."""
     from parsl.serialize import unpack_apply_message
     func, args, kwargs = unpack_apply_message(function_info["byte code"], user_namespace, copy=False)
     return (func, 'parsl_function_name', args, kwargs)
 
 
 def encode_function(user_namespace, fn, fn_name, fn_args, fn_kwargs):
-    """ Register the given function to the given namespace."""
     # Returns a tuple (code, result_name)
     # code can be exec in the user_namespace to produce result_name.
     prefix = "parsl_"
     args_name = prefix + "args"
     kwargs_name = prefix + "kwargs"
     result_name = prefix + "result"
 
     # Add variables to the namespace to make function call
     user_namespace.update({args_name: fn_args,
                            kwargs_name: fn_kwargs,
                            result_name: result_name})
 
-    if callable(fn):
+    if isinstance(fn, str):
+        code = encode_source_code_function(user_namespace, fn, fn_name, args_name, kwargs_name, result_name)
+    elif callable(fn):
         code = encode_byte_code_function(user_namespace, fn, fn_name, args_name, kwargs_name, result_name)
     else:
         raise ValueError("Function object does not look like a function.")
 
     return (code, result_name)
 
 
+def encode_source_code_function(user_namespace, fn, fn_name, args_name, kwargs_name, result_name):
+    # We drop the first line as it names the parsl decorator used (i.e., @python_app)
+    source = fn.split('\n')[1:]
+    fn_app = "{0} = {1}(*{2}, **{3})".format(result_name, fn_name, args_name, kwargs_name)
+
+    source.append(fn_app)
+
+    code = "\n".join(source)
+    return code
+
+
 def encode_byte_code_function(user_namespace, fn, fn_name, args_name, kwargs_name, result_name):
     user_namespace.update({fn_name: fn})
     code = "{0} = {1}(*{2}, **{3})".format(result_name, fn_name, args_name, kwargs_name)
     return code
 
 
 def load_function(map_file, function_file):
```

### Comparing `parsl-2023.7.24/parsl/executors/taskvine/executor.py` & `parsl-2023.7.3/parsl/executors/taskvine/executor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,290 +1,380 @@
 """ TaskVineExecutor utilizes the TaskVine distributed framework developed by the
 Cooperative Computing Lab (CCL) at Notre Dame to provide a fault-tolerant,
 high-throughput system for delegating Parsl tasks to thousands of remote machines
 """
 
-# Import Python built-in libraries
 import threading
 import multiprocessing
 import logging
+from concurrent.futures import Future
+from ctypes import c_bool
+
 import tempfile
 import hashlib
 import subprocess
 import os
+import socket
 import time
 import pickle
 import queue
 import inspect
 import shutil
 import itertools
-import uuid
-from ctypes import c_bool
-from concurrent.futures import Future
-from typing import List, Optional, Union
 
-# Import Parsl constructs
-import parsl.utils as putils
-from parsl.utils import setproctitle
-from parsl.data_provider.staging import Staging
 from parsl.serialize import pack_apply_message
+import parsl.utils as putils
+from parsl.executors.errors import ExecutorError
 from parsl.data_provider.files import File
 from parsl.errors import OptionalModuleMissing
+from parsl.executors.status_handling import BlockProviderExecutor
 from parsl.providers.base import ExecutionProvider
 from parsl.providers import LocalProvider, CondorProvider
-from parsl.process_loggers import wrap_with_logs
-from parsl.addresses import get_any_address
-from parsl.executors.errors import ExecutorError
-from parsl.executors.errors import UnsupportedFeatureError
-from parsl.executors.status_handling import BlockProviderExecutor
 from parsl.executors.taskvine import exec_parsl_function
-from parsl.executors.taskvine.manager_config import TaskVineManagerConfig
-from parsl.executors.taskvine.factory_config import TaskVineFactoryConfig
-from parsl.executors.taskvine.errors import TaskVineTaskFailure
-from parsl.executors.taskvine.errors import TaskVineManagerFailure
-from parsl.executors.taskvine.errors import TaskVineFactoryFailure
-from parsl.executors.taskvine.utils import ParslTaskToVine
-from parsl.executors.taskvine.utils import VineTaskToParsl
-from parsl.executors.taskvine.utils import ParslFileToVine
+from parsl.process_loggers import wrap_with_logs
+from parsl.utils import setproctitle
 
-# Import other libraries
 import typeguard
+from typing import Dict, List, Optional, Union
+from parsl.data_provider.staging import Staging
+
+from .errors import TaskVineTaskFailure
+from .errors import TaskVineFailure
+
+from collections import namedtuple
 
-# Import TaskVine python modules
 try:
     from ndcctools.taskvine import cvine
     from ndcctools.taskvine import Manager
-    from ndcctools.taskvine import Factory
     from ndcctools.taskvine import Task
+    from ndcctools.taskvine.cvine import VINE_DEFAULT_PORT
     from ndcctools.taskvine.cvine import VINE_ALLOCATION_MODE_MAX_THROUGHPUT
-    from ndcctools.taskvine.cvine import VINE_ALLOCATION_MODE_EXHAUSTIVE_BUCKETING
-    from ndcctools.taskvine.cvine import VINE_ALLOCATION_MODE_MAX
 except ImportError:
     _taskvine_enabled = False
+    VINE_DEFAULT_PORT = 0
 else:
     _taskvine_enabled = True
 
+package_analyze_script = shutil.which("poncho_package_analyze")
+package_create_script = shutil.which("poncho_package_create")
+package_run_script = shutil.which("poncho_package_run")
+
 logger = logging.getLogger(__name__)
 
 
+# Support structure to communicate parsl tasks to the taskvine submit thread.
+ParslTaskToVine = namedtuple('ParslTaskToVine',
+                             'id category cores memory disk gpus priority running_time_min \
+                              env_pkg map_file function_file result_file input_files output_files')
+
+# Support structure to communicate final status of taskvine tasks to parsl
+# result is only valid if result_received is True
+# reason and status are only valid if result_received is False
+VineTaskToParsl = namedtuple('VineTaskToParsl', 'id result_received result reason status')
+
+# Support structure to report parsl filenames to taskvine.
+# parsl_name is the local_name or filepath attribute of a parsl file object.
+# stage tells whether the file should be copied by taskvine to the workers.
+# cache tells whether the file should be cached at workers. Only valid if stage == True
+ParslFileToVine = namedtuple('ParslFileToVine', 'parsl_name stage cache')
+
+
 class TaskVineExecutor(BlockProviderExecutor, putils.RepresentationMixin):
-    """Executor to use TaskVine dynamic workflow system
+    """Executor to use TaskVine batch system
 
     The TaskVineExecutor system utilizes the TaskVine framework to
     efficiently delegate Parsl apps to remote machines in clusters and
     grids using a fault-tolerant system. Users can run the
     vine_worker program on remote machines to connect to the
     TaskVineExecutor, and Parsl apps will then be sent out to these
     machines for execution and retrieval.
 
-    This Executor sets up configurations for the TaskVine manager, TaskVine
-    factory, and run both in separate processes. Sending tasks and receiving
-    results are done through multiprocessing module native to Python.
 
     Parameters
     ----------
 
         label: str
             A human readable label for the executor, unique
-            with respect to other executors.
+            with respect to other TaskVine master programs.
             Default is "TaskVineExecutor".
 
-        use_factory: bool
-            Choose to whether use either the Parsl provider or
-            TaskVine factory to scale workers.
+        project_name: str
+            If a project_name is given, then TaskVine will periodically
+            report its status and performance back to the global TaskVine catalog,
+            which can be viewed here:  http://ccl.cse.nd.edu/software/taskvine/status
+            Default is None.  Overrides address.
+
+        project_password_file: str
+            Optional password file for the taskvine project. Default is None.
+
+        address: str
+            The ip to contact this taskvine master process.
+            If not given, uses the address of the current machine as returned
+            by socket.gethostname().
+            Ignored if project_name is specified.
+
+        port: int
+            TCP port on Parsl submission machine for TaskVine workers
+            to connect to. Workers will connect to Parsl using this port.
+
+            If 0, TaskVine will allocate a port number automatically.
+            In this case, environment variables can be used to influence the
+            choice of port, documented here:
+            https://cctools.readthedocs.io/en/stable/api/html/taskvine_8h.html#a47ac70464e357e4dfcb0722fee6c44a0
+            Default is VINE_DEFAULT_PORT.
+
+        env: dict{str}
+            Dictionary that contains the environmental variables that
+            need to be set on the TaskVine worker machine.
+
+        shared_fs: bool
+            Define if working in a shared file system or not. If Parsl
+            and the TaskVine workers are on a shared file system, TaskVine
+            does not need to transfer and rename files for execution.
             Default is False.
 
-        manager_config: TaskVineManagerConfig
-            Configuration for the TaskVine manager. Default
+        use_cache: bool
+            Whether workers should cache files of tasks.
+            Default is True.
+
+        source: bool
+            Choose whether to transfer parsl app information as
+            source code. (Note: this increases throughput for
+            @python_apps, but the implementation does not include
+            functionality for @bash_apps, and thus source=False
+            must be used for programs utilizing @bash_apps.)
+            Default is False. Set to True if pack is True.
+
+        pack: bool
+            Use conda-pack to prepare a self-contained Python evironment for
+            each task. This greatly increases task latency, but does not
+            require a common environment or shared FS on execution nodes.
+            Implies source=True. Default is False.
+
+        pack_env: str
+            An already prepared environment tarball using poncho_package_create
+            to attach to each task.
+            Default is "".
+
+        extra_pkgs: list
+            List of extra pip/conda package names to include when packing
+            the environment. This may be useful if the app executes other
+            (possibly non-Python) programs provided via pip or conda.
+            Scanning the app source for imports would not detect these
+            dependencies, so they need to be manually specified.
+
+        autolabel: bool
+            Use the Resource Monitor to automatically determine resource
+            labels based on observed task behavior.
+
+        autolabel_window: int
+            Set the number of tasks considered for autolabeling. TaskVine
+            will wait for a series of N tasks with steady resource
+            requirements before making a decision on labels. Increasing
+            this parameter will reduce the number of failed tasks due to
+            resource exhaustion when autolabeling, at the cost of increased
+            resources spent collecting stats.
+
+        autocategory: bool
+            Place each app in its own category by default. If all
+            invocations of an app have similar performance characteristics,
+            this will provide a reasonable set of categories automatically.
+            Default is True.
+
+        max_retries: int
+            Set the number of retries that TaskVine will make when a task
+            fails. This is distinct from Parsl level retries configured in
+            parsl.config.Config. Set to None to allow TaskVine to retry
+            tasks forever. By default, this is set to 1, so that all retries
+            will be managed by Parsl.
+
+        init_command: str
+            Command line to run before executing a task in a worker.
+            Default is ''.
+
+        worker_options: str
+            Extra options passed to vine_worker. Default is ''.
+
+        worker_executable: str
+            The command used to invoke vine_worker. This can be used
+            when the worker needs to be wrapped inside some other command
+            (for example, to run the worker inside a container). Default is
+            'vine_worker'.
+
+        function_dir: str
+            The directory where serialized function invocations are placed
+            to be sent to workers. If undefined, this defaults to a directory
+            under runinfo/. If shared_filesystem=True, then this directory
+            must be visible from both the submitting side and workers.
+
+        wait_for_workers: int
+            The number of workers to wait for before running any task.
+            Default is 0, so the manager won't wait for workers to connect.
+
+        enable_peer_transfers: bool
+            Option to enable transferring files between workers.
+            Default is True.
 
-        factory_config: TaskVineFactoryConfig
-            Configuration for the TaskVine factory.
-            Use of factory is disabled by default.
+        full_debug: bool
+            Whether to enable full debug mode for monitoring in TaskVine.
+            Default is False.
 
         provider: ExecutionProvider
             The Parsl provider that will spawn worker processes.
             Default to spawning one local vine worker process.
 
-        storage_access: List[Staging]
+        storage_access: Optional[List[Staging]]
             Define Parsl file staging providers for this executor.
             Default is None.
     """
 
     radio_mode = "filesystem"
 
     @typeguard.typechecked
     def __init__(self,
                  label: str = "TaskVineExecutor",
-                 use_factory: bool = False,
-                 manager_config: TaskVineManagerConfig = TaskVineManagerConfig(),
-                 factory_config: TaskVineFactoryConfig = TaskVineFactoryConfig(),
-                 provider: Optional[ExecutionProvider] = LocalProvider(init_blocks=1),
+                 project_name: Optional[str] = None,
+                 project_password_file: Optional[str] = None,
+                 address: Optional[str] = None,
+                 port: int = VINE_DEFAULT_PORT,
+                 env: Optional[Dict] = None,
+                 shared_fs: bool = False,
+                 use_cache: bool = True,
+                 source: bool = False,
+                 pack: bool = False,
+                 pack_env: str = "",
+                 extra_pkgs: Optional[List[str]] = None,
+                 autolabel: bool = False,
+                 autolabel_window: int = 1,
+                 autocategory: bool = True,
+                 max_retries: int = 1,
+                 init_command: str = "",
+                 worker_options: str = "",
+                 worker_executable: str = 'vine_worker',
+                 function_dir: Optional[str] = None,
+                 wait_for_workers: int = 0,
+                 enable_peer_transfers: bool = True,
+                 full_debug: bool = False,
+                 provider: ExecutionProvider = LocalProvider(),
                  storage_access: Optional[List[Staging]] = None):
-
-        # If TaskVine factory is used, disable the Parsl provider
-        if use_factory:
-            provider = None
-
-        # Initialize the parent class with the execution provider and block error handling enabled.
         BlockProviderExecutor.__init__(self, provider=provider,
                                        block_error_handler=True)
-
-        # Raise an exception if there's a problem importing TaskVine
         if not _taskvine_enabled:
             raise OptionalModuleMissing(['taskvine'], "TaskVineExecutor requires the taskvine module.")
 
-        # Executor configurations
         self.label = label
-        self.use_factory = use_factory
-        self.manager_config = manager_config
-        self.factory_config = factory_config
+        self.project_name = project_name
+        self.project_password_file = project_password_file
+        self.address = address
+        self.port = port
+        self.env = env
+        self.shared_fs = shared_fs
+        self.use_cache = use_cache
+        self.source = True if pack else source
+        self.pack = pack
+        self.pack_env = pack_env
+        self.extra_pkgs = extra_pkgs or []
+        self.autolabel = autolabel
+        self.autolabel_window = autolabel_window
+        self.autocategory = autocategory
+        self.max_retries = max_retries
+        self.init_command = init_command
+        self.worker_options = worker_options
+        self.worker_executable = worker_executable
+        self.function_dir = function_dir
+        self.wait_for_workers = wait_for_workers
+        self.enable_peer_transfers = enable_peer_transfers
+        self.full_debug = full_debug
         self.storage_access = storage_access
 
-        # Queue to send ready tasks from TaskVine executor process to TaskVine manager process
-        self.ready_task_queue: multiprocessing.Queue = multiprocessing.Queue()
+        # Queue to send tasks from TaskVine executor process to TaskVine manager process
+        self.task_queue: multiprocessing.Queue = multiprocessing.Queue()
 
-        # Queue to send finished tasks from TaskVine manager process to TaskVine executor process
-        self.finished_task_queue: multiprocessing.Queue = multiprocessing.Queue()
+        # Queue to send tasks from TaskVine manager process to TaskVine executor process
+        self.collector_queue: multiprocessing.Queue = multiprocessing.Queue()
 
-        # Value to signal whether the manager and factory processes should stop running
+        self.blocks: Dict[str, str] = {}  # track Parsl blocks
+        self.executor_task_counter = -1  # task id starts from 0
         self.should_stop = multiprocessing.Value(c_bool, False)
 
-        # TaskVine manager process
-        self.submit_process = None
-
-        # TaskVine factory process
-        self.factory_process = None
+        # mapping of function's unique memory address to its solved environment
+        self.cached_envs: Dict[int, str] = {}
 
-        # Executor thread to collect results from TaskVine manager and set
-        # tasks' futures to done status.
-        self.collector_thread = None
+        if not self.address:
+            self.address = socket.gethostname()
 
-        # track task id of submitted parsl tasks
-        # task ids are incremental and start from 0
-        self.executor_task_counter = 0
+        if self.project_password_file is not None and not os.path.exists(self.project_password_file):
+            raise TaskVineFailure('Could not find password file: {}'.format(self.project_password_file))
 
-        # track number of tasks that are waiting/running
-        self.outstanding_tasks = 0
-
-        # Lock for threads to access self.outstanding_tasks attribute
-        self.outstanding_tasks_lock = threading.Lock()
-
-        # Threading lock to manage self.tasks dictionary object, which maps a task id
-        # to its future object.
-        self.tasks_lock = threading.Lock()
-
-        # Worker command to be given to an execution provider (e.g., local or Condor)
-        self.worker_command = ""
-
-        # Path to directory that holds all tasks' data and results, only used when
-        # manager's task mode is 'regular'.
-        self.function_data_dir = ""
-
-        # helper scripts to prepare package tarballs for Parsl apps
-        self.package_analyze_script = shutil.which("poncho_package_analyze")
-        self.package_create_script = shutil.which("poncho_package_create")
+        # Build foundations of the launch command
+        self.launch_cmd = ("python3 exec_parsl_function.py {mapping} {function} {result}")
+        if self.init_command != "":
+            self.launch_cmd = self.init_command + "; " + self.launch_cmd
 
     def _get_launch_command(self, block_id):
-        # Implements BlockProviderExecutor's abstract method.
-        # This executor uses different terminology for worker/launch
-        # commands than in htex.
+        # this executor uses different terminology for worker/launch
+        # commands than in htex
         return f"PARSL_WORKER_BLOCK_ID={block_id} {self.worker_command}"
 
-    def __synchronize_manager_factory_comm_settings(self):
-        # Synchronize the communication settings between the manager and the factory
-        # so the factory can direct workers to contact the manager.
-
-        # If the manager can choose any available port (port number = 0),
-        # then it must have a project name
-        # so the factory can look it up. Otherwise the factory process will not know the
-        # port number as it's only chosen when the TaskVine manager process is run.
-        if self.manager_config.port == 0 and self.manager_config.project_name is None:
-            self.manager_config.project_name = "parsl-vine-" + str(uuid.uuid4())
-
-        # guess the host name if the project name is not given
-        if not self.manager_config.project_name:
-            self.manager_config.address = get_any_address()
-
-        # Factory communication settings are overridden by manager communication settings.
-        self.factory_config._project_port = self.manager_config.port
-        self.factory_config._project_address = self.manager_config.address
-        self.factory_config._project_name = self.manager_config.project_name
-        self.factory_config._project_password_file = self.manager_config.project_password_file
-
-    def __create_data_and_logging_dirs(self):
-        # Create neccessary data and logging directories
-
-        # Use the current run directory from Parsl
-        run_dir = self.run_dir
-
-        # Create directories for data and results
-        self.function_data_dir = os.path.join(run_dir, self.label, "function_data")
-        log_dir = os.path.join(run_dir, self.label)
-        logger.debug("function data directory: {}\nlog directory: {}".format(self.function_data_dir, log_dir))
-        os.makedirs(log_dir)
-        os.makedirs(self.function_data_dir)
-
-        # put TaskVine logs inside run directory of Parsl by default
-        if self.manager_config.vine_log_dir is None:
-            self.manager_config.vine_log_dir = log_dir
-            self.factory_config.scratch_dir = log_dir
-
     def start(self):
         """Create submit process and collector thread to create, send, and
         retrieve Parsl tasks within the TaskVine system.
         """
+        self.tasks_lock = threading.Lock()
 
-        # Synchronize connection and communication settings between the manager and factory
-        self.__synchronize_manager_factory_comm_settings()
-
-        # Create data and logging dirs
-        self.__create_data_and_logging_dirs()
+        # Create directories for data and results
+        if not self.function_dir:
+            self.function_data_dir = os.path.join(self.run_dir, self.label, "function_data")
+        else:
+            tp = str(time.time())
+            tx = os.path.join(self.function_dir, tp)
+            os.makedirs(tx)
+            self.function_data_dir = os.path.join(self.function_dir, tp, self.label, "function_data")
+        self.vine_log_dir = os.path.join(self.run_dir, self.label)
+        logger.debug("function data directory: {}\nlog directory: {}".format(self.function_data_dir, self.vine_log_dir))
+        os.makedirs(self.vine_log_dir)
+        os.makedirs(self.function_data_dir)
 
         logger.debug("Starting TaskVineExecutor")
 
-        # Create a process to run the TaskVine manager.
-        submit_process_kwargs = {"ready_task_queue": self.ready_task_queue,
-                                 "finished_task_queue": self.finished_task_queue,
+        # Create a Process to perform TaskVine submissions
+        submit_process_kwargs = {"task_queue": self.task_queue,
+                                 "launch_cmd": self.launch_cmd,
+                                 "env": self.env,
+                                 "collector_queue": self.collector_queue,
+                                 "full": self.full_debug,
+                                 "shared_fs": self.shared_fs,
+                                 "autolabel": self.autolabel,
+                                 "autolabel_window": self.autolabel_window,
+                                 "autocategory": self.autocategory,
+                                 "max_retries": self.max_retries,
                                  "should_stop": self.should_stop,
-                                 "manager_config": self.manager_config}
+                                 "port": self.port,
+                                 "vine_log_dir": self.vine_log_dir,
+                                 "project_password_file": self.project_password_file,
+                                 "project_name": self.project_name,
+                                 "wait_for_workers": self.wait_for_workers,
+                                 "enable_peer_transfers": self.enable_peer_transfers}
         self.submit_process = multiprocessing.Process(target=_taskvine_submit_wait,
                                                       name="TaskVine-Submit-Process",
                                                       kwargs=submit_process_kwargs)
 
-        # Create a process to run the TaskVine factory if enabled.
-        if self.use_factory:
-            factory_process_kwargs = {"should_stop": self.should_stop,
-                                      "factory_config": self.factory_config}
-            self.factory_process = multiprocessing.Process(target=_taskvine_factory,
-                                                           name="TaskVine-Factory-Process",
-                                                           kwargs=factory_process_kwargs)
-
-        # Run thread to collect results and set tasks' futures.
         self.collector_thread = threading.Thread(target=self._collect_taskvine_results,
-                                                 name="TaskVine-Collector-Thread")
-        # Interpreter can exit without waiting for this thread.
+                                                 name="TaskVine-collector-thread")
         self.collector_thread.daemon = True
 
-        # Begin work
+        # Begin both processes
         self.submit_process.start()
-
-        # Run worker scaler either with Parsl provider or TaskVine factory
-        if self.use_factory:
-            self.factory_process.start()
-        else:
-            self.initialize_scaling()
-
         self.collector_thread.start()
 
-        logger.debug("All components in TaskVineExecutor started")
+        # Initialize scaling for the provider
+        self.initialize_scaling()
 
     def _path_in_task(self, executor_task_id, *path_components):
-        """
-        Only used when task mode is `regular`.
-        Returns a filename fixed and specific to a task.
+        """Returns a filename fixed and specific to a task.
         It is used for the following filename's:
             (not given): The subdirectory per task that contains function, result, etc.
             'function': Pickled file that contains the function to be executed.
             'result': Pickled file that (will) contain the result of the function.
             'map': Pickled file with a dict between local parsl names, and remote taskvine names.
         """
         task_dir = "{:04d}".format(executor_task_id)
@@ -297,40 +387,53 @@
         the Parsl app, so that the files are appropriately specified for the TaskVine task.
 
         Parameters
         ----------
 
         func : function
             Parsl app to be submitted to the TaskVine system
-        resource_specification: dict
-            Dictionary containing relevant info about task.
-            Include information about resources of task, execution mode
-            of task (out of {regular, python, serverless}), and which app
-            type this function was submitted as (out of {python, bash}).
         args : list
             Arguments to the Parsl app
         kwargs : dict
             Keyword arguments to the Parsl app
         """
-
-        # Default execution mode of apps is regular (using TaskVineExecutor serialization and execution mode)
-        exec_mode = resource_specification.get('exec_mode', 'regular')
-
-        logger.debug(f'Got resource specification: {resource_specification}')
-
-        # Detect resources and features of a submitted Parsl app
         cores = None
         memory = None
         disk = None
         gpus = None
         priority = None
         category = None
         running_time_min = None
         if resource_specification and isinstance(resource_specification, dict):
-            for k in resource_specification:
+            logger.debug("Got resource specification: {}".format(resource_specification))
+
+            required_resource_types = set(['cores', 'memory', 'disk'])
+            acceptable_resource_types = set(['cores', 'memory', 'disk', 'gpus', 'priority', 'running_time_min'])
+            keys = set(resource_specification.keys())
+
+            if not keys.issubset(acceptable_resource_types):
+                message = "Task resource specification only accepts these types of resources: {}".format(
+                        ', '.join(acceptable_resource_types))
+                logger.error(message)
+                raise ExecutorError(self, message)
+
+            # this checks that either all of the required resource types are specified, or
+            # that none of them are: the `required_resource_types` are not actually required,
+            # but if one is specified, then they all must be.
+            key_check = required_resource_types.intersection(keys)
+            required_keys_ok = len(key_check) == 0 or key_check == required_resource_types
+            if not self.autolabel and not required_keys_ok:
+                logger.error("Running with `autolabel=False`. In this mode, "
+                             "task resource specification requires "
+                             "three resources to be specified simultaneously: cores, memory, and disk")
+                raise ExecutorError(self, "Task resource specification requires "
+                                          "three resources to be specified simultaneously: cores, memory, and disk. "
+                                          "Try setting autolabel=True if you are unsure of the resource usage")
+
+            for k in keys:
                 if k == 'cores':
                     cores = resource_specification[k]
                 elif k == 'memory':
                     memory = resource_specification[k]
                 elif k == 'disk':
                     disk = resource_specification[k]
                 elif k == 'gpus':
@@ -338,26 +441,24 @@
                 elif k == 'priority':
                     priority = resource_specification[k]
                 elif k == 'category':
                     category = resource_specification[k]
                 elif k == 'running_time_min':
                     running_time_min = resource_specification[k]
 
-        # Assign executor task id to app
-        executor_task_id = self.executor_task_counter
         self.executor_task_counter += 1
+        executor_task_id = self.executor_task_counter
 
-        # Create a per task directory for the function, map, and result files
+        # Create a per task directory for the function, result, map, and result files
         os.mkdir(self._path_in_task(executor_task_id))
 
         input_files = []
         output_files = []
 
-        # Determine whether to stage input files that will exist at the workers
-        # Input and output files are always cached
+        # Determine the input and output files that will exist at the workers:
         input_files += [self._register_file(f) for f in kwargs.get("inputs", []) if isinstance(f, File)]
         output_files += [self._register_file(f) for f in kwargs.get("outputs", []) if isinstance(f, File)]
 
         # Also consider any *arg that looks like a file as an input:
         input_files += [self._register_file(f) for f in args if isinstance(f, File)]
 
         for kwarg, maybe_file in kwargs.items():
@@ -368,91 +469,76 @@
             # For any other keyword that looks like a file, assume it is an input file
             elif isinstance(maybe_file, File):
                 input_files.append(self._register_file(maybe_file))
 
         # Create a Future object and have it be mapped from the task ID in the tasks dictionary
         fu = Future()
         fu.parsl_executor_task_id = executor_task_id
+        logger.debug("Getting tasks_lock to set vine-level task entry")
         with self.tasks_lock:
+            logger.debug("Got tasks_lock to set vine-level task entry")
             self.tasks[str(executor_task_id)] = fu
 
-        logger.debug("Creating task {} for function {} of type {} with args {}".format(executor_task_id, func, type(func), args))
+        logger.debug("Creating task {} for function {} with args {}".format(executor_task_id, func, args))
 
-        function_file = None
-        result_file = None
-        map_file = None
-        # Use executor's serialization method if app mode is 'regular'
-        if exec_mode == 'regular':
-            # Get path to files that will contain the pickled function, result, and map of input and output files
-            function_file = self._path_in_task(executor_task_id, "function")
-            result_file = self._path_in_task(executor_task_id, "result")
-            map_file = self._path_in_task(executor_task_id, "map")
-
-            logger.debug("Creating executor task {} with function at: {} and result to be found at: {}".format(executor_task_id, function_file, result_file))
+        # Pickle the result into object to pass into message buffer
+        function_file = self._path_in_task(executor_task_id, "function")
+        result_file = self._path_in_task(executor_task_id, "result")
+        map_file = self._path_in_task(executor_task_id, "map")
 
-            # Pickle the result into object to pass into message buffer
-            self._serialize_function(function_file, func, args, kwargs)
+        logger.debug("Creating Task {} with function at: {}".format(executor_task_id, function_file))
+        logger.debug("Creating Executor Task {} with result to be found at: {}".format(executor_task_id, result_file))
 
-            # Construct the map file of local filenames at worker
-            self._construct_map_file(map_file, input_files, output_files)
+        self._serialize_function(function_file, func, args, kwargs)
 
-        # Register a tarball containing all package dependencies for this app if instructed
-        if self.manager_config.app_pack:
+        if self.pack:
             env_pkg = self._prepare_package(func, self.extra_pkgs)
         else:
             env_pkg = None
 
+        if self.pack_env:
+            env_pkg = self.pack_env
+
+        logger.debug("Constructing map for local filenames at worker for task {}".format(executor_task_id))
+        self._construct_map_file(map_file, input_files, output_files)
+
         if not self.submit_process.is_alive():
             raise ExecutorError(self, "taskvine Submit Process is not alive")
 
         # Create message to put into the message queue
         logger.debug("Placing task {} on message queue".format(executor_task_id))
-
-        # Put apps into their categories based on function name if enabled
         if category is None:
-            category = func.__name__ if self.manager_config.autocategory else 'parsl-default'
-
-        # support for python and serverless exec mode delayed
-        if exec_mode == 'python' or exec_mode == 'serverless':
-            raise UnsupportedFeatureError(f'Execution mode {exec_mode} is not currently supported.', 'TaskVineExecutor', None)
-        task_info = ParslTaskToVine(executor_id=executor_task_id,
-                                    exec_mode=exec_mode,
-                                    category=category,
-                                    input_files=input_files,
-                                    output_files=output_files,
-                                    map_file=map_file,
-                                    function_file=function_file,
-                                    result_file=result_file,
-                                    cores=cores,
-                                    memory=memory,
-                                    disk=disk,
-                                    gpus=gpus,
-                                    priority=priority,
-                                    running_time_min=running_time_min,
-                                    env_pkg=env_pkg)
-
-        # Send ready task to manager process
-        self.ready_task_queue.put_nowait(task_info)
-
-        # Increment outstanding task counter
-        with self.outstanding_tasks_lock:
-            self.outstanding_tasks += 1
+            category = func.__name__ if self.autocategory else 'parsl-default'
+        self.task_queue.put_nowait(ParslTaskToVine(executor_task_id,
+                                                   category,
+                                                   cores,
+                                                   memory,
+                                                   disk,
+                                                   gpus,
+                                                   priority,
+                                                   running_time_min,
+                                                   env_pkg,
+                                                   map_file,
+                                                   function_file,
+                                                   result_file,
+                                                   input_files,
+                                                   output_files))
 
         return fu
 
     def _construct_worker_command(self):
-        worker_command = self.factory_config.worker_executable
-        if self.factory_config._project_password_file:
-            worker_command += ' --password {}'.format(self.factory_config._project_password_file)
-        if self.factory_config.worker_options:
-            worker_command += ' {}'.format(self.factory_config.worker_options)
-        if self.factory_config._project_name:
-            worker_command += ' -M {}'.format(self.factory_config._project_name)
+        worker_command = self.worker_executable
+        if self.project_password_file:
+            worker_command += ' --password {}'.format(self.project_password_file)
+        if self.worker_options:
+            worker_command += ' {}'.format(self.worker_options)
+        if self.project_name:
+            worker_command += ' -M {}'.format(self.project_name)
         else:
-            worker_command += ' {} {}'.format(self.factory_config._project_address, self.factory_config._project_port)
+            worker_command += ' {} {}'.format(self.address, self.port)
 
         logger.debug("Using worker command: {}".format(worker_command))
         return worker_command
 
     def _patch_providers(self):
         # Add the worker and password file to files that the provider needs to stage.
         # (Currently only for the CondorProvider)
@@ -462,70 +548,81 @@
             self.provider.transfer_input_files.append(path_to_worker)
             if self.project_password_file:
                 self.provider.transfer_input_files.append(self.project_password_file)
 
     def _serialize_function(self, fn_path, parsl_fn, parsl_fn_args, parsl_fn_kwargs):
         """Takes the function application parsl_fn(*parsl_fn_args, **parsl_fn_kwargs)
         and serializes it to the file fn_path."""
-        function_info = {"byte code": pack_apply_message(parsl_fn, parsl_fn_args, parsl_fn_kwargs,
-                                                         buffer_threshold=1024 * 1024)}
+
+        # Either build a dictionary with the source of the function, or pickle
+        # the function directly:
+        if self.source:
+            function_info = {"source code": inspect.getsource(parsl_fn),
+                             "name": parsl_fn.__name__,
+                             "args": parsl_fn_args,
+                             "kwargs": parsl_fn_kwargs}
+        else:
+            function_info = {"byte code": pack_apply_message(parsl_fn, parsl_fn_args, parsl_fn_kwargs,
+                                                             buffer_threshold=1024 * 1024)}
 
         with open(fn_path, "wb") as f_out:
             pickle.dump(function_info, f_out)
 
     def _construct_map_file(self, map_file, input_files, output_files):
         """ Map local filepath of parsl files to the filenames at the execution worker.
         If using a shared filesystem, the filepath is mapped to its absolute filename.
         Otherwise, to its original relative filename. In this later case, taskvine
         recreates any directory hierarchy needed."""
         file_translation_map = {}
         for spec in itertools.chain(input_files, output_files):
-            local_name = spec.parsl_name
-            if self.manager_config.shared_fs:
+            local_name = spec[0]
+            if self.shared_fs:
                 remote_name = os.path.abspath(local_name)
             else:
                 remote_name = local_name
             file_translation_map[local_name] = remote_name
         with open(map_file, "wb") as f_out:
             pickle.dump(file_translation_map, f_out)
 
     def _register_file(self, parsl_file):
         """Generates a tuple (parsl_file.filepath, stage, cache) to give to
-        taskvine. cache is always True.
-        stage is True if the file has a relative path. (i.e., not
+        taskvine. cache is always True if self.use_cache is True.
+        Otherwise, it is set to False.
+        stage is True if the file needs to be copied by taskvine. (i.e., not
         a URL or an absolute path)"""
+
         to_cache = True
+        if not self.use_cache:
+            to_cache = False
+
         to_stage = False
-        if parsl_file.scheme == 'file' or \
-           (parsl_file.local_path and os.path.exists(parsl_file.local_path)):
+        if parsl_file.scheme == 'file' or (parsl_file.local_path and os.path.exists(parsl_file.local_path)):
             to_stage = not os.path.isabs(parsl_file.filepath)
 
         return ParslFileToVine(parsl_file.filepath, to_stage, to_cache)
 
     def _std_output_to_vine(self, fdname, stdfspec):
         """Find the name of the file that will contain stdout or stderr and
         return a ParslFileToVine with it. These files are never cached"""
         fname, mode = putils.get_std_fname_mode(fdname, stdfspec)
         to_stage = not os.path.isabs(fname)
         return ParslFileToVine(fname, stage=to_stage, cache=False)
 
     def _prepare_package(self, fn, extra_pkgs):
-        """ Look at source code of apps to figure out their package depedencies
-        and output a tarball containing those to send along with tasks for execution."""
         fn_id = id(fn)
         fn_name = fn.__name__
         if fn_id in self.cached_envs:
             logger.debug("Skipping analysis of %s, previously got %s", fn_name, self.cached_envs[fn_id])
             return self.cached_envs[fn_id]
         source_code = inspect.getsource(fn).encode()
         pkg_dir = os.path.join(tempfile.gettempdir(), "python_package-{}".format(os.geteuid()))
         os.makedirs(pkg_dir, exist_ok=True)
         with tempfile.NamedTemporaryFile(suffix='.yaml') as spec:
             logger.info("Analyzing dependencies of %s", fn_name)
-            analyze_cmdline = [self.package_analyze_script, exec_parsl_function.__file__, '-', spec.name]
+            analyze_cmdline = [package_analyze_script, exec_parsl_function.__file__, '-', spec.name]
             for p in extra_pkgs:
                 analyze_cmdline += ["--extra-pkg", p]
             subprocess.run(analyze_cmdline, input=source_code, check=True)
             with open(spec.name, mode='rb') as f:
                 spec_hash = hashlib.sha256(f.read()).hexdigest()
                 logger.debug("Spec hash for %s is %s", fn_name, spec_hash)
                 pkg = os.path.join(pkg_dir, "pack-{}.tar.gz".format(spec_hash))
@@ -533,15 +630,15 @@
                 self.cached_envs[fn_id] = pkg
                 logger.debug("Cached package for %s found at %s", fn_name, pkg)
                 return pkg
             (fd, tarball) = tempfile.mkstemp(dir=pkg_dir, prefix='.tmp', suffix='.tar.gz')
             os.close(fd)
             logger.info("Creating dependency package for %s", fn_name)
             logger.debug("Writing deps for %s to %s", fn_name, tarball)
-            subprocess.run([self.package_create_script, spec.name, tarball], stdout=subprocess.DEVNULL, check=True)
+            subprocess.run([package_create_script, spec.name, tarball], stdout=subprocess.DEVNULL, check=True)
             logger.debug("Done with conda-pack; moving %s to %s", tarball, pkg)
             os.rename(tarball, pkg)
             self.cached_envs[fn_id] = pkg
             return pkg
 
     def initialize_scaling(self):
         """ Compose the launch command and call scale out
@@ -558,17 +655,24 @@
                 self.scale_out(blocks=self.provider.init_blocks)
             except Exception as e:
                 logger.error("Initial block scaling out failed: {}".format(e))
                 raise e
 
     @property
     def outstanding(self) -> int:
-        """Count the number of outstanding tasks."""
-        logger.debug(f"Counted {self.outstanding_tasks} outstanding tasks")
-        return self.outstanding_tasks
+        """Count the number of outstanding tasks. This is inefficiently
+        implemented and probably could be replaced with a counter.
+        """
+        outstanding = 0
+        with self.tasks_lock:
+            for fut in self.tasks.values():
+                if not fut.done():
+                    outstanding += 1
+        logger.debug(f"Counted {outstanding} outstanding tasks")
+        return outstanding
 
     @property
     def workers_per_node(self) -> Union[int, float]:
         return 1
 
     def scale_in(self, count):
         """Scale in method. Cancel a given number of blocks
@@ -592,280 +696,243 @@
 
         # Remove the workers that are still going
         kill_ids = [self.blocks[block] for block in self.blocks.keys()]
         if self.provider:
             logger.debug("Cancelling blocks")
             self.provider.cancel(kill_ids)
 
-        # Join all processes before exiting
         logger.debug("Joining on submit process")
         self.submit_process.join()
         logger.debug("Joining on collector thread")
         self.collector_thread.join()
-        if self.use_factory:
-            logger.debug("Joining on factory process")
-            self.factory_process.join()
 
         logger.debug("TaskVine shutdown completed")
         return True
 
     @wrap_with_logs
     def _collect_taskvine_results(self):
-        """Sets the values of tasks' futures completed by taskvine.
+        """Sets the values of tasks' futures of tasks completed by taskvine.
         """
         logger.debug("Starting Collector Thread")
         try:
             while not self.should_stop.value:
                 if not self.submit_process.is_alive():
                     raise ExecutorError(self, "taskvine Submit Process is not alive")
 
-                # Get the result message from the finished_task_queue
+                # Get the result message from the collector_queue
                 try:
-                    task_report = self.finished_task_queue.get(timeout=1)
+                    task_report = self.collector_queue.get(timeout=1)
                 except queue.Empty:
                     continue
 
                 # Obtain the future from the tasks dictionary
                 with self.tasks_lock:
-                    future = self.tasks.pop(task_report.executor_id)
+                    future = self.tasks.pop(task_report.id)
 
-                logger.debug("Updating Future for Parsl Task {}".format(task_report.executor_id))
-                logger.debug(f'task {task_report.executor_id} has result_received set to {task_report.result_received} and result to {task_report.result}')
+                logger.debug("Updating Future for Parsl Task {}".format(task_report.id))
                 if task_report.result_received:
                     future.set_result(task_report.result)
                 else:
                     # If there are no results, then the task failed according to one of
                     # taskvine modes, such as resource exhaustion.
                     future.set_exception(TaskVineTaskFailure(task_report.reason, task_report.result))
-
-                # decrement outstanding task counter
-                with self.outstanding_tasks_lock:
-                    self.outstanding_tasks -= 1
         finally:
-            logger.debug(f"Marking all {self.outstanding} outstanding tasks as failed")
+            logger.debug("Marking all outstanding tasks as failed")
             logger.debug("Acquiring tasks_lock")
             with self.tasks_lock:
                 logger.debug("Acquired tasks_lock")
                 # set exception for tasks waiting for results that taskvine did not execute
                 for fu in self.tasks.values():
                     if not fu.done():
-                        fu.set_exception(TaskVineManagerFailure("taskvine executor failed to execute the task."))
+                        fu.set_exception(TaskVineFailure("taskvine executor failed to execute the task."))
         logger.debug("Exiting Collector Thread")
 
 
 @wrap_with_logs
-def _taskvine_submit_wait(ready_task_queue=None,
-                          finished_task_queue=None,
+def _taskvine_submit_wait(task_queue=multiprocessing.Queue(),
+                          launch_cmd=None,
+                          env=None,
+                          collector_queue=multiprocessing.Queue(),
+                          full=False,
+                          shared_fs=False,
+                          autolabel=False,
+                          autolabel_window=None,
+                          autocategory=True,
+                          max_retries=None,
                           should_stop=None,
-                          manager_config=None
-                          ):
-    """Process to handle Parsl app submissions to the TaskVine objects.
+                          port=VINE_DEFAULT_PORT,
+                          vine_log_dir=None,
+                          project_password_file=None,
+                          project_name=None,
+                          wait_for_workers=0,
+                          enable_peer_transfers=True):
+    """Thread to handle Parsl app submissions to the TaskVine objects.
     Takes in Parsl functions submitted using submit(), and creates a
     TaskVine task with the appropriate specifications, which is then
     submitted to TaskVine. After tasks are completed, processes the
     exit status and exit code of the task, and sends results to the
     TaskVine collector thread.
     To avoid python's global interpreter lock with taskvine's wait, this
     function should be launched as a process, not as a lightweight thread. This
     means that any communication should be done using the multiprocessing
     module capabilities, rather than shared memory.
     """
     logger.debug("Starting TaskVine Submit/Wait Process")
     setproctitle("parsl: TaskVine submit/wait")
 
     # Enable debugging flags and create logging file
-    if manager_config.vine_log_dir is not None:
-        logger.debug("Setting debugging flags and creating logging file at {}".format(manager_config.vine_log_dir))
+    if vine_log_dir is not None:
+        logger.debug("Setting debugging flags and creating logging file at {}".format(vine_log_dir))
 
     # Create TaskVine queue object
     logger.debug("Creating TaskVine Object")
     try:
-        logger.debug("Listening on port {}".format(manager_config.port))
-        m = Manager(port=manager_config.port,
-                    name=manager_config.project_name,
-                    run_info_path=manager_config.vine_log_dir)
+        logger.debug("Listening on port {}".format(port))
+        m = Manager(port=port,
+                    name=project_name,
+                    run_info_path=vine_log_dir)
     except Exception as e:
         logger.error("Unable to create TaskVine object: {}".format(e))
         raise e
 
-    # Specify TaskVine manager attributes
-    if manager_config.project_password_file:
-        m.set_password_file(manager_config.project_password_file)
+    # Specify TaskVine queue attributes
+    if project_password_file:
+        m.set_password_file(project_password_file)
 
-    # Autolabeling resources require monitoring to be enabled
-    if manager_config.autolabel:
+    if autolabel:
         m.enable_monitoring()
-        if manager_config.autolabel_window is not None:
-            m.tune('category-steady-n-tasks', manager_config.autolabel_window)
+        if autolabel_window is not None:
+            m.tune('category-steady-n-tasks', autolabel_window)
 
-    # Specify number of workers to wait for before sending the first task
-    if manager_config.wait_for_workers:
-        m.tune("wait-for-workers", manager_config.wait_for_workers)
+    if wait_for_workers:
+        m.tune("wait-for-workers", wait_for_workers)
 
-    # Enable peer transfer feature between workers if specified
-    if manager_config.enable_peer_transfers:
+    if enable_peer_transfers:
         m.enable_peer_transfers()
 
-    # Get parent pid, useful to shutdown this process when its parent, the taskvine
-    # executor process, exits.
+    # Only write logs when the vine_log_dir is specified, which it most likely will be
+    # if vine_log_dir is not None:
+    if full and autolabel:
+        m.enable_monitoring_full(dirname=vine_log_dir)
+
     orig_ppid = os.getppid()
 
-    result_file_of_task_id = {}  # Mapping executor task id -> result file for active regular tasks.
+    result_file_of_task_id = {}  # Mapping executor task id -> result file for active tasks.
 
     poncho_env_to_file = {}  # Mapping poncho_env file to File object in TaskVine
 
     # Mapping of parsl local file name to TaskVine File object
     # dict[str] -> vine File object
     parsl_file_name_to_vine_file = {}
 
-    # Mapping of tasks from vine id to parsl id
-    # Dict[str] -> str
-    vine_id_to_executor_task_id = {}
-
-    # Find poncho run script to activate an environment tarball
-    poncho_run_script = shutil.which("poncho_package_run")
-
     # Declare helper scripts as cache-able and peer-transferable
-    package_run_script_file = m.declare_file(poncho_run_script, cache=True, peer_transfer=True)
+    package_run_script_file = m.declare_file(package_run_script, cache=True, peer_transfer=True)
     exec_parsl_function_file = m.declare_file(exec_parsl_function.__file__, cache=True, peer_transfer=True)
 
-    logger.debug("Entering main loop of TaskVine manager")
+    # Mapping of tasks from vine id to parsl id
+    # Dict[str] -> str
+    vine_id_to_executor_task_id = {}
 
     while not should_stop.value:
         # Monitor the task queue
         ppid = os.getppid()
         if ppid != orig_ppid:
             logger.debug("new Process")
             break
 
         # Submit tasks
-        while ready_task_queue.qsize() > 0 and not should_stop.value:
-            # Obtain task from ready_task_queue
+        while task_queue.qsize() > 0 and not should_stop.value:
+            # Obtain task from task_queue
             try:
-                task = ready_task_queue.get(timeout=1)
+                task = task_queue.get(timeout=1)
                 logger.debug("Removing executor task from queue")
             except queue.Empty:
-                logger.debug("Queue is empty")
                 continue
-            if task.exec_mode == 'regular':
-                # Create command string
-                launch_cmd = "python3 exec_parsl_function.py {mapping} {function} {result}"
-                if manager_config.init_command != '':
-                    launch_cmd = "{init_cmd};" + launch_cmd
-                command_str = launch_cmd.format(init_cmd=manager_config.init_command,
-                                                mapping=os.path.basename(task.map_file),
-                                                function=os.path.basename(task.function_file),
-                                                result=os.path.basename(task.result_file))
-                logger.debug("Sending executor task {} (mode: regular) with command: {}".format(task.executor_id, command_str))
-                try:
-                    t = Task(command_str)
-                except Exception as e:
-                    logger.error("Unable to create executor task (mode:regular): {}".format(e))
-                    finished_task_queue.put_nowait(VineTaskToParsl(executor_id=task.executor_id,
-                                                                   result_received=False,
-                                                                   result=None,
-                                                                   reason="task could not be created by taskvine",
-                                                                   status=-1))
-                    continue
-            else:
-                raise Exception(f'Unrecognized task mode {task.exec_mode}. Exiting...')
 
-            # Add environment file to the task if possible
-            # Prioritize local poncho environment over global poncho environment
-            # (local: use app_pack, global: use env_pack)
-            poncho_env_file = None
+            # Create command string
+            command_str = launch_cmd.format(mapping=os.path.basename(task.map_file),
+                                            function=os.path.basename(task.function_file),
+                                            result=os.path.basename(task.result_file))
 
-            # check if env_pack is specified
-            if manager_config.env_pack is not None:
-                # check if the environment file is not already created
-                if manager_config.env_pack not in poncho_env_to_file:
-                    # if the environment is already packaged as a tarball, then add the file
-                    # otherwise it is an environment name or path, so create a poncho tarball then add it
-                    if not manager_config.env_pack.endswith('.tar.gz'):
-                        env_tarball = str(uuid.uuid4()) + '.tar.gz'
-                        subprocess.run([poncho_run_script, manager_config.env_pack, env_tarball], stdout=subprocess.DEVNULL, check=True)
-                    poncho_env_file = m.declare_poncho(manager_config.env_pack, cache=True, peer_transfer=True)
-                    poncho_env_to_file[manager_config.env_pack] = poncho_env_file
-                else:
-                    poncho_env_file = poncho_env_to_file[manager_config.env_pack]
+            # Create TaskVine task for the command
+            logger.debug("Sending executor task {} with command: {}".format(task.id, command_str))
+            try:
+                t = Task(command_str)
+            except Exception as e:
+                logger.error("Unable to create executor task: {}".format(e))
+                collector_queue.put_nowait(VineTaskToParsl(id=task.id,
+                                                           result_received=False,
+                                                           result=None,
+                                                           reason="task could not be created by taskvine",
+                                                           status=-1))
+                continue
 
-            # check if app_pack is used, override if possible
+            poncho_env_file = None
             if task.env_pkg is not None:
                 if task.env_pkg not in poncho_env_to_file:
                     poncho_env_file = m.declare_poncho(task.env_pkg, cache=True, peer_transfer=True)
                     poncho_env_to_file[task.env_pkg] = poncho_env_file
                 else:
                     poncho_env_file = poncho_env_to_file[task.env_pkg]
 
-            # Add environment to the task
             if poncho_env_file is not None:
                 t.add_environment(poncho_env_file)
                 t.add_input(package_run_script_file, "poncho_package_run")
 
             t.set_category(task.category)
-            if manager_config.autolabel:
-                if manager_config.autolabel_algorithm == 'max-xput':
-                    m.set_category_mode(task.category, VINE_ALLOCATION_MODE_MAX_THROUGHPUT)
-                elif manager_config.autolabel_algorithm == 'bucketing':
-                    m.set_category_mode(task.category, VINE_ALLOCATION_MODE_EXHAUSTIVE_BUCKETING)
-                elif manager_config.autolabel_algorithm == 'max':
-                    m.set_category_mode(task.category, VINE_ALLOCATION_MODE_MAX)
-                else:
-                    logger.warning(f'Unrecognized autolabeling algorithm named {manager_config.autolabel_algorithm} for taskvine manager.')
-                    raise Exception(f'Unrecognized autolabeling algorithm named {manager_config.autolabel_algorithm} for taskvine manager.')
+            if autolabel:
+                m.set_category_mode(task.category, VINE_ALLOCATION_MODE_MAX_THROUGHPUT)
 
             if task.cores is not None:
                 t.set_cores(task.cores)
             if task.memory is not None:
                 t.set_memory(task.memory)
             if task.disk is not None:
                 t.set_disk(task.disk)
             if task.gpus is not None:
                 t.set_gpus(task.gpus)
             if task.priority is not None:
                 t.set_priority(task.priority)
             if task.running_time_min is not None:
                 t.set_time_min(task.running_time_min)
 
-            if manager_config.max_retries is not None:
-                logger.debug(f"Specifying max_retries {manager_config.max_retries}")
-                t.set_retries(manager_config.max_retries)
+            if max_retries is not None:
+                logger.debug(f"Specifying max_retries {max_retries}")
+                t.set_retries(max_retries)
             else:
                 logger.debug("Not specifying max_retries")
 
             # Specify environment variables for the task
-            if manager_config.env_vars is not None:
-                for var in manager_config.env_vars:
-                    t.set_env_var(str(var), str(manager_config.env_vars[var]))
+            if env is not None:
+                for var in env:
+                    t.set_env_var(str(var), str(env[var]))
 
-            if task.exec_mode == 'regular':
-                # Add helper files that execute parsl functions on remote nodes
-                # only needed for tasks with 'regular' mode
-                t.add_input(exec_parsl_function_file, "exec_parsl_function.py")
+            # Add helper function that execute parsl functions on remote nodes
+            t.add_input(exec_parsl_function_file, "exec_parsl_function.py")
 
-                # Declare and add task-specific function, data, and result files to task
-                task_function_file = m.declare_file(task.function_file, cache=False, peer_transfer=False)
-                t.add_input(task_function_file, "function")
+            # Declare and add task-specific function, data, and result files to task
+            task_function_file = m.declare_file(task.function_file, cache=False, peer_transfer=False)
+            t.add_input(task_function_file, "function")
 
-                task_map_file = m.declare_file(task.map_file, cache=False, peer_transfer=False)
-                t.add_input(task_map_file, "map")
+            task_map_file = m.declare_file(task.map_file, cache=False, peer_transfer=False)
+            t.add_input(task_map_file, "map")
 
-                task_result_file = m.declare_file(task.result_file, cache=False, peer_transfer=False)
-                t.add_output(task_result_file, "result")
+            task_result_file = m.declare_file(task.result_file, cache=False, peer_transfer=False)
+            t.add_output(task_result_file, "result")
 
-                result_file_of_task_id[str(task.executor_id)] = task.result_file
+            result_file_of_task_id[str(task.id)] = task.result_file
 
-            logger.debug("Executor task id: {}".format(task.executor_id))
+            logger.debug("Executor task id: {}".format(task.id))
 
             # Specify input/output files that need to be staged.
             # Absolute paths are assumed to be in shared filesystem, and thus
             # not staged by taskvine.
             # Files that share the same local path are assumed to be the same
             # and thus use the same Vine File object if detected.
-            if not manager_config.shared_fs:
+            if not shared_fs:
                 for spec in task.input_files:
                     if spec.stage:
                         if spec.parsl_name in parsl_file_name_to_vine_file:
                             task_in_file = parsl_file_name_to_vine_file[spec.parsl_name]
                         else:
                             task_in_file = m.declare_file(spec.parsl_name, cache=spec.cache, peer_transfer=True)
                             parsl_file_name_to_vine_file[spec.parsl_name] = task_in_file
@@ -876,80 +943,74 @@
                         if spec.parsl_name in parsl_file_name_to_vine_file:
                             task_out_file = parsl_file_name_to_vine_file[spec.parsl_name]
                         else:
                             task_out_file = m.declare_file(spec.parsl_name, cache=spec.cache, peer_transfer=True)
                         t.add_output(task_out_file, spec.parsl_name)
 
             # Submit the task to the TaskVine object
-            logger.debug("Submitting executor task {}, {} to TaskVine".format(task.executor_id, t))
+            logger.debug("Submitting executor task {} to TaskVine".format(task.id))
             try:
                 vine_id = m.submit(t)
-                logger.debug("Submitted executor task {} to TaskVine".format(task.executor_id))
-                vine_id_to_executor_task_id[str(vine_id)] = str(task.executor_id), task.exec_mode
+                vine_id_to_executor_task_id[str(vine_id)] = str(task.id)
             except Exception as e:
                 logger.error("Unable to submit task to taskvine: {}".format(e))
-                finished_task_queue.put_nowait(VineTaskToParsl(executor_id=task.executor_id,
-                                                               result_received=False,
-                                                               result=None,
-                                                               reason="task could not be submited to taskvine",
-                                                               status=-1))
+                collector_queue.put_nowait(VineTaskToParsl(id=task.id,
+                                                           result_received=False,
+                                                           result=None,
+                                                           reason="task could not be submited to taskvine",
+                                                           status=-1))
                 continue
-
-            logger.debug("Executor task {} submitted as TaskVine task with id {}".format(task.executor_id, vine_id))
+            logger.info("Executor task {} submitted as TaskVine task with id {}".format(task.id, vine_id))
 
         # If the queue is not empty wait on the TaskVine queue for a task
         task_found = True
         if not m.empty():
             while task_found and not should_stop.value:
                 # Obtain the task from the queue
                 t = m.wait(1)
                 if t is None:
                     task_found = False
                     continue
-                logger.debug('Found a task')
-                executor_task_id = vine_id_to_executor_task_id[str(t.id)][0]
-                exec_mode_of_task = vine_id_to_executor_task_id[str(t.id)][1]
+                # When a task is found:
+                executor_task_id = vine_id_to_executor_task_id[str(t.id)]
+                logger.debug("Completed TaskVine task {}, executor task {}".format(t.id, executor_task_id))
+                result_file = result_file_of_task_id.pop(executor_task_id)
                 vine_id_to_executor_task_id.pop(str(t.id))
-                # When a task is found
-                if exec_mode_of_task == 'regular':
-                    result_file = result_file_of_task_id.pop(executor_task_id)
-
-                    logger.debug(f"completed executor task info: {executor_task_id}, {t.category}, {t.command}, {t.std_output}")
-
-                    # A tasks completes 'succesfully' if it has result file,
-                    # and it can be loaded. This may mean that the 'success' is
-                    # an exception.
-                    logger.debug("Looking for result in {}".format(result_file))
-                    try:
-                        with open(result_file, "rb") as f_in:
-                            result = pickle.load(f_in)
-                        logger.debug("Found result in {}".format(result_file))
-                        finished_task_queue.put_nowait(VineTaskToParsl(executor_id=executor_task_id,
-                                                                       result_received=True,
-                                                                       result=result,
-                                                                       reason=None,
-                                                                       status=t.exit_code))
-                    # If a result file could not be generated, explain the
-                    # failure according to taskvine error codes. We generate
-                    # an exception and wrap it with RemoteExceptionWrapper, to
-                    # match the positive case.
-                    except Exception as e:
-                        reason = _explain_taskvine_result(t)
-                        logger.debug("Did not find result in {}".format(result_file))
-                        logger.debug("Wrapper Script status: {}\nTaskVine Status: {}"
-                                     .format(t.exit_code, t.result))
-                        logger.debug("Task with executor id {} / vine id {} failed because:\n{}"
-                                     .format(executor_task_id, t.id, reason))
-                        finished_task_queue.put_nowait(VineTaskToParsl(executor_id=executor_task_id,
-                                                                       result_received=False,
-                                                                       result=e,
-                                                                       reason=reason,
-                                                                       status=t.exit_code))
-                else:
-                    raise Exception(f'Unknown exec mode for executor task {executor_task_id}: {exec_mode_of_task}.')
+
+                logger.debug(f"completed executor task info: {executor_task_id}, {t.category}, {t.command}, {t.std_output}")
+
+                # A tasks completes 'succesfully' if it has result file,
+                # and it can be loaded. This may mean that the 'success' is
+                # an exception.
+                logger.debug("Looking for result in {}".format(result_file))
+                try:
+                    with open(result_file, "rb") as f_in:
+                        result = pickle.load(f_in)
+                    logger.debug("Found result in {}".format(result_file))
+                    collector_queue.put_nowait(VineTaskToParsl(id=executor_task_id,
+                                                               result_received=True,
+                                                               result=result,
+                                                               reason=None,
+                                                               status=t.exit_code))
+                # If a result file could not be generated, explain the
+                # failure according to taskvine error codes. We generate
+                # an exception and wrap it with RemoteExceptionWrapper, to
+                # match the positive case.
+                except Exception as e:
+                    reason = _explain_taskvine_result(t)
+                    logger.debug("Did not find result in {}".format(result_file))
+                    logger.debug("Wrapper Script status: {}\nTaskVine Status: {}"
+                                 .format(t.exit_code, t.result))
+                    logger.debug("Task with executor id {} / vine id {} failed because:\n{}"
+                                 .format(executor_task_id, t.id, reason))
+                    collector_queue.put_nowait(VineTaskToParsl(id=executor_task_id,
+                                                               result_received=False,
+                                                               result=e,
+                                                               reason=reason,
+                                                               status=t.exit_code))
 
     logger.debug("Exiting TaskVine Monitoring Process")
     return 0
 
 
 def _explain_taskvine_result(vine_task):
     """Returns a string with the reason why a task failed according to taskvine."""
@@ -988,62 +1049,7 @@
         reason += "task failed because output transfer fails"
     elif vine_result == cvine.VINE_RESULT_FIXED_LOCATION_MISSING:
         reason += "task failed because no worker could satisfy the fixed \n"
         reason += "location input file requirements"
     else:
         reason += "unable to process TaskVine system failure"
     return reason
-
-
-@wrap_with_logs
-def _taskvine_factory(should_stop, factory_config):
-    logger.debug("Starting TaskVine factory process")
-
-    try:
-        # create the factory according to the project name if given
-        if factory_config._project_name:
-            factory = Factory(batch_type=factory_config.batch_type,
-                              manager_name=factory_config._project_name,
-                              )
-        else:
-            factory = Factory(batch_type=factory_config.batch_type,
-                              manager_host_port=f"{factory_config._project_address}:{factory_config._project_port}",
-                             )
-    except Exception as e:
-        raise TaskVineFactoryFailure(f'Cannot create factory with exception {e}')
-
-    # Set attributes of this factory
-    if factory_config._project_password_file:
-        factory.password = factory_config._project_password_file
-    factory.factory_timeout = factory_config.factory_timeout
-    factory.scratch_dir = factory_config.scratch_dir
-    factory.min_workers = factory_config.min_workers
-    factory.max_workers = factory_config.max_workers
-    factory.workers_per_cycle = factory_config.workers_per_cycle
-
-    if factory_config.worker_options:
-        factory.extra_options = factory_config.worker_options
-    factory.timeout = factory_config.worker_timeout
-    if factory_config.cores:
-        factory.cores = factory_config.cores
-    if factory_config.gpus:
-        factory.gpus = factory_config.gpus
-    if factory_config.memory:
-        factory.memory = factory_config.memory
-    if factory_config.disk:
-        factory.disk = factory_config.disk
-    if factory_config.python_env:
-        factory.python_env = factory_config.python_env
-
-    if factory_config.condor_requirements:
-        factory.condor_requirements = factory_config.condor_requirements
-    if factory_config.batch_options:
-        factory.batch_options = factory_config.batch_options
-
-    # setup factory context and sleep for a second in every loop to
-    # avoid wasting CPU
-    with factory:
-        while not should_stop.value:
-            time.sleep(1)
-
-    logger.debug("Exiting TaskVine factory process")
-    return 0
```

### Comparing `parsl-2023.7.24/parsl/executors/threads.py` & `parsl-2023.7.3/parsl/executors/threads.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,16 +50,17 @@
 
         This method is simply pass through and behaves like a submit call as described
         here `Python docs: <https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor>`_
 
         """
         if resource_specification:
             logger.error("Ignoring the resource specification. "
-                         "Parsl resource specification is not supported in ThreadPool Executor.")
-            raise UnsupportedFeatureError('resource specification', 'ThreadPool Executor', None)
+                         "Parsl resource specification is not supported in ThreadPool Executor. "
+                         "Please check WorkQueue Executor if resource specification is needed.")
+            raise UnsupportedFeatureError('resource specification', 'ThreadPool Executor', 'WorkQueue Executor')
 
         return self.executor.submit(func, *args, **kwargs)
 
     def scale_out(self, workers=1):
         """Scales out the number of active workers by 1.
 
         This method is notImplemented for threads and will raise the error if called.
```

### Comparing `parsl-2023.7.24/parsl/executors/workqueue/exec_parsl_function.py` & `parsl-2023.7.3/parsl/executors/workqueue/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/executors/workqueue/executor.py` & `parsl-2023.7.3/parsl/executors/workqueue/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,23 +392,23 @@
         memory = None
         disk = None
         gpus = None
         priority = None
         category = None
         running_time_min = None
         if resource_specification and isinstance(resource_specification, dict):
-            logger.debug("Got resource_specification: {}".format(resource_specification))
+            logger.debug("Got resource specification: {}".format(resource_specification))
 
             required_resource_types = set(['cores', 'memory', 'disk'])
-            acceptable_fields = set(['cores', 'memory', 'disk', 'gpus', 'priority', 'running_time_min'])
+            acceptable_resource_types = set(['cores', 'memory', 'disk', 'gpus', 'priority', 'running_time_min'])
             keys = set(resource_specification.keys())
 
-            if not keys.issubset(acceptable_fields):
+            if not keys.issubset(acceptable_resource_types):
                 message = "Task resource specification only accepts these types of resources: {}".format(
-                        ', '.join(acceptable_fields))
+                        ', '.join(acceptable_resource_types))
                 logger.error(message)
                 raise ExecutorError(self, message)
 
             # this checks that either all of the required resource types are specified, or
             # that none of them are: the `required_resource_types` are not actually required,
             # but if one is specified, then they all must be.
             key_check = required_resource_types.intersection(keys)
```

### Comparing `parsl-2023.7.24/parsl/executors/workqueue/parsl_coprocess.py` & `parsl-2023.7.3/parsl/executors/workqueue/parsl_coprocess.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/executors/workqueue/parsl_coprocess_stub.py` & `parsl-2023.7.3/parsl/executors/workqueue/parsl_coprocess_stub.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/jobs/job_error_handler.py` & `parsl-2023.7.3/parsl/dataflow/job_error_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-from __future__ import annotations
-
 from typing import List, Dict
 
-import parsl.jobs.job_status_poller as jsp
-
+from parsl.dataflow.executor_status import ExecutorStatus
 from parsl.executors.base import ParslExecutor
-from parsl.jobs.states import JobStatus, JobState
+from parsl.providers.base import JobStatus, JobState
 
 
 class JobErrorHandler:
-    def run(self, status: List[jsp.PollItem]):
+    def run(self, status: List[ExecutorStatus]):
         for es in status:
             self._check_irrecoverable_executor(es)
 
-    def _check_irrecoverable_executor(self, es: jsp.PollItem):
+    def _check_irrecoverable_executor(self, es: ExecutorStatus):
         if not es.executor.error_management_enabled:
             return
         es.executor.handle_errors(self, es.status)
 
     def simple_error_handler(self, executor: ParslExecutor, status: Dict[str, JobStatus], threshold: int):
         (total_jobs, failed_jobs) = self.count_jobs(status)
         if total_jobs >= threshold and failed_jobs == total_jobs:
```

### Comparing `parsl-2023.7.24/parsl/jobs/job_status_poller.py` & `parsl-2023.7.3/parsl/dataflow/job_status_poller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import logging
 import parsl  # noqa F401 (used in string type annotation)
 import time
 import zmq
 from typing import Dict, Sequence
 from typing import List  # noqa F401 (used in type annotation)
 
+from parsl.dataflow.executor_status import ExecutorStatus
+from parsl.dataflow.job_error_handler import JobErrorHandler
+from parsl.dataflow.strategy import Strategy
 from parsl.executors.base import ParslExecutor
-from parsl.jobs.job_error_handler import JobErrorHandler
-from parsl.jobs.states import JobStatus, JobState
-from parsl.jobs.strategy import Strategy
 from parsl.monitoring.message_type import MessageType
 
+from parsl.providers.base import JobStatus, JobState
 
 from parsl.utils import Timer
 
-
 logger = logging.getLogger(__name__)
 
 
-class PollItem:
+class PollItem(ExecutorStatus):
     def __init__(self, executor: ParslExecutor, dfk: "parsl.dataflow.dflow.DataFlowKernel"):
         self._executor = executor
         self._dfk = dfk
         self._interval = executor.status_polling_interval
         self._last_poll_time = 0.0
         self._status = {}  # type: Dict[str, JobStatus]
```

### Comparing `parsl-2023.7.24/parsl/jobs/strategy.py` & `parsl-2023.7.3/parsl/dataflow/strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from __future__ import annotations
 import logging
 import time
 import math
 import warnings
 from typing import Dict, List, Optional
 
-import parsl.jobs.job_status_poller as jsp
-
+from parsl.dataflow.executor_status import ExecutorStatus
 from parsl.executors import HighThroughputExecutor
 from parsl.executors.base import ParslExecutor
 from parsl.executors.status_handling import BlockProviderExecutor
-from parsl.jobs.states import JobState
+from parsl.providers.base import JobState
 from parsl.process_loggers import wrap_with_logs
 
 
 logger = logging.getLogger(__name__)
 
 
 class Strategy:
@@ -132,15 +130,15 @@
 
         logger.debug("Scaling strategy: {0}".format(strategy))
 
     def add_executors(self, executors):
         for executor in executors:
             self.executors[executor.label] = {'idle_since': None}
 
-    def _strategy_noop(self, status: List[jsp.PollItem]) -> None:
+    def _strategy_noop(self, status: List[ExecutorStatus]) -> None:
         """Do nothing.
         """
         logger.debug("strategy_noop: doing nothing")
 
     def _strategy_simple(self, status_list) -> None:
         self._general_strategy(status_list, strategy_type='simple')
```

### Comparing `parsl-2023.7.24/parsl/launchers/__init__.py` & `parsl-2023.7.3/parsl/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/launchers/base.py` & `parsl-2023.7.3/parsl/launchers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/launchers/launchers.py` & `parsl-2023.7.3/parsl/launchers/launchers.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/log_utils.py` & `parsl-2023.7.3/parsl/log_utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/db_manager.py` & `parsl-2023.7.3/parsl/monitoring/db_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/monitoring.py` & `parsl-2023.7.3/parsl/monitoring/monitoring.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 from parsl.process_loggers import wrap_with_logs
 from parsl.utils import setproctitle
 
 from parsl.serialize import deserialize
 
 from parsl.monitoring.message_type import MessageType
 from parsl.monitoring.types import AddressedMonitoringMessage, TaggedMonitoringMessage
-from typing import cast, Any, Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import cast, Any, Callable, Dict, Optional, Sequence, Union
 
 _db_manager_excepts: Optional[Exception]
 
+from typing import Optional, Tuple
+
 
 try:
     from parsl.monitoring.db_manager import dbm_starter
 except Exception as e:
     _db_manager_excepts = e
 else:
     _db_manager_excepts = None
```

### Comparing `parsl-2023.7.24/parsl/monitoring/queries/pandas.py` & `parsl-2023.7.3/parsl/monitoring/queries/pandas.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/radios.py` & `parsl-2023.7.3/parsl/monitoring/radios.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/remote.py` & `parsl-2023.7.3/parsl/monitoring/remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/types.py` & `parsl-2023.7.3/parsl/monitoring/types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/visualization/app.py` & `parsl-2023.7.3/parsl/monitoring/visualization/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/visualization/models.py` & `parsl-2023.7.3/parsl/monitoring/visualization/models.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/visualization/plots/default/task_plots.py` & `parsl-2023.7.3/parsl/monitoring/visualization/plots/default/task_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/visualization/plots/default/workflow_plots.py` & `parsl-2023.7.3/parsl/monitoring/visualization/plots/default/workflow_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py` & `parsl-2023.7.3/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/visualization/static/parsl-logo-white.png` & `parsl-2023.7.3/parsl/monitoring/visualization/static/parsl-logo-white.png`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/visualization/templates/app.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/app.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/visualization/templates/dag.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/dag.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/visualization/templates/layout.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/layout.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/visualization/templates/resource_usage.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/resource_usage.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/visualization/templates/task.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/task.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/visualization/templates/workflow.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/workflow.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/visualization/templates/workflows_summary.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/workflows_summary.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/monitoring/visualization/views.py` & `parsl-2023.7.3/parsl/monitoring/visualization/views.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/multiprocessing.py` & `parsl-2023.7.3/parsl/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/process_loggers.py` & `parsl-2023.7.3/parsl/process_loggers.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/providers/__init__.py` & `parsl-2023.7.3/parsl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/providers/ad_hoc/ad_hoc.py` & `parsl-2023.7.3/parsl/providers/ad_hoc/ad_hoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import os
 import time
 
 from parsl.channels import LocalChannel
-from parsl.jobs.states import JobStatus, JobState
 from parsl.launchers import SimpleLauncher
-from parsl.providers.base import ExecutionProvider
+from parsl.providers.base import ExecutionProvider, JobStatus, JobState
 from parsl.providers.errors import ScriptPathError
 from parsl.utils import RepresentationMixin
 
 logger = logging.getLogger(__name__)
 
 
 class AdHocProvider(ExecutionProvider, RepresentationMixin):
```

### Comparing `parsl-2023.7.24/parsl/providers/aws/aws.py` & `parsl-2023.7.3/parsl/providers/aws/aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
 import logging
 import os
 import time
 from string import Template
 
 from parsl.errors import ConfigurationError
-from parsl.jobs.states import JobState, JobStatus
 from parsl.providers.aws.template import template_string
-from parsl.providers.base import ExecutionProvider
+from parsl.providers.base import ExecutionProvider, JobState, JobStatus
 from parsl.errors import OptionalModuleMissing
 from parsl.utils import RepresentationMixin
 from parsl.launchers import SingleNodeLauncher
 
 logger = logging.getLogger(__name__)
 
 try:
```

### Comparing `parsl-2023.7.24/parsl/providers/azure/azure.py` & `parsl-2023.7.3/parsl/providers/azure/azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
 import logging
 import os
 import time
 from string import Template
 
 from parsl.errors import ConfigurationError
-from parsl.jobs.states import JobState, JobStatus
 from parsl.providers.azure.template import template_string
-from parsl.providers.base import ExecutionProvider
+from parsl.providers.base import ExecutionProvider, JobState, JobStatus
 from parsl.errors import OptionalModuleMissing
 from parsl.utils import RepresentationMixin
 from parsl.launchers import SingleNodeLauncher
 
 logger = logging.getLogger(__name__)
 
 try:
```

### Comparing `parsl-2023.7.24/parsl/providers/cluster_provider.py` & `parsl-2023.7.3/parsl/providers/cluster_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from abc import abstractmethod
 from string import Template
 
 from parsl.providers.errors import SchedulerMissingArgs, ScriptPathError
-from parsl.launchers.base import Launcher
 from parsl.launchers.errors import BadLauncher
 from parsl.providers.base import ExecutionProvider
 
 logger = logging.getLogger(__name__)
 
 
 class ClusterProvider(ExecutionProvider):
@@ -63,15 +62,15 @@
         self.init_blocks = init_blocks
         self.min_blocks = min_blocks
         self.max_blocks = max_blocks
         self.parallelism = parallelism
         self.launcher = launcher
         self.walltime = walltime
         self.cmd_timeout = cmd_timeout
-        if not isinstance(self.launcher, Launcher):
+        if not callable(self.launcher):
             raise BadLauncher(self.launcher)
 
         self.script_dir = None
 
         # Dictionary that keeps track of jobs, keyed on job_id
         self.resources = {}
```

### Comparing `parsl-2023.7.24/parsl/providers/cobalt/cobalt.py` & `parsl-2023.7.3/parsl/providers/cobalt/cobalt.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 
 from parsl.providers.errors import ScaleOutFailed
 from parsl.channels import LocalChannel
 from parsl.launchers import AprunLauncher
 from parsl.providers.cobalt.template import template_string
 from parsl.providers.cluster_provider import ClusterProvider
-from parsl.jobs.states import JobState, JobStatus
+from parsl.providers.base import JobState, JobStatus
 from parsl.utils import RepresentationMixin, wtime_to_minutes
 
 logger = logging.getLogger(__name__)
 
 translate_table = {
     'QUEUED': JobState.PENDING,
     'STARTING': JobState.PENDING,
```

### Comparing `parsl-2023.7.24/parsl/providers/condor/condor.py` & `parsl-2023.7.3/parsl/providers/condor/condor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
 import re
 import time
 import typeguard
 
 from parsl.channels import LocalChannel
-from parsl.jobs.states import JobState, JobStatus
+from parsl.providers.base import JobState, JobStatus
 from parsl.utils import RepresentationMixin
 from parsl.launchers import SingleNodeLauncher
 from parsl.launchers.base import Launcher
 from parsl.providers.condor.template import template_string
 from parsl.providers.cluster_provider import ClusterProvider
 from parsl.providers.errors import ScaleOutFailed
```

### Comparing `parsl-2023.7.24/parsl/providers/condor/template.py` & `parsl-2023.7.3/parsl/providers/condor/template.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/providers/errors.py` & `parsl-2023.7.3/parsl/providers/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/providers/googlecloud/googlecloud.py` & `parsl-2023.7.3/parsl/providers/googlecloud/googlecloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import atexit
 import logging
 import os
 from parsl.launchers import SingleNodeLauncher
-from parsl.jobs.states import JobState, JobStatus
+from parsl.providers.base import JobState, JobStatus
 
 logger = logging.getLogger(__name__)
 
 try:
     import googleapiclient.discovery
 
 except ImportError:
```

### Comparing `parsl-2023.7.24/parsl/providers/grid_engine/grid_engine.py` & `parsl-2023.7.3/parsl/providers/grid_engine/grid_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import time
 
 from parsl.channels import LocalChannel
 from parsl.providers.cluster_provider import ClusterProvider
 from parsl.providers.grid_engine.template import template_string
 from parsl.launchers import SingleNodeLauncher
-from parsl.jobs.states import JobState, JobStatus
+from parsl.providers.base import JobState, JobStatus
 from parsl.utils import RepresentationMixin
 
 logger = logging.getLogger(__name__)
 
 translate_table = {
     'qw': JobState.PENDING,
     'hqw': JobState.PENDING,
```

### Comparing `parsl-2023.7.24/parsl/providers/kubernetes/kube.py` & `parsl-2023.7.3/parsl/providers/kubernetes/kube.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 import time
 from parsl.providers.kubernetes.template import template_string
 
 logger = logging.getLogger(__name__)
 
 from parsl.errors import OptionalModuleMissing
-from parsl.jobs.states import JobState, JobStatus
-from parsl.providers.base import ExecutionProvider
+from parsl.providers.base import ExecutionProvider, JobState, JobStatus
 from parsl.utils import RepresentationMixin
 
 import typeguard
 from typing import Any, Dict, List, Optional, Tuple
 
 try:
     from kubernetes import client, config
```

### Comparing `parsl-2023.7.24/parsl/providers/local/local.py` & `parsl-2023.7.3/parsl/providers/local/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import os
 import time
 
 from parsl.channels import LocalChannel
-from parsl.jobs.states import JobState, JobStatus
 from parsl.launchers import SingleNodeLauncher
-from parsl.providers.base import ExecutionProvider
+from parsl.providers.base import ExecutionProvider, JobState, JobStatus
 from parsl.providers.errors import SchedulerMissingArgs, ScriptPathError, SubmitException
 from parsl.utils import RepresentationMixin
 
 logger = logging.getLogger(__name__)
 
 
 class LocalProvider(ExecutionProvider, RepresentationMixin):
@@ -211,15 +210,15 @@
 
         job_id = None
         remote_pid = None
         if self._should_move_files():
             logger.debug("Pushing start script")
             script_path = self.channel.push_file(script_path, self.channel.script_dir)
 
-        logger.debug("Launching")
+        logger.debug("Launching in remote mode")
         # We need to capture the exit code and the streams, so we put them in files. We also write
         # '-' to the exit code file to isolate potential problems with writing to files in the
         # script directory
         #
         # The basic flow is:
         #   1. write "-" to the exit code file. If this fails, exit
         #   2. Launch the following sequence in the background:
```

### Comparing `parsl-2023.7.24/parsl/providers/lsf/lsf.py` & `parsl-2023.7.3/parsl/providers/lsf/lsf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import time
 import logging
 import math
 
 from parsl.channels import LocalChannel
-from parsl.jobs.states import JobState, JobStatus
 from parsl.launchers import SingleNodeLauncher
 from parsl.providers.cluster_provider import ClusterProvider
 from parsl.providers.lsf.template import template_string
+from parsl.providers.base import JobState, JobStatus
 from parsl.utils import RepresentationMixin, wtime_to_minutes
 
 logger = logging.getLogger(__name__)
 
 translate_table = {
     'PEND': JobState.PENDING,
     'RUN': JobState.RUNNING,
```

### Comparing `parsl-2023.7.24/parsl/providers/pbspro/pbspro.py` & `parsl-2023.7.3/parsl/providers/pbspro/pbspro.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import os
 import time
 import json
 
 from parsl.channels import LocalChannel
-from parsl.jobs.states import JobState, JobStatus
 from parsl.launchers import SingleNodeLauncher
 from parsl.providers.pbspro.template import template_string
 from parsl.providers import TorqueProvider
+from parsl.providers.base import JobState, JobStatus
 
 from parsl.providers.torque.torque import translate_table
 
 logger = logging.getLogger(__name__)
 
 
 class PBSProProvider(TorqueProvider):
```

### Comparing `parsl-2023.7.24/parsl/providers/slurm/slurm.py` & `parsl-2023.7.3/parsl/providers/slurm/slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import re
 import typeguard
 
 from typing import Optional
 
 from parsl.channels import LocalChannel
 from parsl.channels.base import Channel
-from parsl.jobs.states import JobState, JobStatus
 from parsl.launchers import SingleNodeLauncher
 from parsl.launchers.base import Launcher
 from parsl.providers.cluster_provider import ClusterProvider
+from parsl.providers.base import JobState, JobStatus
 from parsl.providers.slurm.template import template_string
 from parsl.utils import RepresentationMixin, wtime_to_minutes
 
 logger = logging.getLogger(__name__)
 
 translate_table = {
     'PD': JobState.PENDING,
```

### Comparing `parsl-2023.7.24/parsl/providers/torque/torque.py` & `parsl-2023.7.3/parsl/providers/torque/torque.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 import time
 
 from parsl.channels import LocalChannel
-from parsl.jobs.states import JobState, JobStatus
 from parsl.launchers import AprunLauncher
+from parsl.providers.base import JobState, JobStatus
 from parsl.providers.torque.template import template_string
 from parsl.providers.cluster_provider import ClusterProvider
 from parsl.utils import RepresentationMixin
 
 logger = logging.getLogger(__name__)
 
 # From the man pages for qstat for PBS/Torque systems
```

### Comparing `parsl-2023.7.24/parsl/serialize/concretes.py` & `parsl-2023.7.3/parsl/serialize/concretes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import dill
-import functools
 import pickle
 import logging
 
 logger = logging.getLogger(__name__)
 from parsl.serialize.base import SerializerBase
 
 from typing import Any
@@ -11,17 +10,20 @@
 
 class PickleSerializer(SerializerBase):
     """ Pickle serialization covers most python objects, with some notable exceptions:
 
     * functions defined in a interpreter/notebook
     * classes defined in local context and not importable using a fully qualified name
     * closures, generators and coroutines
+    * [sometimes] issues with wrapped/decorated functions
     """
 
     _identifier = b'01'
+    _for_code = True
+    _for_data = True
 
     def serialize(self, data: Any) -> bytes:
         return pickle.dumps(data)
 
     def deserialize(self, body: bytes) -> Any:
         return pickle.loads(body)
 
@@ -35,30 +37,15 @@
     * functions defined in a interpreter/notebook
     * classes defined in local context and not importable using a fully qualified name
     * functions that are wrapped/decorated by other functions/classes
     * closures
     """
 
     _identifier = b'02'
+    _for_code = True
+    _for_data = True
 
     def serialize(self, data: Any) -> bytes:
         return dill.dumps(data)
 
     def deserialize(self, body: bytes) -> Any:
         return dill.loads(body)
-
-
-class DillCallableSerializer(SerializerBase):
-    """This serializer is a variant of the DillSerializer that will
-    serialize and deserialize callables using an lru_cache, under the
-    assumption that callables are immutable and so can be cached.
-    """
-
-    _identifier = b'C2'
-
-    @functools.lru_cache
-    def serialize(self, data: Any) -> bytes:
-        return dill.dumps(data)
-
-    @functools.lru_cache
-    def deserialize(self, body: bytes) -> Any:
-        return dill.loads(body)
```

### Comparing `parsl-2023.7.24/parsl/serialize/facade.py` & `parsl-2023.7.3/parsl/serialize/facade.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,31 @@
+from parsl.serialize.concretes import *  # noqa: F403,F401
+from parsl.serialize.base import METHODS_MAP_DATA, METHODS_MAP_CODE, SerializerBase
 import logging
-from typing import Any, Dict, List, Union
 
-import parsl.serialize.concretes as concretes
-from parsl.serialize.base import SerializerBase
+from typing import Any, Dict, List, Tuple, Union
 
 logger = logging.getLogger(__name__)
 
 
-methods_for_code: Dict[bytes, SerializerBase] = {}
+""" Instantiate the appropriate classes
+"""
+methods_for_code = {}
+methods_for_data = {}
 
+for key in METHODS_MAP_CODE:
+    methods_for_code[key] = METHODS_MAP_CODE[key]()
+    methods_for_code[key].enable_caching(maxsize=128)
 
-def register_method_for_code(s: SerializerBase) -> None:
-    methods_for_code[s.identifier] = s
+for key in METHODS_MAP_DATA:
+    methods_for_data[key] = METHODS_MAP_DATA[key]()
 
 
-register_method_for_code(concretes.DillCallableSerializer())
-
-
-methods_for_data: Dict[bytes, SerializerBase] = {}
-
-
-def register_method_for_data(s: SerializerBase) -> None:
-    methods_for_data[s.identifier] = s
-
-
-register_method_for_data(concretes.PickleSerializer())
-register_method_for_data(concretes.DillSerializer())
+def _list_methods() -> Tuple[Dict[bytes, SerializerBase], Dict[bytes, SerializerBase]]:
+    return methods_for_code, methods_for_data
 
 
 def pack_apply_message(func: Any, args: Any, kwargs: Any, buffer_threshold: int = int(128 * 1e6)) -> bytes:
     """Serialize and pack function and parameters
 
     Parameters
     ----------
@@ -65,26 +61,31 @@
     """ Try available serialization methods one at a time
 
     Individual serialization methods might raise a TypeError (eg. if objects are non serializable)
     This method will raise the exception from the last method that was tried, if all methods fail.
     """
     result: Union[bytes, Exception]
     if callable(obj):
-        methods = methods_for_code
+        for method in methods_for_code.values():
+            try:
+                result = method._identifier + b'\n' + method.serialize(obj)
+            except Exception as e:
+                result = e
+                continue
+            else:
+                break
     else:
-        methods = methods_for_data
-
-    for method in methods.values():
-        try:
-            result = method._identifier + b'\n' + method.serialize(obj)
-        except Exception as e:
-            result = e
-            continue
-        else:
-            break
+        for method in methods_for_data.values():
+            try:
+                result = method._identifier + b'\n' + method.serialize(obj)
+            except Exception as e:
+                result = e
+                continue
+            else:
+                break
 
     if isinstance(result, BaseException):
         raise result
     else:
         if len(result) > buffer_threshold:
             logger.warning(f"Serialized object exceeds buffer threshold of {buffer_threshold} bytes, this could cause overflows")
         return result
```

### Comparing `parsl-2023.7.24/parsl/tests/configs/ad_hoc_cluster_htex.py` & `parsl-2023.7.3/parsl/tests/configs/ad_hoc_cluster_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/azure_single_node.py` & `parsl-2023.7.3/parsl/tests/configs/azure_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/bluewaters.py` & `parsl-2023.7.3/parsl/tests/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/bridges.py` & `parsl-2023.7.3/parsl/tests/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/cc_in2p3.py` & `parsl-2023.7.3/parsl/tests/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/comet.py` & `parsl-2023.7.3/parsl/tests/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/cooley_htex.py` & `parsl-2023.7.3/parsl/tests/configs/cooley_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/ec2_single_node.py` & `parsl-2023.7.3/parsl/tests/configs/ec2_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/ec2_spot.py` & `parsl-2023.7.3/parsl/tests/configs/ec2_spot.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/frontera.py` & `parsl-2023.7.3/parsl/tests/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/htex_ad_hoc_cluster.py` & `parsl-2023.7.3/parsl/tests/configs/htex_ad_hoc_cluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/htex_local.py` & `parsl-2023.7.3/parsl/tests/configs/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/htex_local_alternate.py` & `parsl-2023.7.3/parsl/tests/configs/htex_local_alternate.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/htex_local_intask_staging.py` & `parsl-2023.7.3/parsl/tests/configs/htex_local_intask_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/htex_local_rsync_staging.py` & `parsl-2023.7.3/parsl/tests/configs/htex_local_rsync_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/local_threads_globus.py` & `parsl-2023.7.3/parsl/tests/configs/local_threads_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/midway.py` & `parsl-2023.7.3/parsl/tests/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/nscc_singapore.py` & `parsl-2023.7.3/parsl/tests/configs/nscc_singapore.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/osg_htex.py` & `parsl-2023.7.3/parsl/tests/configs/osg_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/petrelkube.py` & `parsl-2023.7.3/parsl/tests/configs/petrelkube.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/summit.py` & `parsl-2023.7.3/parsl/tests/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/swan_htex.py` & `parsl-2023.7.3/parsl/tests/configs/swan_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/theta.py` & `parsl-2023.7.3/parsl/tests/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/configs/user_opts.py` & `parsl-2023.7.3/parsl/tests/configs/user_opts.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/integration/latency.py` & `parsl-2023.7.3/parsl/tests/integration/latency.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/integration/test_channels/test_local_channel.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_local_channel.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/integration/test_channels/test_scp_1.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_scp_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/integration/test_channels/test_ssh_1.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/integration/test_channels/test_ssh_errors.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/integration/test_channels/test_ssh_file_transport.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_file_transport.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/integration/test_channels/test_ssh_interactive.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_interactive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/integration/test_stress/test_python_simple.py` & `parsl-2023.7.3/parsl/tests/integration/test_stress/test_python_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/integration/test_stress/test_python_threads.py` & `parsl-2023.7.3/parsl/tests/integration/test_stress/test_python_threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/manual_tests/htex_local.py` & `parsl-2023.7.3/parsl/tests/manual_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/manual_tests/test_ad_hoc_htex.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_ad_hoc_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/manual_tests/test_basic.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/manual_tests/test_log_filter.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_log_filter.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/manual_tests/test_memory_limits.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_memory_limits.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/manual_tests/test_regression_220.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_regression_220.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/manual_tests/test_udp_simple.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_udp_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/manual_tests/test_worker_count.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_worker_count.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/scaling_tests/htex_local.py` & `parsl-2023.7.3/parsl/tests/scaling_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/scaling_tests/test_scale.py` & `parsl-2023.7.3/parsl/tests/scaling_tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/scaling_tests/wqex_condor.py` & `parsl-2023.7.3/parsl/tests/scaling_tests/wqex_condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/scaling_tests/wqex_local.py` & `parsl-2023.7.3/parsl/tests/scaling_tests/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/site_tests/site_config_selector.py` & `parsl-2023.7.3/parsl/tests/site_tests/site_config_selector.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/site_tests/test_provider.py` & `parsl-2023.7.3/parsl/tests/site_tests/test_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import logging
 import pytest
 import parsl
 import time
 from parsl.app.app import python_app  # , bash_app
-from parsl.jobs.states import JobState
+from parsl.providers.base import JobState
 from parsl.tests.site_tests.site_config_selector import fresh_config
 
 logger = logging.getLogger(__name__)
 
 
 @python_app
 def platform(sleep=10, stdout=None):
```

### Comparing `parsl-2023.7.24/parsl/tests/site_tests/test_site.py` & `parsl-2023.7.3/parsl/tests/site_tests/test_site.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/sites/test_affinity.py` & `parsl-2023.7.3/parsl/tests/sites/test_affinity.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/sites/test_concurrent.py` & `parsl-2023.7.3/parsl/tests/sites/test_concurrent.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Tests of the interfaces to Python's concurrent library"""
+
 from pytest import mark, warns
 
 from parsl import Config, HighThroughputExecutor
 from parsl.concurrent import ParslPoolExecutor
 
 
 def f(x):
     return x + 1
 
 
 def make_config(run_dir):
     return Config(
         executors=[
             HighThroughputExecutor(
-                address="127.0.0.1",
                 max_workers=2,
-                heartbeat_period=2,
-                heartbeat_threshold=4,
             )
         ],
         strategy='none',
         run_dir=str(run_dir)
     )
```

### Comparing `parsl-2023.7.24/parsl/tests/sites/test_dynamic_executor.py` & `parsl-2023.7.3/parsl/tests/sites/test_dynamic_executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/sites/test_ec2.py` & `parsl-2023.7.3/parsl/tests/sites/test_ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/sites/test_local_adhoc.py` & `parsl-2023.7.3/parsl/tests/sites/test_local_adhoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/sites/test_start_method.py` & `parsl-2023.7.3/parsl/tests/sites/test_start_method.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/sites/test_worker_info.py` & `parsl-2023.7.3/parsl/tests/sites/test_worker_info.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_aalst_patterns.py` & `parsl-2023.7.3/parsl/tests/test_aalst_patterns.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_bash_apps/test_basic.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_basic.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,115 @@
+import argparse
 import os
+import pytest
+import shutil
+import time
 import random
 import re
 
-import pytest
-
 import parsl
 from parsl import File
 from parsl.app.app import bash_app
 
+from parsl.tests.configs.local_threads import config
+
 
 @bash_app
-def echo_to_file(inputs=(), outputs=(), stderr=None, stdout=None):
+def echo_to_file(inputs=[], outputs=[], stderr='std.err', stdout='std.out'):
     res = ""
-    for o in outputs:
-        for i in inputs:
+    for i in inputs:
+        for o in outputs:
             res += "echo {} >& {}".format(i, o)
     return res
 
 
 @bash_app
 def foo(x, y, z=10, stdout=None, label=None):
-    return f"echo {x} {y} {z}"
+    return """echo {0} {1} {z}
+    """.format(x, y, z=z)
 
 
 @pytest.mark.issue363
-def test_command_format_1(tmpd_cwd):
-    """Testing command format for BashApps"""
+def test_command_format_1():
+    """Testing command format for BashApps
+    """
 
-    outdir = tmpd_cwd / "outputs"
-    outdir.mkdir()
-    stdout = outdir / "foo-std.out"
+    outdir = os.path.abspath('outputs')
+    stdout = os.path.join(outdir, 'foo-std.out')
+    if os.path.exists(stdout):
+        os.remove(stdout)
+
+    foo_future = foo(1, 4, stdout=stdout)
+    print("[test_command_format_1] foo_future: ", foo_future)
+    contents = None
 
-    foo_future = foo(1, 4, stdout=str(stdout))
-    assert foo_future.result() == 0, "BashApp had non-zero exit code"
+    assert foo_future.result() == 0, "BashApp exited with an error code : {0}".format(
+        foo_future.result())
 
-    so_content = stdout.read_text().strip()
-    assert so_content == "1 4 10"
+    with open(stdout, 'r') as stdout_f:
+        contents = stdout_f.read()
+
+    assert contents == '1 4 10\n', 'Output does not match expected string "1 4 10", Got: "{0}"'.format(
+        contents)
+    return True
 
 
 @pytest.mark.issue363
 def test_auto_log_filename_format():
     """Testing auto log filename format for BashApps
     """
     app_label = "label_test_auto_log_filename_format"
     rand_int = random.randint(1000, 1000000000)
 
     foo_future = foo(1, rand_int, stdout=parsl.AUTO_LOGNAME, label=app_label)
+    print("[test_auto_log_filename_format] foo_future: ", foo_future)
+    contents = None
 
     assert foo_future.result() == 0, "BashApp exited with an error code : {0}".format(
         foo_future.result())
 
     log_fpath = foo_future.stdout
     log_pattern = fr".*/task_\d+_foo_{app_label}"
     assert re.match(log_pattern, log_fpath), 'Output file "{0}" does not match pattern "{1}"'.format(
         log_fpath, log_pattern)
     assert os.path.exists(log_fpath), 'Output file does not exist "{0}"'.format(log_fpath)
     with open(log_fpath, 'r') as stdout_f:
         contents = stdout_f.read()
 
     assert contents == '1 {0} 10\n'.format(rand_int), \
         'Output does not match expected string "1 {0} 10", Got: "{1}"'.format(rand_int, contents)
+    return True
 
 
 @pytest.mark.issue363
-def test_parallel_for(tmpd_cwd, n=3):
-    """Testing a simple parallel for loop"""
-    outdir = tmpd_cwd / "outputs/test_parallel"
-    outdir.mkdir(parents=True)
-    futs = [
-        echo_to_file(
-            inputs=[f"Hello World {i}"],
-            outputs=[File(str(outdir / f"out.{i}.txt"))],
-            stdout=str(outdir / f"std.{i}.out"),
-            stderr=str(outdir / f"std.{i}.err"),
+def test_parallel_for(n=3):
+    """Testing a simple parallel for loop
+    """
+    outdir = os.path.join(os.path.abspath('outputs'), 'test_parallel')
+    if not os.path.exists(outdir):
+        os.makedirs(outdir)
+    else:
+        shutil.rmtree(outdir)
+        os.makedirs(outdir)
+
+    d = {}
+
+    start = time.time()
+    for i in range(0, n):
+        d[i] = echo_to_file(
+            inputs=['Hello World {0}'.format(i)],
+            outputs=[File('{0}/out.{1}.txt'.format(outdir, i))],
+            stdout='{0}/std.{1}.out'.format(outdir, i),
+            stderr='{0}/std.{1}.err'.format(outdir, i),
         )
-        for i in range(n)
-    ]
 
-    for f in futs:
-        f.result()
+    assert len(
+        d.keys()) == n, "Only {0}/{1} keys in dict".format(len(d.keys()), n)
 
-    stdout_file_count = len(list(outdir.glob("*.out")))
-    assert stdout_file_count == n, sorted(outdir.iterdir())
+    [d[i].result() for i in d]
+    print("Duration : {0}s".format(time.time() - start))
+    stdout_file_count = len(
+        [item for item in os.listdir(outdir) if item.endswith('.out')])
+    assert stdout_file_count == n, "Only {0}/{1} files in '{2}' ".format(len(os.listdir('outputs/')),
+                                                                         n, outdir)
+    print("[TEST STATUS] test_parallel_for [SUCCESS]")
+    return d
```

### Comparing `parsl-2023.7.24/parsl/tests/test_bash_apps/test_error_codes.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_error_codes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_bash_apps/test_memoize_ignore_args.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_bash_apps/test_stdout.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_stdout.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import argparse
 import os
 
 import pytest
 
+import parsl
 import parsl.app.errors as perror
 from parsl.app.app import bash_app
+from parsl.tests.configs.local_threads import config
 
 
 @bash_app
-def echo_to_streams(msg, stderr=None, stdout=None):
+def echo_to_streams(msg, stderr='std.err', stdout='std.out'):
     return 'echo "{0}"; echo "{0}" >&2'.format(msg)
 
 
 whitelist = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'configs', '*threads*')
 
 speclist = (
     '/bad/dir/t.out',
@@ -33,68 +36,80 @@
     'bad_mode'
 ]
 
 
 @pytest.mark.issue363
 @pytest.mark.parametrize('spec', speclist, ids=testids)
 def test_bad_stdout_specs(spec):
-    """Testing bad stdout spec cases"""
+    """Testing bad stdout spec cases
+    """
 
     fn = echo_to_streams("Hello world", stdout=spec, stderr='t.err')
 
     try:
         fn.result()
     except Exception as e:
         assert isinstance(e, TypeError) or isinstance(e, perror.BadStdStreamFile), "Exception is wrong type"
     else:
         assert False, "Did not raise expected exception"
 
+    return
+
 
 @pytest.mark.issue363
 def test_bad_stderr_file():
-    """Testing bad stderr file"""
 
+    """ Testing bad stderr file """
+
+    out = "t2.out"
     err = "/bad/dir/t2.err"
 
-    fn = echo_to_streams("Hello world", stderr=err)
+    fn = echo_to_streams("Hello world", stdout=out, stderr=err)
 
     try:
         fn.result()
     except perror.BadStdStreamFile:
         pass
     else:
         assert False, "Did not raise expected exception BadStdStreamFile"
 
     return
 
 
 @pytest.mark.issue363
-def test_stdout_truncate(tmpd_cwd):
-    """Testing truncation of prior content of stdout"""
+def test_stdout_truncate():
+
+    """ Testing truncation of prior content of stdout """
 
-    out = (str(tmpd_cwd / 't1.out'), 'w')
-    err = str(tmpd_cwd / 't1.err')
+    out = ('t1.out', 'w')
+    err = 't1.err'
+    os.system('rm -f ' + out[0] + ' ' + err)
 
     echo_to_streams('hi', stdout=out, stderr=err).result()
     len1 = len(open(out[0]).readlines())
 
     echo_to_streams('hi', stdout=out, stderr=err).result()
     len2 = len(open(out[0]).readlines())
 
-    assert len1 == 1
-    assert len1 == len2
+    assert len1 == len2 == 1, "Line count of output files should both be 1, but: len1={} len2={}".format(len1, len2)
+
+    os.system('rm -f ' + out[0] + ' ' + err)
 
 
 @pytest.mark.issue363
-def test_stdout_append(tmpd_cwd):
-    """Testing appending to prior content of stdout (default open() mode)"""
+def test_stdout_append():
+
+    """ Testing appending to prior content of stdout (default open() mode) """
 
-    out = str(tmpd_cwd / 't1.out')
-    err = str(tmpd_cwd / 't1.err')
+    out = 't1.out'
+    err = 't1.err'
+    os.system('rm -f ' + out + ' ' + err)
 
     echo_to_streams('hi', stdout=out, stderr=err).result()
     len1 = len(open(out).readlines())
 
     echo_to_streams('hi', stdout=out, stderr=err).result()
     len2 = len(open(out).readlines())
 
-    assert len1 == 1 and len2 == 2
+    assert len1 == 1 and len2 == 2, "Line count of output files should be 1 and 2, but:  len1={} len2={}".format(len1, len2)
+
+    os.system('rm -f ' + out + ' ' + err)
```

### Comparing `parsl-2023.7.24/parsl/tests/test_callables.py` & `parsl-2023.7.3/parsl/tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_channels/test_large_output.py` & `parsl-2023.7.3/parsl/tests/test_channels/test_large_output.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_checkpointing/test_periodic.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_periodic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_checkpointing/test_python_checkpoint_1.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_checkpointing/test_python_checkpoint_2.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_checkpointing/test_python_checkpoint_3.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_checkpointing/test_regression_232.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_232.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_checkpointing/test_regression_233.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_233.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_checkpointing/test_regression_239.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_239.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_checkpointing/test_task_exit.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_task_exit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_data/test_file.py` & `parsl-2023.7.3/parsl/tests/test_data/test_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_data/test_file_apps.py` & `parsl-2023.7.3/parsl/tests/test_data/test_file_apps.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,51 +8,53 @@
 def cat(inputs=(), outputs=(), stdout=None, stderr=None):
     infiles = " ".join(i.filepath for i in inputs)
     return f"cat {infiles} &> {outputs[0]}"
 
 
 @pytest.mark.staging_required
 def test_files(setup_data):
-    fs = sorted(setup_data / f for f in setup_data.iterdir())
+    fs = sorted(str(setup_data / f) for f in setup_data.iterdir())
     fs = list(map(File, fs))
     x = cat(
         inputs=fs,
-        outputs=[File(setup_data / "cat_out.txt")],
-        stdout=setup_data / "f_app.out",
-        stderr=setup_data / "f_app.err",
+        outputs=[File(str(setup_data / "cat_out.txt"))],
+        stdout=str(setup_data / "f_app.out"),
+        stderr=str(setup_data / "f_app.err"),
     )
     x.result()
     d_x = x.outputs[0]
     data = open(d_x.filepath).read().strip()
     assert "1\n2" == data, "Per setup_data fixture"
 
 
 @bash_app
 def increment(inputs=(), outputs=(), stdout=None, stderr=None):
-    return (
-        f"x=$(cat {inputs[0]})\n"
-        f"echo $(($x+1)) > {outputs[0]}"
-    )
+    # Place double braces to avoid python complaining about missing keys for {item = $1}
+    return """
+    x=$(cat {i})
+    echo $(($x+1)) > {o}
+    """.format(i=inputs[0], o=outputs[0])
 
 
 @pytest.mark.staging_required
 def test_increment(tmp_path, depth=5):
-    """Test simple pipeline A->B...->N"""
+    """Test simple pipeline A->B...->N
+    """
     # Test setup
     first_fpath = tmp_path / "test0.txt"
     first_fpath.write_text("0\n")
 
-    prev = [File(first_fpath)]
+    prev = [File(str(first_fpath))]
     futs = []
     for i in range(1, depth):
         f = increment(
             inputs=prev,
-            outputs=[File(tmp_path / f"test{i}.txt")],
-            stdout=tmp_path / f"incr{i}.out",
-            stderr=tmp_path / f"incr{i}.err",
+            outputs=[File(str(tmp_path / f"test{i}.txt"))],
+            stdout=str(tmp_path / f"incr{i}.out"),
+            stderr=str(tmp_path / f"incr{i}.err"),
         )
         prev = f.outputs
         futs.append((i, prev[0]))
 
     for i, f in futs:
         data = open(f.result().filepath).read().strip()
         assert data == str(i)
```

### Comparing `parsl-2023.7.24/parsl/tests/test_data/test_file_staging.py` & `parsl-2023.7.3/parsl/tests/test_data/test_file_staging.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from parsl.app.app import bash_app
 from parsl.data_provider.files import File
 
 
 @bash_app
 def cat(inputs=(), outputs=(), stdout=None, stderr=None):
     infiles = " ".join(i.filepath for i in inputs)
-    return f"cat {infiles} &> {outputs[0]}"
+    return f"cat {infiles} &> {outputs[0]}\n"
 
 
 @pytest.mark.staging_required
 def test_regression_200(tmp_path):
     """Regression test for #200. Pickleablility of Files"""
     opath = tmp_path / "test_output.txt"
     fpath = tmp_path / "test.txt"
 
     fpath.write_text("Hello World")
-    f = cat(inputs=[File(fpath)], outputs=[File(opath)])
+    f = cat(inputs=[File(str(fpath))], outputs=[File(str(opath))])
 
     f.result()
     with open(f.outputs[0].filepath) as f:
         data = f.read()
         assert "Hello World" == data
```

### Comparing `parsl-2023.7.24/parsl/tests/test_data/test_output_chain_filenames.py` & `parsl-2023.7.3/parsl/tests/test_data/test_output_chain_filenames.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,46 @@
-from concurrent.futures import Future
+import argparse
+import os
+
+import pytest
+
+import parsl
 
+from concurrent.futures import Future
 from parsl import File
 from parsl.app.app import bash_app
 
 
 @bash_app
-def app1(inputs=(), outputs=(), stdout=None, stderr=None, mock=False):
-    return f"echo 'test' > {outputs[0]}"
+def app1(inputs=[], outputs=[], stdout=None, stderr=None, mock=False):
+    cmd_line = f"""echo 'test' > {outputs[0]}"""
+    return cmd_line
 
 
 @bash_app
-def app2(inputs=(), outputs=(), stdout=None, stderr=None, mock=False):
-    return f"echo '{inputs[0]}' > {outputs[0]}"
+def app2(inputs=[], outputs=[], stdout=None, stderr=None, mock=False):
+
+    with open('somefile.txt', 'w') as f:
+        f.write("%s\n" % inputs[0])
+    cmd_line = f"""echo '{inputs[0]}' > {outputs[0]}"""
+    return cmd_line
 
 
-def test_behavior(tmpd_cwd):
-    expected_path = str(tmpd_cwd / "simple-out.txt")
-    app1_future = app1(
-        inputs=[],
-        outputs=[File(expected_path)]
-    )
+def test_behavior():
+    app1_future = app1(inputs=[],
+                       outputs=[File("simple-out.txt")])
 
     o = app1_future.outputs[0]
     assert isinstance(o, Future)
 
-    app2_future = app2(
-        inputs=[o],
-        outputs=[File(str(tmpd_cwd / "simple-out2.txt"))]
-    )
+    app2_future = app2(inputs=[o],
+                       outputs=[File("simple-out2.txt")])
     app2_future.result()
 
+    expected_name = 'b'
+    with open('somefile.txt', 'r') as f:
+        name = f.read()
+
     with open(app2_future.outputs[0].filepath, 'r') as f:
-        name = f.read().strip()
+        expected_name = f.read()
 
-    assert name == expected_path, "Filename mangled due to DataFuture handling"
+    assert name == expected_name, "Filename mangled due to DataFuture handling"
```

### Comparing `parsl-2023.7.24/parsl/tests/test_docs/test_from_slides.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_from_slides.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_docs/test_tutorial_1.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_tutorial_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_docs/test_workflow1.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_workflow1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_docs/test_workflow2.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_workflow2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_docs/test_workflow3.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_workflow3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_docs/test_workflow4.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_workflow4.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,53 @@
-import pytest
+import os
+import parsl
 
 from parsl.app.app import bash_app, python_app
+from parsl.tests.configs.local_threads import config
 from parsl.data_provider.files import File
 
+import pytest
+
+# parsl.set_stream_logger()
+
 
 @bash_app
-def generate(outputs=()):
-    return "echo 1 &> {o}".format(o=outputs[0])
+def generate(outputs=[]):
+    return "echo $(( RANDOM % (10 - 5 + 1 ) + 5 )) &> {o}".format(o=outputs[0])
 
 
 @bash_app
-def concat(inputs=(), outputs=(), stdout=None, stderr=None):
+def concat(inputs=[], outputs=[], stdout="stdout.txt", stderr='stderr.txt'):
     return "cat {0} >> {1}".format(" ".join(map(lambda x: x.filepath, inputs)), outputs[0])
 
 
 @python_app
-def total(inputs=()):
-    with open(inputs[0].filepath, "r") as f:
-        return sum(int(line) for line in f)
+def total(inputs=[]):
+    total = 0
+    with open(inputs[0].filepath, 'r') as f:
+        for line in f:
+            total += int(line)
+    return total
 
 
 @pytest.mark.staging_required
-@pytest.mark.parametrize("width", (5, 10, 15))
-def test_parallel_dataflow(tmpd_cwd, width):
+def test_parallel_dataflow():
     """Test parallel dataflow from docs on Composing workflows
     """
 
+    if os.path.exists('all.txt'):
+        os.remove('all.txt')
+
     # create 5 files with random numbers
-    output_files = [
-        generate(outputs=[File(str(tmpd_cwd / f"random-{i}.txt"))])
-        for i in range(width)
-    ]
+    output_files = []
+    for i in range(5):
+        if os.path.exists('random-%s.txt' % i):
+            os.remove('random-%s.txt' % i)
+        output_files.append(generate(outputs=[File('random-%s.txt' % i)]))
 
     # concatenate the files into a single file
-    cc = concat(
-        inputs=[i.outputs[0] for i in output_files],
-        outputs=[File(str(tmpd_cwd / "all.txt"))]
-    )
+    cc = concat(inputs=[i.outputs[0]
+                        for i in output_files], outputs=[File("all.txt")])
 
     # calculate the average of the random numbers
     totals = total(inputs=[cc.outputs[0]])
-    assert totals.result() == len(output_files)
+    print(totals.result())
```

### Comparing `parsl-2023.7.24/parsl/tests/test_error_handling/test_htex_missing_worker.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_missing_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_error_handling/test_htex_worker_failure.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_worker_failure.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import pytest
 
+import parsl
 from parsl.app.app import python_app
+from parsl.tests.configs.htex_local import fresh_config
+
 from parsl.executors.high_throughput.errors import WorkerLost
 
 
-def local_config():
-    from parsl.tests.configs.htex_local import fresh_config
+def local_setup():
     config = fresh_config()
     config.executors[0].poll_period = 1
     config.executors[0].max_workers = 1
-    config.executors[0].heartbeat_period = 1
-    return config
+    parsl.load(config)
+
+
+def local_teardown():
+    parsl.dfk().cleanup()
+    parsl.clear()
 
 
 @python_app
 def kill_worker():
-    raise SystemExit(2)
+    import sys
+    sys.exit(2)
 
 
 @pytest.mark.local
 def test_htex_worker_failure():
     with pytest.raises(WorkerLost):
         f = kill_worker()
         f.result()
```

### Comparing `parsl-2023.7.24/parsl/tests/test_error_handling/test_python_walltime.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_python_walltime.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 import pytest
 
 import parsl
 from parsl.app.errors import AppTimeout
 
 
 @parsl.python_app
-def my_app(t=0.0, walltime=0.1):
+def my_app(t, walltime=1):
     import time
-    end = time.monotonic() + t
-    while time.monotonic() < end:
-        time.sleep(0.01)  # work with timeout(); allow access to thread
+    time.sleep(t)
     return 7
 
 
 def test_python_walltime():
     f = my_app(2)
     with pytest.raises(AppTimeout):
         f.result()
 
 
 def test_python_longer_walltime_at_invocation():
-    f = my_app(0.01, walltime=6)
+    f = my_app(1, walltime=6)
     assert f.result() == 7
 
 
 def test_python_walltime_wrapped_names():
-    f = my_app(0.01, walltime=6)
+    f = my_app(1, walltime=6)
     assert f.result() == 7
     assert f.task_def['func'].__name__ == "my_app"
     assert f.task_def['func_name'] == "my_app"
 
 
 def test_python_bad_decorator_args():
```

### Comparing `parsl-2023.7.24/parsl/tests/test_error_handling/test_rand_fail.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_rand_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_error_handling/test_resource_spec.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_error_handling/test_retries.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_retries.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_error_handling/test_retry_handler.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_retry_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_error_handling/test_retry_handler_failure.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_retry_handler_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_error_handling/test_serialization_fail.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_serialization_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_error_handling/test_wrap_with_logs.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_wrap_with_logs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_flux.py` & `parsl-2023.7.3/parsl/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_monitoring/test_basic.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_monitoring/test_db_locks.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_db_locks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_monitoring/test_fuzz_zmq.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_fuzz_zmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_monitoring/test_memoization_representation.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_memoization_representation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_monitoring/test_viz_colouring.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_viz_colouring.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_providers/test_local_provider.py` & `parsl-2023.7.3/parsl/tests/test_providers/test_local_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import socket
 import subprocess
 import tempfile
 import threading
 import time
 
 from parsl.channels import LocalChannel, SSHChannel
-from parsl.jobs.states import JobState
 from parsl.launchers import SingleNodeLauncher
 from parsl.providers import LocalProvider
+from parsl.providers.base import JobState
 
 logger = logging.getLogger(__name__)
 
 
 def _run_tests(p: LocalProvider):
     status = _run(p, '/bin/true')
     assert status.message is None
```

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_arg_input_types.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_arg_input_types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_basic.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_dep_standard_futures.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_dep_standard_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_depfail_propagation.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_depfail_propagation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_fibonacci_iterative.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_fibonacci_iterative.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_fibonacci_recursive.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_fibonacci_recursive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_futures.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_garbage_collect.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_garbage_collect.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,30 @@
-import threading
+import parsl
 import time
 
-import pytest
-
-import parsl
 from parsl.app.app import python_app
-from parsl.tests.configs.local_threads import fresh_config as local_config  # noqa
 
 
 @python_app
-def slow_double(x, may_continue: threading.Event):
-    may_continue.wait()
+def slow_double(x):
+    import time
+    time.sleep(0.1)
     return x * 2
 
 
-@pytest.mark.local
 def test_garbage_collect():
     """ Launches an app with a dependency and waits till it's done and asserts that
     the internal refs were wiped
     """
-    evt = threading.Event()
-    x = slow_double(10, evt)
-    x = slow_double(x, evt)
+    x = slow_double(slow_double(10))
 
-    assert parsl.dfk().tasks[x.tid]['app_fu'] == x, "Tasks table should have app_fu ref before done"
+    if x.done() is False:
+        assert parsl.dfk().tasks[x.tid]['app_fu'] == x, "Tasks table should have app_fu ref before done"
 
-    evt.set()
-    assert x.result() == 10 * 4
+    x.result()
     if parsl.dfk().checkpoint_mode is not None:
         # We explicit call checkpoint if checkpoint_mode is enabled covering
         # cases like manual/periodic where checkpointing may be deferred.
         parsl.dfk().checkpoint()
 
-    time.sleep(0.01)  # Give enough time for task wipes to work
+    time.sleep(0.2)  # Give enough time for task wipes to work
     assert x.tid not in parsl.dfk().tasks, "Task record should be wiped after task completion"
```

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_import_fail.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_import_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_join.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_join.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import pytest
+import time
 
 from parsl import join_app, python_app
 from parsl.dataflow.errors import JoinError
 
+from parsl.tests.configs.local_threads import fresh_config as local_config
 
 RESULT_CONSTANT = 3
 
 
-@python_app
+@python_app(cache=True)
 def inner_app():
+    time.sleep(1)
     return RESULT_CONSTANT
 
 
 @join_app
 def outer_app():
     fut = inner_app()
     return fut
@@ -27,25 +30,32 @@
 def combine(*args):
     """Wait for an arbitrary list of futures and return them as a list"""
     return list(args)
 
 
 @join_app
 def outer_make_a_dag_combine(n):
-    return combine(*(inner_app() for _ in range(n)))
+    futs = []
+    for _ in range(n):
+        futs.append(inner_app())
+    return combine(*futs)
 
 
 @join_app
 def outer_make_a_dag_multi(n):
-    return [inner_app() for _ in range(n)]
+    futs = []
+    for _ in range(n):
+        futs.append(inner_app())
+    return futs
 
 
 def test_result_flow():
     f = outer_app()
-    assert f.result() == RESULT_CONSTANT
+    res = f.result()
+    assert res == RESULT_CONSTANT
 
 
 @join_app
 def join_wrong_type_app():
     return 3
 
 
@@ -53,25 +63,28 @@
     f = join_wrong_type_app()
     with pytest.raises(TypeError):
         f.result()
 
 
 def test_dependency_on_joined():
     g = add_one(outer_app())
-    assert g.result() == RESULT_CONSTANT + 1
+    res = g.result()
+    assert res == RESULT_CONSTANT + 1
 
 
 def test_combine():
     f = outer_make_a_dag_combine(inner_app())
-    assert f.result() == [RESULT_CONSTANT] * RESULT_CONSTANT
+    res = f.result()
+    assert res == [RESULT_CONSTANT] * RESULT_CONSTANT
 
 
 def test_multiple_return():
     f = outer_make_a_dag_multi(inner_app())
-    assert f.result() == [RESULT_CONSTANT] * RESULT_CONSTANT
+    res = f.result()
+    assert res == [RESULT_CONSTANT] * RESULT_CONSTANT
 
 
 class InnerError(RuntimeError):
     pass
 
 
 @python_app
@@ -122,19 +135,7 @@
 
     assert isinstance(e, JoinError)
     assert len(e.dependent_exceptions_tids) == 1
 
     de0 = e.dependent_exceptions_tids[0][0]
     assert isinstance(de0, InnerError)
     assert de0.args[0] == "Error A"
-
-
-@join_app
-def app_no_futures():
-    return []
-
-
-def test_no_futures():
-    # tests that a list of futures that contains no futures will
-    # complete - regression test for issue #2792
-    f = app_no_futures()
-    assert f.result() == []
```

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_memoize_1.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_memoize_2.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_memoize_4.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_4.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,16 +25,17 @@
 
 @python_app(cache=True)
 def noop_app(x, inputs=[], cache=True):
     return None
 
 
 @python_app
-def some_func(_t):
-    pass
+def sleep(t):
+    import time
+    time.sleep(t)
 
 
 def test_python_unmemoizable():
     """Testing behaviour when an unmemoizable parameter is used
     """
     fut = noop_app(Unmemoizable())
     with pytest.raises(ValueError):
@@ -46,18 +47,18 @@
     """
     fut = noop_app(FailingMemoizable())
     with pytest.raises(FailingMemoizerTestError):
         fut.result()
 
 
 def test_python_unmemoizable_after_dep():
-    memoizable_fut = some_func(1)
-    fut = noop_app(Unmemoizable(), inputs=[memoizable_fut])
+    sleep_fut = sleep(1)
+    fut = noop_app(Unmemoizable(), inputs=[sleep_fut])
     with pytest.raises(ValueError):
         fut.result()
 
 
 def test_python_failing_memoizer_afer_dep():
-    memoizable_fut = some_func(1)
-    fut = noop_app(FailingMemoizable(), inputs=[memoizable_fut])
+    sleep_fut = sleep(1)
+    fut = noop_app(FailingMemoizable(), inputs=[sleep_fut])
     with pytest.raises(ValueError):
         fut.result()
```

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_memoize_ignore_args.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_pipeline.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_pipeline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import argparse
 
-import pytest
-
 import parsl
 from parsl.app.app import python_app
 from parsl.tests.configs.local_threads import config
 
 
 @python_app
 def increment(x):
     return x + 1
 
 
 @python_app
-def slow_increment(x):
+def slow_increment(x, dur):
     import time
-    time.sleep(0.001)
+    time.sleep(dur)
     return x + 1
 
 
-@pytest.mark.parametrize("depth", (2, 3))
-def test_increment(depth):
-    """Test simple pipeline A->B...->N"""
-    futs = [increment(0)]
-    futs.extend(increment(futs[i - 1]) for i in range(1, depth))
-    assert sum(f.result() for f in futs) == sum(range(1, depth + 1))
-
+def test_increment(depth=2):
+    """Test simple pipeline A->B...->N
+    """
+    futs = {0: 0}
+    for i in range(1, depth):
+        futs[i] = increment(futs[i - 1])
+
+    print([futs[i].result() for i in futs if not isinstance(futs[i], int)])
+
+
+def test_increment_slow(depth=2):
+    """Test simple pipeline A->B...->N with delay
+    """
+    futs = {0: 0}
+    for i in range(1, depth):
+        futs[i] = slow_increment(futs[i - 1], 0.5)
 
-@pytest.mark.parametrize("depth", (2, 3))
-def test_increment_slow(depth):
-    """Test simple pipeline A->B...->N with delay"""
-    futs = [slow_increment(0)]
-    futs.extend(slow_increment(futs[i - 1]) for i in range(1, depth))
-    assert sum(f.result() for f in futs) == sum(range(1, depth + 1))
+    print(futs[i])
+    print([futs[i].result() for i in futs if not isinstance(futs[i], int)])
```

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_simple.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_timeout.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_timeout.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,29 +11,25 @@
 
 
 def kernel(fail=False):
     if fail:
         raise TimeoutTestSpecificException()
 
 
-def test_timeout():
-    timeout_dur = 0.1
-    try:
-        timeout(kernel, timeout_dur)()  # nominally returns "instantly"
-    except AppTimeout:
-        pytest.skip("Pre-condition failed: result not received in timely fashion")
-        assert False
+@pytest.mark.parametrize("timeout_dur", (0.005, 0.01, 0.1))
+def test_timeout(timeout_dur):
+    timeout(kernel, timeout_dur)()
 
     try:
         time.sleep(timeout_dur + 0.01)  # this is the verification
     except AppTimeout:
         assert False, "Timer was not cancelled!"
 
 
-@pytest.mark.parametrize("timeout_dur", (0.005, 0.01))
+@pytest.mark.parametrize("timeout_dur", (0.005, 0.01, 0.1))
 def test_timeout_after_exception(timeout_dur):
     with pytest.raises(TimeoutTestSpecificException):
         timeout(kernel, timeout_dur)(True)
 
     try:
         time.sleep(timeout_dur + 0.01)  # this is the verification
     except AppTimeout:
```

### Comparing `parsl-2023.7.24/parsl/tests/test_python_apps/test_type5.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_type5.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_regression/test_1480.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_1480.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_regression/test_1653.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_1653.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_regression/test_221.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_221.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_regression/test_226.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_226.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_regression/test_2652.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_2652.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from parsl.jobs.states import JobState
+from parsl.providers.base import JobState
 
 
 @pytest.mark.local
 def test_JobStatus_repr():
     # in Python 3.11, the behavior of enums changed a bit, and so repr
     # (inherited from a superclass) raised an exception rather than
     # returning a string.
```

### Comparing `parsl-2023.7.24/parsl/tests/test_regression/test_69a.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_69a.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_regression/test_854.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_854.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_regression/test_97_parallelism_0.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_97_parallelism_0.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_scaling/test_regression_1621.py` & `parsl-2023.7.3/parsl/tests/test_scaling/test_regression_1621.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,67 @@
-import threading
-
-import pytest
+# this test is intended to ensure that only one block is launched when only
+# one app is invoked. this is a regression test.
 
+import logging
 import parsl
 from parsl.channels import LocalChannel
 from parsl.config import Config
 from parsl.executors import HighThroughputExecutor
 from parsl.launchers import SimpleLauncher
 from parsl.providers import LocalProvider
+import pytest
+
+
+logger = logging.getLogger(__name__)
 
 
 @parsl.python_app
 def app():
     import time
-    time.sleep(1)
+    time.sleep(45)
 
 
 class OneShotLocalProvider(LocalProvider):
     def __init__(self, *args, **kwargs):
+        logger.info("OneShotLocalProvider __init__ with MRO: {}".format(type(self).mro()))
         self.recorded_submits = 0
         super().__init__(*args, **kwargs)
 
     def submit(self, *args, **kwargs):
+        logger.info("OneShotLocalProvider submit")
         self.recorded_submits += 1
         return super().submit(*args, **kwargs)
 
     status_polling_interval = 600
 
 
 @pytest.mark.local
-def test_one_block(tmpd_cwd):
-    """
-    this test is intended to ensure that only one block is launched when only
-    one app is invoked. this is a regression test.
-    """
+def test_one_block():
+
     oneshot_provider = OneShotLocalProvider(
-        channel=LocalChannel(),
-        init_blocks=0,
-        min_blocks=0,
-        max_blocks=10,
-        launcher=SimpleLauncher(),
-    )
+                    channel=LocalChannel(),
+                    init_blocks=0,
+                    min_blocks=0,
+                    max_blocks=10,
+                    launcher=SimpleLauncher(),
+                )
 
     config = Config(
         executors=[
             HighThroughputExecutor(
                 label="htex_local",
-                address="127.0.0.1",
                 worker_debug=True,
                 cores_per_worker=1,
                 provider=oneshot_provider,
-                worker_logdir_root=str(tmpd_cwd)
             )
         ],
         strategy='simple',
     )
 
     parsl.load(config)
-    dfk = parsl.dfk()
-
-    def poller():
-        import time
-        while True:
-            dfk.job_status_poller.poll()
-            time.sleep(0.1)
 
-    threading.Thread(target=poller, daemon=True).start()
-    app().result()
+    f = app()
+    f.result()
     parsl.dfk().cleanup()
     parsl.clear()
 
     assert oneshot_provider.recorded_submits == 1
```

### Comparing `parsl-2023.7.24/parsl/tests/test_scaling/test_scale_down.py` & `parsl-2023.7.3/parsl/tests/test_scaling/test_scale_down.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,80 @@
 import logging
-import time
-
-import pytest
-
 import parsl
+import pytest
+import time
+from parsl import python_app
 
-from parsl import File, python_app
 from parsl.providers import LocalProvider
 from parsl.channels import LocalChannel
+# from parsl.launchers import SimpleLauncher
 from parsl.launchers import SingleNodeLauncher
+
 from parsl.config import Config
 from parsl.executors import HighThroughputExecutor
 
 logger = logging.getLogger(__name__)
 
-_max_blocks = 5
-_min_blocks = 2
-
 
 def local_config():
     return Config(
         executors=[
             HighThroughputExecutor(
-                heartbeat_period=1,
-                heartbeat_threshold=2,
-                poll_period=100,
+                heartbeat_period=2,
+                heartbeat_threshold=6,
+                poll_period=1,
                 label="htex_local",
-                address="127.0.0.1",
                 max_workers=1,
                 provider=LocalProvider(
                     channel=LocalChannel(),
                     init_blocks=0,
-                    max_blocks=_max_blocks,
-                    min_blocks=_min_blocks,
+                    max_blocks=5,
+                    min_blocks=2,
                     launcher=SingleNodeLauncher(),
                 ),
             )
         ],
-        max_idletime=0.5,
+        max_idletime=5,
         strategy='htex_auto_scale',
     )
 
 
 @python_app
-def waiting_app(ident: int, inputs=()):
-    import pathlib
+def sleeper(t):
     import time
-
-    # Approximate an Event by writing to files; the test logic will poll this file
-    with open(inputs[0], "a") as f:
-        f.write(f"Ready: {ident}\n")
-
-    # Similarly, use Event approximation (file check!) by polling.
-    may_finish_file = pathlib.Path(inputs[1])
-    while not may_finish_file.exists():
-        time.sleep(0.01)
+    time.sleep(t)
 
 
 # see issue #1885 for details of failures of this test.
 # at the time of issue #1885 this test was failing frequently
 # in CI.
 @pytest.mark.local
-def test_scale_out(tmpd_cwd, try_assert):
+def test_scale_out():
+    logger.info("start")
     dfk = parsl.dfk()
 
-    num_managers = len(dfk.executors['htex_local'].connected_managers())
-
-    assert num_managers == 0, "Expected 0 managers at start"
+    logger.info("initial asserts")
+    assert len(dfk.executors['htex_local'].connected_managers()) == 0, "Expected 0 managers at start"
     assert dfk.executors['htex_local'].outstanding == 0, "Expected 0 tasks at start"
 
-    ntasks = 10
-    ready_path = tmpd_cwd / "workers_ready"
-    finish_path = tmpd_cwd / "workers_may_continue"
-    ready_path.touch()
-    inputs = [File(str(ready_path)), File(str(finish_path))]
+    logger.info("launching tasks")
+    fus = [sleeper(i) for i in [15 for x in range(0, 10)]]
 
-    futs = [waiting_app(i, inputs=inputs) for i in range(ntasks)]
+    logger.info("waiting for warm up")
+    time.sleep(15)
 
-    while ready_path.read_text().count("\n") < _max_blocks:
-        time.sleep(0.5)
+    logger.info("asserting 5 managers")
+    assert len(dfk.executors['htex_local'].connected_managers()) == 5, "Expected 5 managers after some time"
 
-    assert len(dfk.executors['htex_local'].connected_managers()) == _max_blocks
+    logger.info("waiting for all futures to complete")
+    [x.result() for x in fus]
 
-    finish_path.touch()  # Approximation of Event, via files
-    [x.result() for x in futs]
+    logger.info("asserting 0 outstanding tasks after completion")
+    assert dfk.executors['htex_local'].outstanding == 0, "Expected 0 outstanding tasks after future completion"
 
-    assert dfk.executors['htex_local'].outstanding == 0
+    logger.info("waiting a while for scale down")
+    time.sleep(25)
 
-    def assert_kernel():
-        return len(dfk.executors['htex_local'].connected_managers()) == _min_blocks
+    logger.info("asserting 2 managers remain")
+    assert len(dfk.executors['htex_local'].connected_managers()) == 2, "Expected 2 managers when no tasks, lower bound by min_blocks"
 
-    try_assert(
-        assert_kernel,
-        fail_msg=f"Expected {_min_blocks} managers when no tasks (min_blocks)",
-        timeout_ms=15000,
-    )
+    logger.info("test passed")
```

### Comparing `parsl-2023.7.24/parsl/tests/test_serialization/test_basic.py` & `parsl-2023.7.3/parsl/tests/test_serialization/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_staging/staging_provider.py` & `parsl-2023.7.3/parsl/tests/test_staging/staging_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_staging/test_1316.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_1316.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_staging/test_docs_1.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_docs_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_staging/test_elaborate_noop_file.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_elaborate_noop_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_staging/test_staging_ftp.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_staging/test_staging_ftp_in_task.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_ftp_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_staging/test_staging_globus.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_staging/test_staging_https.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_https.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_staging/test_staging_https_in_task.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_https_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_summary.py` & `parsl-2023.7.3/parsl/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_thread_parallelism.py` & `parsl-2023.7.3/parsl/tests/test_thread_parallelism.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_threads/test_configs.py` & `parsl-2023.7.3/parsl/tests/test_threads/test_configs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/tests/test_threads/test_lazy_errors.py` & `parsl-2023.7.3/parsl/tests/test_threads/test_lazy_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/usage_tracking/usage.py` & `parsl-2023.7.3/parsl/usage_tracking/usage.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.24/parsl/utils.py` & `parsl-2023.7.3/parsl/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import inspect
 import logging
 import os
 import shlex
 import subprocess
 import threading
 import time
-from contextlib import contextmanager
 from types import TracebackType
-from typing import Any, Callable, List, Tuple, Union, Generator, IO, AnyStr, Dict, Optional
 
 import typeguard
+from contextlib import contextmanager
+from typing import Any, Callable, List, Tuple, Union, Generator, IO, AnyStr, Dict, Optional
+
 from typing_extensions import Type
 
 import parsl
 from parsl.version import VERSION
 
 
 try:
@@ -105,29 +106,26 @@
     if not os.path.isdir(last_checkpoint):
         return []
 
     return [last_checkpoint]
 
 
 @typeguard.typechecked
-def get_std_fname_mode(
-    fdname: str,
-    stdfspec: Union[os.PathLike, str, Tuple[str, str], Tuple[os.PathLike, str]]
-) -> Tuple[str, str]:
+def get_std_fname_mode(fdname: str, stdfspec: Union[str, Tuple[str, str]]) -> Tuple[str, str]:
     import parsl.app.errors as pe
-    if isinstance(stdfspec, (str, os.PathLike)):
+    if isinstance(stdfspec, str):
         fname = stdfspec
         mode = 'a+'
     elif isinstance(stdfspec, tuple):
         if len(stdfspec) != 2:
             msg = (f"std descriptor {fdname} has incorrect tuple length "
                    f"{len(stdfspec)}")
             raise pe.BadStdStreamFile(msg, TypeError('Bad Tuple Length'))
         fname, mode = stdfspec
-    return str(fname), mode
+    return fname, mode
 
 
 @contextmanager
 def wait_for_file(path: str, seconds: int = 10) -> Generator[None, None, None]:
     for i in range(0, int(seconds * 100)):
         time.sleep(seconds / 100.)
         if os.path.exists(path):
```

### Comparing `parsl-2023.7.24/parsl.egg-info/PKG-INFO` & `parsl-2023.7.3/parsl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2023.7.24
+Version: 2023.7.3
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2023.07.24.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2023.07.03.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2023.7.24/parsl.egg-info/SOURCES.txt` & `parsl-2023.7.3/parsl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,18 +71,22 @@
 parsl/data_provider/globus.py
 parsl/data_provider/http.py
 parsl/data_provider/rsync.py
 parsl/data_provider/staging.py
 parsl/dataflow/__init__.py
 parsl/dataflow/dflow.py
 parsl/dataflow/errors.py
+parsl/dataflow/executor_status.py
 parsl/dataflow/futures.py
+parsl/dataflow/job_error_handler.py
+parsl/dataflow/job_status_poller.py
 parsl/dataflow/memoization.py
 parsl/dataflow/rundirs.py
 parsl/dataflow/states.py
+parsl/dataflow/strategy.py
 parsl/dataflow/taskrecord.py
 parsl/executors/__init__.py
 parsl/executors/base.py
 parsl/executors/errors.py
 parsl/executors/status_handling.py
 parsl/executors/threads.py
 parsl/executors/flux/__init__.py
@@ -98,28 +102,20 @@
 parsl/executors/high_throughput/probe.py
 parsl/executors/high_throughput/process_worker_pool.py
 parsl/executors/high_throughput/zmq_pipes.py
 parsl/executors/taskvine/__init__.py
 parsl/executors/taskvine/errors.py
 parsl/executors/taskvine/exec_parsl_function.py
 parsl/executors/taskvine/executor.py
-parsl/executors/taskvine/factory_config.py
-parsl/executors/taskvine/manager_config.py
-parsl/executors/taskvine/utils.py
 parsl/executors/workqueue/__init__.py
 parsl/executors/workqueue/errors.py
 parsl/executors/workqueue/exec_parsl_function.py
 parsl/executors/workqueue/executor.py
 parsl/executors/workqueue/parsl_coprocess.py
 parsl/executors/workqueue/parsl_coprocess_stub.py
-parsl/jobs/__init__.py
-parsl/jobs/job_error_handler.py
-parsl/jobs/job_status_poller.py
-parsl/jobs/states.py
-parsl/jobs/strategy.py
 parsl/launchers/__init__.py
 parsl/launchers/base.py
 parsl/launchers/errors.py
 parsl/launchers/launchers.py
 parsl/monitoring/__init__.py
 parsl/monitoring/db_manager.py
 parsl/monitoring/message_type.py
@@ -333,16 +329,14 @@
 parsl/tests/test_error_handling/test_resource_spec.py
 parsl/tests/test_error_handling/test_retries.py
 parsl/tests/test_error_handling/test_retry_handler.py
 parsl/tests/test_error_handling/test_retry_handler_failure.py
 parsl/tests/test_error_handling/test_serialization_fail.py
 parsl/tests/test_error_handling/test_wrap_with_logs.py
 parsl/tests/test_flowcontrol/__init__.py
-parsl/tests/test_htex/__init__.py
-parsl/tests/test_htex/test_htex_zmq_binding.py
 parsl/tests/test_monitoring/__init__.py
 parsl/tests/test_monitoring/test_basic.py
 parsl/tests/test_monitoring/test_db_locks.py
 parsl/tests/test_monitoring/test_fuzz_zmq.py
 parsl/tests/test_monitoring/test_memoization_representation.py
 parsl/tests/test_monitoring/test_viz_colouring.py
 parsl/tests/test_providers/__init__.py
@@ -377,22 +371,22 @@
 parsl/tests/test_regression/test_1480.py
 parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
 parsl/tests/test_regression/test_1653.py
 parsl/tests/test_regression/test_221.py
 parsl/tests/test_regression/test_226.py
 parsl/tests/test_regression/test_2652.py
 parsl/tests/test_regression/test_69a.py
+parsl/tests/test_regression/test_69b.py
 parsl/tests/test_regression/test_854.py
 parsl/tests/test_regression/test_97_parallelism_0.py
 parsl/tests/test_regression/test_98.py
 parsl/tests/test_scaling/__init__.py
 parsl/tests/test_scaling/test_regression_1621.py
 parsl/tests/test_scaling/test_scale_down.py
 parsl/tests/test_serialization/__init__.py
-parsl/tests/test_serialization/test_2555_caching_deserializer.py
 parsl/tests/test_serialization/test_basic.py
 parsl/tests/test_staging/__init__.py
 parsl/tests/test_staging/staging_provider.py
 parsl/tests/test_staging/test_1316.py
 parsl/tests/test_staging/test_docs_1.py
 parsl/tests/test_staging/test_docs_2.py
 parsl/tests/test_staging/test_elaborate_noop_file.py
```

### Comparing `parsl-2023.7.24/parsl.egg-info/requires.txt` & `parsl-2023.7.3/parsl.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 pyzmq>=17.1.2
 typeguard<3,>=2.10
 typing-extensions<5,>=4.6
+types-paramiko
+types-requests
+types-six
 six
 globus-sdk
 dill
 tblib
 requests
 paramiko
 psutil>=5.5.1
```

### Comparing `parsl-2023.7.24/setup.py` & `parsl-2023.7.3/setup.py`

 * *Files identical despite different names*

