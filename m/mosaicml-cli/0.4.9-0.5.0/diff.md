# Comparing `tmp/mosaicml-cli-0.4.9.tar.gz` & `tmp/mosaicml-cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.4.9.tar", last modified: Thu Jun 15 20:53:05 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.5.0.tar", last modified: Mon Jul 24 21:45:35 2023, max compression
```

## Comparing `mosaicml-cli-0.4.9.tar` & `mosaicml-cli-0.5.0.tar`

### file list

```diff
@@ -1,202 +1,209 @@
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.920695 mosaicml-cli-0.4.9/
--rw-r--r--   0 tylerlee   (502) staff       (20)      696 2023-06-15 20:53:05.920546 mosaicml-cli-0.4.9/PKG-INFO
--rw-r--r--   0 tylerlee   (502) staff       (20)     7089 2023-06-13 22:57:11.000000 mosaicml-cli-0.4.9/README.md
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.885680 mosaicml-cli-0.4.9/mcli/
--rw-r--r--   0 tylerlee   (502) staff       (20)     2092 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.9/mcli/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.886401 mosaicml-cli-0.4.9/mcli/api/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/api/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.886886 mosaicml-cli-0.4.9/mcli/api/cluster/
--rw-r--r--   0 tylerlee   (502) staff       (20)      134 2022-11-02 22:22:14.000000 mosaicml-cli-0.4.9/mcli/api/cluster/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4280 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.887223 mosaicml-cli-0.4.9/mcli/api/engine/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/api/engine/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    26224 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/engine/engine.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10824 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/exceptions.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.889526 mosaicml-cli-0.4.9/mcli/api/inference_deployments/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1521 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3297 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5096 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3603 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     8441 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2053 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_ping.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2347 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_predict_inference_deployment.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6474 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_update_inference_deployments.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.890764 mosaicml-cli-0.4.9/mcli/api/mint/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.9/mcli/api/mint/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     7840 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/mint/shell.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2676 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/api/mint/tty.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.891812 mosaicml-cli-0.4.9/mcli/api/model/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1114 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/api/model/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6435 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/model/cluster_details.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4583 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/api/model/inference_deployment.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    11259 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/model/run.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.895731 mosaicml-cli-0.4.9/mcli/api/runs/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1199 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/api/runs/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2964 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_create_run.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4362 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     8930 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    11418 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5364 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_start_run.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5556 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4088 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10619 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.9/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.896223 mosaicml-cli-0.4.9/mcli/api/schema/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/api/schema/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      636 2022-08-23 15:11:52.000000 mosaicml-cli-0.4.9/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.897215 mosaicml-cli-0.4.9/mcli/api/secrets/
--rw-r--r--   0 tylerlee   (502) staff       (20)      309 2022-09-23 17:32:12.000000 mosaicml-cli-0.4.9/mcli/api/secrets/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2386 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3010 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3709 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2354 2022-03-24 04:29:23.000000 mosaicml-cli-0.4.9/mcli/api/typing_future.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.897557 mosaicml-cli-0.4.9/mcli/api/users/
--rw-r--r--   0 tylerlee   (502) staff       (20)      139 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.9/mcli/api/users/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2715 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/api/users/api_get_users.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      920 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/api/utils.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.897908 mosaicml-cli-0.4.9/mcli/cli/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.9/mcli/cli/__init__.py
--rwxr-xr-x   0 tylerlee   (502) staff       (20)     6383 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/cli.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.898487 mosaicml-cli-0.4.9/mcli/cli/common/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.9/mcli/cli/common/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2560 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6937 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.898792 mosaicml-cli-0.4.9/mcli/cli/m_connect/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.9/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6143 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.899300 mosaicml-cli-0.4.9/mcli/cli/m_create/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/cli/m_create/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2385 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_create/m_create.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    16900 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.900141 mosaicml-cli-0.4.9/mcli/cli/m_delete/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6448 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/m_delete/delete.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5804 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.900568 mosaicml-cli-0.4.9/mcli/cli/m_deploy/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.9/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4001 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.901439 mosaicml-cli-0.4.9/mcli/cli/m_describe/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-01-26 00:46:18.000000 mosaicml-cli-0.4.9/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3929 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     9433 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2002 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.903319 mosaicml-cli-0.4.9/mcli/cli/m_get/
--rw-r--r--   0 tylerlee   (502) staff       (20)      467 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     7136 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/clusters.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6447 2023-05-24 19:54:07.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/display.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5668 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4802 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/m_get.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     8027 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2189 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/secrets.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1580 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.9/mcli/cli/m_get/users.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.903708 mosaicml-cli-0.4.9/mcli/cli/m_init/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/cli/m_init/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3908 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/cli/m_init/m_init.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.905003 mosaicml-cli-0.4.9/mcli/cli/m_interactive/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.9/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6793 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    44284 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_interactive/kube_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     9487 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.906198 mosaicml-cli-0.4.9/mcli/cli/m_kube/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_kube/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5523 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_kube/m_get_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1398 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_kube/m_kube.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2050 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_kube/m_merge_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6946 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_kube/utils.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.906503 mosaicml-cli-0.4.9/mcli/cli/m_log/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.9/mcli/cli/m_log/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    11303 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.906792 mosaicml-cli-0.4.9/mcli/cli/m_ping/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1103 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.907192 mosaicml-cli-0.4.9/mcli/cli/m_predict/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1661 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.907519 mosaicml-cli-0.4.9/mcli/cli/m_root/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.9/mcli/cli/m_root/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      536 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.907781 mosaicml-cli-0.4.9/mcli/cli/m_run/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/cli/m_run/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     8219 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.908862 mosaicml-cli-0.4.9/mcli/cli/m_set_unset/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.9/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2964 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1793 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1940 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1421 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      745 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.909184 mosaicml-cli-0.4.9/mcli/cli/m_stop/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.9/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4066 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.909597 mosaicml-cli-0.4.9/mcli/cli/m_util/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-08-10 05:32:44.000000 mosaicml-cli-0.4.9/mcli/cli/m_util/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      797 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/cli/m_util/m_util.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6837 2023-06-13 22:57:06.000000 mosaicml-cli-0.4.9/mcli/cli/m_util/util.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    12143 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/config.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.910986 mosaicml-cli-0.4.9/mcli/models/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1047 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/models/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2103 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/models/gpu_type.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10374 2023-06-13 22:57:11.000000 mosaicml-cli-0.4.9/mcli/models/inference_deployment_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      427 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/models/mcli_cluster.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      456 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/models/mcli_envvar.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6724 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/models/mcli_secret.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    19505 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/models/run_config.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.911291 mosaicml-cli-0.4.9/mcli/objects/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.9/mcli/objects/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.912922 mosaicml-cli-0.4.9/mcli/objects/secrets/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1090 2022-12-07 21:26:59.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.914112 mosaicml-cli-0.4.9/mcli/objects/secrets/create/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1646 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/base.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2244 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2408 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6377 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3858 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3001 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5342 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      783 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1017 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/env_var.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      556 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/gcp.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1267 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/mounted.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      967 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/oci.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      961 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/s3.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1718 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.914387 mosaicml-cli-0.4.9/mcli/proto/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/proto/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1477 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.914608 mosaicml-cli-0.4.9/mcli/sdk/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1976 2023-06-05 23:23:13.000000 mosaicml-cli-0.4.9/mcli/sdk/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.918207 mosaicml-cli-0.4.9/mcli/utils/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.9/mcli/utils/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5315 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/utils/utils_cli.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6073 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/utils/utils_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      740 2022-09-27 01:25:02.000000 mosaicml-cli-0.4.9/mcli/utils/utils_date.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10749 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/utils/utils_docker.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2225 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/utils/utils_epilog.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10774 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/utils/utils_interactive.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4527 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/utils/utils_logging.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2160 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6605 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/mcli/utils/utils_pypi.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3115 2023-03-15 17:23:44.000000 mosaicml-cli-0.4.9/mcli/utils/utils_rich.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5033 2023-06-06 15:18:59.000000 mosaicml-cli-0.4.9/mcli/utils/utils_run_status.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4350 2022-03-30 16:04:08.000000 mosaicml-cli-0.4.9/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1103 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.9/mcli/utils/utils_spinner.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10751 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/utils/utils_string_functions.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1677 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/mcli/utils/utils_types.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1001 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.9/mcli/utils/utils_yaml.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3876 2023-06-15 20:52:49.000000 mosaicml-cli-0.4.9/mcli/version.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.919120 mosaicml-cli-0.4.9/mosaicml_cli.egg-info/
--rw-r--r--   0 tylerlee   (502) staff       (20)      696 2023-06-15 20:53:05.000000 mosaicml-cli-0.4.9/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 tylerlee   (502) staff       (20)     4922 2023-06-15 20:53:05.000000 mosaicml-cli-0.4.9/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)        1 2023-06-15 20:53:05.000000 mosaicml-cli-0.4.9/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)       75 2023-06-15 20:53:05.000000 mosaicml-cli-0.4.9/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)     1655 2023-06-15 20:53:05.000000 mosaicml-cli-0.4.9/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)        5 2023-06-15 20:53:05.000000 mosaicml-cli-0.4.9/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)    31087 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/pyproject.toml
--rw-r--r--   0 tylerlee   (502) staff       (20)       38 2023-06-15 20:53:05.920738 mosaicml-cli-0.4.9/setup.cfg
--rw-r--r--   0 tylerlee   (502) staff       (20)     3057 2023-06-13 22:57:11.000000 mosaicml-cli-0.4.9/setup.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-06-15 20:53:05.920139 mosaicml-cli-0.4.9/tests/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.9/tests/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      618 2023-05-18 17:15:51.000000 mosaicml-cli-0.4.9/tests/conftest.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     7127 2023-06-13 23:01:11.000000 mosaicml-cli-0.4.9/tests/test_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)       62 2022-03-03 05:25:48.000000 mosaicml-cli-0.4.9/tests/test_simple.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6116 2023-05-12 19:35:37.000000 mosaicml-cli-0.4.9/tests/test_upgrade.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.364976 mosaicml-cli-0.5.0/
+-rw-r--r--   0 wai.wu     (502) staff       (20)      696 2023-07-24 21:45:35.364815 mosaicml-cli-0.5.0/PKG-INFO
+-rw-r--r--   0 wai.wu     (502) staff       (20)     7089 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/README.md
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.317674 mosaicml-cli-0.5.0/mcli/
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2122 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/__init__.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.318870 mosaicml-cli-0.5.0/mcli/api/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/__init__.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.319529 mosaicml-cli-0.5.0/mcli/api/cluster/
+-rw-r--r--   0 wai.wu     (502) staff       (20)      134 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/cluster/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     4990 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.320126 mosaicml-cli-0.5.0/mcli/api/engine/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/engine/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    26027 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/engine/engine.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    13444 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/exceptions.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.322658 mosaicml-cli-0.5.0/mcli/api/inference_deployments/
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1521 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     3297 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     5045 2023-07-24 21:17:12.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     3744 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     8413 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2294 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_ping.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2746 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_predict_inference_deployment.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     6499 2023-07-24 21:17:12.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_update_inference_deployments.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.323499 mosaicml-cli-0.5.0/mcli/api/mint/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/mint/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     7840 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/mint/shell.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2676 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/mint/tty.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.324680 mosaicml-cli-0.5.0/mcli/api/model/
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1114 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/model/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     9386 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/api/model/cluster_details.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     4583 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    14890 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/model/run.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.331004 mosaicml-cli-0.5.0/mcli/api/runs/
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1269 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     3814 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_create_interactive_run.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     3034 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     4365 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     8796 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    12239 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     5366 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     5559 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     5573 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_update_run.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     4091 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    10414 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.331633 mosaicml-cli-0.5.0/mcli/api/schema/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/schema/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)      636 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.332698 mosaicml-cli-0.5.0/mcli/api/secrets/
+-rw-r--r--   0 wai.wu     (502) staff       (20)      309 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/secrets/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2386 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2943 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     3665 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2354 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/typing_future.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.333154 mosaicml-cli-0.5.0/mcli/api/users/
+-rw-r--r--   0 wai.wu     (502) staff       (20)      139 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/users/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2715 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/users/api_get_users.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)      920 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/utils.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.333811 mosaicml-cli-0.5.0/mcli/cli/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/cli/__init__.py
+-rwxr-xr-x   0 wai.wu     (502) staff       (20)     6069 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/cli.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.334813 mosaicml-cli-0.5.0/mcli/cli/common/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/cli/common/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2560 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     7499 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.335327 mosaicml-cli-0.5.0/mcli/cli/m_connect/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     6426 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.336166 mosaicml-cli-0.5.0/mcli/cli/m_create/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2385 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    16900 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.336921 mosaicml-cli-0.5.0/mcli/cli/m_delete/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     6448 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     5838 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.337447 mosaicml-cli-0.5.0/mcli/cli/m_deploy/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     4253 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.338322 mosaicml-cli-0.5.0/mcli/cli/m_describe/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     3929 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    13495 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2259 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.340633 mosaicml-cli-0.5.0/mcli/cli/m_get/
+-rw-r--r--   0 wai.wu     (502) staff       (20)      467 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     7068 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     6459 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/display.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     5807 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     4804 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     8967 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/runs.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2189 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1580 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/users.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.341264 mosaicml-cli-0.5.0/mcli/cli/m_init/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     3908 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_init/m_init.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.341830 mosaicml-cli-0.5.0/mcli/cli/m_interactive/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     8423 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.343367 mosaicml-cli-0.5.0/mcli/cli/m_kube/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_kube/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     5523 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_kube/m_get_config.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1398 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_kube/m_kube.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2050 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_kube/m_merge_config.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     6946 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_kube/utils.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.343917 mosaicml-cli-0.5.0/mcli/cli/m_log/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    11354 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.344588 mosaicml-cli-0.5.0/mcli/cli/m_ping/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1411 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.345230 mosaicml-cli-0.5.0/mcli/cli/m_predict/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1905 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.345587 mosaicml-cli-0.5.0/mcli/cli/m_root/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)      536 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.346081 mosaicml-cli-0.5.0/mcli/cli/m_run/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    10779 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.347762 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2964 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1793 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2267 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1656 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)      840 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/organization.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)      745 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.348260 mosaicml-cli-0.5.0/mcli/cli/m_stop/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     4062 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.348691 mosaicml-cli-0.5.0/mcli/cli/m_update/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_update/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     6222 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_update/m_update.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.349788 mosaicml-cli-0.5.0/mcli/cli/m_util/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)      797 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     9034 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_util/util.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.350171 mosaicml-cli-0.5.0/mcli/cli/m_watchdog/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_watchdog/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     3544 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_watchdog/m_watchdog.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    13108 2023-07-24 20:29:09.000000 mosaicml-cli-0.5.0/mcli/config.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.352011 mosaicml-cli-0.5.0/mcli/models/
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1047 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/models/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2103 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/models/gpu_type.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    12287 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)      427 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/models/mcli_cluster.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)      456 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/models/mcli_envvar.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     6728 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/models/mcli_secret.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    17205 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/models/run_config.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.352286 mosaicml-cli-0.5.0/mcli/objects/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/__init__.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.354354 mosaicml-cli-0.5.0/mcli/objects/secrets/
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1090 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.356313 mosaicml-cli-0.5.0/mcli/objects/secrets/create/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1646 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2244 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2408 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     6377 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     3858 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     3001 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     5342 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)      783 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1017 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)      556 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1267 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)      967 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/oci.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)      961 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/s3.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1718 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.356847 mosaicml-cli-0.5.0/mcli/proto/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/proto/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1477 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.357156 mosaicml-cli-0.5.0/mcli/sdk/
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2006 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/sdk/__init__.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.362248 mosaicml-cli-0.5.0/mcli/utils/
+-rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/__init__.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     6318 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/utils/utils_cli.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     4409 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/utils/utils_completers.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     7047 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_config.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)      740 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_date.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    10749 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_docker.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2225 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_epilog.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    10774 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_interactive.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     4527 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_logging.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     2160 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1087 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/utils/utils_model.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     6605 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_pypi.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     3115 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_rich.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     5358 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/utils/utils_run_status.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     4350 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1103 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_spinner.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)    10751 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1677 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_types.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1001 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_yaml.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     3876 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/version.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.363791 mosaicml-cli-0.5.0/mosaicml_cli.egg-info/
+-rw-r--r--   0 wai.wu     (502) staff       (20)      696 2023-07-24 21:45:35.000000 mosaicml-cli-0.5.0/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 wai.wu     (502) staff       (20)     5106 2023-07-24 21:45:35.000000 mosaicml-cli-0.5.0/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 wai.wu     (502) staff       (20)        1 2023-07-24 21:45:35.000000 mosaicml-cli-0.5.0/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 wai.wu     (502) staff       (20)       75 2023-07-24 21:45:35.000000 mosaicml-cli-0.5.0/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 wai.wu     (502) staff       (20)     1654 2023-07-24 21:45:35.000000 mosaicml-cli-0.5.0/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 wai.wu     (502) staff       (20)        5 2023-07-24 21:45:35.000000 mosaicml-cli-0.5.0/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 wai.wu     (502) staff       (20)    31087 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/pyproject.toml
+-rw-r--r--   0 wai.wu     (502) staff       (20)       38 2023-07-24 21:45:35.365020 mosaicml-cli-0.5.0/setup.cfg
+-rw-r--r--   0 wai.wu     (502) staff       (20)     3056 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/setup.py
+drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.364535 mosaicml-cli-0.5.0/tests/
+-rw-r--r--   0 wai.wu     (502) staff       (20)     6449 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/tests/test_config.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)       62 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/tests/test_simple.py
+-rw-r--r--   0 wai.wu     (502) staff       (20)     6116 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.9/PKG-INFO` & `mosaicml-cli-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.9
+Version: 0.5.0
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.9/README.md` & `mosaicml-cli-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/__init__.py` & `mosaicml-cli-0.5.0/mcli/sdk/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,57 @@
-""" MCLI Package """
+"""Primary import target for the Python API"""
 
 from mcli.api.cluster import get_clusters
 from mcli.api.exceptions import MAPIException
 from mcli.api.inference_deployments import (InferenceDeployment, InferenceDeploymentConfig, create_inference_deployment,
-                                            delete_inference_deployment, delete_inference_deployments,
-                                            get_inference_deployment, get_inference_deployment_logs,
-                                            get_inference_deployments, ping, predict, update_inference_deployment,
-                                            update_inference_deployments)
+                                            delete_inference_deployments, get_inference_deployment,
+                                            get_inference_deployment_logs, get_inference_deployments, ping, predict,
+                                            update_inference_deployment, update_inference_deployments)
 from mcli.api.runs import (FinalRunConfig, Run, RunConfig, RunStatus, create_run, delete_run, delete_runs,
                            follow_run_logs, get_run, get_run_logs, get_runs, start_run, start_runs, stop_run, stop_runs,
-                           update_run_metadata, wait_for_run_status, watch_run_status)
+                           update_run, update_run_metadata, wait_for_run_status, watch_run_status)
 from mcli.api.secrets import create_secret, delete_secrets, get_secrets
 from mcli.cli.m_init.m_init import initialize
 from mcli.cli.m_set_unset.api_key import set_api_key
 from mcli.config import FeatureFlag, MCLIConfig
 
-from .version import __version__
-
 __all__ = [
+    'get_clusters',
+    'MAPIException',
+    'InferenceDeployment',
+    'InferenceDeploymentConfig',
     'create_inference_deployment',
-    'create_run',
-    'create_secret',
-    'delete_inference_deployment',
     'delete_inference_deployments',
-    'delete_run',
-    'delete_runs',
-    'delete_secrets',
-    'FeatureFlag',
-    'FinalRunConfig',
-    'follow_run_logs',
-    'get_clusters',
     'get_inference_deployment_logs',
-    'get_inference_deployment',
     'get_inference_deployments',
-    'get_run_logs',
-    'get_run',
-    'get_runs',
-    'get_secrets',
-    'InferenceDeployment',
-    'InferenceDeploymentConfig',
-    'initialize',
-    'MAPIException',
-    'MCLIConfig',
+    'get_inference_deployment',
     'ping',
     'predict',
+    'FinalRunConfig',
     'Run',
     'RunConfig',
     'RunStatus',
-    'set_api_key',
+    'create_run',
+    'delete_run',
+    'delete_runs',
+    'follow_run_logs',
+    'get_run',
+    'get_run_logs',
+    'get_runs',
     'start_run',
     'start_runs',
     'stop_run',
     'stop_runs',
     'update_inference_deployment',
     'update_inference_deployments',
     'update_run_metadata',
+    'update_run',
     'wait_for_run_status',
     'watch_run_status',
+    'create_secret',
+    'delete_secrets',
+    'get_secrets',
+    'initialize',
+    'set_api_key',
+    'FeatureFlag',
+    'MCLIConfig',
 ]
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.5.0/mcli/api/cluster/api_get_clusters.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,41 +44,64 @@
     id
     name
     provider
     allowedSubmissionType
     utilization {{
       clusterInstanceUtils {{
         clusterId
+        name
         gpuType
         gpusPerNode
         numNodes
         gpusUsed
         gpusAvailable
         gpusTotal
       }}
-      activeByUser {{
+      activeRunsByUser{{
         id
         createdAt
         userName
         runName
+        instance
         gpuNum
         scheduling {{
           priority
+          retryOnSystemFailure
+          preemptible
         }}
       }}
-      queuedByUser {{
+      queuedRunsByUser{{
         id
         createdAt
         userName
         runName
+        instance
         gpuNum
         scheduling {{
           priority
+          retryOnSystemFailure
+          preemptible
         }}
       }}
+      activeDeploymentsByUser{{
+        id
+        createdAt
+        userName
+        deploymentName
+        instance
+        gpuNum
+      }}
+      queuedDeploymentsByUser{{
+        id
+        createdAt
+        userName
+        deploymentName
+        instance
+        gpuNum
+      }}
       anonymizeUsers
     }}
   }}
 }}"""
 
 
 @overload
@@ -138,16 +161,22 @@
     variables = {
         VARIABLE_DATA_NAME: {
             'filters': filters
         },
     }
 
     cfg = MCLIConfig.load_config()
-    if cfg.user_id:
-        variables[VARIABLE_DATA_NAME]['entity'] = {'userIds': [cfg.user_id]}
+    cfg.update_entity(
+        variables[VARIABLE_DATA_NAME],
+        # TODO: getClusters needs updates to work well with admin entity filters
+        # For now, don't set the user because this will enable the organization entity
+        # filter to be applied
+        # Note this will exclude clusters granted specifically to a user
+        set_user=False,
+    )
 
     response = run_plural_mapi_request(
         query=QUERY_UTILIZATION if include_utilization else QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=ClusterDetails,
         variables=variables,
     )
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/engine/engine.py` & `mosaicml-cli-0.5.0/mcli/api/engine/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,36 +18,27 @@
 from gql.client import Client, ReconnectingAsyncClientSession
 from gql.transport import AsyncTransport
 from gql.transport.exceptions import TransportQueryError
 from gql.transport.websockets import WebsocketsTransport
 from graphql import DocumentNode
 from websockets.exceptions import ConnectionClosed, PayloadTooBig, WebSocketException
 
-from mcli.api.exceptions import ERROR_API_KEY_MISSING, MAPIException, MCLIConfigError, MultiMAPIException
+from mcli.api.exceptions import ERROR_AUTH_KEY_MISSING, MAPIException, MCLIConfigError, MultiMAPIException
 from mcli.api.schema.generic_model import DeserializableModel
 from mcli.api.utils import check_python_certificates
 from mcli.config import get_timeout
 from mcli.version import __version__
 
 logger = logging.getLogger(__name__)
 
 # pylint: disable-next=invalid-name
 THREADPOOL_WORKERS = 10
 THREADPOOL: Optional[ThreadPoolExecutor] = None
 
 
-def get_common_header(header: Dict[str, str]) -> Dict[str, str]:
-    return {
-        **header,
-        'Content-Type': 'application/json',
-        'x-mosaicml-client': 'mcli',
-        'x-mosaicml-client-version': __version__,
-    }
-
-
 def _create_threadpool() -> ThreadPoolExecutor:
     """Create a global threadpool for requests
     """
     logger.debug("Creating default threadpool")
     global THREADPOOL
     THREADPOOL = ThreadPoolExecutor(max_workers=THREADPOOL_WORKERS, thread_name_prefix='mosaicml-api')
     return THREADPOOL
@@ -68,26 +59,28 @@
 
 class MAPIConnection:
     """Connection to a user's MAPI instance
 
     Args:
         api_key: The user's API key. If not specified, the value of the $MOSAICML_API_KEY
             environment variable will be used. If that does not exist, the value in the
-            user's config file will be used. If that does not exist, a MAPIException will
-            be thrown.
+            user's config file will be used. If that does not exist, then the access token
+            will be used.
+        access_token: The access token in the Main Container.
         endpoint: The MAPI URL to hit for all requests. If not specified, the value of the
             $MOSAICML_API_ENDPOINT environment variable will be used. If that does not
             exist, the default setting will be used.
         pool: An optional threadpool to use for all connection requests. If not provided,
             a shared pool will be used for all requests.
 
     Raises:
         MAPIException: Raised if the user does not have an API key set
     """
     api_key: str
+    access_token: str
     endpoint: str
 
     def __init__(self,
                  api_key: Optional[str] = None,
                  endpoint: Optional[str] = None,
                  pool: Optional[ThreadPoolExecutor] = None):
         self._load_from_environment(api_key, endpoint)
@@ -109,14 +102,16 @@
             api_key = conf.api_key
 
         if not api_key:
             api_key = ''
 
         self.api_key = api_key
 
+        self.access_token = conf.access_token
+
         if endpoint is None:
             endpoint = conf.endpoint
         self.endpoint = endpoint
 
     @staticmethod
     def _set_connection(connection: Optional[MAPIConnection]) -> None:
         """Set the current connection instance
@@ -132,14 +127,28 @@
         """The ThreadPoolExecutor that will contain all MAPI requests
         """
         if self._pool is None:
             self._pool = THREADPOOL or _create_threadpool()
 
         return self._pool
 
+    @property
+    def request_header(self):
+        if len(self.api_key) == 0 and len(self.access_token) == 0:
+            raise MCLIConfigError(ERROR_AUTH_KEY_MISSING)
+
+        # Use the API key to auth, if specified. Otherwise, use the JWT token
+        auth = self.api_key if len(self.api_key) != 0 else f'Bearer {self.access_token}'
+        return {
+            'Authorization': auth,
+            'Content-Type': 'application/json',
+            'x-mosaicml-client': 'mcli',
+            'x-mosaicml-client-version': __version__
+        }
+
     def create_websocket_connection(self) -> Client:
         if self._client is None:
             # Start the event loop if it's not already running
             if not self._loop.is_running():
                 logger.debug("Starting threaded asyncio event loop")
                 self.pool.submit(start_background_loop, self._loop, self._terminate)
 
@@ -163,15 +172,15 @@
 
     @property
     def client(self) -> Client:
         return self.create_websocket_connection()
 
     async def _create_gql_client(self) -> Client:
         ws_endpoint = self.endpoint.replace("http://", "ws://").replace("https://", "wss://")
-        headers = get_common_header({'Authorization': self.api_key})
+        headers = self.request_header
         logger.debug(f"Connecting to websocket server at endpoint {ws_endpoint}")
         transport = WebsocketsTransport(url=ws_endpoint, init_payload=headers)
         return Client(transport=transport, fetch_schema_from_transport=False)
 
     def subscribe(
         self,
         query: DocumentNode,
@@ -411,15 +420,15 @@
         exception status codes
     """
     if not connection:
         connection = MAPIConnection.get_current_connection()
 
     future = connection.pool.submit(
         _threaded_plural_mapi_request,
-        api_key=connection.api_key,
+        headers=connection.request_header,
         endpoint=connection.endpoint,
         query=query,
         variables=variables,
         query_function=query_function,
         model_type=return_model_type,
     )
     future = cast('Future[List[ModelT]]', future)
@@ -455,61 +464,57 @@
         exception status codes
     """
     if not connection:
         connection = MAPIConnection.get_current_connection()
 
     future = connection.pool.submit(
         _threaded_paginated_mapi_request,
-        api_key=connection.api_key,
+        headers=connection.request_header,
         endpoint=connection.endpoint,
         query=query,
         variables=variables,
         query_function=query_function,
         model_type=return_model_type,
     )
     future = cast('Future[List[ModelT]]', future)
 
     return future
 
 
 def _threaded_paginated_mapi_request(
-    api_key: str,
+    headers: Dict[str, str],
     endpoint: str,
     query: str,
     variables: Optional[Dict[str, Any]],
     query_function: str,
     model_type: Optional[Type[ModelT]],
 ) -> List[ModelT]:
     """Run a graphql request in a thread and return a list of items
     """
-    if not api_key:
-        raise MCLIConfigError(ERROR_API_KEY_MISSING)
     try:
-        response = _run_graphql_request(api_key, endpoint, query, variables)
+        response = _run_graphql_request(headers, endpoint, query, variables)
     except requests.exceptions.ConnectionError as e:
         mapi_error = MAPIException.from_requests_error(e)
         raise mapi_error from e
 
     return _deserialize_response(response, query_function, model_type, paginated=True)
 
 
 def _threaded_plural_mapi_request(
-    api_key: str,
+    headers: Dict[str, str],
     endpoint: str,
     query: str,
     variables: Optional[Dict[str, Any]],
     query_function: str,
     model_type: Optional[Type[ModelT]],
 ) -> List[ModelT]:
     """Run a graphql request in a thread and return a list of items
     """
-    if not api_key:
-        raise MCLIConfigError(ERROR_API_KEY_MISSING)
     try:
-        response = _run_graphql_request(api_key, endpoint, query, variables)
+        response = _run_graphql_request(headers, endpoint, query, variables)
     except requests.exceptions.ConnectionError as e:
         mapi_error = MAPIException.from_requests_error(e)
         raise mapi_error from e
 
     return _deserialize_response(response, query_function, model_type)
 
 
@@ -540,87 +545,66 @@
         exception status codes
     """
     if not connection:
         connection = MAPIConnection.get_current_connection()
 
     future = connection.pool.submit(
         _threaded_singular_mapi_request,
-        api_key=connection.api_key,
+        headers=connection.request_header,
         endpoint=connection.endpoint,
         query=query,
         variables=variables,
         query_function=query_function,
         model_type=return_model_type,
     )
     future = cast('Future[ModelT]', future)
 
     return future
 
 
 def _threaded_singular_mapi_request(
-    api_key: str,
+    headers: Dict[str, str],
     endpoint: str,
     query: str,
     variables: Optional[Dict[str, Any]],
     query_function: str,
     model_type: Optional[Type[ModelT]],
 ) -> ModelT:
     """Run a graphql request in a thread and return a single item
 
     Raises:
         MAPIException: Raised if no items were found
     """
 
     items = _threaded_plural_mapi_request(
-        api_key=api_key,
+        headers=headers,
         endpoint=endpoint,
         query=query,
         variables=variables,
         query_function=query_function,
         model_type=model_type,
     )
     if len(items) == 1:
         return items[0]
     else:
         raise MAPIException(status=HTTPStatus.INTERNAL_SERVER_ERROR,
                             message='Request returned no items, but expected 1')
 
 
-def _threaded_empty_mapi_request(
-    api_key: str,
-    endpoint: str,
-    query: str,
-    variables: Optional[Dict[str, Any]],
-    query_function: str,
-) -> None:
-    """Run a graphql request in a thread and return None if the request succeeded
-    """
-
-    _ = _threaded_plural_mapi_request(
-        api_key=api_key,
-        endpoint=endpoint,
-        query=query,
-        variables=variables,
-        query_function=query_function,
-        model_type=None,
-    )
-
-
 def _run_graphql_request(
-    api_key: str,
+    headers: Dict[str, str],
     endpoint: str,
     query: str,
     variables: Optional[Dict[str, Any]] = None,
 ) -> Dict[str, Any]:
 
     if variables is None:
         variables = {}
     variables = {key.replace('$', ''): value for key, value in variables.items()}
 
-    headers = get_common_header({'authorization': api_key})
     payload = json.dumps({'query': query, 'variables': variables})
 
     # Don't want timeout since this will be run in a background thread
     # pylint: disable-next=missing-timeout
     response = requests.request(
         'POST',
         endpoint,
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/exceptions.py` & `mosaicml-cli-0.5.0/mcli/api/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from websockets.exceptions import ConnectionClosedError, InvalidStatusCode
 
 from mcli.utils.utils_logging import FAIL
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_MESSAGE = 'Unknown Error'
-ERROR_API_KEY_MISSING = 'No API key found. Please create one and set it using `mcli set api-key`.'
+ERROR_AUTH_KEY_MISSING = 'No API key or auth token was found. To create an API key, use `mcli set api-key`.'
 
 
 class MCLIException(Exception):
     """Base custom exception that MCLI will raise
 
     All errors should inherit this base so that expected errors can be properly caught
     """
@@ -49,14 +49,81 @@
 
 
 class MCLIDeploymentConfigValidationError(MCLIException):
     """Exception raised when DeploymentConfig cannot be finalized
     """
 
 
+class InferenceServerException(MCLIException):
+    """Exception raised when inference deployment server requests fail
+    """
+    status: HTTPStatus
+    message: str
+    e: Exception
+    description: Optional[str] = None
+
+    def __init__(self, status: HTTPStatus, message: str = DEFAULT_MESSAGE, description: Optional[str] = None):
+        super().__init__()
+        self.status = status
+        self.message = message
+        self.description = description
+
+    def __str__(self) -> str:
+        error_message = f'Inference Deployment Server Error {self.status.value}: {self.message}'
+
+        if self.description:
+            error_message = f'{error_message}. {self.description}'
+
+        return error_message
+
+    @classmethod
+    def from_server_error_response(cls, error: str, code: int) -> InferenceServerException:
+        """Initializes a new exception based on error dict from a Infernece Server response
+        """
+        try:
+            status = HTTPStatus(code)
+        except ValueError:
+            logger.debug(f'Unknown status code {code}. Setting to 500')
+            status = HTTPStatus.INTERNAL_SERVER_ERROR
+
+        message = error if error else DEFAULT_MESSAGE
+        description = None
+        if code == 503:
+            description = """Inference deployment could not be reached. It is likely
+            either not yet ready or is currently failing. Check `mcli describe deployment
+            <deployment>` and if the deployment is failing, try `mcli get deployment logs <deployment>`
+            to see what\'s wrong"""
+
+        return InferenceServerException(status=status, message=message, description=description)
+
+    @classmethod
+    def from_bad_response(cls, response: requests.Response) -> InferenceServerException:
+        return InferenceServerException(
+            status=HTTPStatus(response.status_code),
+            message=response.reason,
+        )
+
+    @classmethod
+    def from_requests_error(cls, error: requests.exceptions.RequestException) -> InferenceServerException:
+        """Initializes a new exception based on a requests RequestException
+        """
+        msg = 'Unable to connect'
+        if error.args:
+            con = error.args[0]
+            try:
+                # Try to get the destination we tried to connect to
+                # if the app is fully not accessible
+                source = f'http://{con.pool.host}{con.url}'
+            except AttributeError:
+                pass
+            else:
+                msg = f'{msg} to {source}'
+        return InferenceServerException(status=HTTPStatus.SERVICE_UNAVAILABLE, message=msg)
+
+
 class MAPIException(MCLIException):
     """Exceptions raised when a request to MAPI fails
 
     Args:
         status: The status code for the exception
         message: A brief description of the error
         description: An optional longer description of the error
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.5.0/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     future: bool = False,
 ):
     """Delete an inference deployment in the MosaicML Cloud
 
     If it is currently running the deployment will first be stopped.
 
     Args:
-        deploymnet: An inference deployments or inference deployment name to delete
+        deployment: An inference deployments or inference deployment name to delete
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised. If ``future`` is ``True``, this
             value will be ignored.
         future: Return the output as a :type concurrent.futures.Future:. If True, the
             call to `delete_inference_deployments` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the :type InferenceDeployment: output, use ``return_value.result()``
@@ -111,15 +111,15 @@
     future: bool = False,
 ):
     """Delete a list of inference deployments in the MosaicML Cloud
 
     Any deployments that are currently running will first be stopped.
 
     Args:
-        deploymnets: A list of inference deployments or inference deployment names to delete
+        deployments: A list of inference deployments or inference deployment names to delete
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised. If ``future`` is ``True``, this
             value will be ignored.
         future: Return the output as a :type concurrent.futures.Future:. If True, the
             call to `delete_inference_deployments` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the :type InferenceDeployment: output, use ``return_value.result()``
@@ -134,18 +134,15 @@
     filters = {}
     if deployment_names:
         filters['name'] = {'in': deployment_names}
 
     variables = {VARIABLE_DATA_NAME: {'filters': filters}}
 
     cfg = MCLIConfig.load_config()
-    if cfg.user_id:
-        variables[VARIABLE_DATA_NAME]['entity'] = {
-            'userIds': [cfg.user_id],
-        }
+    cfg.update_entity(variables[VARIABLE_DATA_NAME], set_user=False)
 
     response = run_plural_mapi_request(
         query=QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=InferenceDeployment,
         variables=variables,
     )
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_get_inference_deployment_logs.py` & `mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_get_inference_deployment_logs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from concurrent.futures import Future
 from typing import Any, Dict, Generator, Optional, Union, overload
 
 from typing_extensions import Literal
 
 from mcli.api.model.inference_deployment import InferenceDeployment
 from mcli.api.runs.api_get_run_logs import _get_logs
+from mcli.config import MCLIConfig
 
 QUERY_FUNCTION = 'getInferenceDeploymentLogs'
 VARIABLE_DATA_NAME = 'getInferenceDeploymentLogsInput'
 QUERY = f"""
 subscription Subscription(${VARIABLE_DATA_NAME}: GetInferenceDeploymentLogsInput!) {{
     {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME})
 }}"""
@@ -77,14 +78,18 @@
     deployment_name = deployment.name if isinstance(deployment, InferenceDeployment) else deployment
 
     filters: Dict[str, Any] = {'name': deployment_name}
     if restart:
         filters['restartCount'] = restart
 
     variables = {VARIABLE_DATA_NAME: filters}
+
+    cfg = MCLIConfig.load_config()
+    cfg.update_entity(variables[VARIABLE_DATA_NAME], set_user=False)
+
     for message in _get_logs(QUERY, variables, QUERY_FUNCTION):
         if not future:
             try:
                 yield message.result(timeout)
             except StopAsyncIteration:
                 break
         else:
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,16 +193,15 @@
         VARIABLE_DATA_NAME: {
             'filters': filters,
             'includeDeleted': False,
         },
     }
 
     cfg = MCLIConfig.load_config()
-    if cfg.user_id:
-        variables[VARIABLE_DATA_NAME]['entity'] = {'userIds': [cfg.user_id]}
+    cfg.update_entity(variables[VARIABLE_DATA_NAME], set_user=False)
 
     response = run_plural_mapi_request(
         query=QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=InferenceDeployment,
         variables=variables,
     )
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_ping.py` & `mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_ping.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from http import HTTPStatus
 from typing import Callable, Optional, Union, cast
 
 import requests
 import validators
 from requests import Response
 
-from mcli.api.exceptions import MAPIException
+from mcli.api.exceptions import InferenceServerException, MAPIException
 from mcli.api.inference_deployments import get_inference_deployments
 from mcli.api.model.inference_deployment import InferenceDeployment
 
 __all__ = ['ping']
 
 
 def ping(
@@ -38,14 +38,15 @@
         deployment_objs = get_inference_deployments(deployments=[deployment])
         if len(deployment_objs) == 0:
             raise MAPIException(HTTPStatus.NOT_FOUND, f'No inference deployment found with name {deployment}.')
         deployment = deployment_objs[0]
     base_url = deployment
     if isinstance(deployment, InferenceDeployment):
         base_url = f'https://{deployment.public_dns}'
-    resp: Response = requests.get(url=f'{base_url}/ping', timeout=timeout)
-
-    if resp.ok:
-        return {"status": resp.status_code}
-    else:
-        resp.raise_for_status()
-        return {}
+    try:
+        resp: Response = requests.get(url=f'{base_url}/ping', timeout=timeout)
+        if resp.ok:
+            return {"status": resp.status_code}
+        else:
+            raise InferenceServerException.from_server_error_response(resp.content.decode().strip(), resp.status_code)
+    except requests.exceptions.ConnectionError as e:
+        raise InferenceServerException.from_requests_error(e) from e
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from typing import Any, Callable, Dict, Optional, Union, cast
 
 import requests
 import validators
 from requests import Response
 
 from mcli import config
-from mcli.api.exceptions import MAPIException
+from mcli.api.exceptions import InferenceServerException, MAPIException
 from mcli.api.inference_deployments import get_inference_deployments
 from mcli.api.model.inference_deployment import InferenceDeployment
 
 __all__ = ['predict']
 
 
 def predict(
     deployment: Union[InferenceDeployment, str],
     inputs: Dict[str, Any],
     *,
     timeout: Optional[float] = 20,
-) -> dict:
-    """Sends input to \'/predict\' endpoint of an inference deployment on the MosaicML
+) -> Dict[str, Any]:
+    """Sends input to \'/infer\' endpoint of an inference deployment on the MosaicML
     platform. Runs prediction on input and returns output produced by the model.
     Arguments:
         deployment: The deployment to make a prediction with. Can be a InferenceDeployment object,
             the name of an deployment, or a string which is of the form https://<deployment dns>.
         input: Input data to run prediction on in the form of dictionary
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised.
@@ -45,13 +45,18 @@
     api_key = conf.api_key
     headers = {
         'authorization': api_key,
     }
     base_url = deployment
     if isinstance(deployment, InferenceDeployment):
         base_url = f'https://{deployment.public_dns}'
-    resp: Response = requests.post(url=f'{base_url}/predict', timeout=timeout, json=inputs, headers=headers)
-    if resp.ok:
-        return resp.json()
-    else:
-        resp.raise_for_status()
-        return {}
+    try:
+        resp: Response = requests.post(url=f'{base_url}/predict', timeout=timeout, json=inputs, headers=headers)
+        if resp.ok:
+            try:
+                return resp.json()
+            except requests.JSONDecodeError as e:
+                raise InferenceServerException.from_bad_response(resp) from e
+        else:
+            raise InferenceServerException.from_server_error_response(resp.content.decode().strip(), resp.status_code)
+    except requests.exceptions.ConnectionError as e:
+        raise InferenceServerException.from_requests_error(e) from e
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/inference_deployments/api_update_inference_deployments.py` & `mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_update_inference_deployments.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,31 +64,35 @@
     deployment: Optional[Union[str, InferenceDeployment]],
     updates: Dict[str, Any],
     *,
     timeout: Optional[float] = 10,
     future: bool = False,
 ):
     """Updates a single inference deployment that has been launched in the MosaicML platform
+
     Any deployments that are currently running will not be interrupted.
+
     Args:
-        deployments: A list of inference deployments or inference deployment names to update
+        deployment: An inference deployment or inference deployment name to update
         updates: A dictionary of inference deployment fields to update
-            (eg. {image: 'new_image', replicas: 2})
+            (eg. {"image": "new_image", "replicas": 2})
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised. If ``future`` is ``True``, this
             value will be ignored.
         future: Return the output as a :type concurrent.futures.Future:. If True, the
             call to `update_inference_deployments` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the :type InferenceDeployment: output, use ``return_value.result()``
             with an optional ``timeout`` argument.
-    Returns:
-        A list of :type InferenceDeployment: for the inference deployments that were updated
+
     Raises:
-        MAPIException: Raised when a MAPI communication error occurs
+        MAPIException: Raised if updating the deployment failed
+
+    Returns:
+        A :type InferenceDeployment: for the deployment that was updated
     """
     deployments = cast(Union[List[str], List[InferenceDeployment]], [deployment])
     name = deployment.name if isinstance(deployment, InferenceDeployment) else deployment
     error_message = f"Deployment {name} not found"
 
     if future:
         res = update_inference_deployments(deployments=deployments, updates=updates, timeout=None, future=True)
@@ -125,48 +129,51 @@
 def update_inference_deployments(
     deployments: Union[List[str], List[InferenceDeployment]],
     updates: Dict[str, Any],
     *,
     timeout: Optional[float] = 10,
     future: bool = False,
 ):
-    """Update a list of inference deployments in the MosaicML Cloud
+    """Updates a list of inference deployments that have been launched in the MosaicML platform
+
     Any deployments that are currently running will not be interrupted.
+
     Args:
         deployments: A list of inference deployments or inference deployment names to update
         updates: A dictionary of inference deployment fields to update
-            (eg. {image: 'new_image', replicas: 2})
+            (eg. {"image": "new_image", "replicas": 2})
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised. If ``future`` is ``True``, this
             value will be ignored.
         future: Return the output as a :type concurrent.futures.Future:. If True, the
             call to `update_inference_deployments` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the :type InferenceDeployment: output, use ``return_value.result()``
             with an optional ``timeout`` argument.
+
+    Raises:
+        MAPIException: Raised if updating the deployments failed
+
     Returns:
-        A list of :type InferenceDeployment: for the inference deployments that were updated
+        A list of :type InferenceDeployment: for the deployments that were updated
     """
     # Extract deployment names
     variables = {
         VARIABLE_DATA_GET_DEPLOYMENTS: {
             'filters': {
                 'name': {
                     'in': [d.name if isinstance(d, InferenceDeployment) else d for d in deployments]
                 },
             }
         },
         VARIABLE_DATA_UPDATE_DEPLOYMENTS: updates,
     }
 
     cfg = MCLIConfig.load_config()
-    if cfg.user_id:
-        variables[VARIABLE_DATA_GET_DEPLOYMENTS]['entity'] = {
-            'userIds': [cfg.user_id],
-        }
+    cfg.update_entity(variables[VARIABLE_DATA_GET_DEPLOYMENTS], set_user=False)
 
     response = run_plural_mapi_request(
         query=QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=InferenceDeployment,
         variables=variables,
     )
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/mint/shell.py` & `mosaicml-cli-0.5.0/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/api/mint/tty.py` & `mosaicml-cli-0.5.0/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/api/model/__init__.py` & `mosaicml-cli-0.5.0/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.5.0/mcli/api/model/cluster_details.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,93 +8,161 @@
 from typing import Any, Dict, List, Optional, Set
 
 from dateutil import parser
 
 from mcli.api.exceptions import MAPI_DESERIALIZATION_ERROR
 from mcli.api.schema.generic_model import DeserializableModel
 from mcli.models.run_config import SchedulingConfig, SchedulingTranslation
+from mcli.utils.utils_model import SubmissionType
 from mcli.utils.utils_serializable_dataclass import SerializableDataclass
 
 logger = logging.getLogger(__name__)
 
 
 def check_response(response: Dict[str, Any], expected: Set[str]) -> None:
     missing = expected - set(response)
     if missing:
         raise MAPI_DESERIALIZATION_ERROR
 
 
 @dataclass
+class ClusterUtilizationByDeployment:
+    """Utilization for a specific run on a cluster
+    """
+
+    id: str
+    user: str
+    name: str
+    gpu_num: int
+    instance: str
+    created_at: datetime
+    scheduling: SchedulingConfig = field(default_factory=SchedulingConfig)  # Never used. Only for linting
+
+    @property
+    def display_name(self) -> str:
+        return self.name
+
+    @classmethod
+    def from_mapi_response(cls, response: Dict[str, Any]) -> ClusterUtilizationByDeployment:
+        check_response(response, {'id', 'userName', 'deploymentName', 'gpuNum', 'createdAt', 'instance'})
+        return cls(id=response['id'],
+                   user=response['userName'],
+                   name=response['deploymentName'],
+                   gpu_num=response['gpuNum'],
+                   instance=response['instance'],
+                   created_at=parser.parse(response['createdAt']))
+
+
+@dataclass
 class ClusterUtilizationByRun:
     """Utilization for a specific run on a cluster
     """
 
     id: str
     user: str
-    run_name: str
+    name: str
+    run_name: str  #DEPRECATE
     gpu_num: int
+    instance: str
     created_at: datetime
     scheduling: SchedulingConfig
 
+    @property
+    def display_name(self) -> str:
+        if self.scheduling.get('retry_on_system_failure'):
+            return f'{self.name} 🐕'
+
+        return self.name
+
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> ClusterUtilizationByRun:
-        check_response(response, {'id', 'userName', 'runName', 'gpuNum', 'createdAt'})
+        check_response(response, {'id', 'userName', 'runName', 'gpuNum', 'createdAt', 'instance'})
         return cls(id=response['id'],
                    user=response['userName'],
                    run_name=response['runName'],
+                   name=response['runName'],
                    gpu_num=response['gpuNum'],
+                   instance=response['instance'],
                    created_at=parser.parse(response['createdAt']),
                    scheduling=SchedulingTranslation.from_mapi(response.get('scheduling', {})))
 
 
 @dataclass
 class InstanceUtilization:
     """Utilization on a cluster instance
     """
     cluster_id: str
+    name: str
     gpu_type: str
     gpus_per_node: int
     num_nodes: int
     gpus_used: int
     gpus_available: int
     gpus_total: int
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> InstanceUtilization:
-        check_response(response,
-                       {'clusterId', 'gpuType', 'gpusPerNode', 'numNodes', 'gpusUsed', 'gpusAvailable', 'gpusTotal'})
+        check_response(
+            response,
+            {'clusterId', 'name', 'gpuType', 'gpusPerNode', 'numNodes', 'gpusUsed', 'gpusAvailable', 'gpusTotal'})
         return cls(
             cluster_id=response['clusterId'],
+            name=response['name'],
             gpu_type=response['gpuType'],
             gpus_per_node=response['gpusPerNode'],
             num_nodes=response['numNodes'],
             gpus_used=response['gpusUsed'],
             gpus_available=response['gpusAvailable'],
             gpus_total=response['gpusTotal'],
         )
 
+    def __gt__(self, other: InstanceUtilization):
+        return self.gpus_available == 0 or self.name > other.name
+
 
 @dataclass
 class ClusterUtilization:
     """Utilization on a cluster
     """
     anonymize_users: bool
     cluster_instance_utils: List[InstanceUtilization] = field(default_factory=list)
-    active_by_user: List[ClusterUtilizationByRun] = field(default_factory=list)
-    queued_by_user: List[ClusterUtilizationByRun] = field(default_factory=list)
+    active_by_user: List[ClusterUtilizationByRun] = field(default_factory=list)  #DEPRECATE
+    queued_by_user: List[ClusterUtilizationByRun] = field(default_factory=list)  #DEPRECATE
+    active_runs_by_user: List[ClusterUtilizationByRun] = field(default_factory=list)
+    queued_runs_by_user: List[ClusterUtilizationByRun] = field(default_factory=list)
+    active_deployments_by_user: List[ClusterUtilizationByDeployment] = field(default_factory=list)
+    queued_deployments_by_user: List[ClusterUtilizationByDeployment] = field(default_factory=list)
+
+    def get_submissions(self, submission_type: SubmissionType, is_active: bool):
+        if submission_type is SubmissionType.TRAINING:
+            return self.active_by_user if is_active else self.queued_by_user
+        else:
+            return self.active_deployments_by_user if is_active else self.queued_deployments_by_user
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> ClusterUtilization:
-        check_response(response, {'clusterInstanceUtils', 'activeByUser', 'queuedByUser', 'anonymizeUsers'})
-        return cls(cluster_instance_utils=[
-            InstanceUtilization.from_mapi_response(i) for i in response['clusterInstanceUtils']
-        ],
-                   active_by_user=[ClusterUtilizationByRun.from_mapi_response(i) for i in response['activeByUser']],
-                   queued_by_user=[ClusterUtilizationByRun.from_mapi_response(i) for i in response['queuedByUser']],
-                   anonymize_users=response['anonymizeUsers'])
+        check_response(
+            response, {
+                'clusterInstanceUtils', 'activeRunsByUser', 'queuedRunsByUser', 'activeDeploymentsByUser',
+                'queuedDeploymentsByUser', 'anonymizeUsers'
+            })
+        return cls(
+            cluster_instance_utils=sorted(
+                [InstanceUtilization.from_mapi_response(i) for i in response['clusterInstanceUtils']]),
+            active_by_user=[ClusterUtilizationByRun.from_mapi_response(i) for i in response['activeRunsByUser']],
+            queued_by_user=[ClusterUtilizationByRun.from_mapi_response(i) for i in response['queuedRunsByUser']],
+            active_runs_by_user=[ClusterUtilizationByRun.from_mapi_response(i) for i in response['activeRunsByUser']],
+            queued_runs_by_user=[ClusterUtilizationByRun.from_mapi_response(i) for i in response['queuedRunsByUser']],
+            active_deployments_by_user=[
+                ClusterUtilizationByDeployment.from_mapi_response(i) for i in response['activeDeploymentsByUser']
+            ],
+            queued_deployments_by_user=[
+                ClusterUtilizationByDeployment.from_mapi_response(i) for i in response['queuedDeploymentsByUser']
+            ],
+            anonymize_users=response['anonymizeUsers'])
 
 
 @dataclass
 class Node:
     """Node on an instance for a cluster
     """
     name: str
@@ -157,15 +225,15 @@
     """
 
     name: str
     provider: str = 'MosaicML'
     allow_fractional: bool = False
     allow_multinode: bool = False
     cluster_instances: List[Instance] = field(default_factory=list)
-    submission_type: str = ''
+    submission_type: SubmissionType = field(default_factory=SubmissionType)
     utilization: Optional[ClusterUtilization] = None
 
     kubernetes_context: str = ''
     namespace: str = ''
 
     id: Optional[str] = None
 
@@ -175,13 +243,13 @@
         utilization = None if 'utilization' not in response else ClusterUtilization.from_mapi_response(
             response['utilization'])
         return cls(name=response['name'],
                    provider=get_provider_name(response.get('provider', '')),
                    allow_fractional=response.get('allowFractional', False),
                    allow_multinode=response.get('allowMultinode', False),
                    cluster_instances=[Instance.from_mapi_response(i) for i in response.get('allowedInstances', [])],
-                   submission_type=str(response.get('allowedSubmissionType', '')),
+                   submission_type=SubmissionType.from_mapi(response.get('allowedSubmissionType', '')),
                    utilization=utilization,
                    id=response.get('id'))
 
     def __lt__(self, other: ClusterDetails):
         return self.name < other.name
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.5.0/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/api/model/run.py` & `mosaicml-cli-0.5.0/mcli/api/model/run.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,14 +25,58 @@
         return Node(rank=response.get('rank', 0), name=response.get('name', 'Unknown'))
 
     def to_dict(self):
         return {"rank": str(self.rank), "name": self.name}
 
 
 @dataclass
+class Resumption:
+    """Data from a run resumption. The first instantiation of a Run will
+         have a Resumption with index `0`
+    """
+
+    index: int
+    cluster: str
+    gpus: int
+    cpus: int
+    gpu_type: str
+    node_count: int
+    status: RunStatus
+    started_at: Optional[datetime] = None
+    ended_at: Optional[datetime] = None
+
+    @classmethod
+    def from_mapi_response(cls, response: Dict[str, Any]) -> Resumption:
+        return Resumption(
+            index=response['executionIndex'],
+            cluster=response['clusterName'],
+            gpus=response['gpus'],
+            cpus=response['cpus'],
+            gpu_type=response['gpuType'],
+            node_count=response['nodes'],
+            status=RunStatus.from_string(response['status']),
+            started_at=convert_datetime(response['startTime']) if response['startTime'] else None,
+            ended_at=convert_datetime(response['endTime']) if response['endTime'] else None,
+        )
+
+    def to_dict(self):
+        return {
+            "index": self.index,
+            "cluster": self.cluster,
+            "gpus": str(self.gpus),
+            "cpus": str(self.cpus),
+            "gpu_type": self.gpu_type,
+            "node_count": str(self.node_count),
+            "status": str(self.status),
+            "started_at": str(self.started_at),
+            "ended_at": str(self.ended_at),
+        }
+
+
+@dataclass
 class RunLifecycle:
     """Status of a run at a moment in time
     """
 
     resumption_id: int
     status: RunStatus
     started_at: datetime
@@ -89,22 +133,24 @@
     retry_on_system_failure: bool
     cluster: str
     gpus: int
     gpu_type: str
     cpus: int
     node_count: int
 
+    latest_resumption: Resumption
     max_retries: Optional[int] = None
     started_at: Optional[datetime] = None
     completed_at: Optional[datetime] = None
     reason: Optional[str] = None
     nodes: List[Node] = field(default_factory=list)
     submitted_config: Optional[RunConfig] = None
     metadata: Optional[Dict[str, Any]] = None
     last_resumption_id: Optional[str] = None
+    resumptions: List[Resumption] = field(default_factory=list)
     lifecycle: List[RunLifecycle] = field(default_factory=list)
     image: Optional[str] = None
 
     _required_properties: Tuple[str] = tuple([
         'id',
         'name',
         'status',
@@ -112,15 +158,15 @@
         'completedAt',
         'updatedAt',
         'reason',
         'createdByEmail',
         'priority',
         'preemptible',
         'retryOnSystemFailure',
-        'lastExecution',
+        'resumptions',
     ])
 
     def _get_time_in_status(self, status: RunStatus) -> float:
         """Returns the time spent in a given status
 
         Args:
             status (:class:`~mcli.utils.utils_run_status.RunStatus`): The status to get the time for
@@ -135,14 +181,26 @@
                     ended = status_update.ended_at
                     if not ended:
                         ended = datetime.now(tz=status_update.started_at.tzinfo)
                     res += (ended - status_update.started_at).total_seconds()
         return res
 
     @property
+    def display_name(self) -> str:
+        """The name of the run to display in the CLI
+
+        Returns:
+            The name of the run
+        """
+        if self.retry_on_system_failure:
+            return f'{self.name} 🐕'
+
+        return self.name
+
+    @property
     def cumulative_pending_time(self) -> float:
         """Cumulative time spent in the PENDING state
 
         Returns:
             The cumulative time (seconds) spent in the PENDING state
         """
         return self._get_time_in_status(RunStatus.PENDING)
@@ -153,45 +211,49 @@
 
         Returns:
             The cumulative time (seconds) spent in the RUNNING state
         """
         return self._get_time_in_status(RunStatus.RUNNING)
 
     @property
-    def resumptions(self) -> int:
+    def resumption_count(self) -> int:
         """Number of times the run has been resumed
 
         Returns:
             The number of times the run has been resumed
         """
-        return len({i.resumption_id for i in self.lifecycle})
+        return len(self.resumptions)
 
     def clone(
         self,
         name: Optional[str] = None,
         image: Optional[str] = None,
         cluster: Optional[str] = None,
         instance: Optional[str] = None,
         nodes: Optional[int] = None,
         gpu_type: Optional[str] = None,
         gpus: Optional[int] = None,
         priority: Optional[str] = None,
+        preemptible: Optional[bool] = None,
+        max_retries: Optional[int] = None,
     ) -> Run:
         """
         Submits a new run with the same configuration as this run
 
         Args:
             name (str): Override the name of the run
             image (str): Override the image of the run
             cluster (str): Override the cluster of the run
             instance (str): Override the instance of the run
             nodes (int): Override the number of nodes of the run
             gpu_type (str): Override the GPU type of the run
             gpus (int): Override the number of GPUs of the run
             priority (str): Override the priority of the run
+            preemptible (bool): Override whether the run can be stopped and re-queued by higher priority jobs
+            max_retries (int): Override the max number of times the run can be retried
 
         Returns:
             New :class:`~mcli.api.model.run.Run` object
         """
         # pylint: disable-next=import-outside-toplevel
         from mcli.api.runs import create_run
 
@@ -218,14 +280,18 @@
             submitted_config.compute['nodes'] = nodes
         if gpu_type:
             submitted_config.compute['gpu_type'] = gpu_type
         if gpus is not None:
             submitted_config.compute['gpus'] = gpus
         if priority:
             submitted_config.scheduling['priority'] = priority
+        if preemptible is not None:
+            submitted_config.scheduling['preemptible'] = preemptible
+        if max_retries is not None:
+            submitted_config.scheduling['max_retries'] = max_retries
 
         return create_run(submitted_config)
 
     def refresh(self) -> Run:
         """
         Refreshes the data on the run object
 
@@ -256,14 +322,43 @@
         Returns:
             Deleted :class:`~mcli.api.model.run.Run` object
         """
         # pylint: disable-next=import-outside-toplevel
         from mcli.api.runs import delete_run
         return delete_run(self)
 
+    def update(self,
+               preemptible: Optional[bool] = None,
+               priority: Optional[str] = None,
+               max_retries: Optional[int] = None,
+               retry_on_system_failure: Optional[bool] = None) -> Run:
+        """
+        Updates the run's data
+
+        Args:
+            preemptible (bool): Update whether the run can be stopped and re-queued by higher priority jobs;
+                default is False
+            priority (str): Update the priority of the run to `low`, `medium`, or `high`; default is `medium`
+            max_retries (int): Update the max number of times the run can be retried; default is 0
+            retry_on_system_failure (bool): Update whether the run should be retried on system failure
+                (i.e. a node failure); default is False
+
+        Returns:
+            Updated :class:`~mcli.api.model.run.Run` object
+        """
+        # pylint: disable-next=import-outside-toplevel
+        from mcli.api.runs import update_run
+        return update_run(
+            self,
+            preemptible=preemptible,
+            priority=priority,
+            max_retries=max_retries,
+            retry_on_system_failure=retry_on_system_failure,
+        )
+
     def update_metadata(self, metadata: Dict[str, Any]) -> Run:
         """
         Updates the run's metadata
 
         Args:
             metadata (`Dict[str, Any]`): The metadata to update the run with. This will be merged with
                 the existing metadata. Keys not specified in this dictionary will not be modified.
@@ -289,33 +384,38 @@
         if response['startedAt'] is not None:
             started_at = convert_datetime(response['startedAt'])
 
         completed_at = None
         if response['completedAt'] is not None:
             completed_at = convert_datetime(response['completedAt'])
 
+        resumptions = [Resumption.from_mapi_response(r) for r in response['resumptions']]
+        latest_resumption = resumptions[-1]
+
         args = {
             'run_uid': response['id'],
             'name': response['name'],
             'created_at': convert_datetime(response['createdAt']),
             'started_at': started_at,
             'completed_at': completed_at,
             'updated_at': convert_datetime(response['updatedAt']),
             'status': RunStatus.from_string(response['status']),
             'reason': response['reason'],
             'created_by': response['createdByEmail'],
             'priority': response['priority'],
             'max_retries': response.get('maxRetries'),
             'preemptible': response['preemptible'],
+            'resumptions': resumptions,
+            'latest_resumption': latest_resumption,
             'retry_on_system_failure': response['retryOnSystemFailure'],
-            'cluster': response['lastExecution']['clusterName'],
-            'gpus': response['lastExecution']['gpus'],
-            'gpu_type': response['lastExecution']['gpuType'],
-            'cpus': response['lastExecution']['cpus'],
-            'node_count': response['lastExecution']['nodes'],
+            'cluster': latest_resumption.cluster,
+            'gpus': latest_resumption.gpus,
+            'gpu_type': latest_resumption.gpu_type,
+            'cpus': latest_resumption.cpus,
+            'node_count': latest_resumption.node_count,
         }
 
         details = response.get('details', {})
         if details:
             submitted_run_input = details.get('originalRunInput')
             args['submitted_config'] = RunConfig.from_mapi_response(
                 submitted_run_input) if submitted_run_input is not None else None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/runs/__init__.py` & `mosaicml-cli-0.5.0/mcli/api/runs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from mcli.api.model.run import Run
 from mcli.api.runs.api_create_run import create_run
 from mcli.api.runs.api_delete_runs import delete_run, delete_runs
 from mcli.api.runs.api_get_run_logs import follow_run_logs, get_run_logs
 from mcli.api.runs.api_get_runs import get_run, get_runs
 from mcli.api.runs.api_start_run import start_run, start_runs
 from mcli.api.runs.api_stop_runs import stop_run, stop_runs
+from mcli.api.runs.api_update_run import update_run
 from mcli.api.runs.api_update_run_metadata import update_run_metadata
 from mcli.api.runs.api_watch_run import wait_for_run_status, watch_run_status
 from mcli.models import ComputeConfig, FinalRunConfig, RunConfig, SchedulingConfig
 from mcli.utils.utils_run_status import RunStatus
 
 __all__ = [
     'ComputeConfig',
@@ -29,10 +30,11 @@
     'get_runs',
     'get_run',
     'start_run',
     'start_runs',
     'stop_run',
     'stop_runs',
     'update_run_metadata',
+    'update_run',
     'wait_for_run_status',
     'watch_run_status',
 ]
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.5.0/mcli/api/runs/api_create_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,20 +26,24 @@
     completedAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
-    lastExecution {{
+    resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
+        executionIndex
+        startTime
+        endTime
+        status
     }}
     details {{
         originalRunInput
         metadata
         lastExecutionId
     }}
   }}
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.5.0/mcli/api/runs/api_delete_runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,20 +26,24 @@
     completedAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
-    lastExecution {{
+    resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
+        executionIndex
+        startTime
+        endTime
+        status
     }}
   }}
 }}"""
 
 
 @overload
 def delete_run(
@@ -144,18 +148,15 @@
     filters = {}
     if run_names:
         filters['name'] = {'in': run_names}
 
     variables = {VARIABLE_DATA_NAME: {'filters': filters}}
 
     cfg = MCLIConfig.load_config()
-    if cfg.user_id:
-        variables[VARIABLE_DATA_NAME]['entity'] = {
-            'userIds': [cfg.user_id],
-        }
+    cfg.update_entity(variables[VARIABLE_DATA_NAME])
 
     response = run_plural_mapi_request(
         query=QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=Run,
         variables=variables,
     )
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.5.0/mcli/api/runs/api_get_run_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,18 +93,15 @@
     if rank is not None:
         filters['nodeRank'] = rank
 
     if resumption is not None:
         filters['attemptIndex'] = resumption
 
     cfg = MCLIConfig.load_config()
-    if cfg.user_id:
-        filters['entity'] = {
-            'userIds': [cfg.user_id],
-        }
+    cfg.update_entity(filters)
 
     variables = {VARIABLE_DATA_NAME: filters}
     for message in _get_logs(QUERY, variables, QUERY_FUNCTION):
         if not future:
             try:
                 yield message.result(timeout)
             except StopAsyncIteration:
@@ -181,18 +178,15 @@
     if rank is not None:
         filters['nodeRank'] = rank
 
     if resumption is not None:
         filters['attemptIndex'] = resumption
 
     cfg = MCLIConfig.load_config()
-    if cfg.user_id:
-        filters['entity'] = {
-            'userIds': [cfg.user_id],
-        }
+    cfg.update_entity(filters)
 
     variables = {VARIABLE_DATA_NAME: filters}
     for message in _get_logs(QUERY, variables, QUERY_FUNCTION):
         if not future:
             try:
                 yield message.result(timeout)
             except StopAsyncIteration:
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.5.0/mcli/api/runs/api_get_runs.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,20 +33,24 @@
     updatedAt
     reason
     createdByEmail
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
-    lastExecution {{
+    resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
+        executionIndex
+        startTime
+        endTime
+        status
     }}
   }}
 }}"""
 
 QUERY_WITH_DETAILS = f"""
 query GetRuns(${VARIABLE_DATA_NAME}: GetRunsInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
@@ -59,20 +63,24 @@
     updatedAt
     reason
     createdByEmail
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
-    lastExecution {{
+    resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
+        executionIndex
+        startTime
+        endTime
+        status
     }}
     details {{
         image
         originalRunInput
         metadata
         lastExecutionId
         lifecycle {{
@@ -105,20 +113,24 @@
     updatedAt
     reason
     createdByEmail
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
-    lastExecution {{
+    resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
+        executionIndex
+        startTime
+        endTime
+        status
     }}
   }}
   }}
 }}"""
 
 
 @overload
@@ -180,69 +192,67 @@
     res = get_runs(runs=runs, timeout=timeout, future=False, include_details=include_details)
     if not res:
         raise MAPIException(HTTPStatus.NOT_FOUND, error_message)
     return res[0]
 
 
 @overload
-def get_runs(
-    runs: Optional[Union[List[str], List[Run]]] = None,
-    *,
-    cluster_names: Optional[Union[List[str], List[Cluster]]] = None,
-    before: Optional[Union[str, datetime]] = None,
-    after: Optional[Union[str, datetime]] = None,
-    gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
-    gpu_nums: Optional[List[int]] = None,
-    statuses: Optional[Union[List[str], List[RunStatus]]] = None,
-    timeout: Optional[float] = 10,
-    future: Literal[False] = False,
-    clusters: Optional[Union[List[str], List[Cluster]]] = None,
-    user_emails: Optional[List[str]] = None,
-    include_details: bool = False,
-    limit: Optional[int] = None,
-) -> List[Run]:
+def get_runs(runs: Optional[Union[List[str], List[Run]]] = None,
+             *,
+             cluster_names: Optional[Union[List[str], List[Cluster]]] = None,
+             before: Optional[Union[str, datetime]] = None,
+             after: Optional[Union[str, datetime]] = None,
+             gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
+             gpu_nums: Optional[List[int]] = None,
+             statuses: Optional[Union[List[str], List[RunStatus]]] = None,
+             timeout: Optional[float] = 10,
+             future: Literal[False] = False,
+             clusters: Optional[Union[List[str], List[Cluster]]] = None,
+             user_emails: Optional[List[str]] = None,
+             include_details: bool = False,
+             limit: Optional[int] = None,
+             include_interactive: Optional[bool] = None) -> List[Run]:
     ...
 
 
 @overload
-def get_runs(
-    runs: Optional[Union[List[str], List[Run]]] = None,
-    *,
-    cluster_names: Optional[Union[List[str], List[Cluster]]] = None,
-    before: Optional[Union[str, datetime]] = None,
-    after: Optional[Union[str, datetime]] = None,
-    gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
-    gpu_nums: Optional[List[int]] = None,
-    statuses: Optional[Union[List[str], List[RunStatus]]] = None,
-    timeout: Optional[float] = None,
-    future: Literal[True] = True,
-    clusters: Optional[Union[List[str], List[Cluster]]] = None,
-    user_emails: Optional[List[str]] = None,
-    include_details: bool = False,
-    limit: Optional[int] = None,
-) -> Future[List[Run]]:
+def get_runs(runs: Optional[Union[List[str], List[Run]]] = None,
+             *,
+             cluster_names: Optional[Union[List[str], List[Cluster]]] = None,
+             before: Optional[Union[str, datetime]] = None,
+             after: Optional[Union[str, datetime]] = None,
+             gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
+             gpu_nums: Optional[List[int]] = None,
+             statuses: Optional[Union[List[str], List[RunStatus]]] = None,
+             timeout: Optional[float] = None,
+             future: Literal[True] = True,
+             clusters: Optional[Union[List[str], List[Cluster]]] = None,
+             user_emails: Optional[List[str]] = None,
+             include_details: bool = False,
+             limit: Optional[int] = None,
+             include_interactive: Optional[bool] = None) -> Future[List[Run]]:
     ...
 
 
 def get_runs(
-    runs: Optional[Union[List[str], List[Run]]] = None,
-    *,
-    cluster_names: Optional[Union[List[str], List[Cluster]]] = None,
-    before: Optional[Union[str, datetime]] = None,
-    after: Optional[Union[str, datetime]] = None,
-    gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
-    gpu_nums: Optional[List[int]] = None,
-    statuses: Optional[Union[List[str], List[RunStatus]]] = None,
-    timeout: Optional[float] = 10,
-    future: bool = False,
-    clusters: Optional[Union[List[str], List[Cluster]]] = None,  # TODO: deprecate
-    user_emails: Optional[List[str]] = None,
-    include_details: bool = False,
-    limit: Optional[int] = None,
-):
+        runs: Optional[Union[List[str], List[Run]]] = None,
+        *,
+        cluster_names: Optional[Union[List[str], List[Cluster]]] = None,
+        before: Optional[Union[str, datetime]] = None,
+        after: Optional[Union[str, datetime]] = None,
+        gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
+        gpu_nums: Optional[List[int]] = None,
+        statuses: Optional[Union[List[str], List[RunStatus]]] = None,
+        timeout: Optional[float] = 10,
+        future: bool = False,
+        clusters: Optional[Union[List[str], List[Cluster]]] = None,  # TODO: deprecate
+        user_emails: Optional[List[str]] = None,
+        include_details: bool = False,
+        limit: Optional[int] = None,
+        include_interactive: Optional[bool] = None):
     """List runs that have been launched in the MosaicML platform
 
     The returned list will contain all of the details stored about the requested runs.
 
     Arguments:
         runs: List of runs on which to get information
         cluster_names: List of cluster names to filter runs. This can be a list of str or
@@ -266,14 +276,15 @@
         future: Return the output as a :type concurrent.futures.Future:. If True, the
             call to `get_runs` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the list of runs, use ``return_value.result()``
             with an optional ``timeout`` argument.
         include_details: If true, will fetch detailed information like run input for each run.
         limit: Maximum number of runs to return. If None, all runs will be returned.
+        include_interactive: Whether the run is interactive or not. If None, all runs will be returned.
 
     Raises:
         MAPIException: If connecting to MAPI, raised when a MAPI communication error occurs
     """
     # We could support run details in pagination, but it goes against the point of the paginated view:
     # This is a view that is meant to be used for listing runs, not for fetching detailed information
     if limit and include_details:
@@ -288,33 +299,36 @@
             date_filters['lt'] = before.astimezone().isoformat() if isinstance(before, datetime) else before
         if after:
             date_filters['gte'] = after.astimezone().isoformat() if isinstance(after, datetime) else after
         filters['createdAt'] = date_filters
     if statuses:
         filters['status'] = {'in': [s.value.upper() if isinstance(s, RunStatus) else s.upper() for s in statuses]}
 
-    cluster_names = cluster_names or clusters  # for backwards compatibility, clusters is supported as cluster_names
+    # for backwards compatibility, clusters is supported as cluster_names
+    cluster_names = cluster_names or clusters
     if cluster_names:
         filters['clusterName'] = {'in': [c.name if isinstance(c, Cluster) else c for c in cluster_names]}
     if gpu_types:
         filters['gpuType'] = {'in': [gt.value if isinstance(gt, GPUType) else gt for gt in gpu_types]}
     if gpu_nums:
         filters['gpuNum'] = {'in': gpu_nums}
 
+    if include_interactive is not None:
+        filters['isInteractive'] = {'equals': include_interactive}
+
     variable_name = VARIABLE_DATA_NAME if limit is None else VARIABLE_DATA_NAME_PAGINATED
     variables = {
         variable_name: {
             'filters': filters,
             'includeDeleted': False,
         },
     }
 
     cfg = MCLIConfig.load_config()
-    if cfg.user_id:
-        variables[variable_name]['entity'] = {'userIds': [cfg.user_id]}
+    cfg.update_entity(variables[variable_name])
     if user_emails:
         if variables[variable_name].get('entity'):
             variables[variable_name]['entity']['emails'] = user_emails
         else:
             variables[variable_name]['entity'] = {'emails': user_emails}
 
     if limit is None:
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.5.0/mcli/api/runs/api_start_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,24 @@
     completedAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
-    lastExecution {{
+   resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
+        executionIndex
+        startTime
+        endTime
+        status
     }}
   }}
 }}"""
 
 
 @overload
 def start_run(
@@ -161,18 +165,15 @@
     filters = {}
     if run_names:
         filters['name'] = {'in': run_names}
 
     variables = {VARIABLE_DATA_NAME: {'filters': filters}}
 
     cfg = MCLIConfig.load_config()
-    if cfg.user_id:
-        variables[VARIABLE_DATA_NAME]['entity'] = {
-            'userIds': [cfg.user_id],
-        }
+    cfg.update_entity(variables[VARIABLE_DATA_NAME])
 
     response = run_plural_mapi_request(
         query=QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=Run,
         variables=variables,
     )
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.5.0/mcli/api/runs/api_stop_runs.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,20 +26,24 @@
     completedAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
-    lastExecution {{
+    resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
+        executionIndex
+        startTime
+        endTime
+        status
     }}
   }}
 }}"""
 
 
 @overload
 def stop_run(
@@ -164,18 +168,15 @@
     filters = {}
     if run_names:
         filters['name'] = {'in': run_names}
 
     variables = {VARIABLE_DATA_NAME: {'filters': filters}}
 
     cfg = MCLIConfig.load_config()
-    if cfg.user_id:
-        variables[VARIABLE_DATA_NAME]['entity'] = {
-            'userIds': [cfg.user_id],
-        }
+    cfg.update_entity(variables[VARIABLE_DATA_NAME])
 
     response = run_plural_mapi_request(
         query=QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=Run,
         variables=variables,
     )
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.5.0/mcli/api/runs/api_update_run_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,20 +27,24 @@
     completedAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
-    lastExecution {{
+    resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
+        executionIndex
+        startTime
+        endTime
+        status
     }}
     details {{
         metadata
     }}
   }}
 }}"""
 
@@ -105,18 +109,15 @@
         },
         VARIABLE_DATA_UPDATE_RUN_METADATA: {
             'metadata': metadata
         },
     }
 
     cfg = MCLIConfig.load_config()
-    if cfg.user_id:
-        variables[VARIABLE_DATA_GET_RUNS]['entity'] = {
-            'userIds': [cfg.user_id],
-        }
+    cfg.update_entity(variables[VARIABLE_DATA_GET_RUNS])
 
     response = run_singular_mapi_request(
         query=QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=Run,
         variables=variables,
     )
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.5.0/mcli/api/runs/api_watch_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,18 +247,14 @@
 
     @staticmethod
     def _get_description(state: RunStatus) -> str:
         if state == RunStatus.QUEUED:
             return 'Waiting for resources to become available...'
         elif state == RunStatus.STARTING:
             return 'Pulling Docker image...'
-        elif state == RunStatus.SCHEDULED:
-            return 'Instance found. Waiting for run to start...'
-        elif state == RunStatus.FAILED_PULL:
-            return 'Failed to pull Docker image...'
         else:
             return state.value.title().replace('_', ' ') + '...'
 
     def follow(self) -> Run:
         run = self.run
         for run in watch_run_status(self.run):
             self.progress.update(self._task,
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.5.0/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.5.0/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.5.0/mcli/api/secrets/api_delete_secrets.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,18 +82,15 @@
     variables = {
         VARIABLE_DATA_NAME: {
             'filters': filters,
         },
     }
 
     cfg = MCLIConfig.load_config()
-    if cfg.user_id:
-        variables[VARIABLE_DATA_NAME]['entity'] = {
-            'userIds': [cfg.user_id],
-        }
+    cfg.update_entity(variables[VARIABLE_DATA_NAME])
 
     response = run_plural_mapi_request(
         query=QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=Secret,
         variables=variables,
     )
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.5.0/mcli/api/secrets/api_get_secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,15 @@
     variables = {
         VARIABLE_DATA_NAME: {
             'filters': filters,
         },
     }
 
     cfg = MCLIConfig.load_config()
-    if cfg.user_id:
-        variables[VARIABLE_DATA_NAME]['entity'] = {'userIds': [cfg.user_id]}
+    cfg.update_entity(variables[VARIABLE_DATA_NAME])
 
     response = run_plural_mapi_request(
         query=QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=Secret,
         variables=variables,
     )
```

### Comparing `mosaicml-cli-0.4.9/mcli/api/typing_future.py` & `mosaicml-cli-0.5.0/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.5.0/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/api/utils.py` & `mosaicml-cli-0.5.0/mcli/api/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/cli.py` & `mosaicml-cli-0.5.0/mcli/cli/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 #!/usr/bin/env python
 # PYTHON_ARGCOMPLETE_OK
 
 """ MCLI Entrypoint """
 import argparse
-import itertools
 import logging
 import sys
-from string import ascii_lowercase
 from typing import Tuple
 
-import argcomplete
-
 from mcli import config
 from mcli.cli.m_connect.m_connect import add_connect_argparser
 from mcli.cli.m_create.m_create import add_create_argparser
 from mcli.cli.m_delete.m_delete import add_delete_argparser
 from mcli.cli.m_deploy.m_deploy import add_deploy_argparser
 from mcli.cli.m_describe.m_describe import add_describe_parser
 from mcli.cli.m_get.m_get import add_get_argparser
 from mcli.cli.m_init.m_init import initialize_mcli
-from mcli.cli.m_interactive.interactive import add_interactive_argparser
-from mcli.cli.m_interactive.m_interactive import add_interactive_argparser as kube_interactive_argparser
+from mcli.cli.m_interactive.m_interactive import add_interactive_argparser
 from mcli.cli.m_kube.m_kube import add_kube_argparser
 from mcli.cli.m_log.m_log import add_log_parser
 from mcli.cli.m_ping.m_ping import add_ping_parser
 from mcli.cli.m_predict.m_predict import add_predict_parser
 from mcli.cli.m_root.m_config import m_get_config
 from mcli.cli.m_run.m_run import add_run_argparser
 from mcli.cli.m_set_unset.m_set import add_set_argparser
 from mcli.cli.m_set_unset.m_unset import add_unset_argparser
 from mcli.cli.m_stop.m_stop import add_stop_parser
+from mcli.cli.m_update.m_update import add_update_argparser
 from mcli.cli.m_util.m_util import add_util_argparser
-from mcli.config import FeatureFlag, MCLIConfig
-from mcli.utils.utils_cli import MCLIArgumentParser, SubmissionType
+from mcli.cli.m_watchdog.m_watchdog import add_watchdog_argparser
+from mcli.utils.utils_cli import MCLIArgumentParser
+from mcli.utils.utils_completers import apply_autocomplete
 from mcli.utils.utils_logging import console_handler
+from mcli.utils.utils_model import SubmissionType
 from mcli.utils.utils_pypi import NeedsUpdateError, check_new_update_available
 from mcli.version import get_formatted_version, print_version
 
 logger = logging.getLogger('mcli')
 logger.setLevel(logging.INFO)
 logger.addHandler(console_handler)
 
@@ -93,36 +91,32 @@
     add_root_commands(subparser=subparser)
     return parser, subparser
 
 
 def get_parser(is_admin: bool = False) -> argparse.ArgumentParser:
     parser, subparser = get_mcli_root('mcli' if not is_admin else 'mcli-admin')
 
-    conf = MCLIConfig.load_config()
-
-    if conf.feature_enabled(FeatureFlag.MCLOUD_INTERACTIVE):
-        add_connect_argparser(subparser=subparser)
-        add_interactive_argparser(subparser=subparser)
-    elif conf.allow_interactive:
-        kube_interactive_argparser(subparser=subparser)
-
+    add_connect_argparser(subparser=subparser)
     add_create_argparser(subparser=subparser)
     add_delete_argparser(subparser=subparser)
     add_deploy_argparser(subparser=subparser)
     add_describe_parser(subparser=subparser)
     add_get_argparser(subparser=subparser, is_admin=is_admin)
+    add_interactive_argparser(subparser=subparser)
+    add_kube_argparser(subparser=subparser)
     add_log_parser(subparser=subparser, submission_type=SubmissionType.TRAINING)
     add_ping_parser(subparser=subparser)
     add_predict_parser(subparser=subparser)
-    add_kube_argparser(subparser=subparser)
     add_run_argparser(subparser=subparser)
-    add_stop_parser(subparser=subparser)
-    add_util_argparser(subparser=subparser)
+    add_update_argparser(subparser=subparser)
     add_set_argparser(subparser=subparser, is_admin=is_admin)
+    add_stop_parser(subparser=subparser)
     add_unset_argparser(subparser=subparser, is_admin=is_admin)
+    add_util_argparser(subparser=subparser)
+    add_watchdog_argparser(subparser=subparser)
 
     return parser
 
 
 def _main(parser: argparse.ArgumentParser) -> int:
     try:
         check_new_update_available()
@@ -162,19 +156,13 @@
     return _main(parser)
 
 
 def main() -> int:
     """The main entrypoint
     """
     parser = get_parser()
-
-    aliases = list(ascii_lowercase) + [''.join(i) for i in itertools.product(ascii_lowercase, repeat=2)]
-    argcomplete.autocomplete(
-        parser,
-        exclude=aliases,
-        always_complete_options='long',  # type: ignore
-    )
+    apply_autocomplete(parser)
     return _main(parser)
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.5.0/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.5.0/mcli/cli/common/run_filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,39 +4,43 @@
 import functools
 import logging
 from typing import Dict, List, Optional, Tuple
 
 from mcli.api.exceptions import MCLIException
 from mcli.api.model.run import Run
 from mcli.api.runs.api_get_runs import get_runs
-from mcli.utils.utils_cli import SubmissionType, comma_separated, date_time_parse
+from mcli.utils import utils_completers
+from mcli.utils.utils_cli import comma_separated, date_time_parse
+from mcli.utils.utils_model import SubmissionType
 from mcli.utils.utils_run_status import RunStatus
 from mcli.utils.utils_spinner import console_status
 from mcli.utils.utils_string_functions import is_glob
 
 logger = logging.getLogger(__name__)
 
 
 def configure_submission_filter_argparser(action: str,
                                           parser: argparse.ArgumentParser,
                                           include_all: bool = True,
                                           submission_type: SubmissionType = SubmissionType.TRAINING) -> None:
-    parser.add_argument(
+    cluster_parser = parser.add_argument(
         '-c',
         '--cluster',
         '-p',
         '--platform',
         dest='cluster_filter',
         metavar='CLUSTER',
         type=comma_separated,
         default=None,
         help=f'{action.capitalize()} {submission_type.value}s on the specified cluster(s). If no other arguments are '
         f'provided, will {action} all {submission_type.value}s on the specified cluster(s). Multiple clusters '
         'should be specified using a comma-separated list, e.g. "cluster1,cluster2"',
     )
+    cluster_parser.completer = utils_completers.ClusterNameCompleter()  # pyright: ignore
+
     parser.add_argument(
         '--before',
         dest='before_filter',
         metavar='DATE/TIME',
         nargs='?',
         type=date_time_parse,
         help=f'{action.capitalize()} {submission_type.value}s created before specific time. Datetimes must be '
@@ -47,58 +51,64 @@
         dest='after_filter',
         metavar='DATE/TIME',
         nargs='?',
         type=date_time_parse,
         help=f'{action.capitalize()} {submission_type.value}s created after specific time. Datetimes must be '
         'surrounded by \'\'. e.g 2023-01-01 or 01-13-2023 or 12:30:23.4 or \'01-13-2023 19:20:21.9\'',
     )
-    parser.add_argument(
+    gpu_type_parser = parser.add_argument(
         '-t',
         '--gpu-type',
         dest='gpu_type_filter',
         metavar='GPU',
         default=None,
         type=comma_separated,
         help=f'{action.capitalize()} {submission_type.value}s with specific GPU type. '
         'Multiple types should be specified using a comma-separated list, e.g. "a100_40gb,v100_16gb"',
     )
+    gpu_type_parser.completer = utils_completers.GPUTypeCompleter()  # pyright: ignore
+
     parser.add_argument(
         '-n',
         '--gpu-num',
         dest='gpu_num_filter',
         metavar='# GPUs',
         default=None,
         type=functools.partial(comma_separated, fun=int),
         help=f'{action.capitalize()} {submission_type.value}s with specific number of GPUs. '
         'Multiple values should be specified using a comma-separated list, e.g. "1,8"',
     )
 
     def status(value: str):
-        if submission_type.value == SubmissionType.TRAINING:
+        if submission_type is SubmissionType.TRAINING:
             res = comma_separated(value, RunStatus.from_string)
             if res == [RunStatus.UNKNOWN] and value != [RunStatus.UNKNOWN.value]:
                 raise TypeError(f'Unknown value {value}')
             return res
         else:
             res = comma_separated(value)
             return res
 
-    parser.add_argument(
+    status_parser = parser.add_argument(
         '-s',
         '--status',
         dest='status_filter',
         default=None,
         metavar='STATUS',
         type=status,
         help=f'{action.capitalize()} {submission_type.value}s with the specified statuses (choices: '
-        f'{", ".join(submission_type.get_status_options())}). Multiple statuses should be specified '
+        f'{", ".join(SubmissionType.get_status_options(submission_type))}). Multiple statuses should be specified '
         'using a comma-separated list, e.g. "failed,pending"',
     )
+    if submission_type is SubmissionType.TRAINING:
+        status_parser.completer = utils_completers.RunStatusCompleter()  # pyright: ignore
+    else:
+        status_parser.completer = utils_completers.DeploymentStatusCompleter()  # pyright: ignore
 
-    if submission_type == SubmissionType.TRAINING:
+    if submission_type is SubmissionType.TRAINING:
         parser.add_argument(
             '-l',
             '--latest',
             action='store_true',
             dest='latest',
             default=False,
             help=f'Connect to the latest {submission_type.value}',
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.5.0/mcli/cli/m_connect/m_connect.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ mcli connect Entrypoint """
 import argparse
 import logging
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 from mcli.api.exceptions import MintException
 from mcli.api.mint import shell
 from mcli.api.model.run import Run, RunStatus
 from mcli.api.runs.api_get_runs import get_run, get_runs
 from mcli.api.runs.api_watch_run import EpilogSpinner as CloudEpilogSpinner
 from mcli.cli.m_get.display import format_timestamp
@@ -38,47 +38,52 @@
         return False
 
     common_log.log_unknown_did_not_start()
     logger.debug(last_status)
     return False
 
 
+def get_runs_to_connect_to(limit: Optional[int] = 10):
+    return get_runs(statuses=[
+        RunStatus.STARTING,
+        RunStatus.RUNNING,
+    ], limit=limit, include_interactive=True)
+
+
 def connect_entrypoint(
     name: Optional[str] = None,
     rank: int = 0,
     latest: bool = False,
     command: Optional[str] = None,
     tmux: Optional[bool] = None,
+    runs: Optional[List[Run]] = None,
     **kwargs,
 ):
     del kwargs
 
     if name:
         run = get_run(name)
     else:
         # If a user doesn't specify a run name, get all starting and running runs
-        available_runs = get_runs(statuses=[RunStatus.STARTING, RunStatus.RUNNING])
+        # When runs are passed in, don't perform another query
+        available_runs = runs or get_runs_to_connect_to()
         if not available_runs:
             logger.error(f'{FAIL} No running runs available to connect to')
             return 1
         elif len(available_runs) == 1:
             # Only one run, connect to this one automatically
             run = available_runs[0]
         else:
             # Multiple options for runs to connect to...
             sorted_runs = sorted(available_runs, key=lambda x: x.created_at, reverse=True)
 
             if latest:
                 # User specified --latest
                 run = sorted_runs[0]
             else:
-                # User didn't specify --latest, so prompt them to choose
-                if len(available_runs) > 10:
-                    # Only show the latest 10 to make the dropdown small
-                    available_runs = sorted_runs[:10]
 
                 def name_formatter(r: Run):
                     if r.started_at:
                         details = f'Started at {format_timestamp(r.started_at)}'
                     else:
                         details = 'Not yet started'
                     return f'{r.name} ({details})'
@@ -137,22 +142,31 @@
     command_grp.add_argument(
         '--tmux',
         action='store_true',
         help='Use tmux as the entrypoint for your run so your session is robust to disconnects',
     )
 
 
+class RunConnectorCompleter:
+
+    def __init__(self, limit: Optional[int] = None):
+        self.limit = limit
+
+    def __call__(self, **kwargs):
+        return get_runs_to_connect_to(limit=self.limit)
+
+
 def configure_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     parser.add_argument(
         'name',
         metavar='RUN',
         default=None,
         nargs='?',
         help='Run name',
-    )
+    ).completer = RunConnectorCompleter()  # pyright: ignore
 
     parser.add_argument(
         '-l',
         '--latest',
         action='store_true',
         dest='latest',
         default=False,
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.5.0/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.5.0/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.5.0/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.5.0/mcli/cli/m_delete/m_delete.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ m delete Entrypoint """
 import argparse
 from typing import List, Optional
 
 from mcli.cli.common.run_filters import configure_submission_filter_argparser
 from mcli.cli.m_delete.delete import delete_deployment, delete_run, delete_secret
-from mcli.utils.utils_cli import CLIExample, Description, SubmissionType, get_example_text
+from mcli.utils.utils_cli import CLIExample, Description, get_example_text
+from mcli.utils.utils_model import SubmissionType
 
 # pylint: disable-next=invalid-name
 _description = Description("""
 The table below shows the objects that you can delete. For each object below, you can
 delete or more of them by name. Each object also supports glob-style selection and --all
 to delete all.
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.5.0/mcli/cli/m_deploy/m_deploy.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import textwrap
 from http import HTTPStatus
 from typing import Optional
 
 from mcli.api.exceptions import MAPIException, MCLIDeploymentConfigValidationError
 from mcli.api.inference_deployments.api_create_inference_deployment import create_inference_deployment
 from mcli.models.inference_deployment_config import InferenceDeploymentConfig
+from mcli.utils import utils_completers
 from mcli.utils.utils_logging import FAIL, OK
 
 logger = logging.getLogger(__name__)
 
 
 def print_help(**kwargs) -> int:
     del kwargs
@@ -95,26 +96,28 @@
     parser.add_argument(
         '-f',
         '--file',
         dest='file',
         help='File from which to load arguments.',
     )
 
-    parser.add_argument(
+    cluster_parser = parser.add_argument(
         '--cluster',
         dest='override_cluster',
         help='Optional override for MCLI cluster',
     )
+    cluster_parser.completer = utils_completers.ClusterNameCompleter()  # pyright: ignore
 
-    parser.add_argument(
+    gpu_type_parser = parser.add_argument(
         '--gpu-type',
         dest='override_gpu_type',
         help='Optional override for GPU type. Valid GPU type depend on'
         ' the cluster and GPU number requested',
     )
+    gpu_type_parser.completer = utils_completers.GPUTypeCompleter()  # pyright: ignore
 
     parser.add_argument(
         '--gpus',
         type=int,
         dest='override_gpu_num',
         help='Optional override for number of GPUs. Valid GPU numbers '
         'depend on the cluster and GPU type',
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.5.0/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.5.0/mcli/cli/m_describe/describe_runs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """Implementation of mcli describe run"""
 from __future__ import annotations
 
 import logging
+from copy import deepcopy
 from dataclasses import asdict, dataclass
+from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, Generator, List, Optional, Tuple, TypeVar
 
+from rich import print as rprint
+from rich.columns import Columns
+from rich.panel import Panel
 from rich.table import Table
 
 from mcli.api.exceptions import cli_error_handler
-from mcli.api.model.run import Node, Run, RunLifecycle
+from mcli.api.model.run import Node, Run, RunLifecycle, RunStatus
 from mcli.cli.common.run_filters import get_runs_with_filters
 from mcli.cli.m_get.display import (MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, create_vertical_display_table,
                                     format_timestamp)
 from mcli.models.run_config import ComputeConfig
 from mcli.utils.utils_logging import FormatString, console, format_string, print_timedelta, seconds_to_str
 
 logger = logging.getLogger(__name__)
@@ -27,55 +32,71 @@
     COMPLETED = 'COMPLETED'
 
 
 class DescribeRunDetailColumns(Enum):
     NAME = 'name'
     RUN_ID = 'run_uid'
     LAST_RESUMPTION_ID = 'last_resumption_id'
+    USER = 'user'
     CLUSTER = 'cluster'
     GPU_TYPE = 'gpu_type'
     GPU_NUM = 'gpu_num'
     CPUS = 'cpus'
     IMAGE = 'image'
     PRIORITY = 'priority'
+    STATUS = 'status'
+    PREEMPTIBLE = 'preemptible'
+    REASON = 'reason'
+    WATCHDOG = 'watchdog'
 
 
 class DescribeRunOriginalInputColumns(Enum):
     SUBMITTED_CONFIG = 'submitted_config'
 
 
-RUN_DETAIL_DISPLAY_NAMES = ['Run Name', 'Run ID', 'Last Resumption ID', 'Cluster', 'Image', 'Priority']
-
+RUN_DETAIL_DISPLAY_NAMES = [
+    'Run Name', 'Run ID', 'Last Resumption ID', 'User', 'Cluster', 'Image', 'Priority', 'Status', 'Preemptible',
+    'Reason', 'Watchdog'
+]
 RUN_LIFECYCLE_DISPLAY_NAMES = ['Status', 'Reached At', 'Duration', 'Reason']
 RUN_NODES_DISPLAY_NAMES = ['Node Name']
 SUBMITTED_CONFIG = ['Run Config']
 
 
 @dataclass
 class DescribeRunDetailDisplayItem(MCLIDisplayItem):
     """Tuple that extracts detailed run data for display purposes"""
     name: str
     run_uid: str
     last_resumption_id: str
+    user: str
     cluster: str
     image: str
     last_resumption_id: str
     priority: str
+    status: str
+    preemptible: bool
+    reason: str
+    watchdog: str
 
     @classmethod
     def from_run(cls, run: Run) -> DescribeRunDetailDisplayItem:
         extracted: Dict[str, Any] = {
             DescribeRunDetailColumns.NAME.value: run.name,
             DescribeRunDetailColumns.RUN_ID.value: run.run_uid,
             DescribeRunDetailColumns.LAST_RESUMPTION_ID.value: run.last_resumption_id,
+            DescribeRunDetailColumns.USER.value: run.created_by,
             DescribeRunDetailColumns.CLUSTER.value: run.cluster,
             DescribeRunDetailColumns.IMAGE.value: run.image,
-            DescribeRunDetailColumns.PRIORITY.value: run.priority.lower(),
+            DescribeRunDetailColumns.PRIORITY.value: run.priority.lower().capitalize(),
+            DescribeRunDetailColumns.STATUS.value: run.status.name.lower().capitalize(),
+            DescribeRunDetailColumns.PREEMPTIBLE.value: run.preemptible,
+            DescribeRunDetailColumns.REASON.value: run.reason,
+            DescribeRunDetailColumns.WATCHDOG.value: run.retry_on_system_failure,
         }
-
         return DescribeRunDetailDisplayItem(**extracted)
 
 
 @dataclass
 class DescribeRunLifecycleDisplayItem(MCLIDisplayItem):
     """Tuple that extracts run data for run lifecycle display purposes"""
     resumption: str
@@ -102,60 +123,134 @@
 
 # Displays
 class MCLIDescribeRunDetailsDisplay(MCLIGetDisplay):
     """ Vertical table view of run details """
 
     def __init__(self, models: List[Run]):
         self.models = sorted(models, key=lambda x: x.created_at, reverse=True)
+        self.include_reason_in_display = any(m.reason for m in models)
 
     @property
     def index_label(self) -> str:
         return ""
 
     def create_custom_table(self, columns: List[str], data: List[Tuple[Any, ...]], names: List[str]) -> Optional[Table]:
-        return create_vertical_display_table(data=data, columns=RUN_DETAIL_DISPLAY_NAMES)
+        column_names = RUN_DETAIL_DISPLAY_NAMES
+        if not self.include_reason_in_display:
+            column_names = deepcopy(RUN_DETAIL_DISPLAY_NAMES)
+            column_names.remove('Reason')
+        return create_vertical_display_table(data=data, columns=column_names)
 
     def __iter__(self) -> Generator[DescribeRunDetailDisplayItem, None, None]:
         for model in self.models:
             item = DescribeRunDetailDisplayItem.from_run(model)
             yield item
 
 
-class MCLIDescribeRunLifecycleDisplay(MCLIGetDisplay):
-    """ Horizontal table view of run lifecycle """
+def format_lifecycle_event(run_name, event: RunLifecycle) -> str:
+    # TODO: move lifecycle event parsing to MAPI
+    if event.status == RunStatus.COMPLETED:
+        return 'Run completed successfully'
+    elif event.status == RunStatus.FAILED:
+        failed_with = ''
+        if event.reason:
+            failed_with = f' with exit code {event.reason}'
+        log_tail = ''
+        if event.resumption_id > 0:
+            log_tail = f' --resumption {event.resumption_id})'
+
+        return f'Run failed{failed_with}\n' + \
+            f'See logs with [blue]mcli logs {run_name}{log_tail}'
+    elif event.status == RunStatus.STOPPED:
+        if event.reason == 'Preempted':
+            return 'Run was preempted'
+        elif event.reason == 'Node Failure':
+            return 'Run was stopped due to node failure'
+    elif event.status == RunStatus.RUNNING:
+        if event.resumption_id == 0:
+            return 'Run started'
+        else:
+            return 'Run resumed'
+    elif event.status == RunStatus.PENDING:
+        if event.resumption_id == 0:
+            return 'Run created'
+        else:
+            return 'Run placed back in the scheduling queue'
+    # We don't want to inundate the user with all Run Statuses,
+    # so let's hide other statuses for now
+    return ''
+
+
+def format_event_log(run_name: str, lifecycle: List[RunLifecycle]) -> Table:
+    grid = Table(title='Event Log', expand=False, padding=(0, 2, 0, 2))
+    grid.add_column(header='Time', justify='left')
+    grid.add_column(header='Resumption', justify='left')
+    grid.add_column(header='Event', justify='left')
+
+    lifecycle = sorted(lifecycle, key=lambda x: (x.resumption_id, x.started_at))
+    current_attempt = 0
+    for event in lifecycle:
+        if event.resumption_id != current_attempt:
+            grid.add_section()
+            current_attempt = event.resumption_id
+        text = format_lifecycle_event(run_name=run_name, event=event)
+        if len(text) > 0:
+            grid.add_row(format_timestamp(event.started_at), str(event.resumption_id), text)
+    return grid
+
+
+def create_lifecycle_event_panel(event: RunLifecycle) -> Panel:
+    duration = print_timedelta(event.ended_at - event.started_at) if event.ended_at else '-'
+    panel_string = event.status.name.lower().capitalize()
+
+    for_description = '\n'
+    if duration and duration != '-':
+        for_description = f'\nFor: {duration}'
+    return Panel(f"At: {format_timestamp(event.started_at)}{for_description}", expand=False, title=panel_string)
 
-    def __init__(self, model: List[RunLifecycle]):
-        self.model = model
-        self.include_reason_in_display = any(m.reason for m in model)
 
-    @property
-    def custom_column_names(self) -> List[str]:
-        if self.include_reason_in_display:
-            return RUN_LIFECYCLE_DISPLAY_NAMES
-        else:
-            return RUN_LIFECYCLE_DISPLAY_NAMES[:-1]
+class MCLIDescribeRunLifecycleDisplay():
+    """ Panel view of run lifecycle """
 
-    def __iter__(self) -> Generator[DescribeRunLifecycleDisplayItem, None, None]:
-        last_index: Optional[int] = None
-        for e in self.model:
-            duration = ''
-            if e.started_at and e.ended_at:
-                duration = print_timedelta(e.ended_at - e.started_at)
-            yield DescribeRunLifecycleDisplayItem(
-                resumption=str(e.resumption_id) if last_index != e.resumption_id else '',
-                status=e.status.display_name,
-                reached_at=format_timestamp(e.started_at),
-                duration=duration,
-                reason=e.reason or '',
-            )
-            last_index = e.resumption_id
+    def __init__(self, model: List[RunLifecycle], created_at: datetime):
+        self.created_at = created_at
+        self.model = model
+        self.include_reason_in_display = any(m.reason for m in model)
 
-    @property
-    def index_label(self) -> str:
-        return 'resumption'
+    def print(self):
+        # Build the visual panels for Run Lifecycle
+        current_resumption = 0
+        all_columns = []
+        curr_columns = []
+        for event in self.model:
+            if current_resumption != event.resumption_id:
+                all_columns.append(Columns(curr_columns))
+                curr_columns = [create_lifecycle_event_panel(event)]
+                current_resumption = event.resumption_id
+            else:
+                curr_columns.append(create_lifecycle_event_panel(event))
+        # add the last resumption's events
+        all_columns.append(Columns(curr_columns))
+
+        # Print the lifecycle events in descending order
+        for idx in range(len(all_columns) - 1, -1, -1):
+            panel_list = all_columns[idx]
+            # Since the resumption index is monotonically increasing and starts at 0,
+            # we can use the index of the array as the resumption_id
+            if 1 == len(all_columns):
+                resumption_string = ""
+            elif idx == 0:
+                resumption_string = "Initial Run:"
+            else:
+                resumption_string = f"Resumption {idx}:"
+
+            if resumption_string:
+                print(resumption_string)
+            rprint(panel_list)
+            print()
 
 
 class MCLIDescribeRunMetadataDisplay(MCLIGetDisplay):
     """ Vertical table view of run metadata """
 
     def __init__(self, metadata: Dict[str, Any]):
         self.columns = sorted(metadata.keys())
@@ -264,35 +359,38 @@
 
     # Compute requests section
     print(format_string('Compute Requests', FormatString.BOLD))
     compute_display = DescribeComputeRequests.from_run(run)
     console.print(compute_display.to_table())
     print()
 
-    # Run lifecycle section
-    print(format_string('Run Lifecycle', FormatString.BOLD))
-    lifecycle_display = MCLIDescribeRunLifecycleDisplay(run.lifecycle)
-    lifecycle_display.print(output)
-    print()
-    print(f'Total Attempts: {run.resumptions:,}')
-    print(f'Total time spent in Pending: {seconds_to_str(run.cumulative_pending_time)}')
-    print(f'Total time spent in Running: {seconds_to_str(run.cumulative_running_time)}')
-    print()
-
     if run.metadata:
         print(format_string('Run Metadata', FormatString.BOLD))
         metadata_display = MCLIDescribeRunMetadataDisplay(run.metadata)
         metadata_display.print(output)
         print()
 
     if run.nodes:
         print(format_string('Run Nodes', FormatString.BOLD))
         node_display = MCLIDescribeRunNodeDisplay(run.nodes)
         node_display.print(output)
         print()
+    # Run lifecycle section
+    print(format_string('Run Lifecycle', FormatString.BOLD))
+    lifecycle_display = MCLIDescribeRunLifecycleDisplay(run.lifecycle, run.created_at)
+    lifecycle_display.print()
+    print()
+    print(f'Number of Resumptions: {run.resumption_count}')
+    print(f'Total time spent in Pending: {seconds_to_str(run.cumulative_pending_time)}')
+    print(f'Total time spent in Running: {seconds_to_str(run.cumulative_running_time)}')
+    print()
+
+    # Run event log section
+    console.print(format_event_log(run.name, run.lifecycle))
+    print()
 
     # Run original input section
     print(format_string('Submitted YAML', FormatString.BOLD))
     print(run.submitted_config)
 
     # TODO: cleanup code to print directly to console after parsing
     # wrap command string within a literal `representer` - dump long str as block
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.5.0/mcli/cli/m_set_unset/m_set.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,56 @@
-""" mcli describe Endpoint """
-from __future__ import annotations
-
+""" mcli set Entrypoint """
 import argparse
-import logging
-
-from mcli.cli.m_describe.describe_inference_deployments import describe_deploy
-from mcli.cli.m_describe.describe_runs import describe_run
 
-logger = logging.getLogger(__name__)
+from mcli.cli.m_set_unset.api_key import configure_api_key_argparser, modify_api_key
+from mcli.cli.m_set_unset.feature_flag import use_feature_flag
+from mcli.cli.m_set_unset.organization import configure_organization_argparser, modify_organization
+from mcli.cli.m_set_unset.user import configure_user_argparser, modify_user
 
 
-def describe_entrypoint(parser, **kwargs):
+def set_entrypoint(**kwargs):
     del kwargs
-    parser.print_help()
-
+    mock_parser = configure_argparser(parser=argparse.ArgumentParser())
+    mock_parser.print_help()
+    return 0
+
+
+def configure_argparser(parser: argparse.ArgumentParser, is_admin: bool = False) -> argparse.ArgumentParser:
+    subparsers = parser.add_subparsers()
+    parser.set_defaults(func=set_entrypoint)
+
+    feature_parser = subparsers.add_parser('feature', help='Activate a feature flag')
+    feature_parser.add_argument('feature', nargs='?', help='The name of the feature flag')
+    feature_parser.set_defaults(func=use_feature_flag, activate=True)
+
+    api_key_parser = subparsers.add_parser(
+        'api-key',
+        help='Set a MosaicML platform API key that will be used in all of your subsequent workloads',
+        description='Set a MosaicML platform API key that will be used in all of your subsequent workloads',
+    )
+    configure_api_key_argparser(api_key_parser)
+    api_key_parser.set_defaults(func=modify_api_key)
 
-def describe_runs_argparser(subparser: argparse._SubParsersAction) -> None:
-    run_parser = subparser.add_parser('run', help='List metadata about a specific run')
-    run_parser.add_argument('run_name',
-                            type=str,
-                            nargs='?',
-                            help='The name of the run. If not provided, will describe the latest run')
-    run_parser.set_defaults(func=describe_run)
+    if is_admin:
+        user_parser = subparsers.add_parser('user', help='Set the user id to use')
+        configure_user_argparser(user_parser)
+        user_parser.set_defaults(func=modify_user)
+
+        org_parser = subparsers.add_parser('organization', aliases=['org'], help='Set the organization id to use')
+        configure_organization_argparser(org_parser)
+        org_parser.set_defaults(func=modify_organization)
 
+    return parser
 
-def describe_deployments_argparser(subparser: argparse._SubParsersAction) -> None:
-    deploy_parser = subparser.add_parser('deployment', help='List metadata about a specific inference deployment')
-    deploy_parser.add_argument('deployment_name', type=str, help='Inference Deployment name')
-    deploy_parser.set_defaults(func=describe_deploy)
 
+def add_set_argparser(subparser: argparse._SubParsersAction, is_admin: bool = False) -> argparse.ArgumentParser:
+    """Adds the set parser to a subparser
 
-def add_describe_parser(subparser: argparse._SubParsersAction) -> argparse.ArgumentParser:
-    describe_parser: argparse.ArgumentParser = subparser.add_parser(
-        'describe',
-        help='Get detailed information on an object',
+    Args:
+        subparser: the Subparser to add the Use parser to
+    """
+    set_parser: argparse.ArgumentParser = subparser.add_parser(
+        'set',
+        help='Set local configuration variables',
     )
-    return _configure_argparser(parser=describe_parser)
-
-
-def _configure_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
-    subparsers = parser.add_subparsers(title='MCLI Objects',
-                                       description='The table below shows the objects that you can describe',
-                                       help='DESCRIPTION',
-                                       metavar='OBJECT')
-    parser.set_defaults(func=describe_entrypoint, parser=parser)
-    describe_runs_argparser(subparser=subparsers)
-    describe_deployments_argparser(subparser=subparsers)
-    return parser
+    set_parser = configure_argparser(parser=set_parser, is_admin=is_admin)
+    return set_parser
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.5.0/mcli/cli/m_get/clusters.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from rich.table import Table
 
 from mcli.api.cluster import get_clusters as api_get_cluster
 from mcli.api.exceptions import cli_error_handler
 from mcli.api.model.cluster_details import ClusterDetails
 from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, create_display_table
-from mcli.utils.utils_cli import SubmissionType
 from mcli.utils.utils_logging import FormatString, format_string
+from mcli.utils.utils_model import SubmissionType
 
 logger = logging.getLogger(__name__)
 
 
 def get_gpu_description(gpus: int, nodes: int, allow_fractional: bool, allow_multinode: bool) -> str:
     """Get a string showing possible `gpus` values for the instance
 
@@ -56,20 +56,20 @@
         options.extend(['...', f'{nodes * gpus}'])
     elif nodes == 3:
         options.append(f'{3 * gpus}')
 
     return ','.join(options)
 
 
-def get_nodes_description(nodes: int, allow_multinode: bool) -> str:
+def get_nodes_description(nodes: int) -> str:
     """Get a string showing possible `nodes` values for the instance
     """
     if nodes == 0:
         return '-'
-    if not allow_multinode or nodes == 1:
+    if nodes == 1:
         return '1'
     else:
         return f'≤{nodes}'
 
 
 @dataclass
 class ClusterDisplayItem(MCLIDisplayItem):
@@ -104,19 +104,19 @@
 
     def __iter__(self) -> Generator[ClusterDisplayItem, None, None]:
         for c in self.cluster:
             for instance in sorted(c.cluster_instances, reverse=True):
 
                 # cpu instance sometimes captures non-worker nodes, so we'll just set
                 # the value to 1 (unless it was 0)
-                nodes = get_nodes_description(instance.nodes, c.allow_multinode)
+                nodes = get_nodes_description(instance.nodes)
                 if instance.name == 'cpu' and nodes != '-':
                     nodes = '1'
 
-                if self.submission_type.name == c.submission_type:
+                if self.submission_type is c.submission_type:
                     yield ClusterDisplayItem(
                         id=c.id if self.include_ids else None,
                         name=c.name,
                         provider=c.provider,
                         instance=instance.name,
                         nodes=nodes,
                         gpu_type=instance.gpu_type.lower(),
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_get/display.py` & `mosaicml-cli-0.5.0/mcli/cli/m_get/display.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
     def to_table(self, items: List[Dict[str, Any]]) -> Table:
 
         def _to_str(obj: Any) -> str:
             return yaml.safe_dump(obj, default_flow_style=None).strip() if not isinstance(obj, str) else obj
 
         column_names = self.override_column_ordering or [
-            key for key, val in items[0].items() if val and key != self.index_label
+            key for key, val in items[0].items() if val is not None and key != self.index_label
         ]
         columns, names = [], []
         for item in items:
             if self.index_label:
                 names.append(item[self.index_label])
             columns.append(tuple(_to_str(item[key]) for key in column_names))
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.5.0/mcli/cli/m_get/inference_deployments.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,37 +8,39 @@
 
 from mcli import config
 from mcli.api.exceptions import cli_error_handler
 from mcli.api.model.inference_deployment import InferenceDeployment
 from mcli.cli.common.deployment_filters import get_deployments_with_filters
 from mcli.cli.common.run_filters import configure_submission_filter_argparser
 from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, format_timestamp
-from mcli.utils.utils_cli import SubmissionType
+from mcli.utils.utils_model import SubmissionType
 
 
 class InferenceDeploymentColumns(Enum):
     ID = 'id'
     NAME = 'name'
     USER = 'user'
     CLUSTER = 'cluster'
     GPU_TYPE = 'gpu_type'
     GPU_NUM = 'gpu_num'
+    REPLICAS = 'replicas'
     CREATED_TIME = 'created_time'
     STATUS = 'status'
 
 
 @dataclass
 class InferenceDeploymentDisplayItem(MCLIDisplayItem):
     """Tuple that extracts deployment data for display purposes.
     """
     name: str
     gpu_num: str
     created_time: str
     status: str
     user: str
+    replicas: str
     cluster: Optional[str] = None
     gpu_type: Optional[str] = None
     id: Optional[str] = None
 
     @classmethod
     def from_deployment(cls,
                         deployment: InferenceDeployment,
@@ -46,15 +48,16 @@
         extracted: Dict[str, str] = {
             InferenceDeploymentColumns.NAME.value: deployment.name,
             InferenceDeploymentColumns.USER.value: deployment.created_by,
             InferenceDeploymentColumns.GPU_NUM.value: str(deployment.config.gpu_num),
             InferenceDeploymentColumns.CREATED_TIME.value: format_timestamp(deployment.created_at),
             InferenceDeploymentColumns.STATUS.value: deployment.status,
             InferenceDeploymentColumns.CLUSTER.value: deployment.config.cluster,
-            InferenceDeploymentColumns.GPU_TYPE.value: deployment.config.gpu_type
+            InferenceDeploymentColumns.GPU_TYPE.value: str(deployment.config.gpu_type),
+            InferenceDeploymentColumns.REPLICAS.value: str(deployment.config.replicas)
         }
         if include_ids:
             extracted[InferenceDeploymentColumns.ID.value] = deployment.deployment_uid
 
         return InferenceDeploymentDisplayItem(**extracted)
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.5.0/mcli/cli/m_get/m_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from mcli import config
 from mcli.cli.m_get import cli_get_secrets, get_clusters, get_users
 from mcli.cli.m_get.display import OutputDisplay
 from mcli.cli.m_get.inference_deployments import get_deployments_argparser
 from mcli.cli.m_get.runs import get_runs_argparser
 from mcli.cli.m_log.m_log import add_log_parser
 from mcli.models.mcli_secret import SecretType
-from mcli.utils.utils_cli import SubmissionType
+from mcli.utils.utils_model import SubmissionType
 
 
 def get_entrypoint(parser, **kwargs) -> int:
     del kwargs
     parser.print_help()
     return 0
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.5.0/mcli/cli/m_get/runs.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,84 +23,99 @@
 GPUS_PER_NODE = 8
 
 
 class RunColumns(Enum):
     ID = 'id'
     NAME = 'name'
     USER = 'user'
-    CLUSTER = 'cluster'
-    INSTANCE = 'instance'
-    NODES = 'nodes'
     CREATED_TIME = 'created_time'
+    RESUMPTION = 'resumption'
+    STATUS = 'status'
     START_TIME = 'start_time'
     END_TIME = 'end_time'
-    STATUS = 'status'
+    CLUSTER = 'cluster'
+    INSTANCE = 'instance'
+    NODES = 'nodes'
 
 
 @dataclass
 class RunDisplayItem(MCLIDisplayItem):
     """Tuple that extracts run data for display purposes.
     """
     name: str
-    nodes: str
+    user: str
     created_time: str
+    resumption: str
+    nodes: str
     start_time: str
     end_time: str
     status: str
-    user: str
     instance: str
     cluster: Optional[str] = None
     id: Optional[str] = None
 
     @classmethod
-    def from_run(cls, run: Run, include_ids: bool = False) -> RunDisplayItem:
-        display_status = run.status.display_name
-        if run.reason:
-            display_status = f"{display_status} ({run.reason})"
-        instance = get_instance_name(run)
-        extracted: Dict[str, str] = {
-            RunColumns.NAME.value: run.name,
-            RunColumns.USER.value: run.created_by,
-            RunColumns.CLUSTER.value: run.cluster,
-            RunColumns.INSTANCE.value: instance,
-            RunColumns.NODES.value: str(run.node_count),
-            RunColumns.CREATED_TIME.value: format_timestamp(run.created_at),
-            RunColumns.START_TIME.value: format_timestamp(run.started_at),
-            RunColumns.END_TIME.value: format_timestamp(run.completed_at),
-            RunColumns.STATUS.value: display_status,
-        }
-        if include_ids:
-            extracted[RunColumns.ID.value] = run.run_uid
+    def from_run(cls, run: Run, include_ids: bool = False) -> List[RunDisplayItem]:
+        run_rows = []
+        run.resumptions.sort(key=lambda resumption: resumption.index)
+        for resumption in run.resumptions[::-1]:
+            index = resumption.index
+            extracted: Dict[str, str] = {}
+            display_status = resumption.status.display_name
+            if index == len(run.resumptions) - 1:
+                extracted[RunColumns.NAME.value] = run.display_name
+                extracted[RunColumns.USER.value] = run.created_by
+                extracted[RunColumns.CREATED_TIME.value] = format_timestamp(run.created_at)
+                if run.reason:
+                    display_status = f"{display_status} ({run.reason})"
+            else:
+                extracted[RunColumns.NAME.value] = ''
+                extracted[RunColumns.USER.value] = ''
+                extracted[RunColumns.CREATED_TIME.value] = ''
+            extracted[RunColumns.RESUMPTION.value] = str(index)
+            extracted[RunColumns.CLUSTER.value] = resumption.cluster
+            extracted[RunColumns.INSTANCE.value] = get_instance_name(run)
+            extracted[RunColumns.NODES.value] = str(resumption.node_count)
+            extracted[RunColumns.START_TIME.value] = format_timestamp(resumption.started_at)
+            extracted[RunColumns.END_TIME.value] = format_timestamp(resumption.ended_at)
+            extracted[RunColumns.STATUS.value] = display_status
+            if include_ids:
+                extracted[RunColumns.ID.value] = run.run_uid
 
-        return RunDisplayItem(**extracted)
+            run_rows.append(RunDisplayItem(**extracted))
+        return run_rows
 
 
 class MCLIRunDisplay(MCLIGetDisplay):
     """Display manager for runs
     """
 
     def __init__(self, models: List[Run], include_ids: bool = False):
         self.models = sorted(models, key=lambda x: x.created_at, reverse=True)
         self.include_ids = include_ids
+        self.include_resumptions = any(len(m.resumptions) > 1 for m in self.models)
 
     @property
     def override_column_ordering(self) -> Optional[List[str]]:
         cols = []
         for c in RunColumns:
             if c == RunColumns.NAME:
                 continue
             if not self.include_ids and c == RunColumns.ID:
                 continue
+            if not self.include_resumptions and c == RunColumns.RESUMPTION:
+                continue
             cols.append(c.value)
         return cols
 
     def __iter__(self) -> Generator[RunDisplayItem, None, None]:
         for model in self.models:
-            item = RunDisplayItem.from_run(model, include_ids=self.include_ids)
-            yield item
+            items = RunDisplayItem.from_run(model, include_ids=self.include_ids)
+            for item in items:
+                yield item
 
 
 def get_instance_name(run: Run) -> str:
     """Get the run's instance name
 
     We'll try to create a human-readable name based on the gpu number and type (ie 8x v100),
     if possible.
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.5.0/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_get/users.py` & `mosaicml-cli-0.5.0/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.5.0/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.5.0/mcli/cli/m_interactive/m_interactive.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,62 @@
 """
 mcloud interactive
 """
 
 import argparse
 import logging
-from typing import Optional
+from typing import List, Optional
 
 from mcli.api.cluster import get_clusters
 from mcli.api.exceptions import MintException
 from mcli.api.mint import shell
-from mcli.api.model.run import RunConfig
-from mcli.api.runs.api_create_run import create_run
-from mcli.cli.m_connect.m_connect import configure_connection_argparser, get_tmux_command, wait_for_run
+from mcli.api.model.run import Run, RunConfig
+from mcli.api.runs.api_create_interactive_run import create_interactive_run
+from mcli.api.runs.api_get_runs import get_runs
+from mcli.cli.m_connect.m_connect import (configure_connection_argparser, connect_entrypoint, get_tmux_command,
+                                          wait_for_run)
+from mcli.utils import utils_completers
+from mcli.utils.utils_interactive import choose_one
 from mcli.utils.utils_logging import FAIL
+from mcli.utils.utils_run_status import RunStatus
 from mcli.utils.utils_types import get_hours_type
 
 logger = logging.getLogger(__name__)
 
 
+def create_or_connect(runs_on_cluster: List[Run], cluster: str):
+    result = None
+    create_new_run = True
+
+    if not runs_on_cluster:
+        # If there's no current runs on the cluster, automatically create a new interactive run
+        return create_new_run
+
+    num_runs = len(runs_on_cluster)
+    if num_runs == 1:
+        run_name = runs_on_cluster[0].name
+        result = choose_one(f"You already have an interactive run {run_name} on {cluster}. Would you like to:",
+                            [f"Connect to existing run {run_name}", "Continue creating new interactive run"])
+    else:
+        result = choose_one(f"You already have {num_runs} interactive runs on {cluster}",
+                            ["Connect to an existing run", "Continue creating new interactive run"])
+
+    if result != "Continue creating new interactive run":
+        create_new_run = False
+
+    return create_new_run
+
+
 def interactive(
     name: Optional[str] = None,
     cluster: Optional[str] = None,
     gpu_type: Optional[str] = None,
     gpus: Optional[int] = None,
     hours: Optional[float] = None,
-    image: str = 'mosaicml/pytorch',
+    image: Optional[str] = None,
     rank: int = 0,
     connect: bool = True,
     command: Optional[str] = None,
     **kwargs,
 ) -> int:
     del kwargs
 
@@ -39,39 +67,48 @@
         elif len(clusters) == 1:
             cluster = clusters[0].name
         else:
             values = ", ".join([c.name for c in clusters])
             raise RuntimeError('Multiple clusters available. Please use the --cluster argument to set the '
                                f'cluster to use for interactive. Available clusters: {values}')
 
-    run_config = RunConfig(
-        name=name or f'interactive-{(gpu_type or "none").replace("_", "-")}-{gpus or 0}'.lower(),
-        image=image,
-        command=f'sleep {int(3600 * (hours or 1))}',
-        gpu_num=gpus,
-        gpu_type=gpu_type,
-        cluster=cluster,
-        optimization_level=0,
-    )
-
-    run = create_run(run_config)
-    ready = wait_for_run(run)
-    if not ready:
-        return 1
-
-    if not connect:
+    runs_on_cluster = get_runs(statuses=[RunStatus.STARTING, RunStatus.RUNNING],
+                               cluster_names=[cluster],
+                               include_interactive=True)
+
+    create_new_run = create_or_connect(runs_on_cluster, cluster)
+
+    if create_new_run:
+        run_config = RunConfig(
+            name=name,
+            image=image,
+            gpu_num=gpus,
+            gpu_type=gpu_type,
+            cluster=cluster,
+        )
+
+        run = create_interactive_run(run_config, hours=hours)
+        ready = wait_for_run(run)
+        if not ready:
+            return 1
+
+        if not connect:
+            return 0
+
+        try:
+            mint_shell = shell.MintShell(run.name, rank=rank)
+            mint_shell.connect(command=command)
+        except MintException as e:
+            logger.error(f'{FAIL} {e}')
+            return 1
         return 0
 
-    try:
-        mint_shell = shell.MintShell(run.name, rank=rank)
-        mint_shell.connect(command=command)
-    except MintException as e:
-        logger.error(f'{FAIL} {e}')
-        return 1
-    return 0
+    else:
+        # Prompt the user to connect to the runs on the cluster they provided
+        return connect_entrypoint(runs=runs_on_cluster)
 
 
 def interactive_entrypoint(
     name: Optional[str] = None,
     cluster: Optional[str] = None,
     gpu_type: Optional[str] = None,
     gpus: Optional[int] = None,
@@ -90,16 +127,16 @@
     if hours and hrs:
         logger.error(f'{FAIL} The duration of your interactive session was specified twice. '
                      'Please use only the positional argument or --hours. '
                      'See mcli interactive --help for more details.')
 
     hours = hrs or hours
     if hours is None:
-        logger.error(f'{FAIL} Please specify the duration of your interactive session. '
-                     'See mcli interactive --help for details.')
+        logger.error(f"{FAIL} Please specify the duration of your interactive session. "
+                     'See mcli interactive --help for details')
         return 1
 
     if tmux:
         command = get_tmux_command()
 
     return interactive(
         name=name,
@@ -147,27 +184,32 @@
         help='Docker image to use',
     )
 
     cluster_arguments = parser.add_argument_group(
         'Compute settings',
         'These settings are used to determine the cluster and compute resources to use for your interactive session',
     )
-    cluster_arguments.add_argument('--cluster',
-                                   default=None,
-                                   metavar='CLUSTER',
-                                   help='Cluster where your interactive session should run. If you '
-                                   'only have one available, that one will be selected by default. '
-                                   'Depending on your cluster, you\'ll have access to different GPU types and counts. '
-                                   'See the available combinations above. ')
+    cluster_parser = cluster_arguments.add_argument(
+        '--cluster',
+        default=None,
+        metavar='CLUSTER',
+        help='Cluster where your interactive session should run. If you '
+        'only have one available, that one will be selected by default. '
+        'Depending on your cluster, you\'ll have access to different GPU types and counts. '
+        'See the available combinations above. ',
+    )
+    cluster_parser.completer = utils_completers.ClusterNameCompleter()  # pyright: ignore
 
-    cluster_arguments.add_argument(
+    gpu_type_parser = cluster_arguments.add_argument(
         '--gpu-type',
         metavar='TYPE',
         help='Type of GPU to use. Valid GPU types depend on the cluster and GPU numbers requested',
     )
+    gpu_type_parser.completer = utils_completers.GPUTypeCompleter()  # pyright: ignore
+
     cluster_arguments.add_argument(
         '--gpus',
         type=int,
         metavar='NGPUs',
         help='Number of GPUs to run interactively. Valid GPU numbers depend on the cluster and GPU type',
     )
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_kube/m_get_config.py` & `mosaicml-cli-0.5.0/mcli/cli/m_kube/m_get_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_kube/m_kube.py` & `mosaicml-cli-0.5.0/mcli/cli/m_kube/m_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_kube/m_merge_config.py` & `mosaicml-cli-0.5.0/mcli/cli/m_kube/m_merge_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_kube/utils.py` & `mosaicml-cli-0.5.0/mcli/cli/m_kube/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.5.0/mcli/cli/m_log/m_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from mcli.api.inference_deployments.api_get_inference_deployment_logs import get_inference_deployment_logs
 from mcli.api.model.inference_deployment import InferenceDeployment
 from mcli.api.model.run import Run
 from mcli.api.runs.api_get_run_logs import follow_run_logs, get_run_logs
 from mcli.api.runs.api_watch_run import EpilogSpinner as CloudEpilogSpinner
 from mcli.cli.common.deployment_filters import get_deployments_with_filters
 from mcli.cli.common.run_filters import get_runs_with_filters
-from mcli.utils.utils_cli import SubmissionType
-from mcli.utils.utils_epilog import CommonLog
+from mcli.utils import utils_completers
 from mcli.utils.utils_logging import FAIL, INFO, err_console
+from mcli.utils.utils_model import SubmissionType
 from mcli.utils.utils_run_status import RunStatus
 
 logger = logging.getLogger(__name__)
 
 # pylint: disable-next=invalid-name
 RUN_LOG_EXAMPLES = """
 
@@ -78,17 +78,14 @@
                 f'{INFO} Run {run.name} has failed. {err_message} Defaulting to show the first failed node rank.')
         failed = True
 
     if follow and run.status.before(RunStatus.RUNNING):
         with CloudEpilogSpinner(run, RunStatus.RUNNING) as watcher:
             run = watcher.follow()
 
-    if run.status == RunStatus.FAILED_PULL:
-        CommonLog(logger).log_pod_failed_pull(run.name, run.image)
-        return '', 1
     elif run.status.before(RunStatus.QUEUED, inclusive=True):
         # Pod still waiting to be scheduled. Return
         logger.error(f'{FAIL} Run {run.name} has not been scheduled')
         return '', 1
     elif run.status.before(RunStatus.RUNNING):
         # Pod still not running, probably because follow==False
         logger.error(f'{FAIL} Run has not yet started. You can check the status with `mcli get runs` '
@@ -128,15 +125,15 @@
     return last_line, 0
 
 
 def get_with_filters(submission_type: SubmissionType,
                      name: Optional[str] = None,
                      latest: bool = False) -> Union[List[Run], List[InferenceDeployment]]:
     name_filter = [name] if name else None
-    if submission_type == SubmissionType.TRAINING:
+    if submission_type is SubmissionType.TRAINING:
         return get_runs_with_filters(name_filter=name_filter, latest=latest)
     else:
         return get_deployments_with_filters(name_filter=name_filter)
 
 
 # pylint: disable-next=too-many-statements
 def get_logs(
@@ -164,15 +161,14 @@
                     f'{INFO} No {submission_type_str} name provided. Displaying log of latest {submission_type_str}: '
                     f'[cyan]{submissions[0].name}[/]')
             else:
                 submissions = get_with_filters(submission_type, submission_name, latest=True)
                 if not submissions:
                     raise MAPIException(status=HTTPStatus.NOT_FOUND,
                                         message=f'Could not find {submission_type_str}: [red]{submission_name}[/]')
-
         last_line: Optional[str] = None
         #Have to check type to satisfy pyright
         if isinstance(submissions[0], Run):
             last_line, err = _get_run_logs(submissions[0], follow, rank, failed, resumption)
             if err == 1:
                 return 1
         elif isinstance(submissions[0], InferenceDeployment):
@@ -202,31 +198,38 @@
 
     return 0
 
 
 def configure_deployments_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     parser.set_defaults(func=partial(get_logs, SubmissionType.INFERENCE))
 
-    parser.add_argument('submission_name',
-                        metavar='DEPLOYMENT',
-                        help='The name of the inference deployment to fetch logs for.')
+    submission_parser = parser.add_argument(
+        'submission_name',
+        metavar='DEPLOYMENT',
+        help='The name of the inference deployment to fetch logs for.',
+    )
+    submission_parser.completer = utils_completers.DeploymentNameCompleter()  # pyright: ignore
     parser.add_argument('--restart',
                         type=int,
                         default=None,
                         help='Which restart to fetch logs for. If not provided, will fetch logs of most recent restart')
 
     return parser
 
 
 def configure_runs_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     parser.set_defaults(func=partial(get_logs, SubmissionType.TRAINING))
-    parser.add_argument('submission_name',
-                        metavar='RUN',
-                        nargs='?',
-                        help='The name of the run. If not provided, will return the logs of the latest run')
+    submimssion_name_parser = parser.add_argument(
+        'submission_name',
+        metavar='RUN',
+        nargs='?',
+        help='The name of the run. If not provided, will return the logs of the latest run',
+    )
+    submimssion_name_parser.completer = utils_completers.RunNameCompleter()  # pyright: ignore
+
     parser.add_argument(
         '--resumption',
         type=int,
         default=None,
         metavar='N',
         dest='resumption',
         help='Resumption (0-indexed) of the run logs that you\'d like to view. '
@@ -265,14 +268,14 @@
     """
 
     log_parser: argparse.ArgumentParser = subparser.add_parser(
         'logs',
         aliases=['log'],
         help=f'View the logs from a specific {submission_type.value.lower()}',
         description=f'View the logs of an ongoing, completed or failed {submission_type.value.lower()}',
-        epilog=RUN_LOG_EXAMPLES if submission_type == SubmissionType.TRAINING else DEPLOYMENT_LOG_EXAMPLES,
+        epilog=RUN_LOG_EXAMPLES if submission_type is SubmissionType.TRAINING else DEPLOYMENT_LOG_EXAMPLES,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     log_parser = configure_runs_argparser(
-        log_parser) if submission_type == SubmissionType.TRAINING else configure_deployments_argparser(log_parser)
+        log_parser) if submission_type is SubmissionType.TRAINING else configure_deployments_argparser(log_parser)
 
     return log_parser
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.5.0/mcli/cli/m_ping/m_ping.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ mcli ping entrypoint """
 import argparse
 import logging
 
 from requests import HTTPError
 
-from mcli.api.exceptions import MAPIException
+from mcli.api.exceptions import InferenceServerException, MAPIException
 from mcli.sdk import ping as api_ping
+from mcli.utils import utils_completers
 from mcli.utils.utils_logging import FAIL
 
 logger = logging.getLogger(__name__)
 
 
 def ping(
     deployment: str,
@@ -25,17 +26,25 @@
         return 1
     except RuntimeError as e:
         logger.error(f'{FAIL} {e}')
         return 1
     except MAPIException as e:
         logger.error(f'{FAIL} {e}')
         return 1
+    except InferenceServerException as e:
+        logger.error(f'{FAIL} {e}')
+        return 1
 
 
 def add_ping_parser(subparser: argparse._SubParsersAction):
     ping_parser: argparse.ArgumentParser = subparser.add_parser(
         'ping',
         help='Ping a inference deployment in the MosaicML platform for health metrics',
     )
-    ping_parser.add_argument('deployment', metavar='DEPLOYMENT', help='The name or url of the inference deployment.')
+    deployment_parser = ping_parser.add_argument(
+        'deployment',
+        metavar='DEPLOYMENT',
+        help='The name or url of the inference deployment.',
+    )
+    deployment_parser.completer = utils_completers.DeploymentNameCompleter()  # pyright: ignore
 
     ping_parser.set_defaults(func=ping)
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.5.0/mcli/cli/m_predict/m_predict.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import logging
 from pprint import pprint
 from typing import Any, Dict
 
 import yaml
 from requests import HTTPError
 
-from mcli.api.exceptions import MAPIException
+from mcli.api.exceptions import InferenceServerException, MAPIException
 from mcli.sdk import predict
+from mcli.utils import utils_completers
 from mcli.utils.utils_logging import FAIL
 
 logger = logging.getLogger(__name__)
 
 
 def predict_cli(
     inputs: Dict[str, Any],
@@ -30,24 +31,30 @@
         return 1
     except RuntimeError as e:
         logger.error(f'{FAIL} {e}')
         return 1
     except MAPIException as e:
         logger.error(f'{FAIL} {e}')
         return 1
+    except InferenceServerException as e:
+        logger.error(f'{FAIL} {e}')
+        return 1
 
 
 def add_predict_parser(subparser: argparse._SubParsersAction):
     predict_parser: argparse.ArgumentParser = subparser.add_parser(
         'predict',
         help='Run prediction on a model in the MosaicML Cloud with given inputs. Returns forward pass result',
     )
-    predict_parser.add_argument('deployment',
-                                metavar='DEPLOYMENT',
-                                help='The name or url of the deployment to run inference on')
+    deployment_parser = predict_parser.add_argument(
+        'deployment',
+        metavar='DEPLOYMENT',
+        help='The name or url of the deployment to run inference on',
+    )
+    deployment_parser.completer = utils_completers.DeploymentNameCompleter()  # pyright: ignore
 
     predict_parser.add_argument(
         '--input',
         '--inputs',
         '-i',
         dest='inputs',
         required=True,
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.5.0/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.5.0/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.5.0/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.5.0/mcli/cli/m_set_unset/m_unset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ mcli unset Entrypoint """
 import argparse
 
 from mcli.cli.m_set_unset.feature_flag import use_feature_flag
+from mcli.cli.m_set_unset.organization import modify_organization
 from mcli.cli.m_set_unset.user import modify_user
 
 
 def unset_entrypoint(**kwargs):
     del kwargs
     mock_parser = configure_argparser(parser=argparse.ArgumentParser())
     mock_parser.print_help()
@@ -20,14 +21,17 @@
     feature_parser.add_argument('feature', nargs='?', help='The name of the feature flag')
     feature_parser.set_defaults(func=use_feature_flag, activate=False)
 
     if is_admin:
         user_parser = subparsers.add_parser('user', help='Unset the user id')
         user_parser.set_defaults(func=modify_user)
 
+        org_parser = subparsers.add_parser('organization', aliases=['org'], help='Unset the organization id')
+        org_parser.set_defaults(func=modify_organization)
+
     return parser
 
 
 def add_unset_argparser(subparser: argparse._SubParsersAction, is_admin: bool = False) -> argparse.ArgumentParser:
     """Adds the unset parser to a subparser
 
     Args:
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.5.0/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.5.0/mcli/cli/m_stop/m_stop.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     if not runs:
         extra = '' if stop_all else ' matching the specified criteria'
         logger.error(f'{WARN} No runs found{extra}.')
         return 1
 
     # skip runs that have already been stopped or don't need to be stopped
-    filtered_runs = [r for r in runs if r.status <= RunStatus.STOPPING]
+    filtered_runs = [r for r in runs if not r.status.is_terminal()]
 
     skipped_runs = len(runs) - len(filtered_runs)
     if not filtered_runs:
         if skipped_runs == 1:
             logger.error(f'{WARN} This run has already been stopped or has already finished')
         else:
             logger.error(f'{WARN} These runs have already been stopped or have already finished')
```

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.5.0/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/cli/m_util/util.py` & `mosaicml-cli-0.5.0/mcli/cli/m_util/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,128 +1,155 @@
 """ mcli util helpers """
 
 import logging
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from http import HTTPStatus
-from typing import Any, Dict, Generator, List, Optional
+from typing import Any, Dict, Generator, List, Optional, Union
 
 import yaml
 from rich.style import Style
 from rich.table import Table
 
 from mcli.api.cluster import get_clusters
 from mcli.api.exceptions import MAPIErrorMessages, MAPIException, cli_error_handler
-from mcli.api.model.cluster_details import ClusterDetails, ClusterUtilizationByRun
+from mcli.api.model.cluster_details import ClusterDetails, ClusterUtilizationByDeployment, ClusterUtilizationByRun
 from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay
 from mcli.utils.utils_logging import print_timedelta
+from mcli.utils.utils_model import SubmissionType
 
 logger = logging.getLogger(__name__)
 
 
 def get_row_color(node: dict) -> Optional[str]:
     """Get the row color using the serialized NodeInfo data
     """
     gpus_used = int(node.get("gpus_used", 0))
     gpus_available = int(node.get("gpus_available", 0))
 
     if gpus_used == 0 and gpus_available == 0:
         return "bright_black"  # gray
 
+    if gpus_available == 0:
+        return "red"
+
     if gpus_available > 0:
         return "green"
 
     return None
 
 
 @dataclass
-class UtilizationInfo(MCLIDisplayItem):
+class RunUtilizationInfo(MCLIDisplayItem):
     pos: int
-    name: str
+    name: Optional[str]
     run_name: str
     user: str
     age: str
     gpus: int
     priority: str
 
 
-class UtilizationDisplay(MCLIGetDisplay):
-    """Display information about the node
+@dataclass
+class DeploymentUtilizationInfo(MCLIDisplayItem):
+    name: Optional[str]
+    deployment_name: str
+    user: str
+    age: str
+    gpus: int
+
+
+class SubmissionUtilizationDisplay(MCLIGetDisplay):
+    """Display information about the node for submissions
     """
 
     @property
     def index_label(self) -> str:
         if self.num_clusters == 1:
-            return "run_name" if self.is_active_runs else "pos"
+            if self.submission_type is SubmissionType.INFERENCE:
+                return "deployment_name"
+            else:
+                return "run_name" if self.is_active else "pos"
         else:
             return "name"
 
-    def __init__(self, clusters: List[ClusterDetails], is_active_runs=True):
+    def __init__(self,
+                 clusters: List[ClusterDetails],
+                 is_active=True,
+                 submission_type: SubmissionType = SubmissionType.TRAINING):
         self.clusters = clusters
         self.num_clusters = len({i.name for i in clusters})
-        self.is_active_runs = is_active_runs
+        self.is_active = is_active
+        self.submission_type = submission_type
 
-    def format_active_run_name(self, r: ClusterUtilizationByRun) -> str:
-        return f'[cyan]{r.run_name}[/]'
+    def format_active_submission_name(self, r: Union[ClusterUtilizationByRun, ClusterUtilizationByDeployment]) -> str:
+        return f'[cyan]{r.display_name}[/]'
 
-    def format_pending_run_name(self, r: ClusterUtilizationByRun) -> str:
-        return f'[yellow]{r.run_name}[/]'
+    def format_pending_submission_name(self, r: Union[ClusterUtilizationByRun, ClusterUtilizationByDeployment]) -> str:
+        return f'[yellow]{r.display_name}[/]'
 
     def format_priority(self, priority: Optional[str]) -> str:
         if not priority or priority == 'DEFAULT':
             return 'medium'
         return priority.lower()
 
     def get_list(self) -> List[Dict[str, Any]]:
         items = super().get_list()
-        if not self.is_active_runs:
-            # Pending runs should have the index included
+        if not self.is_active:
+            # Pending submissions should have the index included
             return items
-        # Remove 'pos' from active runs
+        # Remove 'pos' from active submissions
         for item in items:
             item.pop('pos', None)
         return items
 
     def __iter__(self) -> Generator[MCLIDisplayItem, None, None]:
         for cluster in self.clusters:
             assert cluster.utilization
-            runs = cluster.utilization.active_by_user
-            if not self.is_active_runs:
-                runs = cluster.utilization.queued_by_user
-            for i, by_user in enumerate(runs):
-                # A priority value may not exist, so default it
-                priority = self.format_priority(by_user.scheduling.get('priority', None))
+            submissions = cluster.utilization.get_submissions(self.submission_type, self.is_active)
+            for i, by_user in enumerate(submissions):
                 cluster_name = cluster.name
                 if self.num_clusters == 1:
                     # Exclude cluster name from table completely when there's only one cluster
-                    cluster_name = ''
+                    cluster_name = None
                 elif i > 0:
                     # Skip cluster name if it was the same as the previous
                     cluster_name = ''
 
-                if self.is_active_runs:
-                    name = self.format_active_run_name(by_user)
+                if self.is_active:
+                    name = self.format_active_submission_name(by_user)
                 else:
-                    name = self.format_pending_run_name(by_user)
-
-                yield UtilizationInfo(
-                    i + 1,
-                    cluster_name,
-                    name,
-                    by_user.user,
-                    print_timedelta(datetime.now(timezone.utc) - by_user.created_at),
-                    by_user.gpu_num,
-                    priority,
-                )
+                    name = self.format_pending_submission_name(by_user)
+                if self.submission_type is SubmissionType.TRAINING:
+                    # A priority value may not exist, so default it
+                    priority = self.format_priority(by_user.scheduling.get('priority', None))
+                    yield RunUtilizationInfo(
+                        i + 1,
+                        cluster_name,
+                        name,
+                        by_user.user,
+                        print_timedelta(datetime.now(timezone.utc) - by_user.created_at),
+                        by_user.gpu_num,
+                        priority,
+                    )
+                else:
+                    yield DeploymentUtilizationInfo(
+                        cluster_name,
+                        name,
+                        by_user.user,
+                        print_timedelta(datetime.now(timezone.utc) - by_user.created_at),
+                        by_user.gpu_num,
+                    )
 
 
 @dataclass
 class ClusterInfo(MCLIDisplayItem):
     name: str
-    gpu_instance_type: str
+    instance_name: str
+    node_info: str
     gpus_available: int
     gpus_used: int
     gpus_total: int
 
 
 class ClusterDisplay(MCLIGetDisplay):
     """Display information about the node
@@ -131,19 +158,25 @@
     def __init__(self, clusters: List[ClusterDetails]):
         self.clusters = sorted(clusters)
         self.num_clusters = len({i.name for i in clusters})
 
     def __iter__(self) -> Generator[MCLIDisplayItem, None, None]:
         for cluster in self.clusters:
             assert cluster.utilization
+            cluster_name = cluster.name
+            valid_instances_displayed = 0
             for inst in cluster.utilization.cluster_instance_utils:
                 if inst.gpu_type == "None":
                     continue
+                if valid_instances_displayed > 0:
+                    cluster_name = ''
+                valid_instances_displayed += 1
                 yield ClusterInfo(
-                    cluster.name,
+                    cluster_name,
+                    inst.name,
                     str(inst.gpus_per_node) + "x" + inst.gpu_type,
                     inst.gpus_available,
                     inst.gpus_used,
                     inst.gpus_total,
                 )
 
     def to_table(self, items: List[Dict[str, Any]]) -> Table:
@@ -179,25 +212,37 @@
         c = get_clusters(clusters=clusters, include_utilization=True)
     except MAPIException as e:
         if e.status == HTTPStatus.NOT_FOUND:
             e.message = MAPIErrorMessages.NOT_FOUND_CLUSTER.value
         raise e
 
     if len(c) == 0:
-        raise MAPIException(HTTPStatus.NOT_FOUND, MAPIErrorMessages.NOT_FOUND_CLUSTER.value)
-
-    agg = ''
-    if len({cluster.name for cluster in c}) > 1:
-        agg = ' by Cluster'
-    print(f'GPU Instances{agg}:')
-    cluster_display = ClusterDisplay(c)
-    cluster_display.print(OutputDisplay.TABLE)
-
-    if not hide_users:
-        print(f'\nActive Runs{agg}:')
-        active_runs_display = UtilizationDisplay(c, is_active_runs=True)
-        active_runs_display.print(OutputDisplay.TABLE)
-        print(f'\nQueued Runs{agg}:')
-        queued_runs_display = UtilizationDisplay(c, is_active_runs=False)
-        queued_runs_display.print(OutputDisplay.TABLE)
+        raise MAPIException(HTTPStatus.NOT_FOUND, f'No clusters found with name(s): {clusters}')
+    # for submission_type in SubmissionType:
+    for i, submission_type in enumerate(SubmissionType):
+        submission_cluster = [cluster for cluster in c if cluster.submission_type is submission_type]
+        if len(submission_cluster) == 0:
+            continue
+        agg = ''
+        if len({cluster.name for cluster in submission_cluster}) > 1:
+            agg = ' by Cluster'
+
+        print(f'{submission_type.name.capitalize()} Instances{agg}:')
+        cluster_display = ClusterDisplay(submission_cluster)
+        cluster_display.print(OutputDisplay.TABLE)
+
+        if not hide_users:
+            print(f'\nActive {submission_type.value}s{agg}:')
+            active_display = SubmissionUtilizationDisplay(submission_cluster,
+                                                          submission_type=submission_type,
+                                                          is_active=True)
+            active_display.print(OutputDisplay.TABLE)
+
+            print(f'\nQueued {submission_type.value}s{agg}:')
+            queued_display = SubmissionUtilizationDisplay(submission_cluster,
+                                                          submission_type=submission_type,
+                                                          is_active=False)
+            queued_display.print(OutputDisplay.TABLE)
 
+        if i < len(SubmissionType) - 1:
+            print("\n")
     return 0
```

### Comparing `mosaicml-cli-0.4.9/mcli/config.py` & `mosaicml-cli-0.5.0/mcli/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,26 +51,25 @@
 env_path_override_config('MCLI_CONFIG_PATH')
 
 UPDATE_CHECK_FREQUENCY_DAYS: float = 2
 
 MCLI_MODE_ENV: str = 'MCLI_MODE'
 env_str_override_config(MCLI_MODE_ENV)
 
-MCLI_INTERACTIVE_ENV: str = 'MCLI_INTERACTIVE'
-env_str_override_config(MCLI_INTERACTIVE_ENV)
-
 MCLI_TIMEOUT_ENV = 'MCLI_TIMEOUT'
 env_str_override_config(MCLI_TIMEOUT_ENV)
 
 MCLI_DISABLE_UPGRADE_CHECK_ENV: str = 'MCLI_DISABLE_UPGRADE_CHECK'
 env_str_override_config(MCLI_DISABLE_UPGRADE_CHECK_ENV)
 
 # Used for local dev and testing
 MOSAICML_API_KEY_ENV: str = 'MOSAICML_API_KEY'
 
+MOSAICML_ACCESS_TOKEN_FILE_ENV: str = 'MOSAICML_ACCESS_TOKEN_FILE'
+
 ADMIN_MODE = False
 
 
 def get_timeout(default_timeout: Optional[float] = None) -> Optional[float]:
     timeout_env = os.environ.get(MCLI_TIMEOUT_ENV)
 
     if timeout_env:
@@ -79,15 +78,14 @@
     return default_timeout
 
 
 class FeatureFlag(Enum):
     """Enum for mcli feature flags
     """
     ALPHA_TESTER = 'ALPHA_TESTER'
-    MCLOUD_INTERACTIVE = 'MCLOUD_INTERACTIVE'
 
     @staticmethod
     def get_external_features() -> Set[FeatureFlag]:
         return set()
 
 
 class MCLIMode(Enum):
@@ -169,46 +167,78 @@
     last_update_check: datetime = field(default_factory=datetime.now)
 
     # MCloud environments w/ API keys
     # Most users will be in PROD, so this will likely only be touched internally
     mcloud_envs: Dict[str, str] = field(default_factory=dict)
 
     _user_id: Optional[str] = None
+    _organization_id: Optional[str] = None
 
     @property
     def user_id(self):
         # User id is only relevant in admin mode. If using normal mcli, it should always
         # set to be blank and the user just needs to authenticate through their api key
         if ADMIN_MODE:
             return self._user_id
         return None
 
     @user_id.setter
     def user_id(self, value: Optional[str]):
         self._user_id = value
 
+    @property
+    def organization_id(self):
+        if ADMIN_MODE:
+            return self._organization_id
+        return None
+
+    @organization_id.setter
+    def organization_id(self, value: Optional[str]):
+        self._organization_id = value
+
+    def update_entity(
+        self,
+        variables: Dict[str, Any],
+        *,
+        set_user: bool = True,
+        set_org: bool = True,
+    ):
+        if not ADMIN_MODE:
+            return
+
+        set_user &= (self.user_id is not None)
+        set_org &= (self.organization_id is not None)
+
+        if not set_user and not set_org:
+            return
+
+        variables['entity'] = variables.get('entity', {})
+
+        if set_user:
+            variables['entity']['userIds'] = [self.user_id]
+
+        if set_org:
+            variables['entity']['organizationIds'] = [self.organization_id]
+
+        logger.info(f'Making mapi query with entity {variables["entity"]}')
+
     @classmethod
     def empty(cls) -> MCLIConfig:
         conf = MCLIConfig()
         return conf
 
     @property
     def internal(self) -> bool:
         return self.mcli_mode.is_internal()
 
     @property
     def mcli_mode(self) -> MCLIMode:
         return MCLIMode.from_env()
 
     @property
-    def allow_interactive(self) -> bool:
-        interactive_env = os.environ.get(MCLI_INTERACTIVE_ENV, 'false').lower()
-        return interactive_env == 'true' or self.internal
-
-    @property
     def disable_upgrade(self) -> bool:
         disable_env = os.environ.get(MCLI_DISABLE_UPGRADE_CHECK_ENV, 'false').lower()
         return disable_env == 'true'
 
     @property
     def endpoint(self) -> str:
         """The user's MAPI endpoint
@@ -225,14 +255,23 @@
 
     @property
     def api_key(self):
         """The user's configured MCloud API key
         """
         return self.get_api_key(env_override=True)
 
+    @property
+    def access_token(self):
+        access_token_file = os.environ.get(MOSAICML_ACCESS_TOKEN_FILE_ENV, None)
+        if access_token_file:
+            with open(access_token_file, 'r', encoding='UTF-8') as f:
+                access_token = f.read()
+                return access_token
+        return ''
+
     @api_key.setter
     def api_key(self, value: str):
         if self.mcli_mode.is_alternate():
             # If the user is using an alternative mcloud, set that API key
             self.mcloud_envs[self.mcli_mode.value] = value
         else:
             self.MOSAICML_API_KEY = value
@@ -276,14 +315,17 @@
 
         if self.mcloud_envs:
             res['mcloud_envs'] = self.mcloud_envs
 
         if self._user_id:
             res['_user_id'] = self._user_id
 
+        if self._organization_id:
+            res['_organization_id'] = self._organization_id
+
         return res
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> MCLIConfig:
         # Remove any unknown or false feature flags
         known_feature_flags = {f.value for f in FeatureFlag}
         feature_flags = {k: v for k, v in data.get('feature_flags', {}).items() if k in known_feature_flags and v}
@@ -297,14 +339,15 @@
 
         return MCLIConfig(
             MOSAICML_API_KEY=data.get('MOSAICML_API_KEY', ''),
             feature_flags=feature_flags,
             last_update_check=last_update_check,
             mcloud_envs=data.get('mcloud_envs', {}),
             _user_id=data.get('_user_id', None),
+            _organization_id=data.get('_organization_id', None),
         )
 
     @classmethod
     def load_config(cls) -> MCLIConfig:
         """Loads the MCLIConfig from local disk
 
         Return:
@@ -325,14 +368,15 @@
         Return:
             Returns true if successful
         """
         logger.debug(f'Saving config to {MCLI_CONFIG_PATH}')
         data = self._get_formatted_dump()
         y = YAML()
         y.explicit_start = True  # type: ignore
+        os.makedirs(os.path.dirname(MCLI_CONFIG_PATH), exist_ok=True)
         with open(MCLI_CONFIG_PATH, 'w', encoding='utf8') as f:
             y.dump(data, f)
         return True
 
     def _get_formatted_dump(self) -> CommentedMap:
         """Gets the ruamel yaml formatted dump of the config
         """
@@ -350,20 +394,14 @@
             feature (FeatureFlag): The feature to check
         """
 
         if not self.internal and feature not in FeatureFlag.get_external_features():
             # Only enable select features for external use
             return False
 
-        # Force internal users onto mint, but give them the option to disable it
-        if self.internal and feature == FeatureFlag.MCLOUD_INTERACTIVE:
-            if os.environ.get('MCLI_DISABLE_MINT', 'false').lower() == 'true':
-                return False
-            return True
-
         if feature.value in self.feature_flags:
             enabled = self.feature_flags.get(feature.value, False)
             return bool(enabled)
 
         return False
 
     def __str__(self) -> str:
```

### Comparing `mosaicml-cli-0.4.9/mcli/models/__init__.py` & `mosaicml-cli-0.5.0/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/models/gpu_type.py` & `mosaicml-cli-0.5.0/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.5.0/mcli/models/inference_deployment_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 import yaml
 from typing_extensions import TypedDict
 
 from mcli.api.exceptions import MAPIException, MCLIDeploymentConfigValidationError
 from mcli.api.schema.generic_model import DeserializableModel
 from mcli.models.run_config import _clean_run_name
-from mcli.utils.utils_config import (BaseSubmissionConfig, EnvVarTranslation, IntegrationTranslation, Translation,
-                                     uuid_generator)
+from mcli.utils.utils_config import (BaseSubmissionConfig, ComputeConfig, ComputeTranslation, EnvVarTranslation,
+                                     IntegrationTranslation, Translation, uuid_generator)
 from mcli.utils.utils_string_functions import validate_image
 
 logger = logging.getLogger(__name__)
 
 DEPLOYMENT_CONFIG_UID_LENGTH = 6
 
 
@@ -26,35 +26,44 @@
     downloader: str
     download_parameters: Dict[str, str]
     model_handler: str
     model_parameters: Dict[str, str]
     backend: Optional[str]
 
 
+class BatchingConfig(TypedDict, total=False):
+    """Typed dictionary for model configs"""
+    max_batch_size: int
+    max_timeout_ms: int
+
+
 @dataclass
 class FinalInferenceDeploymentConfig(DeserializableModel):
     """A finalized deployment configuration
     This configuration must be complete, with enough details to submit a new deployment to the
     MosaicML Cloud.
     """
 
     deployment_id: str
     name: str
-    gpu_num: int
-    image: str
     replicas: int
-    env_variables: List[Dict[str, str]]
-    integrations: List[Dict[str, Any]]
+    env_variables: List[Dict[str, str]] = field(default_factory=list)
+    integrations: List[Dict[str, Any]] = field(default_factory=list)
 
     metadata: Dict[str, Any] = field(default_factory=dict)
 
     # Model config - optional for backwards-compatibility
     model: ModelConfig = field(default_factory=ModelConfig)
 
-    gpu_type: str = ''
+    batching: BatchingConfig = field(default_factory=BatchingConfig)
+    compute: ComputeConfig = field(default_factory=ComputeConfig)
+
+    gpu_num: Optional[int] = None
+    gpu_type: Optional[str] = None
+    image: str = ''
     command: str = ''
 
     cluster: str = ''
 
     _property_translations = {
         'deployment_id': 'deployment_id',
         'deploymentName': 'name',
@@ -64,53 +73,49 @@
         'image': 'image',
         'command': 'command',
         'replicas': 'replicas',
         'metadata': 'metadata',
         'envVariables': 'env_variables',
         'integrations': 'integrations',
         'model': 'model',
+        'batching': 'batching',
+        'compute': 'compute'
     }
 
+    # Backwards Compatibility
+    _optional_properties = {'metadata', 'envVariables', 'integrations', 'model', 'compute', 'batching'}
+
     def __str__(self) -> str:
         return yaml.safe_dump(asdict(self))
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> FinalInferenceDeploymentConfig:
-
-        # Backwards Compatability
-        if 'metadata' not in response:
-            response['metadata'] = {}
-
-        if 'envVariables' not in response:
-            response['envVariables'] = []
-
-        if 'integrations' not in response:
-            response['integrations'] = []
-
-        if 'model' not in response:
-            response['model'] = {
-                'checkpointPath': '',
-            }
-
-        missing = set(cls._property_translations) - set(response)
+        missing = set(cls._property_translations) - set(response) - cls._optional_properties
         if missing:
             raise MAPIException(
                 status=HTTPStatus.BAD_REQUEST,
                 message=('Missing required key(s) in response to deserialize '
                          f'FinalDeploymentConfig object: {", ".join(missing)}'),
             )
         data = {}
         for k, v in cls._property_translations.items():
+            if k not in response:
+                # This must be an optional property, so skip
+                continue
             value = response[k]
             if v == 'env_variables':
                 value = EnvVarTranslation.from_mapi(value)
             elif v == 'integrations':
                 value = IntegrationTranslation.from_mapi(value)
             elif v == 'model':
                 value = InferenceModelTranslation.from_mapi(value)
+            elif v == 'batching':
+                value = BatchingConfigTranslation.from_mapi(value)
+            elif v == 'compute':
+                value = ComputeTranslation.from_mapi(value)
             data[v] = value
 
         return cls(**data)
 
     @classmethod
     def finalize_config(cls, deployment_config: InferenceDeploymentConfig) -> FinalInferenceDeploymentConfig:
         """Create a :class:`~mcli.models.deployment_config.FinalDeploymentConfig` from the provided
@@ -130,16 +135,14 @@
         model_as_dict = asdict(deployment_config)
 
         missing_fields = [field for field, value in model_as_dict.items() if value is None]
         for missing in missing_fields:
             model_as_dict.pop(missing, None)
 
         # required for FinalDeploymentConfig, even though not required for mcloud
-        if not model_as_dict.get("gpu_num"):
-            model_as_dict["gpu_num"] = 0
 
         if not model_as_dict.get("replicas"):
             model_as_dict["replicas"] = 1
 
         if not model_as_dict.get("metadata"):
             model_as_dict["metadata"] = {}
 
@@ -149,41 +152,43 @@
         })
         model_as_dict['name'] = _clean_run_name(model_as_dict.get('name'))
 
         if isinstance(model_as_dict.get('gpu_type'), int):
             model_as_dict['gpu_type'] = str(model_as_dict['gpu_type'])
 
         image = model_as_dict.get('image')
-        if not image:
-            raise MCLIDeploymentConfigValidationError('An image name must be provided using the keyword [bold]image[/]')
-        elif not validate_image(image):
+        if image and not validate_image(image):
             raise MCLIDeploymentConfigValidationError(f'The image name "{model_as_dict["image"]}" is not valid')
 
         return cls(**model_as_dict)
 
     def to_create_deployment_api_input(self) -> Dict[str, Dict[str, Any]]:
         """Convert a deployment configuration to a proper JSON to pass to MAPI's createDeployment
         Returns:
             Dict[str, Dict[str, Any]]: The deployment configuration as a MAPI deploymentInput JSON
         """
         translations = {v: k for k, v in self._property_translations.items()}
 
         translated_input = {}
         for field_name, value in asdict(self).items():
             translated_name = translations.get(field_name, field_name)
+            if value is None:
+                continue
             if field_name == 'env_variables':
                 value = EnvVarTranslation.to_mapi(value)
             elif field_name == 'integrations':
                 value = IntegrationTranslation.to_mapi(value)
             elif field_name == 'model':
                 value = InferenceModelTranslation.to_mapi(value)
-            elif field_name == "gpu_type" and not value:
-                continue
-            elif field_name == "cluster" and not value:
-                continue
+            elif field_name == "compute":
+                value = ComputeTranslation.to_mapi(value)
+            elif field_name == "batching":
+                value = BatchingConfigTranslation.to_mapi(value)
+            elif field_name in ("image", "gpu_type", "cluster") and not value:
+                continue  # optional field
             translated_input[translated_name] = value
         return {
             'inferenceDeploymentInput': translated_input,
         }
 
 
 @dataclass
@@ -192,44 +197,50 @@
 
     Values in here are not yet validated and some required values may be missing.
 
     Args:
         name (`Optional[str]`): User-defined name of the deployment
         gpu_type (`Optional[str]`): GPU type (optional if only one gpu type for your cluster)
         gpu_num (`Optional[int]`): Number of GPUs
-        cluster (`Optional[str]`): Cluster to use (optional if you only have one)
         image (`Optional[str]`): Docker image (e.g. `mosaicml/composer`)
         command (`str`): Command to use when a deployment starts
-        replicas (`Optional[int]`): Number of replicas to create
         env_variables (`List[Dict[str, str]]`): List of environment variables
         integrations (`List[Dict[str, Any]]`): List of integrations
+        compute (`ComputeConfig`): The compute to use for the inference deployment.
+        replicas (`Optional[int]`): Number of replicas to create
+        batching (`BatchingConfig`): The dynamic batching configuration.
+        cluster (`Optional[str]`): Deprecated. Cluster to use (optional if you only have one)
     """
     name: Optional[str] = None
     gpu_type: Optional[str] = None
     gpu_num: Optional[int] = None
     cluster: Optional[str] = None
     image: Optional[str] = None
     replicas: Optional[int] = None
     command: Optional[str] = None
     metadata: Optional[Dict[str, Any]] = None
     env_variables: List[Dict[str, str]] = field(default_factory=list)
     integrations: List[Dict[str, Any]] = field(default_factory=list)
     model: ModelConfig = field(default_factory=ModelConfig)
+    batching: BatchingConfig = field(default_factory=BatchingConfig)
+    compute: ComputeConfig = field(default_factory=ComputeConfig)
 
     _property_translations = {
         'deploymentName': 'name',
         'gpuNum': 'gpu_num',
         'cluster': 'cluster',
         'image': 'image',
         'command': 'command',
         'replicas': 'replicas',
         'metadata': 'metadata',
         'envVariables': 'env_variables',
         'integrations': 'integrations',
         'model': 'model',
+        'batching': 'batching',
+        'compute': 'compute'
     }
 
     _required_display_properties = {'name', 'image', 'command', 'replicas'}
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> InferenceDeploymentConfig:
         data = {}
@@ -240,14 +251,18 @@
             value = response[k]
             if v == 'env_variables':
                 value = EnvVarTranslation.from_mapi(value)
             elif v == 'integrations':
                 value = IntegrationTranslation.from_mapi(value)
             elif v == 'model':
                 value = InferenceModelTranslation.from_mapi(value)
+            elif v == 'batching':
+                value = BatchingConfigTranslation.from_mapi(value)
+            elif v == 'compute':
+                value = ComputeConfig(**value)
             data[v] = value
 
         return cls(**data)
 
 
 class InferenceModelTranslation(Translation[ModelConfig, Dict[str, Any]]):
     """Translate model configs to and from MAPI"""
@@ -272,7 +287,30 @@
     def to_mapi(cls, value: ModelConfig) -> Dict[str, Any]:
         translated_config = {}
         for mcli_key, val in value.items():
             mapi_key = cls._property_translations.get(mcli_key)
             translated_config[mapi_key] = val
 
         return translated_config
+
+
+class BatchingConfigTranslation(Translation[BatchingConfig, Dict[str, Any]]):
+    """Translate batching configs to and from MAPI"""
+
+    _property_translations = {'max_batch_size': 'maxBatchSize', 'max_timeout_ms': 'maxTimeoutMs'}
+
+    @classmethod
+    def from_mapi(cls, value: Dict[str, Any]) -> BatchingConfig:
+        translated_config = {}
+        for mcli_key, mapi_key in cls._property_translations.items():
+            translated_config[mcli_key] = value.get(mapi_key)
+
+        return BatchingConfig(**translated_config)
+
+    @classmethod
+    def to_mapi(cls, value: BatchingConfig) -> Dict[str, Any]:
+        translated_config = {}
+        for mcli_key, val in value.items():
+            mapi_key = cls._property_translations.get(mcli_key)
+            translated_config[mapi_key] = val
+
+        return translated_config
```

### Comparing `mosaicml-cli-0.4.9/mcli/models/mcli_secret.py` & `mosaicml-cli-0.5.0/mcli/models/mcli_secret.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
             )
 
             if secret_type in {SecretType.mounted, SecretType.ssh, SecretType.git, SecretType.gcp}:
                 setattr(secret, 'mount_path', response['metadata']['mountPath'])
             elif secret_type == SecretType.environment:
                 setattr(secret, 'key', response['metadata']['key'])
             elif secret_type in {SecretType.s3}:
-                setattr(secret, 'mount_directory', response['metadata']['mountDirectory'])
+                setattr(secret, 'mount_directory', response['metadata'].get('mountDirectory'))
                 setattr(secret, 'credentials', response.get('value', {}).get('credentials'))
                 setattr(secret, 'config', response.get('value', {}).get('config'))
             elif secret_type in {SecretType.oci}:
                 setattr(secret, 'mount_directory', response['metadata']['mountDirectory'])
                 setattr(secret, 'key_file', response.get('value', {}).get('keyFile'))
                 setattr(secret, 'config', response.get('value', {}).get('config'))
             return secret
```

### Comparing `mosaicml-cli-0.4.9/mcli/models/run_config.py` & `mosaicml-cli-0.5.0/mcli/models/run_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,40 +9,33 @@
 from typing import Any, Dict, Generic, List, Optional, Sequence, TypeVar
 
 import yaml
 from typing_extensions import TypedDict
 
 from mcli.api.exceptions import MAPIException, MCLIRunConfigValidationError
 from mcli.api.schema.generic_model import DeserializableModel
-from mcli.utils.utils_config import BaseSubmissionConfig, uuid_generator
+from mcli.utils.utils_config import BaseSubmissionConfig, ComputeConfig, ComputeTranslation, uuid_generator
 from mcli.utils.utils_string_functions import (MAX_KUBERNETES_LENGTH, camel_case_to_snake_case,
                                                ensure_rfc1123_compatibility, snake_case_to_camel_case, validate_image,
                                                validate_rfc1123_name)
 
 logger = logging.getLogger(__name__)
 RUN_CONFIG_UID_LENGTH = 6
-VALID_OPTIMIZATION_LEVELS = frozenset([0, 1, 2, 3])
-MAX_RUN_NAME_LENGTH = MAX_KUBERNETES_LENGTH - RUN_CONFIG_UID_LENGTH - 1  # -1 for the dash
+MAX_RUN_NAME_LENGTH = MAX_KUBERNETES_LENGTH - \
+    RUN_CONFIG_UID_LENGTH - 1  # -1 for the dash
 
 
 class SchedulingConfig(TypedDict, total=False):
     """Typed dictionary for nested scheduling configurations"""
     priority: Optional[str]
-    resumable: Optional[bool]
+    resumable: Optional[bool]  # TODO: deprecate resumable
+    preemptible: Optional[bool]
+    retryOnSystemFailure: Optional[bool]
     max_retries: Optional[int]
-
-
-class ComputeConfig(TypedDict, total=False):
-    """Typed dictionary for nested compute requests"""
-    cluster: Optional[str]
-    instance: Optional[str]
-    nodes: Optional[int]
-    gpu_type: Optional[str]
-    gpus: Optional[int]
-    cpus: Optional[int]
+    retry_on_system_failure: Optional[bool]
 
 
 def strip_nones(d: Dict[str, Any]) -> Dict[str, Any]:
     """Remove all keys with None values from a dictionary"""
     return {k: v for k, v in d.items() if v is not None}
 
 
@@ -51,26 +44,29 @@
     """A finalized run configuration
 
     This configuration must be complete, with enough details to submit a new run to the
     MosaicML platform.
     """
 
     run_id: str
-    name: str
     cpus: int
-    image: str
     integrations: List[Dict[str, Any]]
     env_variables: List[Dict[str, str]]
 
     parameters: Dict[str, Any]
 
-    gpu_type: Optional[str] = None  # deprecating in favor of compute['gpu_type']
+    image: Optional[str] = None
+    name: Optional[str] = None
+
+    # deprecating in favor of compute['gpu_type']
+    gpu_type: Optional[str] = None
     gpu_num: Optional[int] = None  # deprecating in favor of compute['gpus']
 
-    optimization_level: int = 0
+    optimization_level: int = 0  # deprecated
+
     # Make both optional for initial rollout
     # Eventually make entrypoint required and deprecate command
     command: str = ''
     entrypoint: str = ''
 
     # Platform is deprecated, but not required for backwards compatibility
     cluster: str = ''
@@ -92,15 +88,14 @@
         'run_id': 'run_id',
         'runName': 'name',
         'gpuType': 'gpu_type',
         'gpuNum': 'gpu_num',
         'cpus': 'cpus',
         'cluster': 'cluster',
         'image': 'image',
-        'optimizationLevel': 'optimization_level',
         'integrations': 'integrations',
         'envVariables': 'env_variables',
         'parameters': 'parameters',
         'command': 'command',
         'entrypoint': 'entrypoint',
         'scheduling': 'scheduling',
         'compute': 'compute',
@@ -118,15 +113,16 @@
         return yaml.safe_dump(asdict(self))
 
     def __post_init__(self):
         self.cluster = self.cluster or self.platform
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> FinalRunConfig:
-        missing = set(cls._property_translations) - set(response) - cls._optional_properties
+        missing = set(cls._property_translations) - \
+            set(response) - cls._optional_properties
         if missing:
             raise MAPIException(
                 status=HTTPStatus.BAD_REQUEST,
                 message=
                 f'Missing required key(s) in response to deserialize FinalRunConfig object: {", ".join(missing)}',
             )
         data = {}
@@ -161,28 +157,17 @@
         Returns:
             :class:`~mcli.models.run_config.FinalRunConfig`: The object created using values from the input
 
         Raises:
             :class:`~mcli.api.exceptions.MCLIConfigError`: If MCLI config is not present or is missing information
             :class:`~mcli.api.exceptions.MCLIRunConfigValidationError`: If run_config is not valid
         """
-        # pylint: disable-next=import-outside-toplevel
-        from mcli.config import MCLIConfig
-        conf = MCLIConfig.load_config()
-
         if run_config.cpus is None:
             run_config.cpus = 0
 
-        # MosaicML Agent is disabled for all external users
-        if not conf.internal or run_config.optimization_level is None:
-            # TODO: not all docker images will support adding the MosaicML Agent
-            # If you change the default optimization level for all users, make
-            # sure the hello world documentation (image: bash) still works
-            run_config.optimization_level = 0
-
         if run_config.partitions is not None:
             # Validate provided partition is a list of strings
             if not isinstance(run_config.partitions, Sequence):
                 run_config.partitions = [str(run_config.partitions)]
             else:
                 run_config.partitions = [str(p) for p in run_config.partitions]
 
@@ -196,45 +181,26 @@
         model_as_dict = strip_nones(model_as_dict)
 
         # Fill in default initial values for FinalRunConfig
         model_as_dict.update({
             'run_id': uuid_generator(RUN_CONFIG_UID_LENGTH),
         })
 
-        model_as_dict['name'] = _clean_run_name(model_as_dict.get('name'))
+        if 'name' in model_as_dict:
+            model_as_dict['name'] = _clean_run_name(model_as_dict.get('name'))
 
         if isinstance(model_as_dict.get('gpu_type'), int):
             model_as_dict['gpu_type'] = str(model_as_dict['gpu_type'])
 
-        # Convert and validate optimization level
-        try:
-            model_as_dict['optimization_level'] = int(model_as_dict['optimization_level'])
-            if model_as_dict['optimization_level'] not in VALID_OPTIMIZATION_LEVELS:
-                raise ValueError
-        except ValueError as e:
-            raise MCLIRunConfigValidationError(
-                f'"{model_as_dict["optimization_level"]}" is not a valid optimization level. '
-                f'Please choose from: {", ".join(str(i) for i in VALID_OPTIMIZATION_LEVELS)}') from e
-
         image = model_as_dict.get('image')
         if not image:
             raise MCLIRunConfigValidationError('An image name must be provided using the keyword [bold]image[/]')
         elif not validate_image(image):
             raise MCLIRunConfigValidationError(f'The image name "{model_as_dict["image"]}" is not valid')
 
-        # Do not support specifying both a command and an entrypoint because the two might
-        # conflict with each other
-        if run_config.command and run_config.entrypoint:
-            raise MCLIRunConfigValidationError(
-                'Specifying both [bold]command[/] and [bold]entrypoint[/] as input is not supported.'
-                'Please only specify only one.')
-
-        if not (run_config.command or run_config.entrypoint):
-            raise MCLIRunConfigValidationError('A command to run must be provided using the keyword [bold]command[/]')
-
         return cls(**model_as_dict)
 
     def to_create_run_api_input(self) -> Dict[str, Dict[str, Any]]:
         """Convert a run configuration to a proper JSON to pass to MAPI's createRun
 
         Returns:
             Dict[str, Dict[str, Any]]: The run configuration as a MAPI runInput JSON
@@ -259,14 +225,16 @@
                 pass
             elif field_name == "gpu_type" and not value:
                 continue
             elif field_name == "cluster" and not value:
                 continue
             elif field_name == "platform":
                 continue
+            elif field_name == "optimization_level":
+                continue
             elif isinstance(value, dict):
                 value = strip_nones(value)
 
             translated_input[translated_name] = value
         return {
             'runInput': translated_input,
         }
@@ -369,48 +337,29 @@
 
 
 class SchedulingTranslation(Translation[SchedulingConfig, Dict[str, Any]]):
     """Translate scheduling configs to and from MAPI"""
 
     translations = {
         "maxRetries": "max_retries",
+        "retryOnSystemFailure": "retry_on_system_failure",
     }
 
     @classmethod
     def from_mapi(cls, value: Dict[str, Any]) -> SchedulingConfig:
         extracted = SchedulingConfig(**{cls.translations.get(k, k): v for k, v in value.items() if k != "priorityInt"})
         return extracted
 
     @classmethod
     def to_mapi(cls, value: SchedulingConfig) -> Dict[str, Any]:
         inv = {v: k for k, v in cls.translations.items()}
         processed = {inv.get(k, k): v for k, v in value.items() if v is not None}
         return processed
 
 
-class ComputeTranslation(Translation[ComputeConfig, Dict[str, Any]]):
-    """Translate compute configs to and from MAPI"""
-
-    translations = {
-        "gpuType": "gpu_type",
-        "nodeNames": "node_names",
-    }
-
-    @classmethod
-    def from_mapi(cls, value: Dict[str, Any]) -> ComputeConfig:
-        extracted = ComputeConfig(**{cls.translations.get(k, k): v for k, v in value.items()})
-        return extracted
-
-    @classmethod
-    def to_mapi(cls, value: ComputeConfig) -> Dict[str, Any]:
-        inv = {v: k for k, v in cls.translations.items()}
-        processed = {inv.get(k, k): v for k, v in value.items() if v is not None}
-        return processed
-
-
 def _clean_run_name(run_name: Optional[str]) -> str:
     if run_name is None:
         raise MCLIRunConfigValidationError('A run name must be provided using the keyword [bold]name[/]')
 
     name_validation = validate_rfc1123_name(text=run_name)
     if name_validation.valid:
         return run_name
@@ -453,15 +402,15 @@
     gpu_type: Optional[str] = None
     gpu_num: Optional[int] = None
     cpus: Optional[int] = None
     platform: Optional[str] = None
     cluster: Optional[str] = None
     image: Optional[str] = None
     partitions: Optional[List[str]] = None
-    optimization_level: Optional[int] = None
+    optimization_level: Optional[int] = None  # deprecated
     integrations: List[Dict[str, Any]] = field(default_factory=list)
     env_variables: List[Dict[str, str]] = field(default_factory=list)
     scheduling: SchedulingConfig = field(default_factory=SchedulingConfig)
     compute: ComputeConfig = field(default_factory=ComputeConfig)
     metadata: Dict[str, Any] = field(default_factory=dict)
 
     command: str = ''
@@ -470,15 +419,14 @@
 
     _property_translations = {
         'runName': 'name',
         'gpuNum': 'gpu_num',
         'cpus': 'cpus',
         'cluster': 'cluster',
         'image': 'image',
-        'optimizationLevel': 'optimization_level',
         'integrations': 'integrations',
         'envVariables': 'env_variables',
         'parameters': 'parameters',
         'command': 'command',
         'entrypoint': 'entrypoint',
         'scheduling': 'scheduling',
         'metadata': 'metadata',
```

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.5.0/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.5.0/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/sdk/__init__.py` & `mosaicml-cli-0.5.0/mcli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,61 @@
-"""Primary import target for the Python API"""
+""" MCLI Package """
 
 from mcli.api.cluster import get_clusters
 from mcli.api.exceptions import MAPIException
 from mcli.api.inference_deployments import (InferenceDeployment, InferenceDeploymentConfig, create_inference_deployment,
-                                            delete_inference_deployments, get_inference_deployment,
-                                            get_inference_deployment_logs, get_inference_deployments, ping, predict,
-                                            update_inference_deployment, update_inference_deployments)
+                                            delete_inference_deployment, delete_inference_deployments,
+                                            get_inference_deployment, get_inference_deployment_logs,
+                                            get_inference_deployments, ping, predict, update_inference_deployment,
+                                            update_inference_deployments)
 from mcli.api.runs import (FinalRunConfig, Run, RunConfig, RunStatus, create_run, delete_run, delete_runs,
                            follow_run_logs, get_run, get_run_logs, get_runs, start_run, start_runs, stop_run, stop_runs,
-                           update_run_metadata, wait_for_run_status, watch_run_status)
+                           update_run, update_run_metadata, wait_for_run_status, watch_run_status)
 from mcli.api.secrets import create_secret, delete_secrets, get_secrets
 from mcli.cli.m_init.m_init import initialize
 from mcli.cli.m_set_unset.api_key import set_api_key
 from mcli.config import FeatureFlag, MCLIConfig
 
+from .version import __version__
+
 __all__ = [
-    'get_clusters',
-    'MAPIException',
-    'InferenceDeployment',
-    'InferenceDeploymentConfig',
     'create_inference_deployment',
+    'create_run',
+    'create_secret',
+    'delete_inference_deployment',
     'delete_inference_deployments',
+    'delete_run',
+    'delete_runs',
+    'delete_secrets',
+    'FeatureFlag',
+    'FinalRunConfig',
+    'follow_run_logs',
+    'get_clusters',
     'get_inference_deployment_logs',
-    'get_inference_deployments',
     'get_inference_deployment',
+    'get_inference_deployments',
+    'get_run_logs',
+    'get_run',
+    'get_runs',
+    'get_secrets',
+    'InferenceDeployment',
+    'InferenceDeploymentConfig',
+    'initialize',
+    'MAPIException',
+    'MCLIConfig',
     'ping',
     'predict',
-    'FinalRunConfig',
     'Run',
     'RunConfig',
     'RunStatus',
-    'create_run',
-    'delete_run',
-    'delete_runs',
-    'follow_run_logs',
-    'get_run',
-    'get_run_logs',
-    'get_runs',
+    'set_api_key',
     'start_run',
     'start_runs',
     'stop_run',
     'stop_runs',
     'update_inference_deployment',
     'update_inference_deployments',
     'update_run_metadata',
+    'update_run',
     'wait_for_run_status',
     'watch_run_status',
-    'create_secret',
-    'delete_secrets',
-    'get_secrets',
-    'initialize',
-    'set_api_key',
-    'FeatureFlag',
-    'MCLIConfig',
 ]
```

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_cli.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 """Utility functions for the CLI and CLI testing"""
 import argparse
 import difflib
 import sys
 import textwrap
 from contextlib import contextmanager
 from datetime import datetime
-from enum import Enum
-from typing import Callable, List, NamedTuple, TypeVar
-
-from mcli.utils.utils_run_status import CLI_STATUS_OPTIONS
+from typing import Callable, List, NamedTuple, TypeVar, Union
 
 
 @contextmanager
 def set_argv(args: List[str]):
     """Temporarily override sys.argv
 
     Args:
@@ -153,31 +150,52 @@
     choose_from.sort()
 
     # Return the error string
     default_argparse_error = f'invalid choice: {value!r} (choose from {", ".join(choose_from)})'
     return f'{default_argparse_error}{suggestions_str}'
 
 
+def configure_bool_arg(parser: argparse.ArgumentParser,
+                       field: str,
+                       variable_name: str,
+                       default: Union[bool, None] = None,
+                       true_description: Union[str, None] = None,
+                       false_description: Union[str, None] = None):
+    """Create a boolean argument with a default value such that 
+    `--field` sets the value to True and `--no-field` sets the value to False
+
+    Arg:
+        parser: argument parser to configure
+        field: name of the field to configure bool parser for
+        variable_name: name of the variable to store the value in
+        default: default value of the field (default None)
+        true_description: description of the `--field` argument (default None)
+        false_description: description of the `--no-field` argument (default None)"""
+
+    field_parser = parser.add_mutually_exclusive_group(required=False)
+    field_parser.add_argument(
+        f'--no-{field}',
+        dest=variable_name,
+        action='store_false',
+        default=default,
+        help=true_description,
+    )
+    field_parser.add_argument(f'--{field}',
+                              dest=variable_name,
+                              action='store_true',
+                              default=default,
+                              help=false_description)
+
+
 # This should be used everywhere instead of argparse.ArgumentParser to allow for choice suggestions
 class MCLIArgumentParser(argparse.ArgumentParser):
     """
     MCLI Instance of argparse.ArgumentParser that provides custom choice messages
     """
 
     def _check_value(self, action, value):
         # This overrides argparse.ArgumentParser with identical logic, except
         # specifying and calling get_choice_message
         if action.choices is not None and value not in action.choices:
             args = {'value': value, 'choices': ', '.join(map(repr, action.choices))}
             msg = get_choice_message(value, action)
             raise argparse.ArgumentError(action, msg % args)
-
-
-class SubmissionType(Enum):
-    TRAINING = "Run"
-    INFERENCE = "Inference Deployment"
-
-    def get_status_options(self):
-        if self == SubmissionType.TRAINING:
-            return CLI_STATUS_OPTIONS
-        else:
-            return ["Pending", "Starting", "Ready", "Failed", "Stopped"]
```

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_config.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,25 +3,36 @@
 import logging
 import random
 import string
 import warnings
 from abc import ABC, abstractmethod
 from dataclasses import asdict, dataclass, fields
 from pathlib import Path
-from typing import Any, Dict, Generic, List, TypeVar, Union
+from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 
 import yaml
+from typing_extensions import TypedDict
 
 from mcli.utils.utils_logging import str_presenter
 from mcli.utils.utils_string_functions import camel_case_to_snake_case, snake_case_to_camel_case
 from mcli.utils.utils_yaml import load_yaml
 
 logger = logging.getLogger(__name__)
 
 
+class ComputeConfig(TypedDict, total=False):
+    """Typed dictionary for nested compute requests"""
+    cluster: Optional[str]
+    instance: Optional[str]
+    nodes: Optional[int]
+    gpu_type: Optional[str]
+    gpus: Optional[int]
+    cpus: Optional[int]
+
+
 def uuid_generator(length: int = 10) -> str:
     allowed_characters = string.ascii_lowercase + string.digits
     items = random.choices(population=allowed_characters, k=length)
     return ''.join(items)
 
 
 @dataclass
@@ -174,7 +185,27 @@
             for param, val in params.items():
                 # Translate keys to camel case for MAPI parameters
                 translated_key = camel_case_to_snake_case(param)
                 translated_integration[translated_key] = val
 
             integrations_list.append(translated_integration)
         return integrations_list
+
+
+class ComputeTranslation(Translation[ComputeConfig, Dict[str, Any]]):
+    """Translate compute configs to and from MAPI"""
+
+    translations = {
+        "gpuType": "gpu_type",
+        "nodeNames": "node_names",
+    }
+
+    @classmethod
+    def from_mapi(cls, value: Dict[str, Any]) -> ComputeConfig:
+        extracted = ComputeConfig(**{cls.translations.get(k, k): v for k, v in value.items()})
+        return extracted
+
+    @classmethod
+    def to_mapi(cls, value: ComputeConfig) -> Dict[str, Any]:
+        inv = {v: k for k, v in cls.translations.items()}
+        processed = {inv.get(k, k): v for k, v in value.items() if v is not None}
+        return processed
```

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_date.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_docker.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_logging.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_rich.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_run_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,62 +15,62 @@
 
     @property
     def order(cls) -> List[RunStatus]:
         """Order of pod states, from latest to earliest
         """
         return [
             RunStatus.FAILED,
-            RunStatus.FAILED_PULL,
             RunStatus.STOPPED,
             RunStatus.COMPLETED,
-            RunStatus.STOPPING,
             RunStatus.TERMINATING,
             RunStatus.RUNNING,
             RunStatus.STARTING,
-            RunStatus.SCHEDULED,
             RunStatus.QUEUED,
             RunStatus.PENDING,
             RunStatus.UNKNOWN,
         ]
 
 
 class RunStatus(Enum, metaclass=StatusMeta):
     """Possible statuses of a run
     """
 
-    #: The run has been dispatched and is waiting to be received
-    PENDING = 'PENDING'
+    #####################################
+    # Pending Statuses
+    #####################################
 
-    #: The run has been scheduled and is waiting to be queued
-    SCHEDULED = 'SCHEDULED'
+    #: The run has been submitted and is waiting to be scheduled
+    PENDING = 'PENDING'
 
-    #: The run is queued and is awaiting execution
+    #: The run is awaiting execution
     QUEUED = 'QUEUED'
 
+    #####################################
+    # Active Statuses
+    #####################################
+
     #: The run is starting up and preparing to run
     STARTING = 'STARTING'
 
     #: The run is actively running
     RUNNING = 'RUNNING'
 
     #: The run is in the process of being terminated
     TERMINATING = 'TERMINATING'
 
-    #: The run is in the process of being stopped
-    STOPPING = 'STOPPING'
+    #####################################
+    # Terminal Statuses
+    #####################################
 
     #: The run has finished without any errors
     COMPLETED = 'COMPLETED'
 
     #: The run has stopped
     STOPPED = 'STOPPED'
 
-    #: The run has failed due to a kubernetes error
-    FAILED_PULL = 'FAILED_PULL'
-
     #: The run has failed due to an issue at runtime
     FAILED = 'FAILED'
 
     #: A valid run status cannot be found
     UNKNOWN = 'UNKNOWN'
 
     def __str__(self) -> str:
@@ -128,14 +128,28 @@
             >>> RunStatus.COMPLETED.after(RunStatus.RUNNING)
             True
             >>> RunStatus.RUNNING.after(RunStatus.PENDING)
             True
         """
         return (self > other) or (inclusive and self == other)
 
+    def is_terminal(self) -> bool:
+        """Returns True if this state is terminal
+
+        Returns:
+            If this state is terminal
+
+        Example:
+            >>> RunStatus.RUNNING.is_terminal()
+            False
+            >>> RunStatus.COMPLETED.is_terminal()
+            True
+        """
+        return self.after(RunStatus.COMPLETED, inclusive=True)
+
     @classmethod
     def from_string(cls, run_status: Union[str, RunStatus]) -> RunStatus:
         """Convert a string to a valid RunStatus Enum
 
         If the run status string is not recognized, will return RunStatus.UNKNOWN
         instead of raising a KeyError
         """
```

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_types.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.5.0/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/mcli/version.py` & `mosaicml-cli-0.5.0/mcli/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = '0.4.9'
+__version__ = '0.5.0'
 
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.4.9/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.5.0/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.9
+Version: 0.5.0
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.9/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.5.0/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,22 @@
 mcli/api/mint/shell.py
 mcli/api/mint/tty.py
 mcli/api/model/__init__.py
 mcli/api/model/cluster_details.py
 mcli/api/model/inference_deployment.py
 mcli/api/model/run.py
 mcli/api/runs/__init__.py
+mcli/api/runs/api_create_interactive_run.py
 mcli/api/runs/api_create_run.py
 mcli/api/runs/api_delete_runs.py
 mcli/api/runs/api_get_run_logs.py
 mcli/api/runs/api_get_runs.py
 mcli/api/runs/api_start_run.py
 mcli/api/runs/api_stop_runs.py
+mcli/api/runs/api_update_run.py
 mcli/api/runs/api_update_run_metadata.py
 mcli/api/runs/api_watch_run.py
 mcli/api/schema/__init__.py
 mcli/api/schema/generic_model.py
 mcli/api/secrets/__init__.py
 mcli/api/secrets/api_create_secret.py
 mcli/api/secrets/api_delete_secrets.py
@@ -70,16 +72,14 @@
 mcli/cli/m_get/m_get.py
 mcli/cli/m_get/runs.py
 mcli/cli/m_get/secrets.py
 mcli/cli/m_get/users.py
 mcli/cli/m_init/__init__.py
 mcli/cli/m_init/m_init.py
 mcli/cli/m_interactive/__init__.py
-mcli/cli/m_interactive/interactive.py
-mcli/cli/m_interactive/kube_config.py
 mcli/cli/m_interactive/m_interactive.py
 mcli/cli/m_kube/__init__.py
 mcli/cli/m_kube/m_get_config.py
 mcli/cli/m_kube/m_kube.py
 mcli/cli/m_kube/m_merge_config.py
 mcli/cli/m_kube/utils.py
 mcli/cli/m_log/__init__.py
@@ -93,20 +93,25 @@
 mcli/cli/m_run/__init__.py
 mcli/cli/m_run/m_run.py
 mcli/cli/m_set_unset/__init__.py
 mcli/cli/m_set_unset/api_key.py
 mcli/cli/m_set_unset/feature_flag.py
 mcli/cli/m_set_unset/m_set.py
 mcli/cli/m_set_unset/m_unset.py
+mcli/cli/m_set_unset/organization.py
 mcli/cli/m_set_unset/user.py
 mcli/cli/m_stop/__init__.py
 mcli/cli/m_stop/m_stop.py
+mcli/cli/m_update/__init__.py
+mcli/cli/m_update/m_update.py
 mcli/cli/m_util/__init__.py
 mcli/cli/m_util/m_util.py
 mcli/cli/m_util/util.py
+mcli/cli/m_watchdog/__init__.py
+mcli/cli/m_watchdog/m_watchdog.py
 mcli/models/__init__.py
 mcli/models/gpu_type.py
 mcli/models/inference_deployment_config.py
 mcli/models/mcli_cluster.py
 mcli/models/mcli_envvar.py
 mcli/models/mcli_secret.py
 mcli/models/run_config.py
@@ -128,33 +133,33 @@
 mcli/objects/secrets/create/s3.py
 mcli/objects/secrets/create/ssh.py
 mcli/proto/__init__.py
 mcli/proto/mint_pb2.py
 mcli/sdk/__init__.py
 mcli/utils/__init__.py
 mcli/utils/utils_cli.py
+mcli/utils/utils_completers.py
 mcli/utils/utils_config.py
 mcli/utils/utils_date.py
 mcli/utils/utils_docker.py
 mcli/utils/utils_epilog.py
 mcli/utils/utils_interactive.py
 mcli/utils/utils_logging.py
 mcli/utils/utils_message_decoding.py
+mcli/utils/utils_model.py
 mcli/utils/utils_pypi.py
 mcli/utils/utils_rich.py
 mcli/utils/utils_run_status.py
 mcli/utils/utils_serializable_dataclass.py
 mcli/utils/utils_spinner.py
 mcli/utils/utils_string_functions.py
 mcli/utils/utils_types.py
 mcli/utils/utils_yaml.py
 mosaicml_cli.egg-info/PKG-INFO
 mosaicml_cli.egg-info/SOURCES.txt
 mosaicml_cli.egg-info/dependency_links.txt
 mosaicml_cli.egg-info/entry_points.txt
 mosaicml_cli.egg-info/requires.txt
 mosaicml_cli.egg-info/top_level.txt
-tests/__init__.py
-tests/conftest.py
 tests/test_config.py
 tests/test_simple.py
 tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.9/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.5.0/mosaicml_cli.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,53 +3,53 @@
 backoff>=2.2.1
 docker>=5.0.3
 gql[websockets]>=3.4.0
 prompt_toolkit>=3.0.29
 protobuf>=3.20.0
 pyyaml>=5.4.1
 questionary>=1.10.0
-rich>=10.16.2
+rich>=12.6.0
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 validators>=0.20.0
 
 [all]
-yapf>=0.33.0
-sphinx-argparse==0.4.0
+sphinxext-opengraph==0.8.2
+build>=0.10.0
+sphinx-panels==0.6.0
 sphinxcontrib-serializinghtml==1.1.5
-sphinxemoji==0.2.0
 docutils>=0.17.0
-pylint>=2.12.2
-sphinx==4.4.0
-sphinxcontrib-devhelp>=1.0.2
+pytest-cov>=4.0.0
 pre-commit>=2.17.0
-sphinx-panels==0.6.0
-pytest>=6.2.5
-sphinx-copybutton==0.5.2
-sphinx-markdown-tables==0.0.17
 pyright==1.1.256
-sphinxcontrib-images>=0.9.4
-sphinx_external_toc==0.3.0
-toml>=0.10.2
-sphinxcontrib-qthelp>=1.0.3
-twine>=4.0.2
-sphinxcontrib-applehelp>=1.0.2
-radon>=5.1.0
+sphinxcontrib-devhelp>=1.0.2
 sphinxcontrib-htmlhelp>=2.0.0
-sphinx-design
+sphinxcontrib-applehelp>=1.0.2
 furo==2022.9.29
-sphinx-rtd-theme==1.0.0
-sphinxcontrib-jsmath>=1.0.1
-pytest-cov>=4.0.0
+yapf>=0.33.0
+pylint>=2.12.2
 pytest-mock>=3.7.0
-myst-parser>=0.16.1
+radon>=5.1.0
+sphinx==4.4.0
+sphinxemoji==0.2.0
+sphinxcontrib-qthelp>=1.0.3
+sphinx-copybutton==0.5.2
+sphinx-argparse==0.4.0
 sphinxcontrib-katex==0.9.4
-sphinxext-opengraph==0.8.2
-build>=0.10.0
+sphinxcontrib-images>=0.9.4
+sphinxcontrib-jsmath>=1.0.1
+myst-parser>=0.16.1
+sphinx-markdown-tables==0.0.17
+toml>=0.10.2
+sphinx-rtd-theme==1.0.0
+pytest>=6.2.5
 isort>=5.9.3
+twine>=4.0.2
+sphinx-design
+sphinx_external_toc==0.3.0
 
 [dev]
 build>=0.10.0
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright==1.1.256
```

### Comparing `mosaicml-cli-0.4.9/pyproject.toml` & `mosaicml-cli-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.9/setup.py` & `mosaicml-cli-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     'backoff>=2.2.1',
     'docker>=5.0.3',
     'gql[websockets]>=3.4.0',
     'prompt_toolkit>=3.0.29',
     'protobuf>=3.20.0',
     'pyyaml>=5.4.1',
     'questionary>=1.10.0',
-    'rich>=10.16.2',
+    'rich>=12.6.0',
     'ruamel.yaml>=0.17.21',
     'typing_extensions>=4.0.1',
     'validators>=0.20.0',
 ]
 
 extra_deps = {}
```

### Comparing `mosaicml-cli-0.4.9/tests/test_config.py` & `mosaicml-cli-0.5.0/tests/test_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 from contextlib import contextmanager
 
 import pytest
 
-from mcli.config import (MCLI_INTERACTIVE_ENV, MCLI_MODE_ENV, MOSAICML_API_ENDPOINT, MOSAICML_API_ENDPOINT_DEV,
-                         MOSAICML_API_ENDPOINT_ENV, MOSAICML_API_ENDPOINT_LOCAL, MOSAICML_API_KEY_ENV, FeatureFlag,
-                         MCLIConfig, MCLIMode)
+from mcli.config import (MCLI_MODE_ENV, MOSAICML_API_ENDPOINT, MOSAICML_API_ENDPOINT_DEV, MOSAICML_API_ENDPOINT_ENV,
+                         MOSAICML_API_ENDPOINT_LOCAL, MOSAICML_API_KEY_ENV, FeatureFlag, MCLIConfig, MCLIMode)
 
 
 @contextmanager
 def clear_envs(*envs):
     values = {}
     for k in envs:
         values[k] = os.environ.pop(k, None)
@@ -182,26 +181,7 @@
         assert conf.mcloud_envs[MCLIMode.LOCAL.value] == local_api_key
         assert conf.MOSAICML_API_KEY == prod_api_key
 
         # Also env override
         env_api_key = 'some-env-api-key'
         os.environ[MOSAICML_API_KEY_ENV] = env_api_key
         assert conf.api_key == env_api_key
-
-
-def test_interactive_enabled(new_mcli_setup):
-    with clear_envs(MCLI_INTERACTIVE_ENV, MCLI_MODE_ENV):
-        conf = MCLIConfig.empty()
-        assert conf.allow_interactive is False
-
-        for value in ('true', 'TRUE'):
-            os.environ[MCLI_INTERACTIVE_ENV] = value
-            assert conf.allow_interactive is True
-
-        for value in ('false', 'unknown'):
-            os.environ[MCLI_INTERACTIVE_ENV] = value
-            assert conf.allow_interactive is False
-
-        del os.environ[MCLI_INTERACTIVE_ENV]
-
-        os.environ[MCLI_MODE_ENV] = MCLIMode.INTERNAL.value
-        assert conf.allow_interactive is True
```

### Comparing `mosaicml-cli-0.4.9/tests/test_upgrade.py` & `mosaicml-cli-0.5.0/tests/test_upgrade.py`

 * *Files identical despite different names*

