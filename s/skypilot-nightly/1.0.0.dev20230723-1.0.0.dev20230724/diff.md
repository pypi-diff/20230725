# Comparing `tmp/skypilot-nightly-1.0.0.dev20230723.tar.gz` & `tmp/skypilot-nightly-1.0.0.dev20230724.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot-nightly-1.0.0.dev20230723.tar", last modified: Sun Jul 23 10:40:45 2023, max compression
+gzip compressed data, was "skypilot-nightly-1.0.0.dev20230724.tar", last modified: Mon Jul 24 10:40:48 2023, max compression
```

## Comparing `skypilot-nightly-1.0.0.dev20230723.tar` & `skypilot-nightly-1.0.0.dev20230724.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.170248 skypilot-nightly-1.0.0.dev20230723/
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-23 10:40:45.170248 skypilot-nightly-1.0.0.dev20230723/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 10:40:45.170248 skypilot-nightly-1.0.0.dev20230723/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-23 10:40:37.000000 skypilot-nightly-1.0.0.dev20230723/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.150249 skypilot-nightly-1.0.0.dev20230723/sky/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-23 10:40:37.000000 skypilot-nightly-1.0.0.dev20230723/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.150249 skypilot-nightly-1.0.0.dev20230723/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.150249 skypilot-nightly-1.0.0.dev20230723/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)   112970 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   202208 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.154249 skypilot-nightly-1.0.0.dev20230723/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/backends/onprem_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.154249 skypilot-nightly-1.0.0.dev20230723/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (123)   167453 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.154249 skypilot-nightly-1.0.0.dev20230723/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41169 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    46375 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.154249 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    23188 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.154249 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.158248 skypilot-nightly-1.0.0.dev20230723/sky/data/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    89247 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.158248 skypilot-nightly-1.0.0.dev20230723/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.158248 skypilot-nightly-1.0.0.dev20230723/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/provision/aws/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.158248 skypilot-nightly-1.0.0.dev20230723/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    42860 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.158248 skypilot-nightly-1.0.0.dev20230723/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-23 10:40:37.000000 skypilot-nightly-1.0.0.dev20230723/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.158248 skypilot-nightly-1.0.0.dev20230723/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/log_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.146249 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.158248 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.158248 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/aws/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.158248 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/azure/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.162248 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/gcp/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/gcp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.162248 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.162248 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/lambda_cloud/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.162248 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/oci/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.162248 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/scp/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/scp/scp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.162248 skypilot-nightly-1.0.0.dev20230723/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/ray_patches/job_head.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.166248 skypilot-nightly-1.0.0.dev20230723/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/spot/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.166248 skypilot-nightly-1.0.0.dev20230723/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.166248 skypilot-nightly-1.0.0.dev20230723/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.166248 skypilot-nightly-1.0.0.dev20230723/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.166248 skypilot-nightly-1.0.0.dev20230723/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/templates/gcp-tpu-create.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/templates/gcp-tpu-delete.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/templates/spot-controller.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.166248 skypilot-nightly-1.0.0.dev20230723/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.166248 skypilot-nightly-1.0.0.dev20230723/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.166248 skypilot-nightly-1.0.0.dev20230723/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/env_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/tpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.170248 skypilot-nightly-1.0.0.dev20230723/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-23 10:40:45.000000 skypilot-nightly-1.0.0.dev20230723/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-23 10:40:45.000000 skypilot-nightly-1.0.0.dev20230723/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 10:40:45.000000 skypilot-nightly-1.0.0.dev20230723/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-23 10:40:45.000000 skypilot-nightly-1.0.0.dev20230723/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-23 10:40:45.000000 skypilot-nightly-1.0.0.dev20230723/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-23 10:40:45.000000 skypilot-nightly-1.0.0.dev20230723/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:45.170248 skypilot-nightly-1.0.0.dev20230723/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/tests/test_onprem.py
--rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/tests/test_pycryptodome_version.py
--rw-r--r--   0 runner    (1001) docker     (123)   125880 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/tests/test_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-23 10:40:34.000000 skypilot-nightly-1.0.0.dev20230723/tests/test_wheels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.446782 skypilot-nightly-1.0.0.dev20230724/
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-24 10:40:48.446782 skypilot-nightly-1.0.0.dev20230724/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:40:48.446782 skypilot-nightly-1.0.0.dev20230724/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-24 10:40:39.000000 skypilot-nightly-1.0.0.dev20230724/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.382781 skypilot-nightly-1.0.0.dev20230724/sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-24 10:40:39.000000 skypilot-nightly-1.0.0.dev20230724/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.386781 skypilot-nightly-1.0.0.dev20230724/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.390781 skypilot-nightly-1.0.0.dev20230724/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113020 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   202208 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.390781 skypilot-nightly-1.0.0.dev20230724/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/backends/onprem_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.394781 skypilot-nightly-1.0.0.dev20230724/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167528 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.398781 skypilot-nightly-1.0.0.dev20230724/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41169 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46375 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.402781 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23188 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.406781 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.410781 skypilot-nightly-1.0.0.dev20230724/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89247 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.410781 skypilot-nightly-1.0.0.dev20230724/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.410781 skypilot-nightly-1.0.0.dev20230724/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/provision/aws/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.410781 skypilot-nightly-1.0.0.dev20230724/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42860 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.414781 skypilot-nightly-1.0.0.dev20230724/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-24 10:40:39.000000 skypilot-nightly-1.0.0.dev20230724/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.418781 skypilot-nightly-1.0.0.dev20230724/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/log_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.370781 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.418781 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.422782 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/aws/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.422782 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/azure/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.426782 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/gcp/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/gcp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.426782 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.430781 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/lambda_cloud/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.430781 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/oci/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.430781 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/scp/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/scp/scp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.434782 skypilot-nightly-1.0.0.dev20230724/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/ray_patches/job_head.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.434782 skypilot-nightly-1.0.0.dev20230724/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/spot/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.434782 skypilot-nightly-1.0.0.dev20230724/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.434782 skypilot-nightly-1.0.0.dev20230724/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.434782 skypilot-nightly-1.0.0.dev20230724/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.438782 skypilot-nightly-1.0.0.dev20230724/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/templates/gcp-tpu-create.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/templates/gcp-tpu-delete.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/templates/spot-controller.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.438782 skypilot-nightly-1.0.0.dev20230724/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.442782 skypilot-nightly-1.0.0.dev20230724/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.442782 skypilot-nightly-1.0.0.dev20230724/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/env_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/tpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.442782 skypilot-nightly-1.0.0.dev20230724/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-24 10:40:48.000000 skypilot-nightly-1.0.0.dev20230724/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-24 10:40:48.000000 skypilot-nightly-1.0.0.dev20230724/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:40:48.000000 skypilot-nightly-1.0.0.dev20230724/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 10:40:48.000000 skypilot-nightly-1.0.0.dev20230724/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-24 10:40:48.000000 skypilot-nightly-1.0.0.dev20230724/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 10:40:48.000000 skypilot-nightly-1.0.0.dev20230724/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:40:48.446782 skypilot-nightly-1.0.0.dev20230724/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/tests/test_onprem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/tests/test_pycryptodome_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125916 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/tests/test_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 10:40:35.000000 skypilot-nightly-1.0.0.dev20230724/tests/test_wheels.py
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/LICENSE` & `skypilot-nightly-1.0.0.dev20230724/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230724/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230724/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230723
+Version: 1.0.0.dev20230724
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230723
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230724
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/README.md` & `skypilot-nightly-1.0.0.dev20230724/README.md`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/pyproject.toml` & `skypilot-nightly-1.0.0.dev20230724/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/setup.py` & `skypilot-nightly-1.0.0.dev20230724/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/__init__.py` & `skypilot-nightly-1.0.0.dev20230724/sky/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The SkyPilot package."""
 import os
 
 # Replaced with the current commit when building the wheels.
-__commit__ = '1fdb21931821eb7fcdaa4dec3ec940721975580d'
-__version__ = '1.0.0-dev20230723'
+__commit__ = 'f5526d43b49f5e8bf184f73c58193d9d203cdc1e'
+__version__ = '1.0.0-dev20230724'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 # Keep this order to avoid cyclic imports
 from sky import backends
 from sky import benchmark
 from sky import clouds
 from sky.clouds.service_catalog import list_accelerators
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/adaptors/aws.py` & `skypilot-nightly-1.0.0.dev20230724/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/adaptors/azure.py` & `skypilot-nightly-1.0.0.dev20230724/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/adaptors/cloudflare.py` & `skypilot-nightly-1.0.0.dev20230724/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/adaptors/docker.py` & `skypilot-nightly-1.0.0.dev20230724/sky/adaptors/docker.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/adaptors/gcp.py` & `skypilot-nightly-1.0.0.dev20230724/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/adaptors/ibm.py` & `skypilot-nightly-1.0.0.dev20230724/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/adaptors/oci.py` & `skypilot-nightly-1.0.0.dev20230724/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/authentication.py` & `skypilot-nightly-1.0.0.dev20230724/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/backends/backend.py` & `skypilot-nightly-1.0.0.dev20230724/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/backends/backend_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/backends/backend_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -906,15 +906,16 @@
             **{
                 'cluster_name': cluster_name,
                 'num_nodes': num_nodes,
                 'disk_size': to_provision.disk_size,
                 # If the current code is run by controller, propagate the real
                 # calling user which should've been passed in as the
                 # SKYPILOT_USER env var (see spot-controller.yaml.j2).
-                'user': os.environ.get('SKYPILOT_USER', getpass.getuser()),
+                'user': get_cleaned_username(os.environ.get(
+                    'SKYPILOT_USER', '')),
 
                 # AWS only:
                 # Temporary measure, as deleting per-cluster SGs is too slow.
                 # See https://github.com/skypilot-org/skypilot/pull/742.
                 # Generate the name of the security group we're looking for.
                 # (username, last 4 chars of hash of hostname): for uniquefying
                 # users on shared-account scenarios.
@@ -1319,30 +1320,30 @@
 
 def generate_cluster_name():
     # TODO: change this ID formatting to something more pleasant.
     # User name is helpful in non-isolated accounts, e.g., GCP, Azure.
     return f'sky-{uuid.uuid4().hex[:4]}-{get_cleaned_username()}'
 
 
-def get_cleaned_username() -> str:
-    """Cleans the current username to be used as part of a cluster name.
+def get_cleaned_username(username: str = '') -> str:
+    """Cleans the username to be used as part of a cluster name.
 
     Clean up includes:
      1. Making all characters lowercase
      2. Removing any non-alphanumeric characters (excluding hyphens)
      3. Removing any numbers and/or hyphens at the start of the username.
      4. Removing any hyphens at the end of the username
 
     e.g. 1SkY-PiLot2- becomes sky-pilot2.
 
     Returns:
       A cleaned username that will pass the regex in
       check_cluster_name_is_valid().
     """
-    username = getpass.getuser()
+    username = username or getpass.getuser()
     username = username.lower()
     username = re.sub(r'[^a-z0-9-]', '', username)
     username = re.sub(r'^[0-9-]+', '', username)
     username = re.sub(r'-$', '', username)
     return username
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/backends/cloud_vm_ray_backend.py` & `skypilot-nightly-1.0.0.dev20230724/sky/backends/cloud_vm_ray_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/backends/docker_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/backends/local_docker_backend.py` & `skypilot-nightly-1.0.0.dev20230724/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-nightly-1.0.0.dev20230724/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/backends/onprem_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/backends/onprem_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/backends/wheel_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/benchmark/benchmark_state.py` & `skypilot-nightly-1.0.0.dev20230724/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/benchmark/benchmark_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/check.py` & `skypilot-nightly-1.0.0.dev20230724/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/cli.py` & `skypilot-nightly-1.0.0.dev20230724/sky/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -2622,15 +2622,16 @@
                     f'{operation} reserved cluster(s) '
                     f'{reserved_clusters_str} with other cluster(s) '
                     f'{names_str} is currently not supported.\n'
                     f'Please omit the reserved cluster(s) {reserved_clusters}.')
             if not down:
                 raise click.UsageError(
                     f'{operation} reserved cluster(s) '
-                    f'{reserved_clusters_str} is currently not supported.')
+                    f'{reserved_clusters_str} is currently not supported. '
+                    'It will be auto-stopped after all spot jobs finish.')
             else:
                 # TODO(zhwu): We can only have one reserved cluster (spot
                 # controller).
                 assert len(reserved_clusters) == 1, reserved_clusters
                 _hint_or_raise_for_down_spot_controller(reserved_clusters[0])
                 confirm_str = 'delete'
                 user_input = click.prompt(
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/cloud_stores.py` & `skypilot-nightly-1.0.0.dev20230724/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/__init__.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/aws.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/azure.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/cloud.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/gcp.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/ibm.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/local.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/local.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/oci.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/scp.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/__init__.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/common.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/config.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/oci_catalog.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/clouds/service_catalog/scp_catalog.py` & `skypilot-nightly-1.0.0.dev20230724/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/core.py` & `skypilot-nightly-1.0.0.dev20230724/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/dag.py` & `skypilot-nightly-1.0.0.dev20230724/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/data/data_transfer.py` & `skypilot-nightly-1.0.0.dev20230724/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/data/data_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/data/mounting_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/data/storage.py` & `skypilot-nightly-1.0.0.dev20230724/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/data/storage_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/exceptions.py` & `skypilot-nightly-1.0.0.dev20230724/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/execution.py` & `skypilot-nightly-1.0.0.dev20230724/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/global_user_state.py` & `skypilot-nightly-1.0.0.dev20230724/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/optimizer.py` & `skypilot-nightly-1.0.0.dev20230724/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/provision/__init__.py` & `skypilot-nightly-1.0.0.dev20230724/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/provision/aws/instance.py` & `skypilot-nightly-1.0.0.dev20230724/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/provision/gcp/instance.py` & `skypilot-nightly-1.0.0.dev20230724/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/provision/gcp/instance_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/resources.py` & `skypilot-nightly-1.0.0.dev20230724/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/setup_files/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230724/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/setup_files/setup.py` & `skypilot-nightly-1.0.0.dev20230724/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/sky_logging.py` & `skypilot-nightly-1.0.0.dev20230724/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/LICENSE` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/attempt_skylet.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/autostop_lib.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/configs.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/constants.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,13 +47,19 @@
 # Port on the remote spot controller that the dashboard is running on.
 SPOT_DASHBOARD_REMOTE_PORT = 5000
 
 # Install conda on the remote cluster if it is not already installed.
 # We do not install the latest conda with python 3.11 because ray has not
 # officially supported it yet.
 # https://github.com/ray-project/ray/issues/31606
+# We use python 3.10 to be consistent with the python version of the
+# AWS's Deep Learning AMI's default conda environment.
 CONDA_INSTALLATION_COMMANDS = (
-    '(which conda > /dev/null 2>&1 && conda init > /dev/null) || '
-    '(wget -nc https://repo.anaconda.com/miniconda/Miniconda3-py39_23.5.2-0-Linux-x86_64.sh -O Miniconda3-Linux-x86_64.sh && '  # pylint: disable=line-too-long
+    'which conda > /dev/null 2>&1 || '
+    '(wget -nc https://repo.anaconda.com/miniconda/Miniconda3-py310_23.5.2-0-Linux-x86_64.sh -O Miniconda3-Linux-x86_64.sh && '  # pylint: disable=line-too-long
     'bash Miniconda3-Linux-x86_64.sh -b && '
     'eval "$(~/miniconda3/bin/conda shell.bash hook)" && conda init && '
-    'conda config --set auto_activate_base true);')
+    'conda config --set auto_activate_base true); '
+    # Only run `conda init` if the conda is not installed under /opt/conda,
+    # which is the case for VMs created on GCP, and running `conda init` will
+    # cause error and waiting for the error to be reported: #2273.
+    'which conda | grep /opt/conda || conda init > /dev/null;')
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/events.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/job_lib.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/log_lib.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/aws/config.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/aws/node_provider.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/aws/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/aws/utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/azure/azure-config-template.json` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/azure/config.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/azure/node_provider.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/gcp/config.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/gcp/constants.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/gcp/node.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/gcp/node.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/gcp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/gcp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/ibm/node_provider.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/ibm/utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/lambda_cloud/lambda_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/lambda_cloud/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/oci/config.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/oci/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/oci/node_provider.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/oci/query_helper.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/scp/config.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/scp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/providers/scp/scp_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/providers/scp/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/ray_patches/__init__.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/ray_patches/worker.py.patch` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/skylet.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skylet/subprocess_daemon.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/skypilot_config.py` & `skypilot-nightly-1.0.0.dev20230724/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/spot/__init__.py` & `skypilot-nightly-1.0.0.dev20230724/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/spot/constants.py` & `skypilot-nightly-1.0.0.dev20230724/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/spot/controller.py` & `skypilot-nightly-1.0.0.dev20230724/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/spot/dashboard/dashboard.py` & `skypilot-nightly-1.0.0.dev20230724/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/spot/dashboard/static/favicon.ico` & `skypilot-nightly-1.0.0.dev20230724/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/spot/dashboard/templates/index.html` & `skypilot-nightly-1.0.0.dev20230724/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/spot/recovery_strategy.py` & `skypilot-nightly-1.0.0.dev20230724/sky/spot/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/spot/spot_state.py` & `skypilot-nightly-1.0.0.dev20230724/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/spot/spot_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/status_lib.py` & `skypilot-nightly-1.0.0.dev20230724/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/task.py` & `skypilot-nightly-1.0.0.dev20230724/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/templates/aws-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230724/sky/templates/aws-ray.yml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -175,26 +175,24 @@
 # items!
 #
 # Increment the following for catching performance bugs easier:
 #   current num items (num SSH connections): 1
 setup_commands:
   # Disable `unattended-upgrades` to prevent apt-get from hanging. It should be called at the beginning before the process started to avoid being blocked. (This is a temporary fix.)
   # Create ~/.ssh/config file in case the file does not exist in the custom image.
-  # Make sure python3 & pip3 are available on this image.
   # We set auto_activate_base to be false for pre-installed conda.
   # This also kills the service that is holding the lock on dpkg (problem only exists on aws/azure, not gcp)
   # Line 'sudo bash ..': set the ulimit as suggested by ray docs for performance. https://docs.ray.io/en/latest/cluster/vms/user-guides/large-cluster-best-practices.html#system-configuration
   # Line 'sudo grep ..': set the number of threads per process to unlimited to avoid ray job submit stucking issue when the number of running ray jobs increase.
   # Line 'mkdir -p ..': disable host key check
   # Line 'python3 -c ..': patch the buggy ray files and enable `-o allow_other` option for `goofys`
   - mkdir -p ~/.ssh; touch ~/.ssh/config;
-    pip3 --version > /dev/null 2>&1 || (curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py && python3 get-pip.py && echo "PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc);
+    {{ conda_installation_commands }}
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
-    {{ conda_installation_commands }}
     source ~/.bashrc;
     (pip3 list | grep "ray " | grep {{ray_version}} 2>&1 > /dev/null || pip3 install --exists-action w -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app;
     (pip3 list | grep "skypilot " && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[aws]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
     python3 -c "from sky.skylet.ray_patches import patch; patch()" || exit 1;
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/templates/azure-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230724/sky/templates/azure-ray.yml.j2`

 * *Files 6% similar despite different names*

```diff
@@ -106,15 +106,14 @@
 # items!
 #
 # Increment the following for catching performance bugs easier:
 #   current num items (num SSH connections): 1
 setup_commands:
   # Disable `unattended-upgrades` to prevent apt-get from hanging. It should be called at the beginning before the process started to avoid being blocked. (This is a temporary fix.)
   # Create ~/.ssh/config file in case the file does not exist in the image.
-  # Make sure python3 & pip3 are available on this image.
   # Line 'sudo bash ..': set the ulimit as suggested by ray docs for performance. https://docs.ray.io/en/latest/cluster/vms/user-guides/large-cluster-best-practices.html#system-configuration
   # Line 'sudo grep ..': set the number of threads per process to unlimited to avoid ray job submit stucking issue when the number of running ray jobs increase.
   # Line 'mkdir -p ..': disable host key check
   # Line 'python3 -c ..': patch the buggy ray files and enable `-o allow_other` option for `goofys`
   # This also kills the service that is holding the lock on dpkg (problem only exists on aws/azure, not gcp)
   - function mylsof { p=$(for pid in /proc/{0..9}*; do i=$(basename "$pid"); for file in "$pid"/fd/*; do link=$(readlink -e "$file"); if [ "$link" = "$1" ]; then echo "$i"; fi; done; done); echo "$p"; };
     sudo systemctl stop unattended-upgrades || true;
@@ -123,18 +122,17 @@
     p=$(mylsof "/var/lib/dpkg/lock-frontend"); echo "$p";
     sudo kill -9 `echo "$p" | tail -n 1` || true;
     sudo rm /var/lib/dpkg/lock-frontend;
     sudo pkill -9 dpkg;
     sudo pkill -9 apt-get;
     sudo dpkg --configure --force-overwrite -a;
     mkdir -p ~/.ssh; touch ~/.ssh/config;
-    pip3 --version > /dev/null 2>&1 || (curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py && python3 get-pip.py && echo "PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc);
+    {{ conda_installation_commands }}
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
-    {{ conda_installation_commands }}
     source ~/.bashrc;
     (pip3 list | grep "ray " | grep {{ray_version}} 2>&1 > /dev/null || pip3 install --exists-action w -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app && touch ~/.sudo_as_admin_successful;
     (pip3 list | grep "skypilot " && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[azure]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
     python3 -c "from sky.skylet.ray_patches import patch; patch()" || exit 1;
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/templates/gcp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230724/sky/templates/gcp-ray.yml.j2`

 * *Files 4% similar despite different names*

```diff
@@ -160,15 +160,14 @@
 # items!
 #
 # Increment the following for catching performance bugs easier:
 #   current num items (num SSH connections): 1  (+1 if tpu_vm)
 setup_commands:
   # Disable `unattended-upgrades` to prevent apt-get from hanging. It should be called at the beginning before the process started to avoid being blocked. (This is a temporary fix.)
   # Line 'mkdir -p ..': Create ~/.ssh/config file in case the file does not exist in the custom image.
-  # Line 'pip3 --v ..': Make sure python3 & pip3 are available on this image.
   # Line 'which conda ..': some images (TPU VM) do not install conda by
   # default. 'source ~/.bashrc' is needed so conda takes effect for the next
   # commands.
   # Line 'sudo bash ..': set the ulimit as suggested by ray docs for performance. https://docs.ray.io/en/latest/cluster/vms/user-guides/large-cluster-best-practices.html#system-configuration
   # Line 'sudo grep ..': set the number of threads per process to unlimited to avoid ray job submit stucking issue when the number of running ray jobs increase.
   # Line 'mkdir -p ..': disable host key check
   # Line 'python3 -c ..': patch the buggy ray files and enable `-o allow_other` option for `goofys`
@@ -179,18 +178,17 @@
     p=$(mylsof "/var/lib/dpkg/lock-frontend"); echo "$p";
     sudo kill -9 `echo "$p" | tail -n 1` || true;
     sudo rm /var/lib/dpkg/lock-frontend;
     sudo pkill -9 dpkg;
     sudo pkill -9 apt-get;
     sudo dpkg --configure --force-overwrite -a;
     mkdir -p ~/.ssh; touch ~/.ssh/config;
-    pip3 --version > /dev/null 2>&1 || (curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py && python3 get-pip.py && echo "PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc);
+    {{ conda_installation_commands }}
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
-    {{ conda_installation_commands }}
     source ~/.bashrc;
   {%- if tpu_vm %}
     test -f /home/gcpuser/miniconda3/etc/profile.d/conda.sh && source /home/gcpuser/miniconda3/etc/profile.d/conda.sh && conda activate base || true;
     pip3 install --upgrade google-api-python-client;
   {%- endif %}
     (pip3 list | grep "ray " | grep {{ray_version}} 2>&1 > /dev/null || pip3 install --exists-action w -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app;
     (pip3 list | grep "skypilot " && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[gcp]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/templates/ibm-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230724/sky/templates/ibm-ray.yml.j2`

 * *Files 5% similar despite different names*

```diff
@@ -81,33 +81,31 @@
 # connection, which is expensive. Try your best to co-locate commands into fewer
 # items!
 #
 # Increment the following for catching performance bugs easier:
 #   current num items (num SSH connections): 1
 setup_commands:
   # Create ~/.ssh/config file in case the file does not exist in the custom image.
-  # Make sure python3 & pip3 are available on this image.
   # We set auto_activate_base to be false for pre-installed conda.
   # This also kills the service that is holding the lock on dpkg (problem only exists on aws/azure, not gcp)
   # Line 'sudo bash ..': set the ulimit as suggested by ray docs for performance. https://docs.ray.io/en/latest/cluster/vms/user-guides/large-cluster-best-practices.html#system-configuration
   # Line 'sudo grep ..': set the number of threads per process to unlimited to avoid ray job submit stucking issue when the number of running ray jobs increase.
   # Line 'mkdir -p ..': disable host key check
   # Line 'python3 -c ..': patch the buggy ray files and enable `-o allow_other` option for `goofys`
   - sudo systemctl stop unattended-upgrades || true;
     sudo systemctl disable unattended-upgrades || true;
     sudo sed -i 's/Unattended-Upgrade "1"/Unattended-Upgrade "0"/g' /etc/apt/apt.conf.d/20auto-upgrades || true;
     sudo kill -9 `sudo lsof /var/lib/dpkg/lock-frontend | awk '{print $2}' | tail -n 1` || true;
     sudo pkill -9 apt-get;
     sudo pkill -9 dpkg;
     sudo dpkg --configure -a;
     mkdir -p ~/.ssh; touch ~/.ssh/config;
-    pip3 --version > /dev/null 2>&1 || (curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py && python3 get-pip.py && echo "PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc);
+    {{ conda_installation_commands }}
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
-    {{ conda_installation_commands }}
     source ~/.bashrc;
     (pip3 list | grep ray | grep {{ray_version}} 2>&1 > /dev/null || pip3 install -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app;
     (pip3 list | grep skypilot && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[ibm]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
     python3 -c "from sky.skylet.ray_patches import patch; patch()" || exit 1;
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/templates/lambda-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230724/sky/templates/lambda-ray.yml.j2`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -69,17 +69,17 @@
     sudo sed -i 's/Unattended-Upgrade "1"/Unattended-Upgrade "0"/g' /etc/apt/apt.conf.d/20auto-upgrades || true;
     sudo kill -9 `sudo lsof /var/lib/dpkg/lock-frontend | awk '{print $2}' | tail -n 1` || true;
     sudo pkill -9 apt-get;
     sudo pkill -9 dpkg;
     sudo dpkg --configure -a;
     mkdir -p ~/.ssh; touch ~/.ssh/config;
     rm ~/.local/bin/pip ~/.local/bin/pip3 ~/.local/bin/pip3.8 ~/.local/bin/pip3.10;
+    {{ conda_installation_commands }}
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
-    {{ conda_installation_commands }}
     source ~/.bashrc;
     (pip3 list | grep "ray " | grep {{ray_version}} 2>&1 > /dev/null || pip3 install --exists-action w -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app && touch ~/.sudo_as_admin_successful;
     (pip3 list | grep "skypilot " && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[lambda]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
     python3 -c "from sky.skylet.ray_patches import patch; patch()" || exit 1;
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/templates/local-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230724/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/templates/oci-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230724/sky/templates/oci-ray.yml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -90,18 +90,17 @@
     sudo sed -i 's/Unattended-Upgrade "1"/Unattended-Upgrade "0"/g' /etc/apt/apt.conf.d/20auto-upgrades || true;
     sudo kill -9 `sudo lsof /var/lib/dpkg/lock-frontend | awk '{print $2}' | tail -n 1` || true;
     sudo pkill -9 apt-get;
     sudo pkill -9 dpkg;
     sudo dpkg --configure -a;
     ([ `sudo lshw -class display | grep "NVIDIA Corporation" | wc -l` -gt 0 ]) && (sudo which nvidia-smi > /dev/null || ( sudo apt-get install nvidia-driver-530-open -y && sudo apt-get install nvidia-driver-525-server -y ) || true);
     mkdir -p ~/.ssh; touch ~/.ssh/config;
-    pip3 --version > /dev/null 2>&1 || (curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py && python3 get-pip.py && echo "PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc);
+    {{ conda_installation_commands }}
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
-    {{ conda_installation_commands }}
     source ~/.bashrc;
     pip3 install oci;
     (pip3 list | grep ray | grep {{ray_version}} 2>&1 > /dev/null || pip3 install -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app && touch ~/.sudo_as_admin_successful;
     (pip3 list | grep skypilot && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/templates/scp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230724/sky/templates/scp-ray.yml.j2`

 * *Files 3% similar despite different names*

```diff
@@ -59,26 +59,24 @@
 # items!
 #
 # Increment the following for catching performance bugs easier:
 #   current num items (num SSH connections): 1
 setup_commands:
   # Disable `unattended-upgrades` to prevent apt-get from hanging. It should be called at the beginning before the process started to avoid being blocked. (This is a temporary fix.)
   # Create ~/.ssh/config file in case the file does not exist in the custom image.
-  # Make sure python3 & pip3 are available on this image.
   # We set auto_activate_base to be false for pre-installed conda.
   # This also kills the service that is holding the lock on dpkg (problem only exists on aws/azure, not gcp)
   # Line 'sudo bash ..': set the ulimit as suggested by ray docs for performance. https://docs.ray.io/en/latest/cluster/vms/user-guides/large-cluster-best-practices.html#system-configuration
   # Line 'sudo grep ..': set the number of threads per process to unlimited to avoid ray job submit stucking issue when the number of running ray jobs increase.
   # Line 'mkdir -p ..': disable host key check
   # Line 'python3 -c ..': patch the buggy ray files and enable `-o allow_other` option for `goofys`
   - mkdir -p ~/.ssh; touch ~/.ssh/config;
-    pip3 --version > /dev/null 2>&1 || (curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py && python3 get-pip.py && echo "PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc);
+    {{ conda_installation_commands }}
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
-    {{ conda_installation_commands }}
     source ~/.bashrc;
     (pip3 list | grep "ray " | grep {{ray_version}} 2>&1 > /dev/null || pip3 install --exists-action w -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app;
     (pip3 list | grep "skypilot " && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[scp]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
     python3 -c "from sky.skylet.ray_patches import patch; patch()" || exit 1;
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/templates/spot-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20230724/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/usage/constants.py` & `skypilot-nightly-1.0.0.dev20230724/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/usage/usage_lib.py` & `skypilot-nightly-1.0.0.dev20230724/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/utils/accelerator_registry.py` & `skypilot-nightly-1.0.0.dev20230724/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/utils/cli_utils/status_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/utils/command_runner.py` & `skypilot-nightly-1.0.0.dev20230724/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/utils/common_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/utils/dag_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/utils/db_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/utils/env_options.py` & `skypilot-nightly-1.0.0.dev20230724/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/utils/log_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/utils/schemas.py` & `skypilot-nightly-1.0.0.dev20230724/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/utils/subprocess_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/utils/timeline.py` & `skypilot-nightly-1.0.0.dev20230724/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/utils/tpu_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/utils/tpu_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/utils/ux_utils.py` & `skypilot-nightly-1.0.0.dev20230724/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/sky/utils/validator.py` & `skypilot-nightly-1.0.0.dev20230724/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/skypilot_nightly.egg-info/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230724/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230723
+Version: 1.0.0.dev20230724
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230723
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230724
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot-nightly-1.0.0.dev20230724/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/skypilot_nightly.egg-info/requires.txt` & `skypilot-nightly-1.0.0.dev20230724/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/tests/test_cli.py` & `skypilot-nightly-1.0.0.dev20230724/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/tests/test_config.py` & `skypilot-nightly-1.0.0.dev20230724/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/tests/test_jobs.py` & `skypilot-nightly-1.0.0.dev20230724/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/tests/test_list_accelerators.py` & `skypilot-nightly-1.0.0.dev20230724/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/tests/test_onprem.py` & `skypilot-nightly-1.0.0.dev20230724/tests/test_onprem.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/tests/test_optimizer_dryruns.py` & `skypilot-nightly-1.0.0.dev20230724/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/tests/test_optimizer_random_dag.py` & `skypilot-nightly-1.0.0.dev20230724/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/tests/test_smoke.py` & `skypilot-nightly-1.0.0.dev20230724/tests/test_smoke.py`

 * *Files 0% similar despite different names*

```diff
@@ -2863,5006 +2863,5008 @@
 0000b2e0: 2020 2020 2066 2773 6b79 206c 6f67 7320       f'sky logs 
 0000b2f0: 7b6e 616d 657d 2036 202d 2d73 7461 7475  {name} 6 --statu
 0000b300: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
 0000b310: 6627 736b 7920 6c6f 6773 207b 6e61 6d65  f'sky logs {name
 0000b320: 7d20 3720 2d2d 7374 6174 7573 272c 0a20  } 7 --status',. 
 0000b330: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
 0000b340: 2020 6627 736b 7920 646f 776e 202d 7920    f'sky down -y 
-0000b350: 7b6e 616d 657d 272c 0a20 2020 2029 0a20  {name}',.    ). 
-0000b360: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
-0000b370: 7465 7374 290a 0a0a 2320 2d2d 2d2d 2d2d  test)...# ------
-0000b380: 2d2d 2d2d 2053 7562 6d69 7474 696e 6720  ---- Submitting 
-0000b390: 6d75 6c74 6970 6c65 2074 6173 6b73 2074  multiple tasks t
-0000b3a0: 6f20 7468 6520 7361 6d65 2063 6c75 7374  o the same clust
-0000b3b0: 6572 2e20 2d2d 2d2d 2d2d 2d2d 2d2d 0a40  er. ----------.@
-0000b3c0: 7079 7465 7374 2e6d 6172 6b2e 6e6f 5f6c  pytest.mark.no_l
-0000b3d0: 616d 6264 615f 636c 6f75 6420 2023 204c  ambda_cloud  # L
-0000b3e0: 616d 6264 6120 436c 6f75 6420 646f 6573  ambda Cloud does
-0000b3f0: 206e 6f74 2068 6176 6520 4b38 3020 6770   not have K80 gp
-0000b400: 7573 0a40 7079 7465 7374 2e6d 6172 6b2e  us.@pytest.mark.
-0000b410: 6e6f 5f69 626d 2020 2320 4942 4d20 436c  no_ibm  # IBM Cl
-0000b420: 6f75 6420 646f 6573 206e 6f74 2068 6176  oud does not hav
-0000b430: 6520 4b38 3020 6770 7573 0a40 7079 7465  e K80 gpus.@pyte
-0000b440: 7374 2e6d 6172 6b2e 6e6f 5f73 6370 2020  st.mark.no_scp  
-0000b450: 2320 5343 5020 646f 6573 206e 6f74 2073  # SCP does not s
-0000b460: 7570 706f 7274 206e 756d 5f6e 6f64 6573  upport num_nodes
-0000b470: 203e 2031 2079 6574 0a40 7079 7465 7374   > 1 yet.@pytest
-0000b480: 2e6d 6172 6b2e 6e6f 5f6f 6369 2020 2320  .mark.no_oci  # 
-0000b490: 4f43 4920 436c 6f75 6420 646f 6573 206e  OCI Cloud does n
-0000b4a0: 6f74 2068 6176 6520 4b38 3020 6770 7573  ot have K80 gpus
-0000b4b0: 0a64 6566 2074 6573 745f 6d75 6c74 695f  .def test_multi_
-0000b4c0: 6563 686f 2867 656e 6572 6963 5f63 6c6f  echo(generic_clo
-0000b4d0: 7564 3a20 7374 7229 3a0a 2020 2020 6e61  ud: str):.    na
-0000b4e0: 6d65 203d 205f 6765 745f 636c 7573 7465  me = _get_cluste
-0000b4f0: 725f 6e61 6d65 2829 0a20 2020 2074 6573  r_name().    tes
-0000b500: 7420 3d20 5465 7374 280a 2020 2020 2020  t = Test(.      
-0000b510: 2020 276d 756c 7469 5f65 6368 6f27 2c0a    'multi_echo',.
-0000b520: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
-0000b530: 2020 2020 2020 6627 7079 7468 6f6e 2065        f'python e
-0000b540: 7861 6d70 6c65 732f 6d75 6c74 695f 6563  xamples/multi_ec
-0000b550: 686f 2e70 7920 7b6e 616d 657d 207b 6765  ho.py {name} {ge
-0000b560: 6e65 7269 635f 636c 6f75 647d 272c 0a20  neric_cloud}',. 
-0000b570: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
-0000b580: 7020 3132 3027 2c0a 2020 2020 2020 2020  p 120',.        
-0000b590: 5d20 2b0a 2020 2020 2020 2020 2320 456e  ] +.        # En
-0000b5a0: 7375 7265 206a 6f62 7320 7375 6363 6565  sure jobs succee
-0000b5b0: 6465 642e 0a20 2020 2020 2020 205b 6627  ded..        [f'
-0000b5c0: 736b 7920 6c6f 6773 207b 6e61 6d65 7d20  sky logs {name} 
-0000b5d0: 7b69 202b 2031 7d20 2d2d 7374 6174 7573  {i + 1} --status
-0000b5e0: 2720 666f 7220 6920 696e 2072 616e 6765  ' for i in range
-0000b5f0: 2833 3229 5d20 2b0a 2020 2020 2020 2020  (32)] +.        
-0000b600: 2320 456e 7375 7265 206d 6f6e 6974 6f72  # Ensure monitor
-0000b610: 2f61 7574 6f73 6361 6c65 7220 6469 646e  /autoscaler didn
-0000b620: 2774 2063 7261 7368 206f 6e20 7468 6520  't crash on the 
-0000b630: 2761 7373 6572 7420 6e6f 740a 2020 2020  'assert not.    
-0000b640: 2020 2020 2320 756e 6675 6c66 696c 6c65      # unfulfille
-0000b650: 6427 2065 7272 6f72 2e20 2049 6620 7072  d' error.  If pr
-0000b660: 6f63 6573 7320 6e6f 7420 666f 756e 642c  ocess not found,
-0000b670: 2067 7265 702d 3e73 7368 2072 6574 7572   grep->ssh retur
-0000b680: 6e73 2031 2e0a 2020 2020 2020 2020 5b66  ns 1..        [f
-0000b690: 2773 7368 207b 6e61 6d65 7d20 5c27 7073  'ssh {name} \'ps
-0000b6a0: 2061 7578 207c 2067 7265 7020 225b 2f5d   aux | grep "[/]
-0000b6b0: 226d 6f6e 6974 6f72 2e70 795c 2727 5d2c  "monitor.py\''],
-0000b6c0: 0a20 2020 2020 2020 2066 2773 6b79 2064  .        f'sky d
-0000b6d0: 6f77 6e20 2d79 207b 6e61 6d65 7d27 2c0a  own -y {name}',.
-0000b6e0: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
-0000b6f0: 3230 202a 2036 302c 0a20 2020 2029 0a20  20 * 60,.    ). 
-0000b700: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
-0000b710: 7465 7374 290a 0a0a 2320 2d2d 2d2d 2d2d  test)...# ------
-0000b720: 2d2d 2d2d 2054 6173 6b3a 2031 206e 6f64  ---- Task: 1 nod
-0000b730: 6520 7472 6169 6e69 6e67 2e20 2d2d 2d2d  e training. ----
-0000b740: 2d2d 2d2d 2d2d 0a40 7079 7465 7374 2e6d  ------.@pytest.m
-0000b750: 6172 6b2e 6e6f 5f6c 616d 6264 615f 636c  ark.no_lambda_cl
-0000b760: 6f75 6420 2023 204c 616d 6264 6120 436c  oud  # Lambda Cl
-0000b770: 6f75 6420 646f 6573 206e 6f74 2068 6176  oud does not hav
-0000b780: 6520 5631 3030 2067 7075 730a 4070 7974  e V100 gpus.@pyt
-0000b790: 6573 742e 6d61 726b 2e6e 6f5f 6962 6d20  est.mark.no_ibm 
-0000b7a0: 2023 2049 424d 2063 6c6f 7564 2063 7572   # IBM cloud cur
-0000b7b0: 7265 6e74 6c79 2064 6f65 736e 2774 2070  rently doesn't p
-0000b7c0: 726f 7669 6465 2070 7562 6c69 6320 696d  rovide public im
-0000b7d0: 6167 6520 7769 7468 2043 5544 410a 4070  age with CUDA.@p
-0000b7e0: 7974 6573 742e 6d61 726b 2e6e 6f5f 7363  ytest.mark.no_sc
-0000b7f0: 7020 2023 2053 4350 2064 6f65 7320 6e6f  p  # SCP does no
-0000b800: 7420 6861 7665 2056 3130 3020 2831 3647  t have V100 (16G
-0000b810: 4229 2047 5055 732e 2052 756e 2074 6573  B) GPUs. Run tes
-0000b820: 745f 7363 705f 6875 6767 696e 6766 6163  t_scp_huggingfac
-0000b830: 6520 696e 7374 6561 642e 0a64 6566 2074  e instead..def t
-0000b840: 6573 745f 6875 6767 696e 6766 6163 6528  est_huggingface(
-0000b850: 6765 6e65 7269 635f 636c 6f75 643a 2073  generic_cloud: s
-0000b860: 7472 293a 0a20 2020 206e 616d 6520 3d20  tr):.    name = 
-0000b870: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
-0000b880: 6528 290a 2020 2020 7465 7374 203d 2054  e().    test = T
-0000b890: 6573 7428 0a20 2020 2020 2020 2027 6875  est(.        'hu
-0000b8a0: 6767 696e 6766 6163 655f 676c 7565 5f69  ggingface_glue_i
-0000b8b0: 6d64 625f 6170 7027 2c0a 2020 2020 2020  mdb_app',.      
-0000b8c0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-0000b8d0: 6627 736b 7920 6c61 756e 6368 202d 7920  f'sky launch -y 
-0000b8e0: 2d63 207b 6e61 6d65 7d20 2d2d 636c 6f75  -c {name} --clou
-0000b8f0: 6420 7b67 656e 6572 6963 5f63 6c6f 7564  d {generic_cloud
-0000b900: 7d20 6578 616d 706c 6573 2f68 7567 6769  } examples/huggi
-0000b910: 6e67 6661 6365 5f67 6c75 655f 696d 6462  ngface_glue_imdb
-0000b920: 5f61 7070 2e79 616d 6c27 2c0a 2020 2020  _app.yaml',.    
-0000b930: 2020 2020 2020 2020 6627 736b 7920 6c6f          f'sky lo
-0000b940: 6773 207b 6e61 6d65 7d20 3120 2d2d 7374  gs {name} 1 --st
-0000b950: 6174 7573 272c 2020 2320 456e 7375 7265  atus',  # Ensure
-0000b960: 2074 6865 206a 6f62 2073 7563 6365 6564   the job succeed
-0000b970: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-0000b980: 6627 736b 7920 6578 6563 207b 6e61 6d65  f'sky exec {name
-0000b990: 7d20 6578 616d 706c 6573 2f68 7567 6769  } examples/huggi
-0000b9a0: 6e67 6661 6365 5f67 6c75 655f 696d 6462  ngface_glue_imdb
-0000b9b0: 5f61 7070 2e79 616d 6c27 2c0a 2020 2020  _app.yaml',.    
-0000b9c0: 2020 2020 2020 2020 6627 736b 7920 6c6f          f'sky lo
-0000b9d0: 6773 207b 6e61 6d65 7d20 3220 2d2d 7374  gs {name} 2 --st
-0000b9e0: 6174 7573 272c 2020 2320 456e 7375 7265  atus',  # Ensure
-0000b9f0: 2074 6865 206a 6f62 2073 7563 6365 6564   the job succeed
-0000ba00: 6564 2e0a 2020 2020 2020 2020 5d2c 0a20  ed..        ],. 
-0000ba10: 2020 2020 2020 2066 2773 6b79 2064 6f77         f'sky dow
-0000ba20: 6e20 2d79 207b 6e61 6d65 7d27 2c0a 2020  n -y {name}',.  
-0000ba30: 2020 290a 2020 2020 7275 6e5f 6f6e 655f    ).    run_one_
-0000ba40: 7465 7374 2874 6573 7429 0a0a 0a40 7079  test(test)...@py
-0000ba50: 7465 7374 2e6d 6172 6b2e 6c61 6d62 6461  test.mark.lambda
-0000ba60: 5f63 6c6f 7564 0a64 6566 2074 6573 745f  _cloud.def test_
-0000ba70: 6c61 6d62 6461 5f68 7567 6769 6e67 6661  lambda_huggingfa
-0000ba80: 6365 2867 656e 6572 6963 5f63 6c6f 7564  ce(generic_cloud
-0000ba90: 3a20 7374 7229 3a0a 2020 2020 6e61 6d65  : str):.    name
-0000baa0: 203d 205f 6765 745f 636c 7573 7465 725f   = _get_cluster_
-0000bab0: 6e61 6d65 2829 0a20 2020 2074 6573 7420  name().    test 
-0000bac0: 3d20 5465 7374 280a 2020 2020 2020 2020  = Test(.        
-0000bad0: 276c 616d 6264 615f 6875 6767 696e 6766  'lambda_huggingf
-0000bae0: 6163 655f 676c 7565 5f69 6d64 625f 6170  ace_glue_imdb_ap
-0000baf0: 7027 2c0a 2020 2020 2020 2020 5b0a 2020  p',.        [.  
-0000bb00: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-0000bb10: 6c61 756e 6368 202d 7920 2d63 207b 6e61  launch -y -c {na
-0000bb20: 6d65 7d20 7b4c 414d 4244 415f 5459 5045  me} {LAMBDA_TYPE
-0000bb30: 7d20 6578 616d 706c 6573 2f68 7567 6769  } examples/huggi
-0000bb40: 6e67 6661 6365 5f67 6c75 655f 696d 6462  ngface_glue_imdb
-0000bb50: 5f61 7070 2e79 616d 6c27 2c0a 2020 2020  _app.yaml',.    
-0000bb60: 2020 2020 2020 2020 6627 736b 7920 6c6f          f'sky lo
-0000bb70: 6773 207b 6e61 6d65 7d20 3120 2d2d 7374  gs {name} 1 --st
-0000bb80: 6174 7573 272c 2020 2320 456e 7375 7265  atus',  # Ensure
-0000bb90: 2074 6865 206a 6f62 2073 7563 6365 6564   the job succeed
-0000bba0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-0000bbb0: 6627 736b 7920 6578 6563 207b 6e61 6d65  f'sky exec {name
-0000bbc0: 7d20 7b4c 414d 4244 415f 5459 5045 7d20  } {LAMBDA_TYPE} 
-0000bbd0: 6578 616d 706c 6573 2f68 7567 6769 6e67  examples/hugging
-0000bbe0: 6661 6365 5f67 6c75 655f 696d 6462 5f61  face_glue_imdb_a
-0000bbf0: 7070 2e79 616d 6c27 2c0a 2020 2020 2020  pp.yaml',.      
-0000bc00: 2020 2020 2020 6627 736b 7920 6c6f 6773        f'sky logs
-0000bc10: 207b 6e61 6d65 7d20 3220 2d2d 7374 6174   {name} 2 --stat
-0000bc20: 7573 272c 2020 2320 456e 7375 7265 2074  us',  # Ensure t
-0000bc30: 6865 206a 6f62 2073 7563 6365 6564 6564  he job succeeded
-0000bc40: 2e0a 2020 2020 2020 2020 5d2c 0a20 2020  ..        ],.   
-0000bc50: 2020 2020 2066 2773 6b79 2064 6f77 6e20       f'sky down 
-0000bc60: 2d79 207b 6e61 6d65 7d27 2c0a 2020 2020  -y {name}',.    
-0000bc70: 290a 2020 2020 7275 6e5f 6f6e 655f 7465  ).    run_one_te
-0000bc80: 7374 2874 6573 7429 0a0a 0a40 7079 7465  st(test)...@pyte
-0000bc90: 7374 2e6d 6172 6b2e 7363 700a 6465 6620  st.mark.scp.def 
-0000bca0: 7465 7374 5f73 6370 5f68 7567 6769 6e67  test_scp_hugging
-0000bcb0: 6661 6365 2867 656e 6572 6963 5f63 6c6f  face(generic_clo
-0000bcc0: 7564 3a20 7374 7229 3a0a 2020 2020 6e61  ud: str):.    na
-0000bcd0: 6d65 203d 205f 6765 745f 636c 7573 7465  me = _get_cluste
-0000bce0: 725f 6e61 6d65 2829 0a20 2020 206e 756d  r_name().    num
-0000bcf0: 5f6f 665f 6770 755f 6c61 756e 6368 203d  _of_gpu_launch =
-0000bd00: 2031 0a20 2020 2074 6573 7420 3d20 5465   1.    test = Te
-0000bd10: 7374 280a 2020 2020 2020 2020 2753 4350  st(.        'SCP
-0000bd20: 5f68 7567 6769 6e67 6661 6365 5f67 6c75  _huggingface_glu
-0000bd30: 655f 696d 6462 5f61 7070 272c 0a20 2020  e_imdb_app',.   
-0000bd40: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-0000bd50: 2020 2066 2773 6b79 206c 6175 6e63 6820     f'sky launch 
-0000bd60: 2d79 202d 6320 7b6e 616d 657d 207b 5343  -y -c {name} {SC
-0000bd70: 505f 5459 5045 7d20 7b53 4350 5f47 5055  P_TYPE} {SCP_GPU
-0000bd80: 5f56 3130 307d 3a7b 6e75 6d5f 6f66 5f67  _V100}:{num_of_g
-0000bd90: 7075 5f6c 6175 6e63 687d 2065 7861 6d70  pu_launch} examp
-0000bda0: 6c65 732f 6875 6767 696e 6766 6163 655f  les/huggingface_
-0000bdb0: 676c 7565 5f69 6d64 625f 6170 702e 7961  glue_imdb_app.ya
-0000bdc0: 6d6c 272c 0a20 2020 2020 2020 2020 2020  ml',.           
-0000bdd0: 2066 2773 6b79 206c 6f67 7320 7b6e 616d   f'sky logs {nam
-0000bde0: 657d 2031 202d 2d73 7461 7475 7327 2c20  e} 1 --status', 
-0000bdf0: 2023 2045 6e73 7572 6520 7468 6520 6a6f   # Ensure the jo
-0000be00: 6220 7375 6363 6565 6465 642e 0a20 2020  b succeeded..   
-0000be10: 2020 2020 2020 2020 2066 2773 6b79 2065           f'sky e
-0000be20: 7865 6320 7b6e 616d 657d 207b 5343 505f  xec {name} {SCP_
-0000be30: 5459 5045 7d20 7b53 4350 5f47 5055 5f56  TYPE} {SCP_GPU_V
-0000be40: 3130 307d 3a7b 6e75 6d5f 6f66 5f67 7075  100}:{num_of_gpu
-0000be50: 5f6c 6175 6e63 687d 2065 7861 6d70 6c65  _launch} example
-0000be60: 732f 6875 6767 696e 6766 6163 655f 676c  s/huggingface_gl
-0000be70: 7565 5f69 6d64 625f 6170 702e 7961 6d6c  ue_imdb_app.yaml
-0000be80: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-0000be90: 2773 6b79 206c 6f67 7320 7b6e 616d 657d  'sky logs {name}
-0000bea0: 2032 202d 2d73 7461 7475 7327 2c20 2023   2 --status',  #
-0000beb0: 2045 6e73 7572 6520 7468 6520 6a6f 6220   Ensure the job 
-0000bec0: 7375 6363 6565 6465 642e 0a20 2020 2020  succeeded..     
-0000bed0: 2020 205d 2c0a 2020 2020 2020 2020 6627     ],.        f'
-0000bee0: 736b 7920 646f 776e 202d 7920 7b6e 616d  sky down -y {nam
-0000bef0: 657d 272c 0a20 2020 2029 0a20 2020 2072  e}',.    ).    r
-0000bf00: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
-0000bf10: 290a 0a0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  )...# ----------
-0000bf20: 2054 5055 2e20 2d2d 2d2d 2d2d 2d2d 2d2d   TPU. ----------
-0000bf30: 0a40 7079 7465 7374 2e6d 6172 6b2e 6763  .@pytest.mark.gc
-0000bf40: 700a 6465 6620 7465 7374 5f74 7075 2829  p.def test_tpu()
-0000bf50: 3a0a 2020 2020 6e61 6d65 203d 205f 6765  :.    name = _ge
-0000bf60: 745f 636c 7573 7465 725f 6e61 6d65 2829  t_cluster_name()
-0000bf70: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
-0000bf80: 280a 2020 2020 2020 2020 2774 7075 5f61  (.        'tpu_a
-0000bf90: 7070 272c 0a20 2020 2020 2020 205b 0a20  pp',.        [. 
-0000bfa0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-0000bfb0: 206c 6175 6e63 6820 2d79 202d 6320 7b6e   launch -y -c {n
-0000bfc0: 616d 657d 2065 7861 6d70 6c65 732f 7470  ame} examples/tp
-0000bfd0: 752f 7470 755f 6170 702e 7961 6d6c 272c  u/tpu_app.yaml',
-0000bfe0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000bff0: 6b79 206c 6f67 7320 7b6e 616d 657d 2031  ky logs {name} 1
-0000c000: 272c 2020 2320 456e 7375 7265 2074 6865  ',  # Ensure the
-0000c010: 206a 6f62 2066 696e 6973 6865 642e 0a20   job finished.. 
-0000c020: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-0000c030: 206c 6f67 7320 7b6e 616d 657d 2031 202d   logs {name} 1 -
-0000c040: 2d73 7461 7475 7327 2c20 2023 2045 6e73  -status',  # Ens
-0000c050: 7572 6520 7468 6520 6a6f 6220 7375 6363  ure the job succ
-0000c060: 6565 6465 642e 0a20 2020 2020 2020 2020  eeded..         
-0000c070: 2020 2066 2773 6b79 206c 6175 6e63 6820     f'sky launch 
-0000c080: 2d79 202d 6320 7b6e 616d 657d 2065 7861  -y -c {name} exa
-0000c090: 6d70 6c65 732f 7470 752f 7470 755f 6170  mples/tpu/tpu_ap
-0000c0a0: 702e 7961 6d6c 207c 2067 7265 7020 2254  p.yaml | grep "T
-0000c0b0: 5055 202e 2a20 616c 7265 6164 7920 6578  PU .* already ex
-0000c0c0: 6973 7473 2227 2c20 2023 2045 6e73 7572  ists"',  # Ensur
-0000c0d0: 6520 736b 7920 6c61 756e 6368 2077 6f6e  e sky launch won
-0000c0e0: 2774 2063 7265 6174 6520 616e 6f74 6865  't create anothe
-0000c0f0: 7220 5450 552e 0a20 2020 2020 2020 205d  r TPU..        ]
-0000c100: 2c0a 2020 2020 2020 2020 6627 736b 7920  ,.        f'sky 
-0000c110: 646f 776e 202d 7920 7b6e 616d 657d 272c  down -y {name}',
-0000c120: 0a20 2020 2020 2020 2074 696d 656f 7574  .        timeout
-0000c130: 3d33 3020 2a20 3630 2c20 2023 2063 616e  =30 * 60,  # can
-0000c140: 2074 616b 6520 3e32 3020 6d69 6e73 0a20   take >20 mins. 
-0000c150: 2020 2029 0a20 2020 2072 756e 5f6f 6e65     ).    run_one
-0000c160: 5f74 6573 7428 7465 7374 290a 0a0a 2320  _test(test)...# 
-0000c170: 2d2d 2d2d 2d2d 2d2d 2d2d 2054 5055 2056  ---------- TPU V
-0000c180: 4d2e 202d 2d2d 2d2d 2d2d 2d2d 2d0a 4070  M. ----------.@p
-0000c190: 7974 6573 742e 6d61 726b 2e67 6370 0a64  ytest.mark.gcp.d
-0000c1a0: 6566 2074 6573 745f 7470 755f 766d 2829  ef test_tpu_vm()
-0000c1b0: 3a0a 2020 2020 6e61 6d65 203d 205f 6765  :.    name = _ge
-0000c1c0: 745f 636c 7573 7465 725f 6e61 6d65 2829  t_cluster_name()
-0000c1d0: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
-0000c1e0: 280a 2020 2020 2020 2020 2774 7075 5f76  (.        'tpu_v
-0000c1f0: 6d5f 6170 7027 2c0a 2020 2020 2020 2020  m_app',.        
-0000c200: 5b0a 2020 2020 2020 2020 2020 2020 6627  [.            f'
-0000c210: 736b 7920 6c61 756e 6368 202d 7920 2d63  sky launch -y -c
-0000c220: 207b 6e61 6d65 7d20 6578 616d 706c 6573   {name} examples
-0000c230: 2f74 7075 2f74 7075 766d 5f6d 6e69 7374  /tpu/tpuvm_mnist
-0000c240: 2e79 616d 6c27 2c0a 2020 2020 2020 2020  .yaml',.        
-0000c250: 2020 2020 6627 736b 7920 6c6f 6773 207b      f'sky logs {
-0000c260: 6e61 6d65 7d20 3127 2c20 2023 2045 6e73  name} 1',  # Ens
-0000c270: 7572 6520 7468 6520 6a6f 6220 6669 6e69  ure the job fini
-0000c280: 7368 6564 2e0a 2020 2020 2020 2020 2020  shed..          
-0000c290: 2020 6627 736b 7920 6c6f 6773 207b 6e61    f'sky logs {na
-0000c2a0: 6d65 7d20 3120 2d2d 7374 6174 7573 272c  me} 1 --status',
-0000c2b0: 2020 2320 456e 7375 7265 2074 6865 206a    # Ensure the j
-0000c2c0: 6f62 2073 7563 6365 6564 6564 2e0a 2020  ob succeeded..  
-0000c2d0: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-0000c2e0: 7374 6f70 202d 7920 7b6e 616d 657d 272c  stop -y {name}',
-0000c2f0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000c300: 3d24 2873 6b79 2073 7461 7475 7320 7b6e  =$(sky status {n
-0000c310: 616d 657d 202d 2d72 6566 7265 7368 293b  ame} --refresh);
-0000c320: 2065 6368 6f20 2224 7322 3b20 6563 686f   echo "$s"; echo
-0000c330: 3b20 6563 686f 3b20 6563 686f 2022 2473  ; echo; echo "$s
-0000c340: 2220 207c 2067 7265 7020 7b6e 616d 657d  "  | grep {name}
-0000c350: 207c 2067 7265 7020 5354 4f50 5045 4427   | grep STOPPED'
-0000c360: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
-0000c370: 636c 7573 7465 7220 6973 2053 544f 5050  cluster is STOPP
-0000c380: 4544 2e0a 2020 2020 2020 2020 2020 2020  ED..            
-0000c390: 2320 5573 6520 7265 7472 793a 2067 7561  # Use retry: gua
-0000c3a0: 7264 2061 6761 696e 7374 2074 7261 6e73  rd against trans
-0000c3b0: 6965 6e74 2065 7272 6f72 7320 6f62 7365  ient errors obse
-0000c3c0: 7276 6564 2066 6f72 0a20 2020 2020 2020  rved for.       
-0000c3d0: 2020 2020 2023 206a 7573 742d 7374 6f70       # just-stop
-0000c3e0: 7065 6420 5450 5520 564d 7320 2823 3936  ped TPU VMs (#96
-0000c3f0: 3229 2e0a 2020 2020 2020 2020 2020 2020  2)..            
-0000c400: 6627 736b 7920 7374 6172 7420 2d2d 7265  f'sky start --re
-0000c410: 7472 792d 756e 7469 6c2d 7570 202d 7920  try-until-up -y 
-0000c420: 7b6e 616d 657d 272c 0a20 2020 2020 2020  {name}',.       
-0000c430: 2020 2020 2066 2773 6b79 2065 7865 6320       f'sky exec 
-0000c440: 7b6e 616d 657d 2065 7861 6d70 6c65 732f  {name} examples/
-0000c450: 7470 752f 7470 7576 6d5f 6d6e 6973 742e  tpu/tpuvm_mnist.
-0000c460: 7961 6d6c 272c 0a20 2020 2020 2020 2020  yaml',.         
-0000c470: 2020 2066 2773 6b79 206c 6f67 7320 7b6e     f'sky logs {n
-0000c480: 616d 657d 2032 202d 2d73 7461 7475 7327  ame} 2 --status'
-0000c490: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
-0000c4a0: 6a6f 6220 7375 6363 6565 6465 642e 0a20  job succeeded.. 
-0000c4b0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-0000c4c0: 2073 746f 7020 2d79 207b 6e61 6d65 7d27   stop -y {name}'
-0000c4d0: 2c0a 2020 2020 2020 2020 5d2c 0a20 2020  ,.        ],.   
-0000c4e0: 2020 2020 2066 2773 6b79 2064 6f77 6e20       f'sky down 
-0000c4f0: 2d79 207b 6e61 6d65 7d27 2c0a 2020 2020  -y {name}',.    
-0000c500: 2020 2020 7469 6d65 6f75 743d 3330 202a      timeout=30 *
-0000c510: 2036 302c 2020 2320 6361 6e20 7461 6b65   60,  # can take
-0000c520: 2033 3020 6d69 6e73 0a20 2020 2029 0a20   30 mins.    ). 
-0000c530: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
-0000c540: 7465 7374 290a 0a0a 2320 2d2d 2d2d 2d2d  test)...# ------
-0000c550: 2d2d 2d2d 2054 5055 2056 4d20 506f 642e  ---- TPU VM Pod.
-0000c560: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 4070 7974   ----------.@pyt
-0000c570: 6573 742e 6d61 726b 2e67 6370 0a64 6566  est.mark.gcp.def
-0000c580: 2074 6573 745f 7470 755f 766d 5f70 6f64   test_tpu_vm_pod
-0000c590: 2829 3a0a 2020 2020 6e61 6d65 203d 205f  ():.    name = _
-0000c5a0: 6765 745f 636c 7573 7465 725f 6e61 6d65  get_cluster_name
-0000c5b0: 2829 0a20 2020 2074 6573 7420 3d20 5465  ().    test = Te
-0000c5c0: 7374 280a 2020 2020 2020 2020 2774 7075  st(.        'tpu
-0000c5d0: 5f70 6f64 272c 0a20 2020 2020 2020 205b  _pod',.        [
-0000c5e0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000c5f0: 6b79 206c 6175 6e63 6820 2d79 202d 6320  ky launch -y -c 
-0000c600: 7b6e 616d 657d 2065 7861 6d70 6c65 732f  {name} examples/
-0000c610: 7470 752f 7470 7576 6d5f 6d6e 6973 742e  tpu/tpuvm_mnist.
-0000c620: 7961 6d6c 202d 2d67 7075 7320 7470 752d  yaml --gpus tpu-
-0000c630: 7632 2d33 3220 2d2d 7573 652d 7370 6f74  v2-32 --use-spot
-0000c640: 202d 2d7a 6f6e 6520 6575 726f 7065 2d77   --zone europe-w
-0000c650: 6573 7434 2d61 272c 0a20 2020 2020 2020  est4-a',.       
-0000c660: 2020 2020 2066 2773 6b79 206c 6f67 7320       f'sky logs 
-0000c670: 7b6e 616d 657d 2031 272c 2020 2320 456e  {name} 1',  # En
-0000c680: 7375 7265 2074 6865 206a 6f62 2066 696e  sure the job fin
-0000c690: 6973 6865 642e 0a20 2020 2020 2020 2020  ished..         
-0000c6a0: 2020 2066 2773 6b79 206c 6f67 7320 7b6e     f'sky logs {n
-0000c6b0: 616d 657d 2031 202d 2d73 7461 7475 7327  ame} 1 --status'
-0000c6c0: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
-0000c6d0: 6a6f 6220 7375 6363 6565 6465 642e 0a20  job succeeded.. 
-0000c6e0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-0000c6f0: 2020 6627 736b 7920 646f 776e 202d 7920    f'sky down -y 
-0000c700: 7b6e 616d 657d 272c 0a20 2020 2020 2020  {name}',.       
-0000c710: 2074 696d 656f 7574 3d33 3020 2a20 3630   timeout=30 * 60
-0000c720: 2c20 2023 2063 616e 2074 616b 6520 3330  ,  # can take 30
-0000c730: 206d 696e 730a 2020 2020 290a 2020 2020   mins.    ).    
-0000c740: 7275 6e5f 6f6e 655f 7465 7374 2874 6573  run_one_test(tes
-0000c750: 7429 0a0a 0a23 202d 2d2d 2d2d 2d2d 2d2d  t)...# ---------
-0000c760: 2d20 5369 6d70 6c65 2061 7070 732e 202d  - Simple apps. -
-0000c770: 2d2d 2d2d 2d2d 2d2d 2d0a 4070 7974 6573  ---------.@pytes
-0000c780: 742e 6d61 726b 2e6e 6f5f 7363 7020 2023  t.mark.no_scp  #
-0000c790: 2053 4350 2064 6f65 7320 6e6f 7420 7375   SCP does not su
-0000c7a0: 7070 6f72 7420 6e75 6d5f 6e6f 6465 7320  pport num_nodes 
-0000c7b0: 3e20 3120 7965 740a 6465 6620 7465 7374  > 1 yet.def test
-0000c7c0: 5f6d 756c 7469 5f68 6f73 746e 616d 6528  _multi_hostname(
-0000c7d0: 6765 6e65 7269 635f 636c 6f75 643a 2073  generic_cloud: s
-0000c7e0: 7472 293a 0a20 2020 206e 616d 6520 3d20  tr):.    name = 
-0000c7f0: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
-0000c800: 6528 290a 2020 2020 7465 7374 203d 2054  e().    test = T
-0000c810: 6573 7428 0a20 2020 2020 2020 2027 6d75  est(.        'mu
-0000c820: 6c74 695f 686f 7374 6e61 6d65 272c 0a20  lti_hostname',. 
-0000c830: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-0000c840: 2020 2020 2066 2773 6b79 206c 6175 6e63       f'sky launc
-0000c850: 6820 2d79 202d 6320 7b6e 616d 657d 202d  h -y -c {name} -
-0000c860: 2d63 6c6f 7564 207b 6765 6e65 7269 635f  -cloud {generic_
-0000c870: 636c 6f75 647d 2065 7861 6d70 6c65 732f  cloud} examples/
-0000c880: 6d75 6c74 695f 686f 7374 6e61 6d65 2e79  multi_hostname.y
-0000c890: 616d 6c27 2c0a 2020 2020 2020 2020 2020  aml',.          
-0000c8a0: 2020 6627 736b 7920 6c6f 6773 207b 6e61    f'sky logs {na
-0000c8b0: 6d65 7d20 3120 2d2d 7374 6174 7573 272c  me} 1 --status',
-0000c8c0: 2020 2320 456e 7375 7265 2074 6865 206a    # Ensure the j
-0000c8d0: 6f62 2073 7563 6365 6564 6564 2e0a 2020  ob succeeded..  
-0000c8e0: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-0000c8f0: 6c6f 6773 207b 6e61 6d65 7d20 3120 7c20  logs {name} 1 | 
-0000c900: 6772 6570 2022 4d79 2068 6f73 746e 616d  grep "My hostnam
-0000c910: 653a 2220 7c20 7763 202d 6c20 7c20 6772  e:" | wc -l | gr
-0000c920: 6570 2032 272c 2020 2320 456e 7375 7265  ep 2',  # Ensure
-0000c930: 2074 6865 7265 2061 7265 2032 2068 6f73   there are 2 hos
-0000c940: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
-0000c950: 6627 736b 7920 6578 6563 207b 6e61 6d65  f'sky exec {name
-0000c960: 7d20 6578 616d 706c 6573 2f6d 756c 7469  } examples/multi
-0000c970: 5f68 6f73 746e 616d 652e 7961 6d6c 272c  _hostname.yaml',
-0000c980: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000c990: 6b79 206c 6f67 7320 7b6e 616d 657d 2032  ky logs {name} 2
-0000c9a0: 202d 2d73 7461 7475 7327 2c20 2023 2045   --status',  # E
-0000c9b0: 6e73 7572 6520 7468 6520 6a6f 6220 7375  nsure the job su
-0000c9c0: 6363 6565 6465 642e 0a20 2020 2020 2020  cceeded..       
-0000c9d0: 205d 2c0a 2020 2020 2020 2020 6627 736b   ],.        f'sk
-0000c9e0: 7920 646f 776e 202d 7920 7b6e 616d 657d  y down -y {name}
-0000c9f0: 272c 0a20 2020 2029 0a20 2020 2072 756e  ',.    ).    run
-0000ca00: 5f6f 6e65 5f74 6573 7428 7465 7374 290a  _one_test(test).
-0000ca10: 0a0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2054  ..# ---------- T
-0000ca20: 6173 6b3a 206e 3d32 206e 6f64 6573 2077  ask: n=2 nodes w
-0000ca30: 6974 6820 7365 7475 7073 2e20 2d2d 2d2d  ith setups. ----
-0000ca40: 2d2d 2d2d 2d2d 0a40 7079 7465 7374 2e6d  ------.@pytest.m
-0000ca50: 6172 6b2e 6e6f 5f6c 616d 6264 615f 636c  ark.no_lambda_cl
-0000ca60: 6f75 6420 2023 204c 616d 6264 6120 436c  oud  # Lambda Cl
-0000ca70: 6f75 6420 646f 6573 206e 6f74 2068 6176  oud does not hav
-0000ca80: 6520 5631 3030 2067 7075 730a 4070 7974  e V100 gpus.@pyt
-0000ca90: 6573 742e 6d61 726b 2e6e 6f5f 6962 6d20  est.mark.no_ibm 
-0000caa0: 2023 2049 424d 2063 6c6f 7564 2063 7572   # IBM cloud cur
-0000cab0: 7265 6e74 6c79 2064 6f65 736e 2774 2070  rently doesn't p
-0000cac0: 726f 7669 6465 2070 7562 6c69 6320 696d  rovide public im
-0000cad0: 6167 6520 7769 7468 2043 5544 410a 4070  age with CUDA.@p
-0000cae0: 7974 6573 742e 6d61 726b 2e6e 6f5f 7363  ytest.mark.no_sc
-0000caf0: 7020 2023 2053 4350 2064 6f65 7320 6e6f  p  # SCP does no
-0000cb00: 7420 7375 7070 6f72 7420 6e75 6d5f 6e6f  t support num_no
-0000cb10: 6465 7320 3e20 3120 7965 740a 4070 7974  des > 1 yet.@pyt
-0000cb20: 6573 742e 6d61 726b 2e73 6b69 7028 0a20  est.mark.skip(. 
-0000cb30: 2020 2072 6561 736f 6e3d 0a20 2020 2027     reason=.    '
-0000cb40: 5468 6520 7265 736e 6574 5f64 6973 7472  The resnet_distr
-0000cb50: 6962 7574 6564 5f74 665f 6170 7020 6973  ibuted_tf_app is
-0000cb60: 2066 6c61 6b79 2c20 6475 6520 746f 2069   flaky, due to i
-0000cb70: 7420 6661 696c 696e 6720 746f 2064 6574  t failing to det
-0000cb80: 6563 7420 4750 5573 2e27 290a 6465 6620  ect GPUs.').def 
-0000cb90: 7465 7374 5f64 6973 7472 6962 7574 6564  test_distributed
-0000cba0: 5f74 6628 6765 6e65 7269 635f 636c 6f75  _tf(generic_clou
-0000cbb0: 643a 2073 7472 293a 0a20 2020 206e 616d  d: str):.    nam
-0000cbc0: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
-0000cbd0: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
-0000cbe0: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
-0000cbf0: 2027 7265 736e 6574 5f64 6973 7472 6962   'resnet_distrib
-0000cc00: 7574 6564 5f74 665f 6170 7027 2c0a 2020  uted_tf_app',.  
-0000cc10: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-0000cc20: 2020 2020 2320 4e4f 5445 3a20 7275 6e6e      # NOTE: runn
-0000cc30: 696e 6720 6974 2074 7769 6365 2077 696c  ing it twice wil
-0000cc40: 6c20 6861 6e67 2028 736f 6d65 7469 6d65  l hang (sometime
-0000cc50: 733f 2920 2d20 616e 2061 7070 2d6c 6576  s?) - an app-lev
-0000cc60: 656c 2062 7567 2e0a 2020 2020 2020 2020  el bug..        
-0000cc70: 2020 2020 6627 7079 7468 6f6e 2065 7861      f'python exa
-0000cc80: 6d70 6c65 732f 7265 736e 6574 5f64 6973  mples/resnet_dis
-0000cc90: 7472 6962 7574 6564 5f74 665f 6170 702e  tributed_tf_app.
-0000cca0: 7079 207b 6e61 6d65 7d20 7b67 656e 6572  py {name} {gener
-0000ccb0: 6963 5f63 6c6f 7564 7d27 2c0a 2020 2020  ic_cloud}',.    
-0000ccc0: 2020 2020 2020 2020 6627 736b 7920 6c6f          f'sky lo
-0000ccd0: 6773 207b 6e61 6d65 7d20 3120 2d2d 7374  gs {name} 1 --st
-0000cce0: 6174 7573 272c 2020 2320 456e 7375 7265  atus',  # Ensure
-0000ccf0: 2074 6865 206a 6f62 2073 7563 6365 6564   the job succeed
-0000cd00: 6564 2e0a 2020 2020 2020 2020 5d2c 0a20  ed..        ],. 
-0000cd10: 2020 2020 2020 2066 2773 6b79 2064 6f77         f'sky dow
-0000cd20: 6e20 2d79 207b 6e61 6d65 7d27 2c0a 2020  n -y {name}',.  
-0000cd30: 2020 2020 2020 7469 6d65 6f75 743d 3235        timeout=25
-0000cd40: 202a 2036 302c 2020 2320 3235 206d 696e   * 60,  # 25 min
-0000cd50: 7320 2869 7420 7461 6b65 7320 6172 6f75  s (it takes arou
-0000cd60: 6e64 207e 3139 206d 696e 7329 0a20 2020  nd ~19 mins).   
-0000cd70: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
-0000cd80: 6573 7428 7465 7374 290a 0a0a 2320 2d2d  est(test)...# --
-0000cd90: 2d2d 2d2d 2d2d 2d2d 2054 6573 7469 6e67  -------- Testing
-0000cda0: 2047 4350 2073 7461 7274 2061 6e64 2073   GCP start and s
-0000cdb0: 746f 7020 696e 7374 616e 6365 7320 2d2d  top instances --
-0000cdc0: 2d2d 2d2d 2d2d 2d2d 0a40 7079 7465 7374  --------.@pytest
-0000cdd0: 2e6d 6172 6b2e 6763 700a 6465 6620 7465  .mark.gcp.def te
-0000cde0: 7374 5f67 6370 5f73 7461 7274 5f73 746f  st_gcp_start_sto
-0000cdf0: 7028 293a 0a20 2020 206e 616d 6520 3d20  p():.    name = 
-0000ce00: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
-0000ce10: 6528 290a 2020 2020 7465 7374 203d 2054  e().    test = T
-0000ce20: 6573 7428 0a20 2020 2020 2020 2027 6763  est(.        'gc
-0000ce30: 702d 7374 6172 742d 7374 6f70 272c 0a20  p-start-stop',. 
-0000ce40: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-0000ce50: 2020 2020 2066 2773 6b79 206c 6175 6e63       f'sky launc
-0000ce60: 6820 2d79 202d 6320 7b6e 616d 657d 2065  h -y -c {name} e
-0000ce70: 7861 6d70 6c65 732f 6763 705f 7374 6172  xamples/gcp_star
-0000ce80: 745f 7374 6f70 2e79 616d 6c27 2c0a 2020  t_stop.yaml',.  
-0000ce90: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-0000cea0: 6c6f 6773 207b 6e61 6d65 7d20 3120 2d2d  logs {name} 1 --
-0000ceb0: 7374 6174 7573 272c 2020 2320 456e 7375  status',  # Ensu
-0000cec0: 7265 2074 6865 206a 6f62 2073 7563 6365  re the job succe
-0000ced0: 6564 6564 2e0a 2020 2020 2020 2020 2020  eded..          
-0000cee0: 2020 6627 736b 7920 6578 6563 207b 6e61    f'sky exec {na
-0000cef0: 6d65 7d20 6578 616d 706c 6573 2f67 6370  me} examples/gcp
-0000cf00: 5f73 7461 7274 5f73 746f 702e 7961 6d6c  _start_stop.yaml
-0000cf10: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-0000cf20: 2773 6b79 206c 6f67 7320 7b6e 616d 657d  'sky logs {name}
-0000cf30: 2032 202d 2d73 7461 7475 7327 2c20 2023   2 --status',  #
-0000cf40: 2045 6e73 7572 6520 7468 6520 6a6f 6220   Ensure the job 
-0000cf50: 7375 6363 6565 6465 642e 0a20 2020 2020  succeeded..     
-0000cf60: 2020 2020 2020 2066 2773 6b79 2065 7865         f'sky exe
-0000cf70: 6320 7b6e 616d 657d 2022 7072 6c69 6d69  c {name} "prlimi
-0000cf80: 7420 2d6e 202d 2d70 6964 3d5c 2428 7067  t -n --pid=\$(pg
-0000cf90: 7265 7020 2d66 205c 2772 6179 6c65 742f  rep -f \'raylet/
-0000cfa0: 7261 796c 6574 202d 2d72 6179 6c65 745f  raylet --raylet_
-0000cfb0: 736f 636b 6574 5f6e 616d 655c 2729 207c  socket_name\') |
-0000cfc0: 2067 7265 7020 5c27 225c 2731 3034 3835   grep \'"\'10485
-0000cfd0: 3736 2031 3034 3835 3736 5c27 225c 2722  76 1048576\'"\'"
-0000cfe0: 272c 2020 2320 456e 7375 7265 2074 6865  ',  # Ensure the
-0000cff0: 2072 6179 6c65 7420 7072 6f63 6573 7320   raylet process 
-0000d000: 6861 7320 7468 6520 636f 7272 6563 7420  has the correct 
-0000d010: 6669 6c65 2064 6573 6372 6970 746f 7220  file descriptor 
-0000d020: 6c69 6d69 742e 0a20 2020 2020 2020 2020  limit..         
-0000d030: 2020 2066 2773 6b79 206c 6f67 7320 7b6e     f'sky logs {n
-0000d040: 616d 657d 2033 202d 2d73 7461 7475 7327  ame} 3 --status'
-0000d050: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
-0000d060: 6a6f 6220 7375 6363 6565 6465 642e 0a20  job succeeded.. 
-0000d070: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-0000d080: 2073 746f 7020 2d79 207b 6e61 6d65 7d27   stop -y {name}'
-0000d090: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-0000d0a0: 736c 6565 7020 3230 272c 0a20 2020 2020  sleep 20',.     
-0000d0b0: 2020 2020 2020 2066 2773 6b79 2073 7461         f'sky sta
-0000d0c0: 7274 202d 7920 7b6e 616d 657d 202d 6920  rt -y {name} -i 
-0000d0d0: 3127 2c0a 2020 2020 2020 2020 2020 2020  1',.            
-0000d0e0: 6627 736b 7920 6578 6563 207b 6e61 6d65  f'sky exec {name
-0000d0f0: 7d20 6578 616d 706c 6573 2f67 6370 5f73  } examples/gcp_s
-0000d100: 7461 7274 5f73 746f 702e 7961 6d6c 272c  tart_stop.yaml',
-0000d110: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000d120: 6b79 206c 6f67 7320 7b6e 616d 657d 2034  ky logs {name} 4
-0000d130: 202d 2d73 7461 7475 7327 2c20 2023 2045   --status',  # E
-0000d140: 6e73 7572 6520 7468 6520 6a6f 6220 7375  nsure the job su
-0000d150: 6363 6565 6465 642e 0a20 2020 2020 2020  cceeded..       
-0000d160: 2020 2020 2027 736c 6565 7020 3138 3027       'sleep 180'
-0000d170: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-0000d180: 736b 7920 7374 6174 7573 202d 7220 7b6e  sky status -r {n
-0000d190: 616d 657d 207c 2067 7265 7020 2249 4e49  ame} | grep "INI
-0000d1a0: 545c 7c53 544f 5050 4544 2227 2c0a 2020  T\|STOPPED"',.  
-0000d1b0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-0000d1c0: 2066 2773 6b79 2064 6f77 6e20 2d79 207b   f'sky down -y {
-0000d1d0: 6e61 6d65 7d27 2c0a 2020 2020 290a 2020  name}',.    ).  
-0000d1e0: 2020 7275 6e5f 6f6e 655f 7465 7374 2874    run_one_test(t
-0000d1f0: 6573 7429 0a0a 0a23 202d 2d2d 2d2d 2d2d  est)...# -------
-0000d200: 2d2d 2d20 5465 7374 696e 6720 417a 7572  --- Testing Azur
-0000d210: 6520 7374 6172 7420 616e 6420 7374 6f70  e start and stop
-0000d220: 2069 6e73 7461 6e63 6573 202d 2d2d 2d2d   instances -----
-0000d230: 2d2d 2d2d 2d0a 4070 7974 6573 742e 6d61  -----.@pytest.ma
-0000d240: 726b 2e61 7a75 7265 0a64 6566 2074 6573  rk.azure.def tes
-0000d250: 745f 617a 7572 655f 7374 6172 745f 7374  t_azure_start_st
-0000d260: 6f70 2829 3a0a 2020 2020 6e61 6d65 203d  op():.    name =
-0000d270: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
-0000d280: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
-0000d290: 5465 7374 280a 2020 2020 2020 2020 2761  Test(.        'a
-0000d2a0: 7a75 7265 2d73 7461 7274 2d73 746f 7027  zure-start-stop'
-0000d2b0: 2c0a 2020 2020 2020 2020 5b0a 2020 2020  ,.        [.    
-0000d2c0: 2020 2020 2020 2020 6627 736b 7920 6c61          f'sky la
-0000d2d0: 756e 6368 202d 7920 2d63 207b 6e61 6d65  unch -y -c {name
-0000d2e0: 7d20 6578 616d 706c 6573 2f61 7a75 7265  } examples/azure
-0000d2f0: 5f73 7461 7274 5f73 746f 702e 7961 6d6c  _start_stop.yaml
-0000d300: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-0000d310: 2773 6b79 2065 7865 6320 7b6e 616d 657d  'sky exec {name}
-0000d320: 2065 7861 6d70 6c65 732f 617a 7572 655f   examples/azure_
-0000d330: 7374 6172 745f 7374 6f70 2e79 616d 6c27  start_stop.yaml'
-0000d340: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-0000d350: 736b 7920 6c6f 6773 207b 6e61 6d65 7d20  sky logs {name} 
-0000d360: 3120 2d2d 7374 6174 7573 272c 2020 2320  1 --status',  # 
-0000d370: 456e 7375 7265 2074 6865 206a 6f62 2073  Ensure the job s
-0000d380: 7563 6365 6564 6564 2e0a 2020 2020 2020  ucceeded..      
-0000d390: 2020 2020 2020 6627 736b 7920 6578 6563        f'sky exec
-0000d3a0: 207b 6e61 6d65 7d20 2270 726c 696d 6974   {name} "prlimit
-0000d3b0: 202d 6e20 2d2d 7069 643d 5c24 2870 6772   -n --pid=\$(pgr
-0000d3c0: 6570 202d 6620 5c27 7261 796c 6574 2f72  ep -f \'raylet/r
-0000d3d0: 6179 6c65 7420 2d2d 7261 796c 6574 5f73  aylet --raylet_s
-0000d3e0: 6f63 6b65 745f 6e61 6d65 5c27 2920 7c20  ocket_name\') | 
-0000d3f0: 6772 6570 205c 2722 5c27 3130 3438 3537  grep \'"\'104857
-0000d400: 3620 3130 3438 3537 365c 2722 5c27 2227  6 1048576\'"\'"'
-0000d410: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
-0000d420: 7261 796c 6574 2070 726f 6365 7373 2068  raylet process h
-0000d430: 6173 2074 6865 2063 6f72 7265 6374 2066  as the correct f
-0000d440: 696c 6520 6465 7363 7269 7074 6f72 206c  ile descriptor l
-0000d450: 696d 6974 2e0a 2020 2020 2020 2020 2020  imit..          
-0000d460: 2020 6627 736b 7920 6c6f 6773 207b 6e61    f'sky logs {na
-0000d470: 6d65 7d20 3220 2d2d 7374 6174 7573 272c  me} 2 --status',
-0000d480: 2020 2320 456e 7375 7265 2074 6865 206a    # Ensure the j
-0000d490: 6f62 2073 7563 6365 6564 6564 2e0a 2020  ob succeeded..  
-0000d4a0: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-0000d4b0: 7374 6f70 202d 7920 7b6e 616d 657d 272c  stop -y {name}',
-0000d4c0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000d4d0: 6b79 2073 7461 7274 202d 7920 7b6e 616d  ky start -y {nam
-0000d4e0: 657d 202d 6920 3127 2c0a 2020 2020 2020  e} -i 1',.      
-0000d4f0: 2020 2020 2020 6627 736b 7920 6578 6563        f'sky exec
-0000d500: 207b 6e61 6d65 7d20 6578 616d 706c 6573   {name} examples
-0000d510: 2f61 7a75 7265 5f73 7461 7274 5f73 746f  /azure_start_sto
-0000d520: 702e 7961 6d6c 272c 0a20 2020 2020 2020  p.yaml',.       
-0000d530: 2020 2020 2066 2773 6b79 206c 6f67 7320       f'sky logs 
-0000d540: 7b6e 616d 657d 2033 202d 2d73 7461 7475  {name} 3 --statu
-0000d550: 7327 2c20 2023 2045 6e73 7572 6520 7468  s',  # Ensure th
-0000d560: 6520 6a6f 6220 7375 6363 6565 6465 642e  e job succeeded.
-0000d570: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
-0000d580: 6565 7020 3230 3027 2c0a 2020 2020 2020  eep 200',.      
-0000d590: 2020 2020 2020 6627 733d 2428 736b 7920        f's=$(sky 
-0000d5a0: 7374 6174 7573 202d 7220 7b6e 616d 657d  status -r {name}
-0000d5b0: 2920 2626 2065 6368 6f20 2473 2026 2620  ) && echo $s && 
-0000d5c0: 6563 686f 2024 7320 7c20 6772 6570 2022  echo $s | grep "
-0000d5d0: 494e 4954 5c7c 5354 4f50 5045 4422 270a  INIT\|STOPPED"'.
-0000d5e0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-0000d5f0: 2020 2066 2773 6b79 2064 6f77 6e20 2d79     f'sky down -y
-0000d600: 207b 6e61 6d65 7d27 2c0a 2020 2020 2020   {name}',.      
-0000d610: 2020 7469 6d65 6f75 743d 3330 202a 2036    timeout=30 * 6
-0000d620: 302c 2020 2320 3330 206d 696e 730a 2020  0,  # 30 mins.  
-0000d630: 2020 290a 2020 2020 7275 6e5f 6f6e 655f    ).    run_one_
-0000d640: 7465 7374 2874 6573 7429 0a0a 0a23 202d  test(test)...# -
-0000d650: 2d2d 2d2d 2d2d 2d2d 2d20 5465 7374 696e  --------- Testin
-0000d660: 6720 4175 746f 7374 6f70 7069 6e67 202d  g Autostopping -
-0000d670: 2d2d 2d2d 2d2d 2d2d 2d0a 4070 7974 6573  ---------.@pytes
-0000d680: 742e 6d61 726b 2e6e 6f5f 6c61 6d62 6461  t.mark.no_lambda
-0000d690: 5f63 6c6f 7564 2020 2320 4c61 6d62 6461  _cloud  # Lambda
-0000d6a0: 2043 6c6f 7564 2064 6f65 7320 6e6f 7420   Cloud does not 
-0000d6b0: 7375 7070 6f72 7420 7374 6f70 7069 6e67  support stopping
-0000d6c0: 2069 6e73 7461 6e63 6573 0a40 7079 7465   instances.@pyte
-0000d6d0: 7374 2e6d 6172 6b2e 6e6f 5f69 626d 2020  st.mark.no_ibm  
-0000d6e0: 2320 4649 5828 4942 4d29 2073 706f 7261  # FIX(IBM) spora
-0000d6f0: 6469 6361 6c6c 7920 6661 696c 732c 2061  dically fails, a
-0000d700: 7320 7265 7374 6172 7465 6420 776f 726b  s restarted work
-0000d710: 6572 7320 7374 6179 2075 6e69 6e69 7469  ers stay uniniti
-0000d720: 616c 697a 6564 2069 6e64 6566 696e 6974  alized indefinit
-0000d730: 656c 790a 4070 7974 6573 742e 6d61 726b  ely.@pytest.mark
-0000d740: 2e6e 6f5f 7363 7020 2023 2053 4350 2064  .no_scp  # SCP d
-0000d750: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
-0000d760: 6e75 6d5f 6e6f 6465 7320 3e20 3120 7965  num_nodes > 1 ye
-0000d770: 740a 6465 6620 7465 7374 5f61 7574 6f73  t.def test_autos
-0000d780: 746f 7028 6765 6e65 7269 635f 636c 6f75  top(generic_clou
-0000d790: 643a 2073 7472 293a 0a20 2020 206e 616d  d: str):.    nam
-0000d7a0: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
-0000d7b0: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
-0000d7c0: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
-0000d7d0: 2027 6175 746f 7374 6f70 272c 0a20 2020   'autostop',.   
-0000d7e0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-0000d7f0: 2020 2066 2773 6b79 206c 6175 6e63 6820     f'sky launch 
-0000d800: 2d79 202d 6420 2d63 207b 6e61 6d65 7d20  -y -d -c {name} 
-0000d810: 2d2d 6e75 6d2d 6e6f 6465 7320 3220 2d2d  --num-nodes 2 --
-0000d820: 636c 6f75 6420 7b67 656e 6572 6963 5f63  cloud {generic_c
-0000d830: 6c6f 7564 7d20 7465 7374 732f 7465 7374  loud} tests/test
-0000d840: 5f79 616d 6c73 2f6d 696e 696d 616c 2e79  _yamls/minimal.y
-0000d850: 616d 6c27 2c0a 2020 2020 2020 2020 2020  aml',.          
-0000d860: 2020 6627 736b 7920 6175 746f 7374 6f70    f'sky autostop
-0000d870: 202d 7920 7b6e 616d 657d 202d 6920 3127   -y {name} -i 1'
-0000d880: 2c0a 0a20 2020 2020 2020 2020 2020 2023  ,..            #
-0000d890: 2045 6e73 7572 6520 6175 746f 7374 6f70   Ensure autostop
-0000d8a0: 2069 7320 7365 742e 0a20 2020 2020 2020   is set..       
-0000d8b0: 2020 2020 2066 2773 6b79 2073 7461 7475       f'sky statu
-0000d8c0: 7320 7c20 6772 6570 207b 6e61 6d65 7d20  s | grep {name} 
-0000d8d0: 7c20 6772 6570 2022 316d 2227 2c0a 0a20  | grep "1m"',.. 
-0000d8e0: 2020 2020 2020 2020 2020 2023 2045 6e73             # Ens
-0000d8f0: 7572 6520 7468 6520 636c 7573 7465 7220  ure the cluster 
-0000d900: 6973 206e 6f74 2073 746f 7070 6564 2065  is not stopped e
-0000d910: 6172 6c79 2e0a 2020 2020 2020 2020 2020  arly..          
-0000d920: 2020 2773 6c65 6570 2034 3527 2c0a 2020    'sleep 45',.  
-0000d930: 2020 2020 2020 2020 2020 6627 733d 2428            f's=$(
-0000d940: 736b 7920 7374 6174 7573 207b 6e61 6d65  sky status {name
-0000d950: 7d20 2d2d 7265 6672 6573 6829 3b20 6563  } --refresh); ec
-0000d960: 686f 2022 2473 223b 2065 6368 6f3b 2065  ho "$s"; echo; e
-0000d970: 6368 6f3b 2065 6368 6f20 2224 7322 2020  cho; echo "$s"  
-0000d980: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
-0000d990: 6772 6570 2055 5027 2c0a 0a20 2020 2020  grep UP',..     
-0000d9a0: 2020 2020 2020 2023 2045 6e73 7572 6520         # Ensure 
-0000d9b0: 7468 6520 636c 7573 7465 7220 6973 2053  the cluster is S
-0000d9c0: 544f 5050 4544 2e0a 2020 2020 2020 2020  TOPPED..        
-0000d9d0: 2020 2020 2773 6c65 6570 2032 3530 272c      'sleep 250',
-0000d9e0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000d9f0: 3d24 2873 6b79 2073 7461 7475 7320 7b6e  =$(sky status {n
-0000da00: 616d 657d 202d 2d72 6566 7265 7368 293b  ame} --refresh);
-0000da10: 2065 6368 6f20 2224 7322 3b20 6563 686f   echo "$s"; echo
-0000da20: 3b20 6563 686f 3b20 6563 686f 2022 2473  ; echo; echo "$s
-0000da30: 2220 207c 2067 7265 7020 7b6e 616d 657d  "  | grep {name}
-0000da40: 207c 2067 7265 7020 5354 4f50 5045 4427   | grep STOPPED'
-0000da50: 2c0a 0a20 2020 2020 2020 2020 2020 2023  ,..            #
-0000da60: 2045 6e73 7572 6520 7468 6520 636c 7573   Ensure the clus
-0000da70: 7465 7220 6973 2055 5020 616e 6420 7468  ter is UP and th
-0000da80: 6520 6175 746f 7374 6f70 2073 6574 7469  e autostop setti
-0000da90: 6e67 2069 7320 7265 7365 7420 2827 2d27  ng is reset ('-'
-0000daa0: 292e 0a20 2020 2020 2020 2020 2020 2066  )..            f
-0000dab0: 2773 6b79 2073 7461 7274 202d 7920 7b6e  'sky start -y {n
-0000dac0: 616d 657d 272c 0a20 2020 2020 2020 2020  ame}',.         
-0000dad0: 2020 2066 2773 6b79 2073 7461 7475 7320     f'sky status 
-0000dae0: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
-0000daf0: 6772 6570 202d 4520 2255 505c 732b 2d22  grep -E "UP\s+-"
-0000db00: 272c 0a0a 2020 2020 2020 2020 2020 2020  ',..            
-0000db10: 2320 456e 7375 7265 2074 6865 206a 6f62  # Ensure the job
-0000db20: 2073 7563 6365 6564 6564 2e0a 2020 2020   succeeded..    
-0000db30: 2020 2020 2020 2020 6627 736b 7920 6578          f'sky ex
-0000db40: 6563 207b 6e61 6d65 7d20 7465 7374 732f  ec {name} tests/
-0000db50: 7465 7374 5f79 616d 6c73 2f6d 696e 696d  test_yamls/minim
-0000db60: 616c 2e79 616d 6c27 2c0a 2020 2020 2020  al.yaml',.      
-0000db70: 2020 2020 2020 6627 736b 7920 6c6f 6773        f'sky logs
-0000db80: 207b 6e61 6d65 7d20 3220 2d2d 7374 6174   {name} 2 --stat
-0000db90: 7573 272c 0a0a 2020 2020 2020 2020 2020  us',..          
-0000dba0: 2020 2320 5465 7374 2072 6573 7461 7274    # Test restart
-0000dbb0: 696e 6720 7468 6520 6964 6c65 6e65 7373  ing the idleness
-0000dbc0: 2074 696d 6572 2076 6961 2063 616e 6365   timer via cance
-0000dbd0: 6c20 2b20 7265 7365 743a 0a20 2020 2020  l + reset:.     
-0000dbe0: 2020 2020 2020 2066 2773 6b79 2061 7574         f'sky aut
-0000dbf0: 6f73 746f 7020 2d79 207b 6e61 6d65 7d20  ostop -y {name} 
-0000dc00: 2d69 2031 272c 2020 2320 4964 6c65 6e65  -i 1',  # Idlene
-0000dc10: 7373 2073 7461 7274 7320 636f 756e 7469  ss starts counti
-0000dc20: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
-0000dc30: 2773 6c65 6570 2034 3527 2c20 2023 2041  'sleep 45',  # A
-0000dc40: 6c6d 6f73 7420 7265 6163 6865 6420 7468  lmost reached th
-0000dc50: 6520 7468 7265 7368 6f6c 642e 0a20 2020  e threshold..   
-0000dc60: 2020 2020 2020 2020 2066 2773 6b79 2061           f'sky a
-0000dc70: 7574 6f73 746f 7020 2d79 207b 6e61 6d65  utostop -y {name
-0000dc80: 7d20 2d2d 6361 6e63 656c 272c 0a20 2020  } --cancel',.   
-0000dc90: 2020 2020 2020 2020 2066 2773 6b79 2061           f'sky a
-0000dca0: 7574 6f73 746f 7020 2d79 207b 6e61 6d65  utostop -y {name
-0000dcb0: 7d20 2d69 2031 272c 2020 2320 5368 6f75  } -i 1',  # Shou
-0000dcc0: 6c64 2072 6573 7461 7274 2074 6865 2074  ld restart the t
-0000dcd0: 696d 6572 2e0a 2020 2020 2020 2020 2020  imer..          
-0000dce0: 2020 2773 6c65 6570 2034 3527 2c0a 2020    'sleep 45',.  
-0000dcf0: 2020 2020 2020 2020 2020 6627 733d 2428            f's=$(
-0000dd00: 736b 7920 7374 6174 7573 207b 6e61 6d65  sky status {name
-0000dd10: 7d20 2d2d 7265 6672 6573 6829 3b20 6563  } --refresh); ec
-0000dd20: 686f 2022 2473 223b 2065 6368 6f3b 2065  ho "$s"; echo; e
-0000dd30: 6368 6f3b 2065 6368 6f20 2224 7322 207c  cho; echo "$s" |
-0000dd40: 2067 7265 7020 7b6e 616d 657d 207c 2067   grep {name} | g
-0000dd50: 7265 7020 5550 272c 0a20 2020 2020 2020  rep UP',.       
-0000dd60: 2020 2020 2027 736c 6565 7020 3235 3027       'sleep 250'
-0000dd70: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-0000dd80: 733d 2428 736b 7920 7374 6174 7573 207b  s=$(sky status {
-0000dd90: 6e61 6d65 7d20 2d2d 7265 6672 6573 6829  name} --refresh)
-0000dda0: 3b20 6563 686f 2022 2473 223b 2065 6368  ; echo "$s"; ech
-0000ddb0: 6f3b 2065 6368 6f3b 2065 6368 6f20 2224  o; echo; echo "$
-0000ddc0: 7322 2020 7c20 6772 6570 207b 6e61 6d65  s"  | grep {name
-0000ddd0: 7d20 7c20 6772 6570 2053 544f 5050 4544  } | grep STOPPED
-0000dde0: 272c 0a0a 2020 2020 2020 2020 2020 2020  ',..            
-0000ddf0: 2320 5465 7374 2072 6573 7461 7274 696e  # Test restartin
-0000de00: 6720 7468 6520 6964 6c65 6e65 7373 2074  g the idleness t
-0000de10: 696d 6572 2076 6961 2065 7865 633a 0a20  imer via exec:. 
-0000de20: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-0000de30: 2073 7461 7274 202d 7920 7b6e 616d 657d   start -y {name}
-0000de40: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-0000de50: 2773 6b79 2073 7461 7475 7320 7c20 6772  'sky status | gr
-0000de60: 6570 207b 6e61 6d65 7d20 7c20 6772 6570  ep {name} | grep
-0000de70: 202d 4520 2255 505c 732b 2d22 272c 0a20   -E "UP\s+-"',. 
-0000de80: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-0000de90: 2061 7574 6f73 746f 7020 2d79 207b 6e61   autostop -y {na
-0000dea0: 6d65 7d20 2d69 2031 272c 2020 2320 4964  me} -i 1',  # Id
-0000deb0: 6c65 6e65 7373 2073 7461 7274 7320 636f  leness starts co
-0000dec0: 756e 7469 6e67 2e0a 2020 2020 2020 2020  unting..        
-0000ded0: 2020 2020 2773 6c65 6570 2034 3527 2c20      'sleep 45', 
-0000dee0: 2023 2041 6c6d 6f73 7420 7265 6163 6865   # Almost reache
-0000def0: 6420 7468 6520 7468 7265 7368 6f6c 642e  d the threshold.
-0000df00: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000df10: 6b79 2065 7865 6320 7b6e 616d 657d 2065  ky exec {name} e
-0000df20: 6368 6f20 6869 272c 2020 2320 5368 6f75  cho hi',  # Shou
-0000df30: 6c64 2072 6573 7461 7274 2074 6865 2074  ld restart the t
-0000df40: 696d 6572 2e0a 2020 2020 2020 2020 2020  imer..          
-0000df50: 2020 2773 6c65 6570 2034 3527 2c0a 2020    'sleep 45',.  
-0000df60: 2020 2020 2020 2020 2020 6627 733d 2428            f's=$(
-0000df70: 736b 7920 7374 6174 7573 207b 6e61 6d65  sky status {name
-0000df80: 7d20 2d2d 7265 6672 6573 6829 3b20 6563  } --refresh); ec
-0000df90: 686f 2022 2473 223b 2065 6368 6f3b 2065  ho "$s"; echo; e
-0000dfa0: 6368 6f3b 2065 6368 6f20 2224 7322 2020  cho; echo "$s"  
-0000dfb0: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
-0000dfc0: 6772 6570 2055 5027 2c0a 2020 2020 2020  grep UP',.      
-0000dfd0: 2020 2020 2020 2773 6c65 6570 2032 3530        'sleep 250
-0000dfe0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-0000dff0: 2773 3d24 2873 6b79 2073 7461 7475 7320  's=$(sky status 
-0000e000: 7b6e 616d 657d 202d 2d72 6566 7265 7368  {name} --refresh
-0000e010: 293b 2065 6368 6f20 2224 7322 3b20 6563  ); echo "$s"; ec
-0000e020: 686f 3b20 6563 686f 3b20 6563 686f 2022  ho; echo; echo "
-0000e030: 2473 2220 207c 2067 7265 7020 7b6e 616d  $s"  | grep {nam
-0000e040: 657d 207c 2067 7265 7020 5354 4f50 5045  e} | grep STOPPE
-0000e050: 4427 2c0a 2020 2020 2020 2020 5d2c 0a20  D',.        ],. 
-0000e060: 2020 2020 2020 2066 2773 6b79 2064 6f77         f'sky dow
-0000e070: 6e20 2d79 207b 6e61 6d65 7d27 2c0a 2020  n -y {name}',.  
-0000e080: 2020 2020 2020 7469 6d65 6f75 743d 3230        timeout=20
-0000e090: 202a 2036 302c 0a20 2020 2029 0a20 2020   * 60,.    ).   
-0000e0a0: 2072 756e 5f6f 6e65 5f74 6573 7428 7465   run_one_test(te
-0000e0b0: 7374 290a 0a0a 2320 2d2d 2d2d 2d2d 2d2d  st)...# --------
-0000e0c0: 2d2d 2054 6573 7469 6e67 2041 7574 6f64  -- Testing Autod
-0000e0d0: 6f77 6e69 6e67 202d 2d2d 2d2d 2d2d 2d2d  owning ---------
-0000e0e0: 2d0a 4070 7974 6573 742e 6d61 726b 2e6e  -.@pytest.mark.n
-0000e0f0: 6f5f 7363 7020 2023 2053 4350 2064 6f65  o_scp  # SCP doe
-0000e100: 7320 6e6f 7420 7375 7070 6f72 7420 6e75  s not support nu
-0000e110: 6d5f 6e6f 6465 7320 3e20 3120 7965 742e  m_nodes > 1 yet.
-0000e120: 2052 756e 2074 6573 745f 7363 705f 6175   Run test_scp_au
-0000e130: 746f 646f 776e 2069 6e73 7465 6164 2e0a  todown instead..
-0000e140: 6465 6620 7465 7374 5f61 7574 6f64 6f77  def test_autodow
-0000e150: 6e28 6765 6e65 7269 635f 636c 6f75 643a  n(generic_cloud:
-0000e160: 2073 7472 293a 0a20 2020 206e 616d 6520   str):.    name 
-0000e170: 3d20 5f67 6574 5f63 6c75 7374 6572 5f6e  = _get_cluster_n
-0000e180: 616d 6528 290a 2020 2020 7465 7374 203d  ame().    test =
-0000e190: 2054 6573 7428 0a20 2020 2020 2020 2027   Test(.        '
-0000e1a0: 6175 746f 646f 776e 272c 0a20 2020 2020  autodown',.     
-0000e1b0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-0000e1c0: 2066 2773 6b79 206c 6175 6e63 6820 2d79   f'sky launch -y
-0000e1d0: 202d 6420 2d63 207b 6e61 6d65 7d20 2d2d   -d -c {name} --
-0000e1e0: 6e75 6d2d 6e6f 6465 7320 3220 2d2d 636c  num-nodes 2 --cl
-0000e1f0: 6f75 6420 7b67 656e 6572 6963 5f63 6c6f  oud {generic_clo
-0000e200: 7564 7d20 7465 7374 732f 7465 7374 5f79  ud} tests/test_y
-0000e210: 616d 6c73 2f6d 696e 696d 616c 2e79 616d  amls/minimal.yam
-0000e220: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
-0000e230: 6627 736b 7920 6175 746f 7374 6f70 202d  f'sky autostop -
-0000e240: 7920 7b6e 616d 657d 202d 2d64 6f77 6e20  y {name} --down 
-0000e250: 2d69 2031 272c 0a20 2020 2020 2020 2020  -i 1',.         
-0000e260: 2020 2023 2045 6e73 7572 6520 6175 746f     # Ensure auto
-0000e270: 7374 6f70 2069 7320 7365 742e 0a20 2020  stop is set..   
-0000e280: 2020 2020 2020 2020 2066 2773 6b79 2073           f'sky s
-0000e290: 7461 7475 7320 7c20 6772 6570 207b 6e61  tatus | grep {na
-0000e2a0: 6d65 7d20 7c20 6772 6570 2022 316d 2028  me} | grep "1m (
-0000e2b0: 646f 776e 2922 272c 0a20 2020 2020 2020  down)"',.       
-0000e2c0: 2020 2020 2023 2045 6e73 7572 6520 7468       # Ensure th
-0000e2d0: 6520 636c 7573 7465 7220 6973 206e 6f74  e cluster is not
-0000e2e0: 2074 6572 6d69 6e61 7465 6420 6561 726c   terminated earl
-0000e2f0: 792e 0a20 2020 2020 2020 2020 2020 2027  y..            '
-0000e300: 736c 6565 7020 3435 272c 0a20 2020 2020  sleep 45',.     
-0000e310: 2020 2020 2020 2066 2773 3d24 2873 6b79         f's=$(sky
-0000e320: 2073 7461 7475 7320 7b6e 616d 657d 202d   status {name} -
-0000e330: 2d72 6566 7265 7368 293b 2065 6368 6f20  -refresh); echo 
-0000e340: 2224 7322 3b20 6563 686f 3b20 6563 686f  "$s"; echo; echo
-0000e350: 3b20 6563 686f 2022 2473 2220 207c 2067  ; echo "$s"  | g
-0000e360: 7265 7020 7b6e 616d 657d 207c 2067 7265  rep {name} | gre
-0000e370: 7020 5550 272c 0a20 2020 2020 2020 2020  p UP',.         
-0000e380: 2020 2023 2045 6e73 7572 6520 7468 6520     # Ensure the 
-0000e390: 636c 7573 7465 7220 6973 2074 6572 6d69  cluster is termi
-0000e3a0: 6e61 7465 642e 0a20 2020 2020 2020 2020  nated..         
-0000e3b0: 2020 2027 736c 6565 7020 3230 3027 2c0a     'sleep 200',.
-0000e3c0: 2020 2020 2020 2020 2020 2020 6627 733d              f's=
-0000e3d0: 2428 534b 5950 494c 4f54 5f44 4542 5547  $(SKYPILOT_DEBUG
-0000e3e0: 3d30 2073 6b79 2073 7461 7475 7320 7b6e  =0 sky status {n
-0000e3f0: 616d 657d 202d 2d72 6566 7265 7368 2920  ame} --refresh) 
-0000e400: 2626 2065 6368 6f20 2224 7322 2026 2620  && echo "$s" && 
-0000e410: 7b7b 2065 6368 6f20 2224 7322 207c 2067  {{ echo "$s" | g
-0000e420: 7265 7020 7b6e 616d 657d 207c 2067 7265  rep {name} | gre
-0000e430: 7020 2241 7574 6f64 6f77 6e65 6420 636c  p "Autodowned cl
-0000e440: 7573 7465 725c 7c74 6572 6d69 6e61 7465  uster\|terminate
-0000e450: 6420 6f6e 2074 6865 2063 6c6f 7564 223b  d on the cloud";
-0000e460: 207d 7d20 7c7c 207b 7b20 6563 686f 2022   }} || {{ echo "
-0000e470: 2473 2220 7c20 6772 6570 207b 6e61 6d65  $s" | grep {name
-0000e480: 7d20 2626 2065 7869 7420 3120 7c7c 2065  } && exit 1 || e
-0000e490: 7869 7420 303b 207d 7d27 2c0a 2020 2020  xit 0; }}',.    
-0000e4a0: 2020 2020 2020 2020 6627 736b 7920 6c61          f'sky la
-0000e4b0: 756e 6368 202d 7920 2d64 202d 6320 7b6e  unch -y -d -c {n
-0000e4c0: 616d 657d 202d 2d63 6c6f 7564 207b 6765  ame} --cloud {ge
-0000e4d0: 6e65 7269 635f 636c 6f75 647d 202d 2d6e  neric_cloud} --n
-0000e4e0: 756d 2d6e 6f64 6573 2032 202d 2d64 6f77  um-nodes 2 --dow
-0000e4f0: 6e20 7465 7374 732f 7465 7374 5f79 616d  n tests/test_yam
-0000e500: 6c73 2f6d 696e 696d 616c 2e79 616d 6c27  ls/minimal.yaml'
-0000e510: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-0000e520: 736b 7920 7374 6174 7573 207c 2067 7265  sky status | gre
-0000e530: 7020 7b6e 616d 657d 207c 2067 7265 7020  p {name} | grep 
-0000e540: 5550 272c 2020 2320 456e 7375 7265 2074  UP',  # Ensure t
-0000e550: 6865 2063 6c75 7374 6572 2069 7320 5550  he cluster is UP
-0000e560: 2e0a 2020 2020 2020 2020 2020 2020 6627  ..            f'
-0000e570: 736b 7920 6578 6563 207b 6e61 6d65 7d20  sky exec {name} 
-0000e580: 2d2d 636c 6f75 6420 7b67 656e 6572 6963  --cloud {generic
-0000e590: 5f63 6c6f 7564 7d20 7465 7374 732f 7465  _cloud} tests/te
-0000e5a0: 7374 5f79 616d 6c73 2f6d 696e 696d 616c  st_yamls/minimal
-0000e5b0: 2e79 616d 6c27 2c0a 2020 2020 2020 2020  .yaml',.        
-0000e5c0: 2020 2020 6627 736b 7920 7374 6174 7573      f'sky status
-0000e5d0: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
-0000e5e0: 2067 7265 7020 2231 6d20 2864 6f77 6e29   grep "1m (down)
-0000e5f0: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-0000e600: 2773 6c65 6570 2032 3430 272c 0a20 2020  'sleep 240',.   
-0000e610: 2020 2020 2020 2020 2023 2045 6e73 7572           # Ensur
-0000e620: 6520 7468 6520 636c 7573 7465 7220 6973  e the cluster is
-0000e630: 2074 6572 6d69 6e61 7465 642e 0a20 2020   terminated..   
-0000e640: 2020 2020 2020 2020 2066 2773 3d24 2853           f's=$(S
-0000e650: 4b59 5049 4c4f 545f 4445 4255 473d 3020  KYPILOT_DEBUG=0 
-0000e660: 736b 7920 7374 6174 7573 207b 6e61 6d65  sky status {name
-0000e670: 7d20 2d2d 7265 6672 6573 6829 2026 2620  } --refresh) && 
-0000e680: 6563 686f 2022 2473 2220 2626 207b 7b20  echo "$s" && {{ 
-0000e690: 6563 686f 2022 2473 2220 7c20 6772 6570  echo "$s" | grep
-0000e6a0: 207b 6e61 6d65 7d20 7c20 6772 6570 2022   {name} | grep "
-0000e6b0: 4175 746f 646f 776e 6564 2063 6c75 7374  Autodowned clust
-0000e6c0: 6572 5c7c 7465 726d 696e 6174 6564 206f  er\|terminated o
-0000e6d0: 6e20 7468 6520 636c 6f75 6422 3b20 7d7d  n the cloud"; }}
-0000e6e0: 207c 7c20 7b7b 2065 6368 6f20 2224 7322   || {{ echo "$s"
-0000e6f0: 207c 2067 7265 7020 7b6e 616d 657d 2026   | grep {name} &
-0000e700: 2620 6578 6974 2031 207c 7c20 6578 6974  & exit 1 || exit
-0000e710: 2030 3b20 7d7d 272c 0a20 2020 2020 2020   0; }}',.       
-0000e720: 2020 2020 2066 2773 6b79 206c 6175 6e63       f'sky launc
-0000e730: 6820 2d79 202d 6420 2d63 207b 6e61 6d65  h -y -d -c {name
-0000e740: 7d20 2d2d 636c 6f75 6420 7b67 656e 6572  } --cloud {gener
-0000e750: 6963 5f63 6c6f 7564 7d20 2d2d 6e75 6d2d  ic_cloud} --num-
-0000e760: 6e6f 6465 7320 3220 2d2d 646f 776e 2074  nodes 2 --down t
-0000e770: 6573 7473 2f74 6573 745f 7961 6d6c 732f  ests/test_yamls/
-0000e780: 6d69 6e69 6d61 6c2e 7961 6d6c 272c 0a20  minimal.yaml',. 
-0000e790: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-0000e7a0: 2061 7574 6f73 746f 7020 2d79 207b 6e61   autostop -y {na
-0000e7b0: 6d65 7d20 2d2d 6361 6e63 656c 272c 0a20  me} --cancel',. 
-0000e7c0: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
-0000e7d0: 7020 3234 3027 2c0a 2020 2020 2020 2020  p 240',.        
-0000e7e0: 2020 2020 2320 456e 7375 7265 2074 6865      # Ensure the
-0000e7f0: 2063 6c75 7374 6572 2069 7320 7374 696c   cluster is stil
-0000e800: 6c20 5550 2e0a 2020 2020 2020 2020 2020  l UP..          
-0000e810: 2020 6627 733d 2428 534b 5950 494c 4f54    f's=$(SKYPILOT
-0000e820: 5f44 4542 5547 3d30 2073 6b79 2073 7461  _DEBUG=0 sky sta
-0000e830: 7475 7320 7b6e 616d 657d 202d 2d72 6566  tus {name} --ref
-0000e840: 7265 7368 2920 2626 2065 6368 6f20 2224  resh) && echo "$
-0000e850: 7322 2026 2620 6563 686f 2022 2473 2220  s" && echo "$s" 
-0000e860: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
-0000e870: 6772 6570 2055 5027 2c0a 2020 2020 2020  grep UP',.      
-0000e880: 2020 5d2c 0a20 2020 2020 2020 2066 2773    ],.        f's
-0000e890: 6b79 2064 6f77 6e20 2d79 207b 6e61 6d65  ky down -y {name
-0000e8a0: 7d27 2c0a 2020 2020 2020 2020 7469 6d65  }',.        time
-0000e8b0: 6f75 743d 3230 202a 2036 302c 0a20 2020  out=20 * 60,.   
-0000e8c0: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
-0000e8d0: 6573 7428 7465 7374 290a 0a0a 4070 7974  est(test)...@pyt
-0000e8e0: 6573 742e 6d61 726b 2e73 6370 0a64 6566  est.mark.scp.def
-0000e8f0: 2074 6573 745f 7363 705f 6175 746f 646f   test_scp_autodo
-0000e900: 776e 2829 3a0a 2020 2020 6e61 6d65 203d  wn():.    name =
-0000e910: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
-0000e920: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
-0000e930: 5465 7374 280a 2020 2020 2020 2020 2753  Test(.        'S
-0000e940: 4350 5f61 7574 6f64 6f77 6e27 2c0a 2020  CP_autodown',.  
-0000e950: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-0000e960: 2020 2020 6627 736b 7920 6c61 756e 6368      f'sky launch
-0000e970: 202d 7920 2d64 202d 6320 7b6e 616d 657d   -y -d -c {name}
-0000e980: 207b 5343 505f 5459 5045 7d20 7465 7374   {SCP_TYPE} test
-0000e990: 732f 7465 7374 5f79 616d 6c73 2f6d 696e  s/test_yamls/min
-0000e9a0: 696d 616c 2e79 616d 6c27 2c0a 2020 2020  imal.yaml',.    
-0000e9b0: 2020 2020 2020 2020 6627 736b 7920 6175          f'sky au
-0000e9c0: 746f 7374 6f70 202d 7920 7b6e 616d 657d  tostop -y {name}
-0000e9d0: 202d 2d64 6f77 6e20 2d69 2031 272c 0a20   --down -i 1',. 
-0000e9e0: 2020 2020 2020 2020 2020 2023 2045 6e73             # Ens
-0000e9f0: 7572 6520 6175 746f 7374 6f70 2069 7320  ure autostop is 
-0000ea00: 7365 742e 0a20 2020 2020 2020 2020 2020  set..           
-0000ea10: 2066 2773 6b79 2073 7461 7475 7320 7c20   f'sky status | 
-0000ea20: 6772 6570 207b 6e61 6d65 7d20 7c20 6772  grep {name} | gr
-0000ea30: 6570 2022 316d 2028 646f 776e 2922 272c  ep "1m (down)"',
-0000ea40: 0a20 2020 2020 2020 2020 2020 2023 2045  .            # E
-0000ea50: 6e73 7572 6520 7468 6520 636c 7573 7465  nsure the cluste
-0000ea60: 7220 6973 206e 6f74 2074 6572 6d69 6e61  r is not termina
-0000ea70: 7465 6420 6561 726c 792e 0a20 2020 2020  ted early..     
-0000ea80: 2020 2020 2020 2027 736c 6565 7020 3435         'sleep 45
-0000ea90: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-0000eaa0: 2773 6b79 2073 7461 7475 7320 2d2d 7265  'sky status --re
-0000eab0: 6672 6573 6820 7c20 6772 6570 207b 6e61  fresh | grep {na
-0000eac0: 6d65 7d20 7c20 6772 6570 2055 5027 2c0a  me} | grep UP',.
-0000ead0: 2020 2020 2020 2020 2020 2020 2320 456e              # En
-0000eae0: 7375 7265 2074 6865 2063 6c75 7374 6572  sure the cluster
-0000eaf0: 2069 7320 7465 726d 696e 6174 6564 2e0a   is terminated..
-0000eb00: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
-0000eb10: 6570 2032 3030 272c 0a20 2020 2020 2020  ep 200',.       
-0000eb20: 2020 2020 2066 2773 3d24 2853 4b59 5049       f's=$(SKYPI
-0000eb30: 4c4f 545f 4445 4255 473d 3020 736b 7920  LOT_DEBUG=0 sky 
-0000eb40: 7374 6174 7573 202d 2d72 6566 7265 7368  status --refresh
-0000eb50: 2920 2626 2070 7269 6e74 6620 2224 7322  ) && printf "$s"
-0000eb60: 2026 2620 7b7b 2065 6368 6f20 2224 7322   && {{ echo "$s"
-0000eb70: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
-0000eb80: 2067 7265 7020 2241 7574 6f64 6f77 6e65   grep "Autodowne
-0000eb90: 6420 636c 7573 7465 725c 7c74 6572 6d69  d cluster\|termi
-0000eba0: 6e61 7465 6420 6f6e 2074 6865 2063 6c6f  nated on the clo
-0000ebb0: 7564 223b 207d 7d20 7c7c 207b 7b20 6563  ud"; }} || {{ ec
-0000ebc0: 686f 2022 2473 2220 7c20 6772 6570 207b  ho "$s" | grep {
-0000ebd0: 6e61 6d65 7d20 2626 2065 7869 7420 3120  name} && exit 1 
-0000ebe0: 7c7c 2065 7869 7420 303b 207d 7d27 2c0a  || exit 0; }}',.
-0000ebf0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-0000ec00: 7920 6c61 756e 6368 202d 7920 2d64 202d  y launch -y -d -
-0000ec10: 6320 7b6e 616d 657d 207b 5343 505f 5459  c {name} {SCP_TY
-0000ec20: 5045 7d20 2d2d 646f 776e 2074 6573 7473  PE} --down tests
-0000ec30: 2f74 6573 745f 7961 6d6c 732f 6d69 6e69  /test_yamls/mini
-0000ec40: 6d61 6c2e 7961 6d6c 272c 0a20 2020 2020  mal.yaml',.     
-0000ec50: 2020 2020 2020 2066 2773 6b79 2073 7461         f'sky sta
-0000ec60: 7475 7320 7c20 6772 6570 207b 6e61 6d65  tus | grep {name
-0000ec70: 7d20 7c20 6772 6570 2055 5027 2c20 2023  } | grep UP',  #
-0000ec80: 2045 6e73 7572 6520 7468 6520 636c 7573   Ensure the clus
-0000ec90: 7465 7220 6973 2055 502e 0a20 2020 2020  ter is UP..     
-0000eca0: 2020 2020 2020 2066 2773 6b79 2065 7865         f'sky exe
-0000ecb0: 6320 7b6e 616d 657d 207b 5343 505f 5459  c {name} {SCP_TY
-0000ecc0: 5045 7d20 7465 7374 732f 7465 7374 5f79  PE} tests/test_y
-0000ecd0: 616d 6c73 2f6d 696e 696d 616c 2e79 616d  amls/minimal.yam
-0000ece0: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
-0000ecf0: 6627 736b 7920 7374 6174 7573 207c 2067  f'sky status | g
-0000ed00: 7265 7020 7b6e 616d 657d 207c 2067 7265  rep {name} | gre
-0000ed10: 7020 2231 6d20 2864 6f77 6e29 2227 2c0a  p "1m (down)"',.
-0000ed20: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
-0000ed30: 6570 2032 3030 272c 0a20 2020 2020 2020  ep 200',.       
-0000ed40: 2020 2020 2023 2045 6e73 7572 6520 7468       # Ensure th
-0000ed50: 6520 636c 7573 7465 7220 6973 2074 6572  e cluster is ter
-0000ed60: 6d69 6e61 7465 642e 0a20 2020 2020 2020  minated..       
-0000ed70: 2020 2020 2066 2773 3d24 2853 4b59 5049       f's=$(SKYPI
-0000ed80: 4c4f 545f 4445 4255 473d 3020 736b 7920  LOT_DEBUG=0 sky 
-0000ed90: 7374 6174 7573 202d 2d72 6566 7265 7368  status --refresh
-0000eda0: 2920 2626 2070 7269 6e74 6620 2224 7322  ) && printf "$s"
-0000edb0: 2026 2620 7b7b 2065 6368 6f20 2224 7322   && {{ echo "$s"
-0000edc0: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
-0000edd0: 2067 7265 7020 2241 7574 6f64 6f77 6e65   grep "Autodowne
-0000ede0: 6420 636c 7573 7465 725c 7c74 6572 6d69  d cluster\|termi
-0000edf0: 6e61 7465 6420 6f6e 2074 6865 2063 6c6f  nated on the clo
-0000ee00: 7564 223b 207d 7d20 7c7c 207b 7b20 6563  ud"; }} || {{ ec
-0000ee10: 686f 2022 2473 2220 7c20 6772 6570 207b  ho "$s" | grep {
-0000ee20: 6e61 6d65 7d20 2626 2065 7869 7420 3120  name} && exit 1 
-0000ee30: 7c7c 2065 7869 7420 303b 207d 7d27 2c0a  || exit 0; }}',.
-0000ee40: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-0000ee50: 7920 6c61 756e 6368 202d 7920 2d64 202d  y launch -y -d -
-0000ee60: 6320 7b6e 616d 657d 207b 5343 505f 5459  c {name} {SCP_TY
-0000ee70: 5045 7d20 2d2d 646f 776e 2074 6573 7473  PE} --down tests
-0000ee80: 2f74 6573 745f 7961 6d6c 732f 6d69 6e69  /test_yamls/mini
-0000ee90: 6d61 6c2e 7961 6d6c 272c 0a20 2020 2020  mal.yaml',.     
-0000eea0: 2020 2020 2020 2066 2773 6b79 2061 7574         f'sky aut
-0000eeb0: 6f73 746f 7020 2d79 207b 6e61 6d65 7d20  ostop -y {name} 
-0000eec0: 2d2d 6361 6e63 656c 272c 0a20 2020 2020  --cancel',.     
-0000eed0: 2020 2020 2020 2027 736c 6565 7020 3230         'sleep 20
-0000eee0: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
-0000eef0: 2320 456e 7375 7265 2074 6865 2063 6c75  # Ensure the clu
-0000ef00: 7374 6572 2069 7320 7374 696c 6c20 5550  ster is still UP
-0000ef10: 2e0a 2020 2020 2020 2020 2020 2020 6627  ..            f'
-0000ef20: 733d 2428 534b 5950 494c 4f54 5f44 4542  s=$(SKYPILOT_DEB
-0000ef30: 5547 3d30 2073 6b79 2073 7461 7475 7320  UG=0 sky status 
-0000ef40: 2d2d 7265 6672 6573 6829 2026 2620 7072  --refresh) && pr
-0000ef50: 696e 7466 2022 2473 2220 2626 2065 6368  intf "$s" && ech
-0000ef60: 6f20 2224 7322 207c 2067 7265 7020 7b6e  o "$s" | grep {n
-0000ef70: 616d 657d 207c 2067 7265 7020 5550 272c  ame} | grep UP',
-0000ef80: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
-0000ef90: 2020 2020 6627 736b 7920 646f 776e 202d      f'sky down -
-0000efa0: 7920 7b6e 616d 657d 272c 0a20 2020 2020  y {name}',.     
-0000efb0: 2020 2074 696d 656f 7574 3d32 3520 2a20     timeout=25 * 
-0000efc0: 3630 2c0a 2020 2020 290a 2020 2020 7275  60,.    ).    ru
-0000efd0: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
-0000efe0: 0a0a 0a64 6566 205f 6765 745f 6361 6e63  ...def _get_canc
-0000eff0: 656c 5f74 6173 6b5f 7769 7468 5f63 6c6f  el_task_with_clo
-0000f000: 7564 286e 616d 652c 2063 6c6f 7564 2c20  ud(name, cloud, 
-0000f010: 7469 6d65 6f75 743d 3135 202a 2036 3029  timeout=15 * 60)
-0000f020: 3a0a 2020 2020 7465 7374 203d 2054 6573  :.    test = Tes
-0000f030: 7428 0a20 2020 2020 2020 2066 277b 636c  t(.        f'{cl
-0000f040: 6f75 647d 2d63 616e 6365 6c2d 7461 736b  oud}-cancel-task
-0000f050: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
-0000f060: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
-0000f070: 6175 6e63 6820 2d63 207b 6e61 6d65 7d20  aunch -c {name} 
-0000f080: 6578 616d 706c 6573 2f72 6573 6e65 745f  examples/resnet_
-0000f090: 6170 702e 7961 6d6c 202d 2d63 6c6f 7564  app.yaml --cloud
-0000f0a0: 207b 636c 6f75 647d 202d 7920 2d64 272c   {cloud} -y -d',
-0000f0b0: 0a20 2020 2020 2020 2020 2020 2023 2057  .            # W
-0000f0c0: 6169 7420 7468 6520 4750 5520 7072 6f63  ait the GPU proc
-0000f0d0: 6573 7320 746f 2073 7461 7274 2e0a 2020  ess to start..  
-0000f0e0: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
-0000f0f0: 2036 3027 2c0a 2020 2020 2020 2020 2020   60',.          
-0000f100: 2020 6627 736b 7920 6578 6563 207b 6e61    f'sky exec {na
-0000f110: 6d65 7d20 226e 7669 6469 612d 736d 6920  me} "nvidia-smi 
-0000f120: 7c20 6772 6570 2070 7974 686f 6e22 272c  | grep python"',
-0000f130: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000f140: 6b79 206c 6f67 7320 7b6e 616d 657d 2032  ky logs {name} 2
-0000f150: 202d 2d73 7461 7475 7327 2c20 2023 2045   --status',  # E
-0000f160: 6e73 7572 6520 7468 6520 6a6f 6220 7375  nsure the job su
-0000f170: 6363 6565 6465 642e 0a20 2020 2020 2020  cceeded..       
-0000f180: 2020 2020 2066 2773 6b79 2063 616e 6365       f'sky cance
-0000f190: 6c20 2d79 207b 6e61 6d65 7d20 3127 2c0a  l -y {name} 1',.
-0000f1a0: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
-0000f1b0: 6570 2036 3027 2c0a 2020 2020 2020 2020  ep 60',.        
-0000f1c0: 2020 2020 2320 6368 6563 6b20 6966 2074      # check if t
-0000f1d0: 6865 2070 7974 686f 6e20 6a6f 6220 6973  he python job is
-0000f1e0: 2067 6f6e 652e 0a20 2020 2020 2020 2020   gone..         
-0000f1f0: 2020 2066 2773 6b79 2065 7865 6320 7b6e     f'sky exec {n
-0000f200: 616d 657d 2022 2120 6e76 6964 6961 2d73  ame} "! nvidia-s
-0000f210: 6d69 207c 2067 7265 7020 7079 7468 6f6e  mi | grep python
-0000f220: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-0000f230: 6627 736b 7920 6c6f 6773 207b 6e61 6d65  f'sky logs {name
-0000f240: 7d20 3320 2d2d 7374 6174 7573 272c 2020  } 3 --status',  
-0000f250: 2320 456e 7375 7265 2074 6865 206a 6f62  # Ensure the job
-0000f260: 2073 7563 6365 6564 6564 2e0a 2020 2020   succeeded..    
-0000f270: 2020 2020 5d2c 0a20 2020 2020 2020 2066      ],.        f
-0000f280: 2773 6b79 2064 6f77 6e20 2d79 207b 6e61  'sky down -y {na
-0000f290: 6d65 7d27 2c0a 2020 2020 2020 2020 7469  me}',.        ti
-0000f2a0: 6d65 6f75 743d 7469 6d65 6f75 742c 0a20  meout=timeout,. 
-0000f2b0: 2020 2029 0a20 2020 2072 6574 7572 6e20     ).    return 
-0000f2c0: 7465 7374 0a0a 0a23 202d 2d2d 2d2d 2d2d  test...# -------
-0000f2d0: 2d2d 2d20 5465 7374 696e 6720 6073 6b79  --- Testing `sky
-0000f2e0: 2063 616e 6365 6c60 202d 2d2d 2d2d 2d2d   cancel` -------
-0000f2f0: 2d2d 2d0a 4070 7974 6573 742e 6d61 726b  ---.@pytest.mark
-0000f300: 2e61 7773 0a40 7079 7465 7374 2e6d 6172  .aws.@pytest.mar
-0000f310: 6b2e 736b 6970 280a 2020 2020 7265 6173  k.skip(.    reas
-0000f320: 6f6e 3d27 5468 6520 7265 736e 6574 5f61  on='The resnet_a
-0000f330: 7070 2069 7320 666c 616b 792c 2064 7565  pp is flaky, due
-0000f340: 2074 6f20 5446 2066 6169 6c69 6e67 2074   to TF failing t
-0000f350: 6f20 6465 7465 6374 2047 5055 732e 2729  o detect GPUs.')
-0000f360: 0a64 6566 2074 6573 745f 6361 6e63 656c  .def test_cancel
-0000f370: 5f61 7773 2829 3a0a 2020 2020 6e61 6d65  _aws():.    name
-0000f380: 203d 205f 6765 745f 636c 7573 7465 725f   = _get_cluster_
-0000f390: 6e61 6d65 2829 0a20 2020 2074 6573 7420  name().    test 
-0000f3a0: 3d20 5f67 6574 5f63 616e 6365 6c5f 7461  = _get_cancel_ta
-0000f3b0: 736b 5f77 6974 685f 636c 6f75 6428 6e61  sk_with_cloud(na
-0000f3c0: 6d65 2c20 2761 7773 2729 0a20 2020 2072  me, 'aws').    r
-0000f3d0: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
-0000f3e0: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
-0000f3f0: 2e67 6370 0a40 7079 7465 7374 2e6d 6172  .gcp.@pytest.mar
-0000f400: 6b2e 736b 6970 280a 2020 2020 7265 6173  k.skip(.    reas
-0000f410: 6f6e 3d27 5468 6520 7265 736e 6574 5f61  on='The resnet_a
-0000f420: 7070 2069 7320 666c 616b 792c 2064 7565  pp is flaky, due
-0000f430: 2074 6f20 5446 2066 6169 6c69 6e67 2074   to TF failing t
-0000f440: 6f20 6465 7465 6374 2047 5055 732e 2729  o detect GPUs.')
-0000f450: 0a64 6566 2074 6573 745f 6361 6e63 656c  .def test_cancel
-0000f460: 5f67 6370 2829 3a0a 2020 2020 6e61 6d65  _gcp():.    name
-0000f470: 203d 205f 6765 745f 636c 7573 7465 725f   = _get_cluster_
-0000f480: 6e61 6d65 2829 0a20 2020 2074 6573 7420  name().    test 
-0000f490: 3d20 5f67 6574 5f63 616e 6365 6c5f 7461  = _get_cancel_ta
-0000f4a0: 736b 5f77 6974 685f 636c 6f75 6428 6e61  sk_with_cloud(na
-0000f4b0: 6d65 2c20 2767 6370 2729 0a20 2020 2072  me, 'gcp').    r
-0000f4c0: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
-0000f4d0: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
-0000f4e0: 2e61 7a75 7265 0a40 7079 7465 7374 2e6d  .azure.@pytest.m
-0000f4f0: 6172 6b2e 736b 6970 280a 2020 2020 7265  ark.skip(.    re
-0000f500: 6173 6f6e 3d27 5468 6520 7265 736e 6574  ason='The resnet
-0000f510: 5f61 7070 2069 7320 666c 616b 792c 2064  _app is flaky, d
-0000f520: 7565 2074 6f20 5446 2066 6169 6c69 6e67  ue to TF failing
-0000f530: 2074 6f20 6465 7465 6374 2047 5055 732e   to detect GPUs.
-0000f540: 2729 0a64 6566 2074 6573 745f 6361 6e63  ').def test_canc
-0000f550: 656c 5f61 7a75 7265 2829 3a0a 2020 2020  el_azure():.    
-0000f560: 6e61 6d65 203d 205f 6765 745f 636c 7573  name = _get_clus
-0000f570: 7465 725f 6e61 6d65 2829 0a20 2020 2074  ter_name().    t
-0000f580: 6573 7420 3d20 5f67 6574 5f63 616e 6365  est = _get_cance
-0000f590: 6c5f 7461 736b 5f77 6974 685f 636c 6f75  l_task_with_clou
-0000f5a0: 6428 6e61 6d65 2c20 2761 7a75 7265 272c  d(name, 'azure',
-0000f5b0: 2074 696d 656f 7574 3d33 3020 2a20 3630   timeout=30 * 60
-0000f5c0: 290a 2020 2020 7275 6e5f 6f6e 655f 7465  ).    run_one_te
-0000f5d0: 7374 2874 6573 7429 0a0a 0a40 7079 7465  st(test)...@pyte
-0000f5e0: 7374 2e6d 6172 6b2e 6e6f 5f6c 616d 6264  st.mark.no_lambd
-0000f5f0: 615f 636c 6f75 6420 2023 204c 616d 6264  a_cloud  # Lambd
-0000f600: 6120 436c 6f75 6420 646f 6573 206e 6f74  a Cloud does not
-0000f610: 2068 6176 6520 5631 3030 2067 7075 730a   have V100 gpus.
-0000f620: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
-0000f630: 6962 6d20 2023 2049 424d 2063 6c6f 7564  ibm  # IBM cloud
-0000f640: 2063 7572 7265 6e74 6c79 2064 6f65 736e   currently doesn
-0000f650: 2774 2070 726f 7669 6465 2070 7562 6c69  't provide publi
-0000f660: 6320 696d 6167 6520 7769 7468 2043 5544  c image with CUD
-0000f670: 410a 4070 7974 6573 742e 6d61 726b 2e6e  A.@pytest.mark.n
-0000f680: 6f5f 7363 7020 2023 2053 4350 2064 6f65  o_scp  # SCP doe
-0000f690: 7320 6e6f 7420 7375 7070 6f72 7420 6e75  s not support nu
-0000f6a0: 6d5f 6e6f 6465 7320 3e20 3120 7965 740a  m_nodes > 1 yet.
-0000f6b0: 6465 6620 7465 7374 5f63 616e 6365 6c5f  def test_cancel_
-0000f6c0: 7079 746f 7263 6828 6765 6e65 7269 635f  pytorch(generic_
-0000f6d0: 636c 6f75 643a 2073 7472 293a 0a20 2020  cloud: str):.   
-0000f6e0: 206e 616d 6520 3d20 5f67 6574 5f63 6c75   name = _get_clu
-0000f6f0: 7374 6572 5f6e 616d 6528 290a 2020 2020  ster_name().    
-0000f700: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
-0000f710: 2020 2020 2027 6361 6e63 656c 2d70 7974       'cancel-pyt
-0000f720: 6f72 6368 272c 0a20 2020 2020 2020 205b  orch',.        [
-0000f730: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-0000f740: 6b79 206c 6175 6e63 6820 2d63 207b 6e61  ky launch -c {na
-0000f750: 6d65 7d20 2d2d 636c 6f75 6420 7b67 656e  me} --cloud {gen
-0000f760: 6572 6963 5f63 6c6f 7564 7d20 6578 616d  eric_cloud} exam
-0000f770: 706c 6573 2f72 6573 6e65 745f 6469 7374  ples/resnet_dist
-0000f780: 7269 6275 7465 645f 746f 7263 682e 7961  ributed_torch.ya
-0000f790: 6d6c 202d 7920 2d64 272c 0a20 2020 2020  ml -y -d',.     
-0000f7a0: 2020 2020 2020 2023 2057 6169 7420 7468         # Wait th
-0000f7b0: 6520 4750 5520 7072 6f63 6573 7320 746f  e GPU process to
-0000f7c0: 2073 7461 7274 2e0a 2020 2020 2020 2020   start..        
-0000f7d0: 2020 2020 2773 6c65 6570 2039 3027 2c0a      'sleep 90',.
-0000f7e0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-0000f7f0: 7920 6578 6563 207b 6e61 6d65 7d20 226e  y exec {name} "n
-0000f800: 7669 6469 612d 736d 6920 7c20 6772 6570  vidia-smi | grep
-0000f810: 2070 7974 686f 6e22 272c 0a20 2020 2020   python"',.     
-0000f820: 2020 2020 2020 2066 2773 6b79 206c 6f67         f'sky log
-0000f830: 7320 7b6e 616d 657d 2032 202d 2d73 7461  s {name} 2 --sta
-0000f840: 7475 7327 2c20 2023 2045 6e73 7572 6520  tus',  # Ensure 
-0000f850: 7468 6520 6a6f 6220 7375 6363 6565 6465  the job succeede
-0000f860: 642e 0a20 2020 2020 2020 2020 2020 2066  d..            f
-0000f870: 2773 6b79 2063 616e 6365 6c20 2d79 207b  'sky cancel -y {
-0000f880: 6e61 6d65 7d20 3127 2c0a 2020 2020 2020  name} 1',.      
-0000f890: 2020 2020 2020 2773 6c65 6570 2036 3027        'sleep 60'
-0000f8a0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-0000f8b0: 736b 7920 6578 6563 207b 6e61 6d65 7d20  sky exec {name} 
-0000f8c0: 2228 6e76 6964 6961 2d73 6d69 207c 2067  "(nvidia-smi | g
-0000f8d0: 7265 7020 5c27 4e6f 2072 756e 6e69 6e67  rep \'No running
-0000f8e0: 2070 726f 6365 7373 5c27 2920 7c7c 2027   process\') || '
-0000f8f0: 0a20 2020 2020 2020 2020 2020 2023 2045  .            # E
-0000f900: 6e73 7572 6520 586f 7267 2069 7320 7468  nsure Xorg is th
-0000f910: 6520 6f6e 6c79 2070 726f 6365 7373 2072  e only process r
-0000f920: 756e 6e69 6e67 2e0a 2020 2020 2020 2020  unning..        
-0000f930: 2020 2020 275b 205c 2428 6e76 6964 6961      '[ \$(nvidia
-0000f940: 2d73 6d69 207c 2067 7265 7020 2d41 2031  -smi | grep -A 1
-0000f950: 3020 5072 6f63 6573 7365 7320 7c20 6772  0 Processes | gr
-0000f960: 6570 202d 4120 3130 203d 3d3d 207c 2067  ep -A 10 === | g
-0000f970: 7265 7020 2d76 2058 6f72 6729 202d 6571  rep -v Xorg) -eq
-0000f980: 2032 205d 2227 2c0a 2020 2020 2020 2020   2 ]"',.        
-0000f990: 2020 2020 6627 736b 7920 6c6f 6773 207b      f'sky logs {
-0000f9a0: 6e61 6d65 7d20 3320 2d2d 7374 6174 7573  name} 3 --status
-0000f9b0: 272c 2020 2320 456e 7375 7265 2074 6865  ',  # Ensure the
-0000f9c0: 206a 6f62 2073 7563 6365 6564 6564 2e0a   job succeeded..
-0000f9d0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-0000f9e0: 2020 2066 2773 6b79 2064 6f77 6e20 2d79     f'sky down -y
-0000f9f0: 207b 6e61 6d65 7d27 2c0a 2020 2020 2020   {name}',.      
-0000fa00: 2020 7469 6d65 6f75 743d 3230 202a 2036    timeout=20 * 6
-0000fa10: 302c 0a20 2020 2029 0a20 2020 2072 756e  0,.    ).    run
-0000fa20: 5f6f 6e65 5f74 6573 7428 7465 7374 290a  _one_test(test).
-0000fa30: 0a0a 2320 6361 6e27 7420 7573 6520 605f  ..# can't use `_
-0000fa40: 6765 745f 6361 6e63 656c 5f74 6173 6b5f  get_cancel_task_
-0000fa50: 7769 7468 5f63 6c6f 7564 2829 602c 2061  with_cloud()`, a
-0000fa60: 7320 636f 6d6d 616e 6420 606e 7669 6469  s command `nvidi
-0000fa70: 612d 736d 6960 0a23 2072 6571 7569 7265  a-smi`.# require
-0000fa80: 7320 6120 4355 4441 2070 7562 6c69 6320  s a CUDA public 
-0000fa90: 696d 6167 652c 2077 6869 6368 2049 424d  image, which IBM
-0000faa0: 2064 6f65 736e 2774 206f 6666 6572 0a40   doesn't offer.@
-0000fab0: 7079 7465 7374 2e6d 6172 6b2e 6962 6d0a  pytest.mark.ibm.
-0000fac0: 6465 6620 7465 7374 5f63 616e 6365 6c5f  def test_cancel_
-0000fad0: 6962 6d28 293a 0a20 2020 206e 616d 6520  ibm():.    name 
-0000fae0: 3d20 5f67 6574 5f63 6c75 7374 6572 5f6e  = _get_cluster_n
-0000faf0: 616d 6528 290a 2020 2020 7465 7374 203d  ame().    test =
-0000fb00: 2054 6573 7428 0a20 2020 2020 2020 2027   Test(.        '
-0000fb10: 6962 6d2d 6361 6e63 656c 2d74 6173 6b27  ibm-cancel-task'
-0000fb20: 2c0a 2020 2020 2020 2020 5b0a 2020 2020  ,.        [.    
-0000fb30: 2020 2020 2020 2020 6627 736b 7920 6c61          f'sky la
-0000fb40: 756e 6368 202d 7920 2d63 207b 6e61 6d65  unch -y -c {name
-0000fb50: 7d20 2d2d 636c 6f75 6420 6962 6d20 6578  } --cloud ibm ex
-0000fb60: 616d 706c 6573 2f6d 696e 696d 616c 2e79  amples/minimal.y
-0000fb70: 616d 6c27 2c0a 2020 2020 2020 2020 2020  aml',.          
-0000fb80: 2020 6627 736b 7920 6578 6563 207b 6e61    f'sky exec {na
-0000fb90: 6d65 7d20 2d6e 207b 6e61 6d65 7d2d 3120  me} -n {name}-1 
-0000fba0: 2d64 2020 2277 6869 6c65 2074 7275 653b  -d  "while true;
-0000fbb0: 2064 6f20 6563 686f 205c 2748 656c 6c6f   do echo \'Hello
-0000fbc0: 2053 6b79 5069 6c6f 745c 273b 2073 6c65   SkyPilot\'; sle
-0000fbd0: 6570 2032 3b20 646f 6e65 2227 2c0a 2020  ep 2; done"',.  
-0000fbe0: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
-0000fbf0: 2032 3027 2c0a 2020 2020 2020 2020 2020   20',.          
-0000fc00: 2020 6627 736b 7920 7175 6575 6520 7b6e    f'sky queue {n
-0000fc10: 616d 657d 207c 2067 7265 7020 7b6e 616d  ame} | grep {nam
-0000fc20: 657d 2d31 207c 2067 7265 7020 5255 4e4e  e}-1 | grep RUNN
-0000fc30: 494e 4727 2c0a 2020 2020 2020 2020 2020  ING',.          
-0000fc40: 2020 6627 736b 7920 6361 6e63 656c 202d    f'sky cancel -
-0000fc50: 7920 7b6e 616d 657d 2032 272c 0a20 2020  y {name} 2',.   
-0000fc60: 2020 2020 2020 2020 2066 2773 6c65 6570           f'sleep
-0000fc70: 2035 272c 0a20 2020 2020 2020 2020 2020   5',.           
-0000fc80: 2066 2773 6b79 2071 7565 7565 207b 6e61   f'sky queue {na
-0000fc90: 6d65 7d20 7c20 6772 6570 207b 6e61 6d65  me} | grep {name
-0000fca0: 7d2d 3120 7c20 6772 6570 2043 414e 4345  }-1 | grep CANCE
-0000fcb0: 4c4c 4544 272c 0a20 2020 2020 2020 205d  LLED',.        ]
-0000fcc0: 2c0a 2020 2020 2020 2020 6627 736b 7920  ,.        f'sky 
-0000fcd0: 646f 776e 202d 7920 7b6e 616d 657d 272c  down -y {name}',
-0000fce0: 0a20 2020 2029 0a20 2020 2072 756e 5f6f  .    ).    run_o
-0000fcf0: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
-0000fd00: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2054 6573  # ---------- Tes
-0000fd10: 7469 6e67 2075 7365 2d73 706f 7420 6f70  ting use-spot op
-0000fd20: 7469 6f6e 202d 2d2d 2d2d 2d2d 2d2d 2d0a  tion ----------.
-0000fd30: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
-0000fd40: 6c61 6d62 6461 5f63 6c6f 7564 2020 2320  lambda_cloud  # 
-0000fd50: 4c61 6d62 6461 2043 6c6f 7564 2064 6f65  Lambda Cloud doe
-0000fd60: 7320 6e6f 7420 7375 7070 6f72 7420 7370  s not support sp
-0000fd70: 6f74 2069 6e73 7461 6e63 6573 0a40 7079  ot instances.@py
-0000fd80: 7465 7374 2e6d 6172 6b2e 6e6f 5f69 626d  test.mark.no_ibm
-0000fd90: 2020 2320 4942 4d20 436c 6f75 6420 646f    # IBM Cloud do
-0000fda0: 6573 206e 6f74 2073 7570 706f 7274 2073  es not support s
-0000fdb0: 706f 7420 696e 7374 616e 6365 730a 4070  pot instances.@p
-0000fdc0: 7974 6573 742e 6d61 726b 2e6e 6f5f 7363  ytest.mark.no_sc
-0000fdd0: 7020 2023 2053 4350 2064 6f65 7320 6e6f  p  # SCP does no
-0000fde0: 7420 7375 7070 6f72 7420 7370 6f74 2069  t support spot i
-0000fdf0: 6e73 7461 6e63 6573 0a64 6566 2074 6573  nstances.def tes
-0000fe00: 745f 7573 655f 7370 6f74 2867 656e 6572  t_use_spot(gener
-0000fe10: 6963 5f63 6c6f 7564 3a20 7374 7229 3a0a  ic_cloud: str):.
-0000fe20: 2020 2020 2222 2254 6573 7420 7573 652d      """Test use-
-0000fe30: 7370 6f74 2061 6e64 2073 6b79 2065 7865  spot and sky exe
-0000fe40: 632e 2222 220a 2020 2020 6e61 6d65 203d  c.""".    name =
-0000fe50: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
-0000fe60: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
-0000fe70: 5465 7374 280a 2020 2020 2020 2020 2775  Test(.        'u
-0000fe80: 7365 2d73 706f 7427 2c0a 2020 2020 2020  se-spot',.      
-0000fe90: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-0000fea0: 6627 736b 7920 6c61 756e 6368 202d 6320  f'sky launch -c 
-0000feb0: 7b6e 616d 657d 202d 2d63 6c6f 7564 207b  {name} --cloud {
-0000fec0: 6765 6e65 7269 635f 636c 6f75 647d 2074  generic_cloud} t
-0000fed0: 6573 7473 2f74 6573 745f 7961 6d6c 732f  ests/test_yamls/
-0000fee0: 6d69 6e69 6d61 6c2e 7961 6d6c 202d 2d75  minimal.yaml --u
-0000fef0: 7365 2d73 706f 7420 2d79 272c 0a20 2020  se-spot -y',.   
-0000ff00: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
-0000ff10: 6f67 7320 7b6e 616d 657d 2031 202d 2d73  ogs {name} 1 --s
-0000ff20: 7461 7475 7327 2c0a 2020 2020 2020 2020  tatus',.        
-0000ff30: 2020 2020 6627 736b 7920 6578 6563 207b      f'sky exec {
-0000ff40: 6e61 6d65 7d20 6563 686f 2068 6927 2c0a  name} echo hi',.
-0000ff50: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-0000ff60: 7920 6c6f 6773 207b 6e61 6d65 7d20 3220  y logs {name} 2 
-0000ff70: 2d2d 7374 6174 7573 272c 0a20 2020 2020  --status',.     
-0000ff80: 2020 205d 2c0a 2020 2020 2020 2020 6627     ],.        f'
-0000ff90: 736b 7920 646f 776e 202d 7920 7b6e 616d  sky down -y {nam
-0000ffa0: 657d 272c 0a20 2020 2029 0a20 2020 2072  e}',.    ).    r
-0000ffb0: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
-0000ffc0: 290a 0a0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  )...# ----------
-0000ffd0: 2054 6573 7469 6e67 206d 616e 6167 6564   Testing managed
-0000ffe0: 2073 706f 7420 2d2d 2d2d 2d2d 2d2d 2d2d   spot ----------
-0000fff0: 0a40 7079 7465 7374 2e6d 6172 6b2e 6e6f  .@pytest.mark.no
-00010000: 5f6c 616d 6264 615f 636c 6f75 6420 2023  _lambda_cloud  #
-00010010: 204c 616d 6264 6120 436c 6f75 6420 646f   Lambda Cloud do
-00010020: 6573 206e 6f74 2073 7570 706f 7274 2073  es not support s
-00010030: 706f 7420 696e 7374 616e 6365 730a 4070  pot instances.@p
-00010040: 7974 6573 742e 6d61 726b 2e6e 6f5f 6962  ytest.mark.no_ib
-00010050: 6d20 2023 2049 424d 2043 6c6f 7564 2064  m  # IBM Cloud d
-00010060: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
-00010070: 7370 6f74 2069 6e73 7461 6e63 6573 0a40  spot instances.@
-00010080: 7079 7465 7374 2e6d 6172 6b2e 6e6f 5f73  pytest.mark.no_s
-00010090: 6370 2020 2320 5343 5020 646f 6573 206e  cp  # SCP does n
-000100a0: 6f74 2073 7570 706f 7274 2073 706f 7420  ot support spot 
-000100b0: 696e 7374 616e 6365 730a 4070 7974 6573  instances.@pytes
-000100c0: 742e 6d61 726b 2e6d 616e 6167 6564 5f73  t.mark.managed_s
-000100d0: 706f 740a 6465 6620 7465 7374 5f73 706f  pot.def test_spo
-000100e0: 7428 6765 6e65 7269 635f 636c 6f75 643a  t(generic_cloud:
-000100f0: 2073 7472 293a 0a20 2020 2022 2222 5465   str):.    """Te
-00010100: 7374 2074 6865 2073 706f 7420 7961 6d6c  st the spot yaml
-00010110: 2e22 2222 0a20 2020 206e 616d 6520 3d20  .""".    name = 
-00010120: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
-00010130: 6528 290a 2020 2020 7465 7374 203d 2054  e().    test = T
-00010140: 6573 7428 0a20 2020 2020 2020 2027 6d61  est(.        'ma
-00010150: 6e61 6765 642d 7370 6f74 272c 0a20 2020  naged-spot',.   
-00010160: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-00010170: 2020 2066 2773 6b79 2073 706f 7420 6c61     f'sky spot la
-00010180: 756e 6368 202d 6e20 7b6e 616d 657d 2d31  unch -n {name}-1
-00010190: 202d 2d63 6c6f 7564 207b 6765 6e65 7269   --cloud {generi
-000101a0: 635f 636c 6f75 647d 2065 7861 6d70 6c65  c_cloud} example
-000101b0: 732f 6d61 6e61 6765 645f 7370 6f74 2e79  s/managed_spot.y
-000101c0: 616d 6c20 2d79 202d 6427 2c0a 2020 2020  aml -y -d',.    
-000101d0: 2020 2020 2020 2020 6627 736b 7920 7370          f'sky sp
-000101e0: 6f74 206c 6175 6e63 6820 2d6e 207b 6e61  ot launch -n {na
-000101f0: 6d65 7d2d 3220 2d2d 636c 6f75 6420 7b67  me}-2 --cloud {g
-00010200: 656e 6572 6963 5f63 6c6f 7564 7d20 6578  eneric_cloud} ex
-00010210: 616d 706c 6573 2f6d 616e 6167 6564 5f73  amples/managed_s
-00010220: 706f 742e 7961 6d6c 202d 7920 2d64 272c  pot.yaml -y -d',
-00010230: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
-00010240: 6565 7020 3527 2c0a 2020 2020 2020 2020  eep 5',.        
-00010250: 2020 2020 6627 7b5f 5350 4f54 5f51 5545      f'{_SPOT_QUE
-00010260: 5545 5f57 4149 547d 7c20 6772 6570 207b  UE_WAIT}| grep {
-00010270: 6e61 6d65 7d2d 3120 7c20 6865 6164 202d  name}-1 | head -
-00010280: 6e31 207c 2067 7265 7020 2253 5441 5254  n1 | grep "START
-00010290: 494e 475c 7c52 554e 4e49 4e47 2227 2c0a  ING\|RUNNING"',.
-000102a0: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
-000102b0: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
-000102c0: 7c20 6772 6570 207b 6e61 6d65 7d2d 3220  | grep {name}-2 
-000102d0: 7c20 6865 6164 202d 6e31 207c 2067 7265  | head -n1 | gre
-000102e0: 7020 2253 5441 5254 494e 475c 7c52 554e  p "STARTING\|RUN
-000102f0: 4e49 4e47 2227 2c0a 2020 2020 2020 2020  NING"',.        
-00010300: 2020 2020 5f53 504f 545f 4341 4e43 454c      _SPOT_CANCEL
-00010310: 5f57 4149 542e 666f 726d 6174 286a 6f62  _WAIT.format(job
-00010320: 5f6e 616d 653d 6627 7b6e 616d 657d 2d31  _name=f'{name}-1
-00010330: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00010340: 2773 6c65 6570 2035 272c 0a20 2020 2020  'sleep 5',.     
-00010350: 2020 2020 2020 2066 277b 5f53 504f 545f         f'{_SPOT_
-00010360: 5155 4555 455f 5741 4954 7d7c 2067 7265  QUEUE_WAIT}| gre
-00010370: 7020 7b6e 616d 657d 2d31 207c 2068 6561  p {name}-1 | hea
-00010380: 6420 2d6e 3120 7c20 6772 6570 2022 4341  d -n1 | grep "CA
-00010390: 4e43 454c 4c49 4e47 5c7c 4341 4e43 454c  NCELLING\|CANCEL
-000103a0: 4c45 4422 272c 0a20 2020 2020 2020 2020  LED"',.         
-000103b0: 2020 2027 736c 6565 7020 3230 3027 2c0a     'sleep 200',.
-000103c0: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
-000103d0: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
-000103e0: 7c20 6772 6570 207b 6e61 6d65 7d2d 3120  | grep {name}-1 
-000103f0: 7c20 6865 6164 202d 6e31 207c 2067 7265  | head -n1 | gre
-00010400: 7020 4341 4e43 454c 4c45 4427 2c0a 2020  p CANCELLED',.  
-00010410: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
-00010420: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
-00010430: 6772 6570 207b 6e61 6d65 7d2d 3220 7c20  grep {name}-2 | 
-00010440: 6865 6164 202d 6e31 207c 2067 7265 7020  head -n1 | grep 
-00010450: 2252 554e 4e49 4e47 5c7c 5355 4343 4545  "RUNNING\|SUCCEE
-00010460: 4445 4422 272c 0a20 2020 2020 2020 205d  DED"',.        ]
-00010470: 2c0a 2020 2020 2020 2020 2320 544f 444f  ,.        # TODO
-00010480: 287a 6877 7529 3a20 4368 616e 6765 2074  (zhwu): Change t
-00010490: 6f20 5f53 504f 545f 4341 4e43 454c 5f57  o _SPOT_CANCEL_W
-000104a0: 4149 542e 666f 726d 6174 286a 6f62 5f6e  AIT.format(job_n
-000104b0: 616d 653d 6627 7b6e 616d 657d 2d31 202d  ame=f'{name}-1 -
-000104c0: 6e20 7b6e 616d 657d 2d32 2729 2077 6865  n {name}-2') whe
-000104d0: 6e0a 2020 2020 2020 2020 2320 6361 6e63  n.        # canc
-000104e0: 656c 696e 6720 6d75 6c74 6970 6c65 206a  eling multiple j
-000104f0: 6f62 206e 616d 6573 2069 7320 7375 7070  ob names is supp
-00010500: 6f72 7465 642e 0a20 2020 2020 2020 2028  orted..        (
-00010510: 5f53 504f 545f 4341 4e43 454c 5f57 4149  _SPOT_CANCEL_WAI
-00010520: 542e 666f 726d 6174 286a 6f62 5f6e 616d  T.format(job_nam
-00010530: 653d 6627 7b6e 616d 657d 2d31 2729 202b  e=f'{name}-1') +
-00010540: 2027 3b20 2720 2b0a 2020 2020 2020 2020   '; ' +.        
-00010550: 205f 5350 4f54 5f43 414e 4345 4c5f 5741   _SPOT_CANCEL_WA
-00010560: 4954 2e66 6f72 6d61 7428 6a6f 625f 6e61  IT.format(job_na
-00010570: 6d65 3d66 277b 6e61 6d65 7d2d 3227 2929  me=f'{name}-2'))
-00010580: 2c0a 2020 2020 2020 2020 2320 496e 6372  ,.        # Incr
-00010590: 6561 7365 2074 696d 656f 7574 2073 696e  ease timeout sin
-000105a0: 6365 2073 6b79 2073 706f 7420 7175 6575  ce sky spot queu
-000105b0: 6520 2d72 2063 616e 2062 6520 626c 6f63  e -r can be bloc
-000105c0: 6b65 6420 6279 206f 7468 6572 2073 706f  ked by other spo
-000105d0: 7420 7465 7374 732e 0a20 2020 2020 2020  t tests..       
-000105e0: 2074 696d 656f 7574 3d32 3020 2a20 3630   timeout=20 * 60
-000105f0: 2c0a 2020 2020 290a 2020 2020 7275 6e5f  ,.    ).    run_
-00010600: 6f6e 655f 7465 7374 2874 6573 7429 0a0a  one_test(test)..
-00010610: 0a40 7079 7465 7374 2e6d 6172 6b2e 6e6f  .@pytest.mark.no
-00010620: 5f6c 616d 6264 615f 636c 6f75 6420 2023  _lambda_cloud  #
-00010630: 204c 616d 6264 6120 436c 6f75 6420 646f   Lambda Cloud do
-00010640: 6573 206e 6f74 2073 7570 706f 7274 2073  es not support s
-00010650: 706f 7420 696e 7374 616e 6365 730a 4070  pot instances.@p
-00010660: 7974 6573 742e 6d61 726b 2e6e 6f5f 6962  ytest.mark.no_ib
-00010670: 6d20 2023 2049 424d 2043 6c6f 7564 2064  m  # IBM Cloud d
-00010680: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
-00010690: 7370 6f74 2069 6e73 7461 6e63 6573 0a40  spot instances.@
-000106a0: 7079 7465 7374 2e6d 6172 6b2e 6e6f 5f73  pytest.mark.no_s
-000106b0: 6370 2020 2320 5343 5020 646f 6573 206e  cp  # SCP does n
-000106c0: 6f74 2073 7570 706f 7274 2073 706f 7420  ot support spot 
-000106d0: 696e 7374 616e 6365 730a 4070 7974 6573  instances.@pytes
-000106e0: 742e 6d61 726b 2e6d 616e 6167 6564 5f73  t.mark.managed_s
-000106f0: 706f 740a 6465 6620 7465 7374 5f73 706f  pot.def test_spo
-00010700: 745f 7069 7065 6c69 6e65 2867 656e 6572  t_pipeline(gener
-00010710: 6963 5f63 6c6f 7564 3a20 7374 7229 3a0a  ic_cloud: str):.
-00010720: 2020 2020 2222 2254 6573 7420 6120 7370      """Test a sp
-00010730: 6f74 c2a0 7069 7065 6c69 6e65 2e22 2222  ot..pipeline."""
-00010740: 0a20 2020 206e 616d 6520 3d20 5f67 6574  .    name = _get
-00010750: 5f63 6c75 7374 6572 5f6e 616d 6528 290a  _cluster_name().
-00010760: 2020 2020 7465 7374 203d 2054 6573 7428      test = Test(
-00010770: 0a20 2020 2020 2020 2027 7370 6f74 2d70  .        'spot-p
-00010780: 6970 656c 696e 6527 2c0a 2020 2020 2020  ipeline',.      
-00010790: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-000107a0: 6627 736b 7920 7370 6f74 206c 6175 6e63  f'sky spot launc
-000107b0: 6820 2d6e 207b 6e61 6d65 7d20 7465 7374  h -n {name} test
-000107c0: 732f 7465 7374 5f79 616d 6c73 2f70 6970  s/test_yamls/pip
-000107d0: 656c 696e 652e 7961 6d6c 202d 7920 2d64  eline.yaml -y -d
-000107e0: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-000107f0: 736c 6565 7020 3527 2c0a 2020 2020 2020  sleep 5',.      
-00010800: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
-00010810: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
-00010820: 207b 6e61 6d65 7d20 7c20 6865 6164 202d   {name} | head -
-00010830: 6e31 207c 2067 7265 7020 2253 5441 5254  n1 | grep "START
-00010840: 494e 475c 7c52 554e 4e49 4e47 2227 2c0a  ING\|RUNNING"',.
-00010850: 2020 2020 2020 2020 2020 2020 2320 6067              # `g
-00010860: 7265 7020 2d41 2034 207b 6e61 6d65 7d60  rep -A 4 {name}`
-00010870: 2066 696e 6473 2074 6865 206a 6f62 2077   finds the job w
-00010880: 6974 6820 7b6e 616d 657d 2061 6e64 2074  ith {name} and t
-00010890: 6865 2034 206c 696e 6573 0a20 2020 2020  he 4 lines.     
-000108a0: 2020 2020 2020 2023 2061 6674 6572 2069         # after i
-000108b0: 742c 2069 2e65 2e20 7468 6520 3420 7461  t, i.e. the 4 ta
-000108c0: 736b 7320 7769 7468 696e 2074 6865 206a  sks within the j
-000108d0: 6f62 2e0a 2020 2020 2020 2020 2020 2020  ob..            
-000108e0: 2320 6073 6564 202d 6e20 3270 6020 6765  # `sed -n 2p` ge
-000108f0: 7473 2074 6865 2073 6563 6f6e 6420 6c69  ts the second li
-00010900: 6e65 206f 6620 7468 6520 3420 6c69 6e65  ne of the 4 line
-00010910: 732c 2069 2e65 2e20 7468 6520 6669 7273  s, i.e. the firs
-00010920: 740a 2020 2020 2020 2020 2020 2020 2320  t.            # 
-00010930: 7461 736b 2077 6974 6869 6e20 7468 6520  task within the 
-00010940: 6a6f 622e 0a20 2020 2020 2020 2020 2020  job..           
-00010950: 2066 277b 5f53 504f 545f 5155 4555 455f   f'{_SPOT_QUEUE_
-00010960: 5741 4954 7d7c 2067 7265 7020 2d41 2034  WAIT}| grep -A 4
-00010970: 207b 6e61 6d65 7d7c 2073 6564 202d 6e20   {name}| sed -n 
-00010980: 3270 207c 2067 7265 7020 2253 5441 5254  2p | grep "START
-00010990: 494e 475c 7c52 554e 4e49 4e47 2227 2c0a  ING\|RUNNING"',.
-000109a0: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
-000109b0: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
-000109c0: 7c20 6772 6570 202d 4120 3420 7b6e 616d  | grep -A 4 {nam
-000109d0: 657d 7c20 7365 6420 2d6e 2033 7020 7c20  e}| sed -n 3p | 
-000109e0: 6772 6570 2022 5045 4e44 494e 4722 272c  grep "PENDING"',
-000109f0: 0a20 2020 2020 2020 2020 2020 205f 5350  .            _SP
-00010a00: 4f54 5f43 414e 4345 4c5f 5741 4954 2e66  OT_CANCEL_WAIT.f
-00010a10: 6f72 6d61 7428 6a6f 625f 6e61 6d65 3d66  ormat(job_name=f
-00010a20: 277b 6e61 6d65 7d27 292c 0a20 2020 2020  '{name}'),.     
-00010a30: 2020 2020 2020 2027 736c 6565 7020 3527         'sleep 5'
-00010a40: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-00010a50: 7b5f 5350 4f54 5f51 5545 5545 5f57 4149  {_SPOT_QUEUE_WAI
-00010a60: 547d 7c20 6772 6570 202d 4120 3420 7b6e  T}| grep -A 4 {n
-00010a70: 616d 657d 7c20 7365 6420 2d6e 2032 7020  ame}| sed -n 2p 
-00010a80: 7c20 6772 6570 2022 4341 4e43 454c 4c49  | grep "CANCELLI
-00010a90: 4e47 5c7c 4341 4e43 454c 4c45 4422 272c  NG\|CANCELLED"',
-00010aa0: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
-00010ab0: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
-00010ac0: 7d7c 2067 7265 7020 2d41 2034 207b 6e61  }| grep -A 4 {na
-00010ad0: 6d65 7d7c 2073 6564 202d 6e20 3370 207c  me}| sed -n 3p |
-00010ae0: 2067 7265 7020 2243 414e 4345 4c4c 494e   grep "CANCELLIN
-00010af0: 475c 7c43 414e 4345 4c4c 4544 2227 2c0a  G\|CANCELLED"',.
-00010b00: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
-00010b10: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
-00010b20: 7c20 6772 6570 202d 4120 3420 7b6e 616d  | grep -A 4 {nam
-00010b30: 657d 7c20 7365 6420 2d6e 2034 7020 7c20  e}| sed -n 4p | 
-00010b40: 6772 6570 2022 4341 4e43 454c 4c49 4e47  grep "CANCELLING
-00010b50: 5c7c 4341 4e43 454c 4c45 4422 272c 0a20  \|CANCELLED"',. 
-00010b60: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
-00010b70: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
-00010b80: 2067 7265 7020 2d41 2034 207b 6e61 6d65   grep -A 4 {name
-00010b90: 7d7c 2073 6564 202d 6e20 3570 207c 2067  }| sed -n 5p | g
-00010ba0: 7265 7020 2243 414e 4345 4c4c 494e 475c  rep "CANCELLING\
-00010bb0: 7c43 414e 4345 4c4c 4544 2227 2c0a 2020  |CANCELLED"',.  
-00010bc0: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
-00010bd0: 2032 3030 272c 0a20 2020 2020 2020 2020   200',.         
-00010be0: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
-00010bf0: 455f 5741 4954 7d7c 2067 7265 7020 2d41  E_WAIT}| grep -A
-00010c00: 2034 207b 6e61 6d65 7d7c 2073 6564 202d   4 {name}| sed -
-00010c10: 6e20 3270 207c 2067 7265 7020 2243 414e  n 2p | grep "CAN
-00010c20: 4345 4c4c 4544 2227 2c0a 2020 2020 2020  CELLED"',.      
-00010c30: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
-00010c40: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
-00010c50: 202d 4120 3420 7b6e 616d 657d 7c20 7365   -A 4 {name}| se
-00010c60: 6420 2d6e 2033 7020 7c20 6772 6570 2022  d -n 3p | grep "
-00010c70: 4341 4e43 454c 4c45 4422 272c 0a20 2020  CANCELLED"',.   
-00010c80: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
-00010c90: 545f 5155 4555 455f 5741 4954 7d7c 2067  T_QUEUE_WAIT}| g
-00010ca0: 7265 7020 2d41 2034 207b 6e61 6d65 7d7c  rep -A 4 {name}|
-00010cb0: 2073 6564 202d 6e20 3470 207c 2067 7265   sed -n 4p | gre
-00010cc0: 7020 2243 414e 4345 4c4c 4544 2227 2c0a  p "CANCELLED"',.
-00010cd0: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
-00010ce0: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
-00010cf0: 7c20 6772 6570 202d 4120 3420 7b6e 616d  | grep -A 4 {nam
-00010d00: 657d 7c20 7365 6420 2d6e 2035 7020 7c20  e}| sed -n 5p | 
-00010d10: 6772 6570 2022 4341 4e43 454c 4c45 4422  grep "CANCELLED"
-00010d20: 272c 0a20 2020 2020 2020 205d 2c0a 2020  ',.        ],.  
-00010d30: 2020 2020 2020 5f53 504f 545f 4341 4e43        _SPOT_CANC
-00010d40: 454c 5f57 4149 542e 666f 726d 6174 286a  EL_WAIT.format(j
-00010d50: 6f62 5f6e 616d 653d 6627 7b6e 616d 657d  ob_name=f'{name}
-00010d60: 2729 2c0a 2020 2020 2020 2020 2320 496e  '),.        # In
-00010d70: 6372 6561 7365 2074 696d 656f 7574 2073  crease timeout s
-00010d80: 696e 6365 2073 6b79 2073 706f 7420 7175  ince sky spot qu
-00010d90: 6575 6520 2d72 2063 616e 2062 6520 626c  eue -r can be bl
-00010da0: 6f63 6b65 6420 6279 206f 7468 6572 2073  ocked by other s
-00010db0: 706f 7420 7465 7374 732e 0a20 2020 2020  pot tests..     
-00010dc0: 2020 2074 696d 656f 7574 3d33 3020 2a20     timeout=30 * 
-00010dd0: 3630 2c0a 2020 2020 290a 2020 2020 7275  60,.    ).    ru
-00010de0: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
-00010df0: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
-00010e00: 6e6f 5f6c 616d 6264 615f 636c 6f75 6420  no_lambda_cloud 
-00010e10: 2023 204c 616d 6264 6120 436c 6f75 6420   # Lambda Cloud 
-00010e20: 646f 6573 206e 6f74 2073 7570 706f 7274  does not support
-00010e30: 2073 706f 7420 696e 7374 616e 6365 730a   spot instances.
-00010e40: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
-00010e50: 6962 6d20 2023 2049 424d 2043 6c6f 7564  ibm  # IBM Cloud
-00010e60: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
-00010e70: 7420 7370 6f74 2069 6e73 7461 6e63 6573  t spot instances
-00010e80: 0a40 7079 7465 7374 2e6d 6172 6b2e 6e6f  .@pytest.mark.no
-00010e90: 5f73 6370 2020 2320 5343 5020 646f 6573  _scp  # SCP does
-00010ea0: 206e 6f74 2073 7570 706f 7274 2073 706f   not support spo
-00010eb0: 7420 696e 7374 616e 6365 730a 4070 7974  t instances.@pyt
-00010ec0: 6573 742e 6d61 726b 2e6d 616e 6167 6564  est.mark.managed
-00010ed0: 5f73 706f 740a 6465 6620 7465 7374 5f73  _spot.def test_s
-00010ee0: 706f 745f 6661 696c 6564 5f73 6574 7570  pot_failed_setup
-00010ef0: 2867 656e 6572 6963 5f63 6c6f 7564 3a20  (generic_cloud: 
-00010f00: 7374 7229 3a0a 2020 2020 2222 2254 6573  str):.    """Tes
-00010f10: 7420 6d61 6e61 6765 6420 7370 6f74 206a  t managed spot j
-00010f20: 6f62 2077 6974 6820 6661 696c 6564 2073  ob with failed s
-00010f30: 6574 7570 2e22 2222 0a20 2020 206e 616d  etup.""".    nam
-00010f40: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
-00010f50: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
-00010f60: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
-00010f70: 2027 7370 6f74 5f66 6169 6c65 645f 7365   'spot_failed_se
-00010f80: 7475 7027 2c0a 2020 2020 2020 2020 5b0a  tup',.        [.
-00010f90: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-00010fa0: 7920 7370 6f74 206c 6175 6e63 6820 2d6e  y spot launch -n
-00010fb0: 207b 6e61 6d65 7d20 2d2d 636c 6f75 6420   {name} --cloud 
-00010fc0: 7b67 656e 6572 6963 5f63 6c6f 7564 7d20  {generic_cloud} 
-00010fd0: 2d79 202d 6420 7465 7374 732f 7465 7374  -y -d tests/test
-00010fe0: 5f79 616d 6c73 2f66 6169 6c65 645f 7365  _yamls/failed_se
-00010ff0: 7475 702e 7961 6d6c 272c 0a20 2020 2020  tup.yaml',.     
-00011000: 2020 2020 2020 2027 736c 6565 7020 3333         'sleep 33
-00011010: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
-00011020: 2320 4d61 6b65 2073 7572 6520 7468 6520  # Make sure the 
-00011030: 6a6f 6220 6661 696c 6564 2071 7569 636b  job failed quick
-00011040: 6c79 2e0a 2020 2020 2020 2020 2020 2020  ly..            
-00011050: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
-00011060: 4149 547d 207c 2067 7265 7020 7b6e 616d  AIT} | grep {nam
-00011070: 657d 207c 2068 6561 6420 2d6e 3120 7c20  e} | head -n1 | 
-00011080: 6772 6570 2022 4641 494c 4544 5f53 4554  grep "FAILED_SET
-00011090: 5550 2227 2c0a 2020 2020 2020 2020 5d2c  UP"',.        ],
-000110a0: 0a20 2020 2020 2020 205f 5350 4f54 5f43  .        _SPOT_C
-000110b0: 414e 4345 4c5f 5741 4954 2e66 6f72 6d61  ANCEL_WAIT.forma
-000110c0: 7428 6a6f 625f 6e61 6d65 3d6e 616d 6529  t(job_name=name)
-000110d0: 2c0a 2020 2020 2020 2020 2320 496e 6372  ,.        # Incr
-000110e0: 6561 7365 2074 696d 656f 7574 2073 696e  ease timeout sin
-000110f0: 6365 2073 6b79 2073 706f 7420 7175 6575  ce sky spot queu
-00011100: 6520 2d72 2063 616e 2062 6520 626c 6f63  e -r can be bloc
-00011110: 6b65 6420 6279 206f 7468 6572 2073 706f  ked by other spo
-00011120: 7420 7465 7374 732e 0a20 2020 2020 2020  t tests..       
-00011130: 2074 696d 656f 7574 3d32 3020 2a20 3630   timeout=20 * 60
-00011140: 2c0a 2020 2020 290a 2020 2020 7275 6e5f  ,.    ).    run_
-00011150: 6f6e 655f 7465 7374 2874 6573 7429 0a0a  one_test(test)..
-00011160: 0a40 7079 7465 7374 2e6d 6172 6b2e 6e6f  .@pytest.mark.no
-00011170: 5f6c 616d 6264 615f 636c 6f75 6420 2023  _lambda_cloud  #
-00011180: 204c 616d 6264 6120 436c 6f75 6420 646f   Lambda Cloud do
-00011190: 6573 206e 6f74 2073 7570 706f 7274 2073  es not support s
-000111a0: 706f 7420 696e 7374 616e 6365 730a 4070  pot instances.@p
-000111b0: 7974 6573 742e 6d61 726b 2e6e 6f5f 6962  ytest.mark.no_ib
-000111c0: 6d20 2023 2049 424d 2043 6c6f 7564 2064  m  # IBM Cloud d
-000111d0: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
-000111e0: 7370 6f74 2069 6e73 7461 6e63 6573 0a40  spot instances.@
-000111f0: 7079 7465 7374 2e6d 6172 6b2e 6e6f 5f73  pytest.mark.no_s
-00011200: 6370 2020 2320 5343 5020 646f 6573 206e  cp  # SCP does n
-00011210: 6f74 2073 7570 706f 7274 2073 706f 7420  ot support spot 
-00011220: 696e 7374 616e 6365 730a 4070 7974 6573  instances.@pytes
-00011230: 742e 6d61 726b 2e6d 616e 6167 6564 5f73  t.mark.managed_s
-00011240: 706f 740a 6465 6620 7465 7374 5f73 706f  pot.def test_spo
-00011250: 745f 7069 7065 6c69 6e65 5f66 6169 6c65  t_pipeline_faile
-00011260: 645f 7365 7475 7028 6765 6e65 7269 635f  d_setup(generic_
-00011270: 636c 6f75 643a 2073 7472 293a 0a20 2020  cloud: str):.   
-00011280: 2022 2222 5465 7374 206d 616e 6167 6564   """Test managed
-00011290: 2073 706f 7420 6a6f 6220 7769 7468 2066   spot job with f
-000112a0: 6169 6c65 6420 7365 7475 7020 666f 7220  ailed setup for 
-000112b0: 6120 7069 7065 6c69 6e65 2e22 2222 0a20  a pipeline.""". 
-000112c0: 2020 206e 616d 6520 3d20 5f67 6574 5f63     name = _get_c
-000112d0: 6c75 7374 6572 5f6e 616d 6528 290a 2020  luster_name().  
-000112e0: 2020 7465 7374 203d 2054 6573 7428 0a20    test = Test(. 
-000112f0: 2020 2020 2020 2027 7370 6f74 5f70 6970         'spot_pip
-00011300: 656c 696e 655f 6661 696c 6564 5f73 6574  eline_failed_set
-00011310: 7570 272c 0a20 2020 2020 2020 205b 0a20  up',.        [. 
-00011320: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-00011330: 2073 706f 7420 6c61 756e 6368 202d 6e20   spot launch -n 
-00011340: 7b6e 616d 657d 202d 7920 2d64 2074 6573  {name} -y -d tes
-00011350: 7473 2f74 6573 745f 7961 6d6c 732f 6661  ts/test_yamls/fa
-00011360: 696c 6564 5f73 6574 7570 5f70 6970 656c  iled_setup_pipel
-00011370: 696e 652e 7961 6d6c 272c 0a20 2020 2020  ine.yaml',.     
-00011380: 2020 2020 2020 2027 736c 6565 7020 3830         'sleep 80
-00011390: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
-000113a0: 2320 4d61 6b65 2073 7572 6520 7468 6520  # Make sure the 
-000113b0: 6a6f 6220 6661 696c 6564 2071 7569 636b  job failed quick
-000113c0: 6c79 2e0a 2020 2020 2020 2020 2020 2020  ly..            
-000113d0: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
-000113e0: 4149 547d 207c 2067 7265 7020 7b6e 616d  AIT} | grep {nam
-000113f0: 657d 207c 2068 6561 6420 2d6e 3120 7c20  e} | head -n1 | 
-00011400: 6772 6570 2022 4641 494c 4544 5f53 4554  grep "FAILED_SET
-00011410: 5550 2227 2c0a 2020 2020 2020 2020 2020  UP"',.          
-00011420: 2020 2320 5461 736b 2030 2073 686f 756c    # Task 0 shoul
-00011430: 6420 6265 2053 5543 4345 4544 4544 2e0a  d be SUCCEEDED..
-00011440: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
-00011450: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
-00011460: 207c 2067 7265 7020 2d41 2034 207b 6e61   | grep -A 4 {na
-00011470: 6d65 7d7c 2073 6564 202d 6e20 3270 207c  me}| sed -n 2p |
-00011480: 2067 7265 7020 2253 5543 4345 4544 4544   grep "SUCCEEDED
-00011490: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-000114a0: 2320 5461 736b 2031 2073 686f 756c 6420  # Task 1 should 
-000114b0: 6265 2046 4149 4c45 445f 5345 5455 502e  be FAILED_SETUP.
-000114c0: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
-000114d0: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
-000114e0: 7d20 7c20 6772 6570 202d 4120 3420 7b6e  } | grep -A 4 {n
-000114f0: 616d 657d 7c20 7365 6420 2d6e 2033 7020  ame}| sed -n 3p 
-00011500: 7c20 6772 6570 2022 4641 494c 4544 5f53  | grep "FAILED_S
-00011510: 4554 5550 2227 2c0a 2020 2020 2020 2020  ETUP"',.        
-00011520: 2020 2020 2320 5461 736b 2032 2073 686f      # Task 2 sho
-00011530: 756c 6420 6265 2043 414e 4345 4c4c 4544  uld be CANCELLED
-00011540: 2e0a 2020 2020 2020 2020 2020 2020 6627  ..            f'
-00011550: 7b5f 5350 4f54 5f51 5545 5545 5f57 4149  {_SPOT_QUEUE_WAI
-00011560: 547d 207c 2067 7265 7020 2d41 2034 207b  T} | grep -A 4 {
-00011570: 6e61 6d65 7d7c 2073 6564 202d 6e20 3470  name}| sed -n 4p
-00011580: 207c 2067 7265 7020 2243 414e 4345 4c4c   | grep "CANCELL
-00011590: 4544 2227 2c0a 2020 2020 2020 2020 2020  ED"',.          
-000115a0: 2020 2320 5461 736b 2033 2073 686f 756c    # Task 3 shoul
-000115b0: 6420 6265 2043 414e 4345 4c4c 4544 2e0a  d be CANCELLED..
-000115c0: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
-000115d0: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
-000115e0: 207c 2067 7265 7020 2d41 2034 207b 6e61   | grep -A 4 {na
-000115f0: 6d65 7d7c 2073 6564 202d 6e20 3570 207c  me}| sed -n 5p |
-00011600: 2067 7265 7020 2243 414e 4345 4c4c 4544   grep "CANCELLED
-00011610: 2227 2c0a 2020 2020 2020 2020 5d2c 0a20  "',.        ],. 
-00011620: 2020 2020 2020 205f 5350 4f54 5f43 414e         _SPOT_CAN
-00011630: 4345 4c5f 5741 4954 2e66 6f72 6d61 7428  CEL_WAIT.format(
-00011640: 6a6f 625f 6e61 6d65 3d6e 616d 6529 2c0a  job_name=name),.
-00011650: 2020 2020 2020 2020 2320 496e 6372 6561          # Increa
-00011660: 7365 2074 696d 656f 7574 2073 696e 6365  se timeout since
-00011670: 2073 6b79 2073 706f 7420 7175 6575 6520   sky spot queue 
-00011680: 2d72 2063 616e 2062 6520 626c 6f63 6b65  -r can be blocke
-00011690: 6420 6279 206f 7468 6572 2073 706f 7420  d by other spot 
-000116a0: 7465 7374 732e 0a20 2020 2020 2020 2074  tests..        t
-000116b0: 696d 656f 7574 3d33 3020 2a20 3630 2c0a  imeout=30 * 60,.
-000116c0: 2020 2020 290a 2020 2020 7275 6e5f 6f6e      ).    run_on
-000116d0: 655f 7465 7374 2874 6573 7429 0a0a 0a23  e_test(test)...#
-000116e0: 202d 2d2d 2d2d 2d2d 2d2d 2d20 5465 7374   ---------- Test
-000116f0: 696e 6720 6d61 6e61 6765 6420 7370 6f74  ing managed spot
-00011700: 2072 6563 6f76 6572 7920 2d2d 2d2d 2d2d   recovery ------
-00011710: 2d2d 2d2d 0a0a 0a40 7079 7465 7374 2e6d  ----...@pytest.m
-00011720: 6172 6b2e 6177 730a 4070 7974 6573 742e  ark.aws.@pytest.
-00011730: 6d61 726b 2e6d 616e 6167 6564 5f73 706f  mark.managed_spo
-00011740: 740a 6465 6620 7465 7374 5f73 706f 745f  t.def test_spot_
-00011750: 7265 636f 7665 7279 5f61 7773 2861 7773  recovery_aws(aws
-00011760: 5f63 6f6e 6669 675f 7265 6769 6f6e 293a  _config_region):
-00011770: 0a20 2020 2022 2222 5465 7374 206d 616e  .    """Test man
-00011780: 6167 6564 2073 706f 7420 7265 636f 7665  aged spot recove
-00011790: 7279 2e22 2222 0a20 2020 206e 616d 6520  ry.""".    name 
-000117a0: 3d20 5f67 6574 5f63 6c75 7374 6572 5f6e  = _get_cluster_n
-000117b0: 616d 6528 290a 2020 2020 7265 6769 6f6e  ame().    region
-000117c0: 203d 2061 7773 5f63 6f6e 6669 675f 7265   = aws_config_re
-000117d0: 6769 6f6e 0a20 2020 2074 6573 7420 3d20  gion.    test = 
-000117e0: 5465 7374 280a 2020 2020 2020 2020 2773  Test(.        's
-000117f0: 706f 745f 7265 636f 7665 7279 5f61 7773  pot_recovery_aws
-00011800: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
-00011810: 2020 2020 2020 2020 2066 2773 6b79 2073           f'sky s
-00011820: 706f 7420 6c61 756e 6368 202d 2d63 6c6f  pot launch --clo
-00011830: 7564 2061 7773 202d 2d72 6567 696f 6e20  ud aws --region 
-00011840: 7b72 6567 696f 6e7d 202d 6e20 7b6e 616d  {region} -n {nam
-00011850: 657d 2022 6563 686f 2053 4b59 5049 4c4f  e} "echo SKYPILO
-00011860: 545f 5441 534b 5f49 443a 205c 2453 4b59  T_TASK_ID: \$SKY
-00011870: 5049 4c4f 545f 5441 534b 5f49 443b 2073  PILOT_TASK_ID; s
-00011880: 6c65 6570 2031 3830 3022 2020 2d79 202d  leep 1800"  -y -
-00011890: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
-000118a0: 2773 6c65 6570 2033 3630 272c 0a20 2020  'sleep 360',.   
-000118b0: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
-000118c0: 545f 5155 4555 455f 5741 4954 7d7c 2067  T_QUEUE_WAIT}| g
-000118d0: 7265 7020 7b6e 616d 657d 207c 2068 6561  rep {name} | hea
-000118e0: 6420 2d6e 3120 7c20 6772 6570 2022 5255  d -n1 | grep "RU
-000118f0: 4e4e 494e 4722 272c 0a20 2020 2020 2020  NNING"',.       
-00011900: 2020 2020 2066 2752 554e 5f49 443d 2428       f'RUN_ID=$(
-00011910: 736b 7920 7370 6f74 206c 6f67 7320 2d6e  sky spot logs -n
-00011920: 207b 6e61 6d65 7d20 2d2d 6e6f 2d66 6f6c   {name} --no-fol
-00011930: 6c6f 7720 7c20 6772 6570 2053 4b59 5049  low | grep SKYPI
-00011940: 4c4f 545f 5441 534b 5f49 4420 7c20 6375  LOT_TASK_ID | cu
-00011950: 7420 2d64 3a20 2d66 3229 3b20 6563 686f  t -d: -f2); echo
-00011960: 2022 2452 554e 5f49 4422 207c 2074 6565   "$RUN_ID" | tee
-00011970: 202f 746d 702f 7b6e 616d 657d 2d72 756e   /tmp/{name}-run
-00011980: 2d69 6427 2c0a 2020 2020 2020 2020 2020  -id',.          
-00011990: 2020 2320 5465 726d 696e 6174 6520 7468    # Terminate th
-000119a0: 6520 636c 7573 7465 7220 6d61 6e75 616c  e cluster manual
-000119b0: 6c79 2e0a 2020 2020 2020 2020 2020 2020  ly..            
-000119c0: 2866 2761 7773 2065 6332 2074 6572 6d69  (f'aws ec2 termi
-000119d0: 6e61 7465 2d69 6e73 7461 6e63 6573 202d  nate-instances -
-000119e0: 2d72 6567 696f 6e20 7b72 6567 696f 6e7d  -region {region}
-000119f0: 202d 2d69 6e73 7461 6e63 652d 6964 7320   --instance-ids 
-00011a00: 2428 270a 2020 2020 2020 2020 2020 2020  $('.            
-00011a10: 2066 2761 7773 2065 6332 2064 6573 6372   f'aws ec2 descr
-00011a20: 6962 652d 696e 7374 616e 6365 7320 2d2d  ibe-instances --
-00011a30: 7265 6769 6f6e 207b 7265 6769 6f6e 7d20  region {region} 
-00011a40: 270a 2020 2020 2020 2020 2020 2020 2066  '.             f
-00011a50: 272d 2d66 696c 7465 7273 204e 616d 653d  '--filters Name=
-00011a60: 7461 673a 7261 792d 636c 7573 7465 722d  tag:ray-cluster-
-00011a70: 6e61 6d65 2c56 616c 7565 733d 7b6e 616d  name,Values={nam
-00011a80: 657d 2a20 270a 2020 2020 2020 2020 2020  e}* '.          
-00011a90: 2020 2066 272d 2d71 7565 7279 2052 6573     f'--query Res
-00011aa0: 6572 7661 7469 6f6e 735b 5d2e 496e 7374  ervations[].Inst
-00011ab0: 616e 6365 735b 5d2e 496e 7374 616e 6365  ances[].Instance
-00011ac0: 4964 2027 0a20 2020 2020 2020 2020 2020  Id '.           
-00011ad0: 2020 272d 2d6f 7574 7075 7420 7465 7874    '--output text
-00011ae0: 2927 292c 0a20 2020 2020 2020 2020 2020  )'),.           
-00011af0: 2027 736c 6565 7020 3130 3027 2c0a 2020   'sleep 100',.  
-00011b00: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
-00011b10: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
-00011b20: 6772 6570 207b 6e61 6d65 7d20 7c20 6865  grep {name} | he
-00011b30: 6164 202d 6e31 207c 2067 7265 7020 2252  ad -n1 | grep "R
-00011b40: 4543 4f56 4552 494e 4722 272c 0a20 2020  ECOVERING"',.   
-00011b50: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
-00011b60: 3230 3027 2c0a 2020 2020 2020 2020 2020  200',.          
-00011b70: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
-00011b80: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
-00011b90: 6d65 7d20 7c20 6865 6164 202d 6e31 207c  me} | head -n1 |
-00011ba0: 2067 7265 7020 2252 554e 4e49 4e47 2227   grep "RUNNING"'
-00011bb0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-00011bc0: 5255 4e5f 4944 3d24 2863 6174 202f 746d  RUN_ID=$(cat /tm
-00011bd0: 702f 7b6e 616d 657d 2d72 756e 2d69 6429  p/{name}-run-id)
-00011be0: 3b20 6563 686f 2024 5255 4e5f 4944 3b20  ; echo $RUN_ID; 
-00011bf0: 736b 7920 7370 6f74 206c 6f67 7320 2d6e  sky spot logs -n
-00011c00: 207b 6e61 6d65 7d20 2d2d 6e6f 2d66 6f6c   {name} --no-fol
-00011c10: 6c6f 7720 7c20 6772 6570 2053 4b59 5049  low | grep SKYPI
-00011c20: 4c4f 545f 5441 534b 5f49 4420 7c20 6772  LOT_TASK_ID | gr
-00011c30: 6570 2022 2452 554e 5f49 4422 272c 0a20  ep "$RUN_ID"',. 
-00011c40: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-00011c50: 2020 5f53 504f 545f 4341 4e43 454c 5f57    _SPOT_CANCEL_W
-00011c60: 4149 542e 666f 726d 6174 286a 6f62 5f6e  AIT.format(job_n
-00011c70: 616d 653d 6e61 6d65 292c 0a20 2020 2020  ame=name),.     
-00011c80: 2020 2074 696d 656f 7574 3d32 3520 2a20     timeout=25 * 
-00011c90: 3630 2c0a 2020 2020 290a 2020 2020 7275  60,.    ).    ru
-00011ca0: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
-00011cb0: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
-00011cc0: 6763 700a 4070 7974 6573 742e 6d61 726b  gcp.@pytest.mark
-00011cd0: 2e6d 616e 6167 6564 5f73 706f 740a 6465  .managed_spot.de
-00011ce0: 6620 7465 7374 5f73 706f 745f 7265 636f  f test_spot_reco
-00011cf0: 7665 7279 5f67 6370 2829 3a0a 2020 2020  very_gcp():.    
-00011d00: 2222 2254 6573 7420 6d61 6e61 6765 6420  """Test managed 
-00011d10: 7370 6f74 2072 6563 6f76 6572 792e 2222  spot recovery.""
-00011d20: 220a 2020 2020 6e61 6d65 203d 205f 6765  ".    name = _ge
-00011d30: 745f 636c 7573 7465 725f 6e61 6d65 2829  t_cluster_name()
-00011d40: 0a20 2020 207a 6f6e 6520 3d20 2775 732d  .    zone = 'us-
-00011d50: 6561 7374 342d 6227 0a20 2020 2071 7565  east4-b'.    que
-00011d60: 7279 5f63 6d64 203d 2028 6627 6763 6c6f  ry_cmd = (f'gclo
-00011d70: 7564 2063 6f6d 7075 7465 2069 6e73 7461  ud compute insta
-00011d80: 6e63 6573 206c 6973 7420 2d2d 6669 6c74  nces list --filt
-00011d90: 6572 3d27 0a20 2020 2020 2020 2020 2020  er='.           
-00011da0: 2020 2020 2020 6627 2228 6c61 6265 6c73        f'"(labels
-00011db0: 2e72 6179 2d63 6c75 7374 6572 2d6e 616d  .ray-cluster-nam
-00011dc0: 653a 7b6e 616d 657d 2922 2027 0a20 2020  e:{name})" '.   
-00011dd0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-00011de0: 2d2d 7a6f 6e65 733d 7b7a 6f6e 657d 202d  --zones={zone} -
-00011df0: 2d66 6f72 6d61 743d 2276 616c 7565 286e  -format="value(n
-00011e00: 616d 6529 2227 290a 2020 2020 7465 726d  ame)"').    term
-00011e10: 696e 6174 655f 636d 6420 3d20 2866 2767  inate_cmd = (f'g
-00011e20: 636c 6f75 6420 636f 6d70 7574 6520 696e  cloud compute in
-00011e30: 7374 616e 6365 7320 6465 6c65 7465 202d  stances delete -
-00011e40: 2d7a 6f6e 653d 7b7a 6f6e 657d 270a 2020  -zone={zone}'.  
-00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e60: 2020 2066 2720 2d2d 7175 6965 7420 2428     f' --quiet $(
-00011e70: 7b71 7565 7279 5f63 6d64 7d29 2729 0a20  {query_cmd})'). 
-00011e80: 2020 2074 6573 7420 3d20 5465 7374 280a     test = Test(.
-00011e90: 2020 2020 2020 2020 2773 706f 745f 7265          'spot_re
-00011ea0: 636f 7665 7279 5f67 6370 272c 0a20 2020  covery_gcp',.   
-00011eb0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-00011ec0: 2020 2066 2773 6b79 2073 706f 7420 6c61     f'sky spot la
-00011ed0: 756e 6368 202d 2d63 6c6f 7564 2067 6370  unch --cloud gcp
-00011ee0: 202d 2d7a 6f6e 6520 7b7a 6f6e 657d 202d   --zone {zone} -
-00011ef0: 6e20 7b6e 616d 657d 2022 6563 686f 2053  n {name} "echo S
-00011f00: 4b59 5049 4c4f 545f 5441 534b 5f49 443a  KYPILOT_TASK_ID:
-00011f10: 205c 2453 4b59 5049 4c4f 545f 5441 534b   \$SKYPILOT_TASK
-00011f20: 5f49 443b 2073 6c65 6570 2031 3830 3022  _ID; sleep 1800"
-00011f30: 2020 2d79 202d 6427 2c0a 2020 2020 2020    -y -d',.      
-00011f40: 2020 2020 2020 2773 6c65 6570 2033 3630        'sleep 360
-00011f50: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-00011f60: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
-00011f70: 4954 7d7c 2067 7265 7020 7b6e 616d 657d  IT}| grep {name}
-00011f80: 207c 2068 6561 6420 2d6e 3120 7c20 6772   | head -n1 | gr
-00011f90: 6570 2022 5255 4e4e 494e 4722 272c 0a20  ep "RUNNING"',. 
-00011fa0: 2020 2020 2020 2020 2020 2066 2752 554e             f'RUN
-00011fb0: 5f49 443d 2428 736b 7920 7370 6f74 206c  _ID=$(sky spot l
-00011fc0: 6f67 7320 2d6e 207b 6e61 6d65 7d20 2d2d  ogs -n {name} --
-00011fd0: 6e6f 2d66 6f6c 6c6f 7720 7c20 6772 6570  no-follow | grep
-00011fe0: 2053 4b59 5049 4c4f 545f 5441 534b 5f49   SKYPILOT_TASK_I
-00011ff0: 4420 7c20 6375 7420 2d64 3a20 2d66 3229  D | cut -d: -f2)
-00012000: 3b20 6563 686f 2022 2452 554e 5f49 4422  ; echo "$RUN_ID"
-00012010: 207c 2074 6565 202f 746d 702f 7b6e 616d   | tee /tmp/{nam
-00012020: 657d 2d72 756e 2d69 6427 2c0a 2020 2020  e}-run-id',.    
-00012030: 2020 2020 2020 2020 2320 5465 726d 696e          # Termin
-00012040: 6174 6520 7468 6520 636c 7573 7465 7220  ate the cluster 
-00012050: 6d61 6e75 616c 6c79 2e0a 2020 2020 2020  manually..      
-00012060: 2020 2020 2020 7465 726d 696e 6174 655f        terminate_
-00012070: 636d 642c 0a20 2020 2020 2020 2020 2020  cmd,.           
-00012080: 2027 736c 6565 7020 3130 3027 2c0a 2020   'sleep 100',.  
-00012090: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
-000120a0: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
-000120b0: 6772 6570 207b 6e61 6d65 7d20 7c20 6865  grep {name} | he
-000120c0: 6164 202d 6e31 207c 2067 7265 7020 2252  ad -n1 | grep "R
-000120d0: 4543 4f56 4552 494e 4722 272c 0a20 2020  ECOVERING"',.   
-000120e0: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
-000120f0: 3230 3027 2c0a 2020 2020 2020 2020 2020  200',.          
-00012100: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
-00012110: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
-00012120: 6d65 7d20 7c20 6865 6164 202d 6e31 207c  me} | head -n1 |
-00012130: 2067 7265 7020 2252 554e 4e49 4e47 2227   grep "RUNNING"'
-00012140: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-00012150: 5255 4e5f 4944 3d24 2863 6174 202f 746d  RUN_ID=$(cat /tm
-00012160: 702f 7b6e 616d 657d 2d72 756e 2d69 6429  p/{name}-run-id)
-00012170: 3b20 6563 686f 2024 5255 4e5f 4944 3b20  ; echo $RUN_ID; 
-00012180: 736b 7920 7370 6f74 206c 6f67 7320 2d6e  sky spot logs -n
-00012190: 207b 6e61 6d65 7d20 2d2d 6e6f 2d66 6f6c   {name} --no-fol
-000121a0: 6c6f 7720 7c20 6772 6570 2053 4b59 5049  low | grep SKYPI
-000121b0: 4c4f 545f 5441 534b 5f49 443a 207c 2067  LOT_TASK_ID: | g
-000121c0: 7265 7020 2224 5255 4e5f 4944 2227 2c0a  rep "$RUN_ID"',.
-000121d0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-000121e0: 2020 205f 5350 4f54 5f43 414e 4345 4c5f     _SPOT_CANCEL_
-000121f0: 5741 4954 2e66 6f72 6d61 7428 6a6f 625f  WAIT.format(job_
-00012200: 6e61 6d65 3d6e 616d 6529 2c0a 2020 2020  name=name),.    
-00012210: 2020 2020 7469 6d65 6f75 743d 3235 202a      timeout=25 *
-00012220: 2036 302c 0a20 2020 2029 0a20 2020 2072   60,.    ).    r
-00012230: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
-00012240: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
-00012250: 2e61 7773 0a40 7079 7465 7374 2e6d 6172  .aws.@pytest.mar
-00012260: 6b2e 6d61 6e61 6765 645f 7370 6f74 0a64  k.managed_spot.d
-00012270: 6566 2074 6573 745f 7370 6f74 5f70 6970  ef test_spot_pip
-00012280: 656c 696e 655f 7265 636f 7665 7279 5f61  eline_recovery_a
-00012290: 7773 2861 7773 5f63 6f6e 6669 675f 7265  ws(aws_config_re
-000122a0: 6769 6f6e 293a 0a20 2020 2022 2222 5465  gion):.    """Te
-000122b0: 7374 206d 616e 6167 6564 2073 706f 7420  st managed spot 
-000122c0: 7265 636f 7665 7279 2066 6f72 2061 2070  recovery for a p
-000122d0: 6970 656c 696e 652e 2222 220a 2020 2020  ipeline.""".    
-000122e0: 6e61 6d65 203d 205f 6765 745f 636c 7573  name = _get_clus
-000122f0: 7465 725f 6e61 6d65 2829 0a20 2020 2072  ter_name().    r
-00012300: 6567 696f 6e20 3d20 6177 735f 636f 6e66  egion = aws_conf
-00012310: 6967 5f72 6567 696f 6e0a 2020 2020 6966  ig_region.    if
-00012320: 2072 6567 696f 6e20 213d 2027 7573 2d77   region != 'us-w
-00012330: 6573 742d 3227 3a0a 2020 2020 2020 2020  est-2':.        
-00012340: 7079 7465 7374 2e73 6b69 7028 274f 6e6c  pytest.skip('Onl
-00012350: 7920 7275 6e20 7370 6f74 2070 6970 656c  y run spot pipel
-00012360: 696e 6520 7265 636f 7665 7279 2074 6573  ine recovery tes
-00012370: 7420 696e 2075 732d 7765 7374 2d32 2729  t in us-west-2')
-00012380: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
-00012390: 280a 2020 2020 2020 2020 2773 706f 745f  (.        'spot_
-000123a0: 7069 7065 6c69 6e65 5f72 6563 6f76 6572  pipeline_recover
-000123b0: 795f 6177 7327 2c0a 2020 2020 2020 2020  y_aws',.        
-000123c0: 5b0a 2020 2020 2020 2020 2020 2020 6627  [.            f'
-000123d0: 736b 7920 7370 6f74 206c 6175 6e63 6820  sky spot launch 
-000123e0: 2d6e 207b 6e61 6d65 7d20 7465 7374 732f  -n {name} tests/
-000123f0: 7465 7374 5f79 616d 6c73 2f70 6970 656c  test_yamls/pipel
-00012400: 696e 655f 6177 732e 7961 6d6c 2020 2d79  ine_aws.yaml  -y
-00012410: 202d 6427 2c0a 2020 2020 2020 2020 2020   -d',.          
-00012420: 2020 2773 6c65 6570 2034 3030 272c 0a20    'sleep 400',. 
-00012430: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
-00012440: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
-00012450: 2067 7265 7020 7b6e 616d 657d 207c 2068   grep {name} | h
-00012460: 6561 6420 2d6e 3120 7c20 6772 6570 2022  ead -n1 | grep "
-00012470: 5255 4e4e 494e 4722 272c 0a20 2020 2020  RUNNING"',.     
-00012480: 2020 2020 2020 2066 2752 554e 5f49 443d         f'RUN_ID=
-00012490: 2428 736b 7920 7370 6f74 206c 6f67 7320  $(sky spot logs 
-000124a0: 2d6e 207b 6e61 6d65 7d20 2d2d 6e6f 2d66  -n {name} --no-f
-000124b0: 6f6c 6c6f 7720 7c20 6772 6570 2053 4b59  ollow | grep SKY
-000124c0: 5049 4c4f 545f 5441 534b 5f49 443a 207c  PILOT_TASK_ID: |
-000124d0: 2063 7574 202d 643a 202d 6632 293b 2065   cut -d: -f2); e
-000124e0: 6368 6f20 2224 5255 4e5f 4944 2220 7c20  cho "$RUN_ID" | 
-000124f0: 7465 6520 2f74 6d70 2f7b 6e61 6d65 7d2d  tee /tmp/{name}-
-00012500: 7275 6e2d 6964 272c 0a20 2020 2020 2020  run-id',.       
-00012510: 2020 2020 2066 2752 554e 5f49 4453 3d24       f'RUN_IDS=$
-00012520: 2873 6b79 2073 706f 7420 6c6f 6773 202d  (sky spot logs -
-00012530: 6e20 7b6e 616d 657d 202d 2d6e 6f2d 666f  n {name} --no-fo
-00012540: 6c6c 6f77 207c 2067 7265 7020 2d41 2034  llow | grep -A 4
-00012550: 2053 4b59 5049 4c4f 545f 5441 534b 5f49   SKYPILOT_TASK_I
-00012560: 4453 207c 2063 7574 202d 6422 2922 202d  DS | cut -d")" -
-00012570: 6632 293b 2065 6368 6f20 2224 5255 4e5f  f2); echo "$RUN_
-00012580: 4944 5322 207c 2074 6565 202f 746d 702f  IDS" | tee /tmp/
-00012590: 7b6e 616d 657d 2d72 756e 2d69 6473 272c  {name}-run-ids',
-000125a0: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
-000125b0: 6572 6d69 6e61 7465 2074 6865 2063 6c75  erminate the clu
-000125c0: 7374 6572 206d 616e 7561 6c6c 792e 0a20  ster manually.. 
-000125d0: 2020 2020 2020 2020 2020 2023 2054 6865             # The
-000125e0: 2060 6361 7420 2e2e 2e7c 2072 6576 6020   `cat ...| rev` 
-000125f0: 6973 2074 6f20 7265 7472 6965 7665 2074  is to retrieve t
-00012600: 6865 206a 6f62 5f69 6420 6672 6f6d 2074  he job_id from t
-00012610: 6865 0a20 2020 2020 2020 2020 2020 2023  he.            #
-00012620: 2053 4b59 5049 4c4f 545f 5441 534b 5f49   SKYPILOT_TASK_I
-00012630: 442c 2077 6869 6368 2067 6574 7320 7468  D, which gets th
-00012640: 6520 7365 636f 6e64 2074 6f20 6c61 7374  e second to last
-00012650: 2066 6965 6c64 0a20 2020 2020 2020 2020   field.         
-00012660: 2020 2023 2073 6570 6172 6174 6564 2062     # separated b
-00012670: 7920 602d 602e 0a20 2020 2020 2020 2020  y `-`..         
-00012680: 2020 2028 6627 5350 4f54 5f4a 4f42 5f49     (f'SPOT_JOB_I
-00012690: 443d 6063 6174 202f 746d 702f 7b6e 616d  D=`cat /tmp/{nam
-000126a0: 657d 2d72 756e 2d69 6420 7c20 7265 7620  e}-run-id | rev 
-000126b0: 7c20 270a 2020 2020 2020 2020 2020 2020  | '.            
-000126c0: 2027 6375 7420 2d64 5c27 2d5c 2720 2d66   'cut -d\'-\' -f
-000126d0: 3220 7c20 7265 7660 3b27 0a20 2020 2020  2 | rev`;'.     
-000126e0: 2020 2020 2020 2020 6627 6177 7320 6563          f'aws ec
-000126f0: 3220 7465 726d 696e 6174 652d 696e 7374  2 terminate-inst
-00012700: 616e 6365 7320 2d2d 7265 6769 6f6e 207b  ances --region {
-00012710: 7265 6769 6f6e 7d20 2d2d 696e 7374 616e  region} --instan
-00012720: 6365 2d69 6473 2024 2827 0a20 2020 2020  ce-ids $('.     
-00012730: 2020 2020 2020 2020 6627 6177 7320 6563          f'aws ec
-00012740: 3220 6465 7363 7269 6265 2d69 6e73 7461  2 describe-insta
-00012750: 6e63 6573 202d 2d72 6567 696f 6e20 7b72  nces --region {r
-00012760: 6567 696f 6e7d 2027 0a20 2020 2020 2020  egion} '.       
-00012770: 2020 2020 2020 272d 2d66 696c 7465 7273        '--filters
-00012780: 204e 616d 653d 7461 673a 7261 792d 636c   Name=tag:ray-cl
-00012790: 7573 7465 722d 6e61 6d65 2c56 616c 7565  uster-name,Value
-000127a0: 733d 2a2d 247b 5350 4f54 5f4a 4f42 5f49  s=*-${SPOT_JOB_I
-000127b0: 447d 2027 0a20 2020 2020 2020 2020 2020  D} '.           
-000127c0: 2020 6627 2d2d 7175 6572 7920 5265 7365    f'--query Rese
-000127d0: 7276 6174 696f 6e73 5b5d 2e49 6e73 7461  rvations[].Insta
-000127e0: 6e63 6573 5b5d 2e49 6e73 7461 6e63 6549  nces[].InstanceI
-000127f0: 6420 270a 2020 2020 2020 2020 2020 2020  d '.            
-00012800: 2027 2d2d 6f75 7470 7574 2074 6578 7429   '--output text)
-00012810: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00012820: 2773 6c65 6570 2031 3030 272c 0a20 2020  'sleep 100',.   
-00012830: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
-00012840: 545f 5155 4555 455f 5741 4954 7d7c 2067  T_QUEUE_WAIT}| g
-00012850: 7265 7020 7b6e 616d 657d 207c 2068 6561  rep {name} | hea
-00012860: 6420 2d6e 3120 7c20 6772 6570 2022 5245  d -n1 | grep "RE
-00012870: 434f 5645 5249 4e47 2227 2c0a 2020 2020  COVERING"',.    
-00012880: 2020 2020 2020 2020 2773 6c65 6570 2032          'sleep 2
-00012890: 3030 272c 0a20 2020 2020 2020 2020 2020  00',.           
-000128a0: 2066 277b 5f53 504f 545f 5155 4555 455f   f'{_SPOT_QUEUE_
-000128b0: 5741 4954 7d7c 2067 7265 7020 7b6e 616d  WAIT}| grep {nam
-000128c0: 657d 207c 2068 6561 6420 2d6e 3120 7c20  e} | head -n1 | 
-000128d0: 6772 6570 2022 5255 4e4e 494e 4722 272c  grep "RUNNING"',
-000128e0: 0a20 2020 2020 2020 2020 2020 2066 2752  .            f'R
-000128f0: 554e 5f49 443d 2428 6361 7420 2f74 6d70  UN_ID=$(cat /tmp
-00012900: 2f7b 6e61 6d65 7d2d 7275 6e2d 6964 293b  /{name}-run-id);
-00012910: 2065 6368 6f20 2452 554e 5f49 443b 2073   echo $RUN_ID; s
-00012920: 6b79 2073 706f 7420 6c6f 6773 202d 6e20  ky spot logs -n 
-00012930: 7b6e 616d 657d 202d 2d6e 6f2d 666f 6c6c  {name} --no-foll
-00012940: 6f77 207c 2067 7265 7020 534b 5950 494c  ow | grep SKYPIL
-00012950: 4f54 5f54 4153 4b5f 4944 3a20 7c20 6772  OT_TASK_ID: | gr
-00012960: 6570 2022 2452 554e 5f49 4422 272c 0a20  ep "$RUN_ID"',. 
-00012970: 2020 2020 2020 2020 2020 2066 2752 554e             f'RUN
-00012980: 5f49 4453 3d24 2873 6b79 2073 706f 7420  _IDS=$(sky spot 
-00012990: 6c6f 6773 202d 6e20 7b6e 616d 657d 202d  logs -n {name} -
-000129a0: 2d6e 6f2d 666f 6c6c 6f77 207c 2067 7265  -no-follow | gre
-000129b0: 7020 2d41 2034 2053 4b59 5049 4c4f 545f  p -A 4 SKYPILOT_
-000129c0: 5441 534b 5f49 4453 207c 2063 7574 202d  TASK_IDS | cut -
-000129d0: 6422 2922 202d 6632 293b 2065 6368 6f20  d")" -f2); echo 
-000129e0: 2224 5255 4e5f 4944 5322 207c 2074 6565  "$RUN_IDS" | tee
-000129f0: 202f 746d 702f 7b6e 616d 657d 2d72 756e   /tmp/{name}-run
-00012a00: 2d69 6473 2d6e 6577 272c 0a20 2020 2020  -ids-new',.     
-00012a10: 2020 2020 2020 2066 2764 6966 6620 2f74         f'diff /t
-00012a20: 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d 6964  mp/{name}-run-id
-00012a30: 7320 2f74 6d70 2f7b 6e61 6d65 7d2d 7275  s /tmp/{name}-ru
-00012a40: 6e2d 6964 732d 6e65 7727 2c0a 2020 2020  n-ids-new',.    
-00012a50: 2020 2020 2020 2020 6627 6361 7420 2f74          f'cat /t
-00012a60: 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d 6964  mp/{name}-run-id
-00012a70: 7320 7c20 7365 6420 2d6e 2032 7020 7c20  s | sed -n 2p | 
-00012a80: 6772 6570 2060 6361 7420 2f74 6d70 2f7b  grep `cat /tmp/{
-00012a90: 6e61 6d65 7d2d 7275 6e2d 6964 6027 2c0a  name}-run-id`',.
-00012aa0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00012ab0: 2020 205f 5350 4f54 5f43 414e 4345 4c5f     _SPOT_CANCEL_
-00012ac0: 5741 4954 2e66 6f72 6d61 7428 6a6f 625f  WAIT.format(job_
-00012ad0: 6e61 6d65 3d6e 616d 6529 2c0a 2020 2020  name=name),.    
-00012ae0: 2020 2020 7469 6d65 6f75 743d 3235 202a      timeout=25 *
-00012af0: 2036 302c 0a20 2020 2029 0a20 2020 2072   60,.    ).    r
-00012b00: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
-00012b10: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
-00012b20: 2e67 6370 0a40 7079 7465 7374 2e6d 6172  .gcp.@pytest.mar
-00012b30: 6b2e 6d61 6e61 6765 645f 7370 6f74 0a64  k.managed_spot.d
-00012b40: 6566 2074 6573 745f 7370 6f74 5f70 6970  ef test_spot_pip
-00012b50: 656c 696e 655f 7265 636f 7665 7279 5f67  eline_recovery_g
-00012b60: 6370 2829 3a0a 2020 2020 2222 2254 6573  cp():.    """Tes
-00012b70: 7420 6d61 6e61 6765 6420 7370 6f74 2072  t managed spot r
-00012b80: 6563 6f76 6572 7920 666f 7220 6120 7069  ecovery for a pi
-00012b90: 7065 6c69 6e65 2e22 2222 0a20 2020 206e  peline.""".    n
-00012ba0: 616d 6520 3d20 5f67 6574 5f63 6c75 7374  ame = _get_clust
-00012bb0: 6572 5f6e 616d 6528 290a 2020 2020 7a6f  er_name().    zo
-00012bc0: 6e65 203d 2027 7573 2d65 6173 7434 2d62  ne = 'us-east4-b
-00012bd0: 270a 2020 2020 7175 6572 795f 636d 6420  '.    query_cmd 
-00012be0: 3d20 2827 6763 6c6f 7564 2063 6f6d 7075  = ('gcloud compu
-00012bf0: 7465 2069 6e73 7461 6e63 6573 206c 6973  te instances lis
-00012c00: 7420 2d2d 6669 6c74 6572 3d27 0a20 2020  t --filter='.   
-00012c10: 2020 2020 2020 2020 2020 2020 2020 2722                '"
-00012c20: 286c 6162 656c 732e 7261 792d 636c 7573  (labels.ray-clus
-00012c30: 7465 722d 6e61 6d65 3a2a 2d24 7b53 504f  ter-name:*-${SPO
-00012c40: 545f 4a4f 425f 4944 7d29 2220 270a 2020  T_JOB_ID})" '.  
-00012c50: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00012c60: 272d 2d7a 6f6e 6573 3d7b 7a6f 6e65 7d20  '--zones={zone} 
-00012c70: 2d2d 666f 726d 6174 3d22 7661 6c75 6528  --format="value(
-00012c80: 6e61 6d65 2922 2729 0a20 2020 2074 6572  name)"').    ter
-00012c90: 6d69 6e61 7465 5f63 6d64 203d 2028 6627  minate_cmd = (f'
-00012ca0: 6763 6c6f 7564 2063 6f6d 7075 7465 2069  gcloud compute i
-00012cb0: 6e73 7461 6e63 6573 2064 656c 6574 6520  nstances delete 
-00012cc0: 2d2d 7a6f 6e65 3d7b 7a6f 6e65 7d27 0a20  --zone={zone}'. 
-00012cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ce0: 2020 2020 6627 202d 2d71 7569 6574 2024      f' --quiet $
-00012cf0: 287b 7175 6572 795f 636d 647d 2927 290a  ({query_cmd})').
-00012d00: 2020 2020 7465 7374 203d 2054 6573 7428      test = Test(
-00012d10: 0a20 2020 2020 2020 2027 7370 6f74 5f70  .        'spot_p
-00012d20: 6970 656c 696e 655f 7265 636f 7665 7279  ipeline_recovery
-00012d30: 5f67 6370 272c 0a20 2020 2020 2020 205b  _gcp',.        [
-00012d40: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-00012d50: 6b79 2073 706f 7420 6c61 756e 6368 202d  ky spot launch -
-00012d60: 6e20 7b6e 616d 657d 2074 6573 7473 2f74  n {name} tests/t
-00012d70: 6573 745f 7961 6d6c 732f 7069 7065 6c69  est_yamls/pipeli
-00012d80: 6e65 5f67 6370 2e79 616d 6c20 202d 7920  ne_gcp.yaml  -y 
-00012d90: 2d64 272c 0a20 2020 2020 2020 2020 2020  -d',.           
-00012da0: 2027 736c 6565 7020 3430 3027 2c0a 2020   'sleep 400',.  
-00012db0: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
-00012dc0: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
-00012dd0: 6772 6570 207b 6e61 6d65 7d20 7c20 6865  grep {name} | he
-00012de0: 6164 202d 6e31 207c 2067 7265 7020 2252  ad -n1 | grep "R
-00012df0: 554e 4e49 4e47 2227 2c0a 2020 2020 2020  UNNING"',.      
-00012e00: 2020 2020 2020 6627 5255 4e5f 4944 3d24        f'RUN_ID=$
-00012e10: 2873 6b79 2073 706f 7420 6c6f 6773 202d  (sky spot logs -
-00012e20: 6e20 7b6e 616d 657d 202d 2d6e 6f2d 666f  n {name} --no-fo
-00012e30: 6c6c 6f77 207c 2067 7265 7020 534b 5950  llow | grep SKYP
-00012e40: 494c 4f54 5f54 4153 4b5f 4944 3a20 7c20  ILOT_TASK_ID: | 
-00012e50: 6375 7420 2d64 3a20 2d66 3229 3b20 6563  cut -d: -f2); ec
-00012e60: 686f 2022 2452 554e 5f49 4422 207c 2074  ho "$RUN_ID" | t
-00012e70: 6565 202f 746d 702f 7b6e 616d 657d 2d72  ee /tmp/{name}-r
-00012e80: 756e 2d69 6427 2c0a 2020 2020 2020 2020  un-id',.        
-00012e90: 2020 2020 6627 5255 4e5f 4944 533d 2428      f'RUN_IDS=$(
-00012ea0: 736b 7920 7370 6f74 206c 6f67 7320 2d6e  sky spot logs -n
-00012eb0: 207b 6e61 6d65 7d20 2d2d 6e6f 2d66 6f6c   {name} --no-fol
-00012ec0: 6c6f 7720 7c20 6772 6570 202d 4120 3420  low | grep -A 4 
-00012ed0: 534b 5950 494c 4f54 5f54 4153 4b5f 4944  SKYPILOT_TASK_ID
-00012ee0: 5320 7c20 6375 7420 2d64 2229 2220 2d66  S | cut -d")" -f
-00012ef0: 3229 3b20 6563 686f 2022 2452 554e 5f49  2); echo "$RUN_I
-00012f00: 4453 2220 7c20 7465 6520 2f74 6d70 2f7b  DS" | tee /tmp/{
-00012f10: 6e61 6d65 7d2d 7275 6e2d 6964 7327 2c0a  name}-run-ids',.
-00012f20: 2020 2020 2020 2020 2020 2020 2320 5465              # Te
-00012f30: 726d 696e 6174 6520 7468 6520 636c 7573  rminate the clus
-00012f40: 7465 7220 6d61 6e75 616c 6c79 2e0a 2020  ter manually..  
-00012f50: 2020 2020 2020 2020 2020 2320 5468 6520            # The 
-00012f60: 6063 6174 202e 2e2e 7c20 7265 7660 2069  `cat ...| rev` i
-00012f70: 7320 746f 2072 6574 7269 6576 6520 7468  s to retrieve th
-00012f80: 6520 6a6f 625f 6964 2066 726f 6d20 7468  e job_id from th
-00012f90: 650a 2020 2020 2020 2020 2020 2020 2320  e.            # 
-00012fa0: 534b 5950 494c 4f54 5f54 4153 4b5f 4944  SKYPILOT_TASK_ID
-00012fb0: 2c20 7768 6963 6820 6765 7473 2074 6865  , which gets the
-00012fc0: 2073 6563 6f6e 6420 746f 206c 6173 7420   second to last 
-00012fd0: 6669 656c 640a 2020 2020 2020 2020 2020  field.          
-00012fe0: 2020 2320 7365 7061 7261 7465 6420 6279    # separated by
-00012ff0: 2060 2d60 2e0a 2020 2020 2020 2020 2020   `-`..          
-00013000: 2020 2866 2753 504f 545f 4a4f 425f 4944    (f'SPOT_JOB_ID
-00013010: 3d60 6361 7420 2f74 6d70 2f7b 6e61 6d65  =`cat /tmp/{name
-00013020: 7d2d 7275 6e2d 6964 207c 2072 6576 207c  }-run-id | rev |
-00013030: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-00013040: 6627 6375 7420 2d64 5c27 2d5c 2720 2d66  f'cut -d\'-\' -f
-00013050: 3220 7c20 7265 7660 3b7b 7465 726d 696e  2 | rev`;{termin
-00013060: 6174 655f 636d 647d 2729 2c0a 2020 2020  ate_cmd}'),.    
-00013070: 2020 2020 2020 2020 2773 6c65 6570 2031          'sleep 1
-00013080: 3030 272c 0a20 2020 2020 2020 2020 2020  00',.           
-00013090: 2066 277b 5f53 504f 545f 5155 4555 455f   f'{_SPOT_QUEUE_
-000130a0: 5741 4954 7d7c 2067 7265 7020 7b6e 616d  WAIT}| grep {nam
-000130b0: 657d 207c 2068 6561 6420 2d6e 3120 7c20  e} | head -n1 | 
-000130c0: 6772 6570 2022 5245 434f 5645 5249 4e47  grep "RECOVERING
-000130d0: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-000130e0: 2773 6c65 6570 2032 3030 272c 0a20 2020  'sleep 200',.   
-000130f0: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
-00013100: 545f 5155 4555 455f 5741 4954 7d7c 2067  T_QUEUE_WAIT}| g
-00013110: 7265 7020 7b6e 616d 657d 207c 2068 6561  rep {name} | hea
-00013120: 6420 2d6e 3120 7c20 6772 6570 2022 5255  d -n1 | grep "RU
-00013130: 4e4e 494e 4722 272c 0a20 2020 2020 2020  NNING"',.       
-00013140: 2020 2020 2066 2752 554e 5f49 443d 2428       f'RUN_ID=$(
-00013150: 6361 7420 2f74 6d70 2f7b 6e61 6d65 7d2d  cat /tmp/{name}-
-00013160: 7275 6e2d 6964 293b 2065 6368 6f20 2452  run-id); echo $R
-00013170: 554e 5f49 443b 2073 6b79 2073 706f 7420  UN_ID; sky spot 
-00013180: 6c6f 6773 202d 6e20 7b6e 616d 657d 202d  logs -n {name} -
-00013190: 2d6e 6f2d 666f 6c6c 6f77 207c 2067 7265  -no-follow | gre
-000131a0: 7020 534b 5950 494c 4f54 5f54 4153 4b5f  p SKYPILOT_TASK_
-000131b0: 4944 3a20 7c20 6772 6570 2022 2452 554e  ID: | grep "$RUN
-000131c0: 5f49 4422 272c 0a20 2020 2020 2020 2020  _ID"',.         
-000131d0: 2020 2066 2752 554e 5f49 4453 3d24 2873     f'RUN_IDS=$(s
-000131e0: 6b79 2073 706f 7420 6c6f 6773 202d 6e20  ky spot logs -n 
-000131f0: 7b6e 616d 657d 202d 2d6e 6f2d 666f 6c6c  {name} --no-foll
-00013200: 6f77 207c 2067 7265 7020 2d41 2034 2053  ow | grep -A 4 S
-00013210: 4b59 5049 4c4f 545f 5441 534b 5f49 4453  KYPILOT_TASK_IDS
-00013220: 207c 2063 7574 202d 6422 2922 202d 6632   | cut -d")" -f2
-00013230: 293b 2065 6368 6f20 2224 5255 4e5f 4944  ); echo "$RUN_ID
-00013240: 5322 207c 2074 6565 202f 746d 702f 7b6e  S" | tee /tmp/{n
-00013250: 616d 657d 2d72 756e 2d69 6473 2d6e 6577  ame}-run-ids-new
-00013260: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-00013270: 2764 6966 6620 2f74 6d70 2f7b 6e61 6d65  'diff /tmp/{name
-00013280: 7d2d 7275 6e2d 6964 7320 2f74 6d70 2f7b  }-run-ids /tmp/{
-00013290: 6e61 6d65 7d2d 7275 6e2d 6964 732d 6e65  name}-run-ids-ne
-000132a0: 7727 2c0a 2020 2020 2020 2020 2020 2020  w',.            
-000132b0: 6627 6361 7420 2f74 6d70 2f7b 6e61 6d65  f'cat /tmp/{name
-000132c0: 7d2d 7275 6e2d 6964 7320 7c20 7365 6420  }-run-ids | sed 
-000132d0: 2d6e 2032 7020 7c20 6772 6570 2060 6361  -n 2p | grep `ca
-000132e0: 7420 2f74 6d70 2f7b 6e61 6d65 7d2d 7275  t /tmp/{name}-ru
-000132f0: 6e2d 6964 6027 2c0a 2020 2020 2020 2020  n-id`',.        
-00013300: 5d2c 0a20 2020 2020 2020 205f 5350 4f54  ],.        _SPOT
-00013310: 5f43 414e 4345 4c5f 5741 4954 2e66 6f72  _CANCEL_WAIT.for
-00013320: 6d61 7428 6a6f 625f 6e61 6d65 3d6e 616d  mat(job_name=nam
-00013330: 6529 2c0a 2020 2020 2020 2020 7469 6d65  e),.        time
-00013340: 6f75 743d 3235 202a 2036 302c 0a20 2020  out=25 * 60,.   
-00013350: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
-00013360: 6573 7428 7465 7374 290a 0a0a 4070 7974  est(test)...@pyt
-00013370: 6573 742e 6d61 726b 2e6e 6f5f 6c61 6d62  est.mark.no_lamb
-00013380: 6461 5f63 6c6f 7564 2020 2320 4c61 6d62  da_cloud  # Lamb
-00013390: 6461 2043 6c6f 7564 2064 6f65 7320 6e6f  da Cloud does no
-000133a0: 7420 7375 7070 6f72 7420 7370 6f74 2069  t support spot i
-000133b0: 6e73 7461 6e63 6573 0a40 7079 7465 7374  nstances.@pytest
-000133c0: 2e6d 6172 6b2e 6e6f 5f69 626d 2020 2320  .mark.no_ibm  # 
-000133d0: 4942 4d20 436c 6f75 6420 646f 6573 206e  IBM Cloud does n
-000133e0: 6f74 2073 7570 706f 7274 2073 706f 7420  ot support spot 
-000133f0: 696e 7374 616e 6365 730a 4070 7974 6573  instances.@pytes
-00013400: 742e 6d61 726b 2e6e 6f5f 7363 7020 2023  t.mark.no_scp  #
-00013410: 2053 4350 2064 6f65 7320 6e6f 7420 7375   SCP does not su
-00013420: 7070 6f72 7420 7370 6f74 2069 6e73 7461  pport spot insta
-00013430: 6e63 6573 0a40 7079 7465 7374 2e6d 6172  nces.@pytest.mar
-00013440: 6b2e 6d61 6e61 6765 645f 7370 6f74 0a64  k.managed_spot.d
-00013450: 6566 2074 6573 745f 7370 6f74 5f72 6563  ef test_spot_rec
-00013460: 6f76 6572 795f 6465 6661 756c 745f 7265  overy_default_re
-00013470: 736f 7572 6365 7328 6765 6e65 7269 635f  sources(generic_
-00013480: 636c 6f75 643a 2073 7472 293a 0a20 2020  cloud: str):.   
-00013490: 2022 2222 5465 7374 206d 616e 6167 6564   """Test managed
-000134a0: 2073 706f 7420 7265 636f 7665 7279 2066   spot recovery f
-000134b0: 6f72 2064 6566 6175 6c74 2072 6573 6f75  or default resou
-000134c0: 7263 6573 2e22 2222 0a20 2020 206e 616d  rces.""".    nam
-000134d0: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
-000134e0: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
-000134f0: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
-00013500: 2027 6d61 6e61 6765 642d 7370 6f74 2d72   'managed-spot-r
-00013510: 6563 6f76 6572 792d 6465 6661 756c 742d  ecovery-default-
-00013520: 7265 736f 7572 6365 7327 2c0a 2020 2020  resources',.    
-00013530: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-00013540: 2020 6627 736b 7920 7370 6f74 206c 6175    f'sky spot lau
-00013550: 6e63 6820 2d6e 207b 6e61 6d65 7d20 2d2d  nch -n {name} --
-00013560: 636c 6f75 6420 7b67 656e 6572 6963 5f63  cloud {generic_c
-00013570: 6c6f 7564 7d20 2273 6c65 6570 2033 3020  loud} "sleep 30 
-00013580: 2626 2073 7564 6f20 7368 7574 646f 776e  && sudo shutdown
-00013590: 206e 6f77 2026 2620 736c 6565 7020 3130   now && sleep 10
-000135a0: 3030 2220 2d79 202d 6427 2c0a 2020 2020  00" -y -d',.    
-000135b0: 2020 2020 2020 2020 2773 6c65 6570 2033          'sleep 3
-000135c0: 3630 272c 0a20 2020 2020 2020 2020 2020  60',.           
-000135d0: 2066 277b 5f53 504f 545f 5155 4555 455f   f'{_SPOT_QUEUE_
-000135e0: 5741 4954 7d7c 2067 7265 7020 7b6e 616d  WAIT}| grep {nam
-000135f0: 657d 207c 2068 6561 6420 2d6e 3120 7c20  e} | head -n1 | 
-00013600: 6772 6570 2022 5255 4e4e 494e 475c 7c52  grep "RUNNING\|R
-00013610: 4543 4f56 4552 494e 4722 272c 0a20 2020  ECOVERING"',.   
-00013620: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00013630: 5f53 504f 545f 4341 4e43 454c 5f57 4149  _SPOT_CANCEL_WAI
-00013640: 542e 666f 726d 6174 286a 6f62 5f6e 616d  T.format(job_nam
-00013650: 653d 6e61 6d65 292c 0a20 2020 2020 2020  e=name),.       
-00013660: 2074 696d 656f 7574 3d32 3520 2a20 3630   timeout=25 * 60
-00013670: 2c0a 2020 2020 290a 2020 2020 7275 6e5f  ,.    ).    run_
-00013680: 6f6e 655f 7465 7374 2874 6573 7429 0a0a  one_test(test)..
-00013690: 0a40 7079 7465 7374 2e6d 6172 6b2e 6177  .@pytest.mark.aw
-000136a0: 730a 4070 7974 6573 742e 6d61 726b 2e6d  s.@pytest.mark.m
-000136b0: 616e 6167 6564 5f73 706f 740a 6465 6620  anaged_spot.def 
-000136c0: 7465 7374 5f73 706f 745f 7265 636f 7665  test_spot_recove
-000136d0: 7279 5f6d 756c 7469 5f6e 6f64 655f 6177  ry_multi_node_aw
-000136e0: 7328 6177 735f 636f 6e66 6967 5f72 6567  s(aws_config_reg
-000136f0: 696f 6e29 3a0a 2020 2020 2222 2254 6573  ion):.    """Tes
-00013700: 7420 6d61 6e61 6765 6420 7370 6f74 2072  t managed spot r
-00013710: 6563 6f76 6572 792e 2222 220a 2020 2020  ecovery.""".    
-00013720: 6e61 6d65 203d 205f 6765 745f 636c 7573  name = _get_clus
-00013730: 7465 725f 6e61 6d65 2829 0a20 2020 2072  ter_name().    r
-00013740: 6567 696f 6e20 3d20 6177 735f 636f 6e66  egion = aws_conf
-00013750: 6967 5f72 6567 696f 6e0a 2020 2020 7465  ig_region.    te
-00013760: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
-00013770: 2020 2027 7370 6f74 5f72 6563 6f76 6572     'spot_recover
-00013780: 795f 6d75 6c74 695f 6e6f 6465 5f61 7773  y_multi_node_aws
-00013790: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
-000137a0: 2020 2020 2020 2020 2066 2773 6b79 2073           f'sky s
-000137b0: 706f 7420 6c61 756e 6368 202d 2d63 6c6f  pot launch --clo
-000137c0: 7564 2061 7773 202d 2d72 6567 696f 6e20  ud aws --region 
-000137d0: 7b72 6567 696f 6e7d 202d 6e20 7b6e 616d  {region} -n {nam
-000137e0: 657d 202d 2d6e 756d 2d6e 6f64 6573 2032  e} --num-nodes 2
-000137f0: 2022 6563 686f 2053 4b59 5049 4c4f 545f   "echo SKYPILOT_
-00013800: 5441 534b 5f49 443a 205c 2453 4b59 5049  TASK_ID: \$SKYPI
-00013810: 4c4f 545f 5441 534b 5f49 443b 2073 6c65  LOT_TASK_ID; sle
-00013820: 6570 2031 3830 3022 2020 2d79 202d 6427  ep 1800"  -y -d'
-00013830: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
-00013840: 6c65 6570 2034 3530 272c 0a20 2020 2020  leep 450',.     
-00013850: 2020 2020 2020 2066 277b 5f53 504f 545f         f'{_SPOT_
-00013860: 5155 4555 455f 5741 4954 7d7c 2067 7265  QUEUE_WAIT}| gre
-00013870: 7020 7b6e 616d 657d 207c 2068 6561 6420  p {name} | head 
-00013880: 2d6e 3120 7c20 6772 6570 2022 5255 4e4e  -n1 | grep "RUNN
-00013890: 494e 4722 272c 0a20 2020 2020 2020 2020  ING"',.         
-000138a0: 2020 2066 2752 554e 5f49 443d 2428 736b     f'RUN_ID=$(sk
-000138b0: 7920 7370 6f74 206c 6f67 7320 2d6e 207b  y spot logs -n {
-000138c0: 6e61 6d65 7d20 2d2d 6e6f 2d66 6f6c 6c6f  name} --no-follo
-000138d0: 7720 7c20 6772 6570 2053 4b59 5049 4c4f  w | grep SKYPILO
-000138e0: 545f 5441 534b 5f49 4420 7c20 6375 7420  T_TASK_ID | cut 
-000138f0: 2d64 3a20 2d66 3229 3b20 6563 686f 2022  -d: -f2); echo "
-00013900: 2452 554e 5f49 4422 207c 2074 6565 202f  $RUN_ID" | tee /
-00013910: 746d 702f 7b6e 616d 657d 2d72 756e 2d69  tmp/{name}-run-i
-00013920: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
-00013930: 2320 5465 726d 696e 6174 6520 7468 6520  # Terminate the 
-00013940: 776f 726b 6572 206d 616e 7561 6c6c 792e  worker manually.
-00013950: 0a20 2020 2020 2020 2020 2020 2028 6627  .            (f'
-00013960: 6177 7320 6563 3220 7465 726d 696e 6174  aws ec2 terminat
-00013970: 652d 696e 7374 616e 6365 7320 2d2d 7265  e-instances --re
-00013980: 6769 6f6e 207b 7265 6769 6f6e 7d20 2d2d  gion {region} --
-00013990: 696e 7374 616e 6365 2d69 6473 2024 2827  instance-ids $('
-000139a0: 0a20 2020 2020 2020 2020 2020 2020 6627  .             f'
-000139b0: 6177 7320 6563 3220 6465 7363 7269 6265  aws ec2 describe
-000139c0: 2d69 6e73 7461 6e63 6573 202d 2d72 6567  -instances --reg
-000139d0: 696f 6e20 7b72 6567 696f 6e7d 2027 0a20  ion {region} '. 
-000139e0: 2020 2020 2020 2020 2020 2020 6627 2d2d              f'--
-000139f0: 6669 6c74 6572 7320 4e61 6d65 3d74 6167  filters Name=tag
-00013a00: 3a72 6179 2d63 6c75 7374 6572 2d6e 616d  :ray-cluster-nam
-00013a10: 652c 5661 6c75 6573 3d7b 6e61 6d65 7d2a  e,Values={name}*
-00013a20: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-00013a30: 274e 616d 653d 7461 673a 7261 792d 6e6f  'Name=tag:ray-no
-00013a40: 6465 2d74 7970 652c 5661 6c75 6573 3d77  de-type,Values=w
-00013a50: 6f72 6b65 7220 270a 2020 2020 2020 2020  orker '.        
-00013a60: 2020 2020 2066 272d 2d71 7565 7279 2052       f'--query R
-00013a70: 6573 6572 7661 7469 6f6e 735b 5d2e 496e  eservations[].In
-00013a80: 7374 616e 6365 735b 5d2e 496e 7374 616e  stances[].Instan
-00013a90: 6365 4964 2027 0a20 2020 2020 2020 2020  ceId '.         
-00013aa0: 2020 2020 272d 2d6f 7574 7075 7420 7465      '--output te
-00013ab0: 7874 2927 292c 0a20 2020 2020 2020 2020  xt)'),.         
-00013ac0: 2020 2027 736c 6565 7020 3530 272c 0a20     'sleep 50',. 
-00013ad0: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
-00013ae0: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
-00013af0: 2067 7265 7020 7b6e 616d 657d 207c 2068   grep {name} | h
-00013b00: 6561 6420 2d6e 3120 7c20 6772 6570 2022  ead -n1 | grep "
-00013b10: 5245 434f 5645 5249 4e47 2227 2c0a 2020  RECOVERING"',.  
-00013b20: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
-00013b30: 2035 3630 272c 0a20 2020 2020 2020 2020   560',.         
-00013b40: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
-00013b50: 455f 5741 4954 7d7c 2067 7265 7020 7b6e  E_WAIT}| grep {n
-00013b60: 616d 657d 207c 2068 6561 6420 2d6e 3120  ame} | head -n1 
-00013b70: 7c20 6772 6570 2022 5255 4e4e 494e 4722  | grep "RUNNING"
-00013b80: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-00013b90: 2752 554e 5f49 443d 2428 6361 7420 2f74  'RUN_ID=$(cat /t
-00013ba0: 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d 6964  mp/{name}-run-id
-00013bb0: 293b 2065 6368 6f20 2452 554e 5f49 443b  ); echo $RUN_ID;
-00013bc0: 2073 6b79 2073 706f 7420 6c6f 6773 202d   sky spot logs -
-00013bd0: 6e20 7b6e 616d 657d 202d 2d6e 6f2d 666f  n {name} --no-fo
-00013be0: 6c6c 6f77 207c 2067 7265 7020 534b 5950  llow | grep SKYP
-00013bf0: 494c 4f54 5f54 4153 4b5f 4944 207c 2063  ILOT_TASK_ID | c
-00013c00: 7574 202d 643a 202d 6632 207c 2067 7265  ut -d: -f2 | gre
-00013c10: 7020 2224 5255 4e5f 4944 2227 2c0a 2020  p "$RUN_ID"',.  
-00013c20: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-00013c30: 205f 5350 4f54 5f43 414e 4345 4c5f 5741   _SPOT_CANCEL_WA
-00013c40: 4954 2e66 6f72 6d61 7428 6a6f 625f 6e61  IT.format(job_na
-00013c50: 6d65 3d6e 616d 6529 2c0a 2020 2020 2020  me=name),.      
-00013c60: 2020 7469 6d65 6f75 743d 3330 202a 2036    timeout=30 * 6
-00013c70: 302c 0a20 2020 2029 0a20 2020 2072 756e  0,.    ).    run
-00013c80: 5f6f 6e65 5f74 6573 7428 7465 7374 290a  _one_test(test).
-00013c90: 0a0a 4070 7974 6573 742e 6d61 726b 2e67  ..@pytest.mark.g
-00013ca0: 6370 0a40 7079 7465 7374 2e6d 6172 6b2e  cp.@pytest.mark.
-00013cb0: 6d61 6e61 6765 645f 7370 6f74 0a64 6566  managed_spot.def
-00013cc0: 2074 6573 745f 7370 6f74 5f72 6563 6f76   test_spot_recov
-00013cd0: 6572 795f 6d75 6c74 695f 6e6f 6465 5f67  ery_multi_node_g
-00013ce0: 6370 2829 3a0a 2020 2020 2222 2254 6573  cp():.    """Tes
-00013cf0: 7420 6d61 6e61 6765 6420 7370 6f74 2072  t managed spot r
-00013d00: 6563 6f76 6572 792e 2222 220a 2020 2020  ecovery.""".    
-00013d10: 6e61 6d65 203d 205f 6765 745f 636c 7573  name = _get_clus
-00013d20: 7465 725f 6e61 6d65 2829 0a20 2020 207a  ter_name().    z
-00013d30: 6f6e 6520 3d20 2775 732d 7765 7374 322d  one = 'us-west2-
-00013d40: 6127 0a20 2020 2023 2055 7365 2027 3a27  a'.    # Use ':'
-00013d50: 2074 6f20 6d61 7463 6820 6173 2074 6865   to match as the
-00013d60: 2063 6c75 7374 6572 206e 616d 6520 7769   cluster name wi
-00013d70: 6c6c 2063 6f6e 7461 696e 2074 6865 2073  ll contain the s
-00013d80: 7566 6669 7820 7769 7468 206a 6f62 2069  uffix with job i
-00013d90: 640a 2020 2020 7175 6572 795f 636d 6420  d.    query_cmd 
-00013da0: 3d20 280a 2020 2020 2020 2020 6627 6763  = (.        f'gc
-00013db0: 6c6f 7564 2063 6f6d 7075 7465 2069 6e73  loud compute ins
-00013dc0: 7461 6e63 6573 206c 6973 7420 2d2d 6669  tances list --fi
-00013dd0: 6c74 6572 3d27 0a20 2020 2020 2020 2066  lter='.        f
-00013de0: 2722 286c 6162 656c 732e 7261 792d 636c  '"(labels.ray-cl
-00013df0: 7573 7465 722d 6e61 6d65 3a7b 6e61 6d65  uster-name:{name
-00013e00: 7d20 414e 4420 6c61 6265 6c73 2e72 6179  } AND labels.ray
-00013e10: 2d6e 6f64 652d 7479 7065 3d77 6f72 6b65  -node-type=worke
-00013e20: 7229 2220 270a 2020 2020 2020 2020 6627  r)" '.        f'
-00013e30: 2d2d 7a6f 6e65 733d 7b7a 6f6e 657d 202d  --zones={zone} -
-00013e40: 2d66 6f72 6d61 743d 2276 616c 7565 286e  -format="value(n
-00013e50: 616d 6529 2227 290a 2020 2020 7465 726d  ame)"').    term
-00013e60: 696e 6174 655f 636d 6420 3d20 2866 2767  inate_cmd = (f'g
-00013e70: 636c 6f75 6420 636f 6d70 7574 6520 696e  cloud compute in
-00013e80: 7374 616e 6365 7320 6465 6c65 7465 202d  stances delete -
-00013e90: 2d7a 6f6e 653d 7b7a 6f6e 657d 270a 2020  -zone={zone}'.  
-00013ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013eb0: 2020 2066 2720 2d2d 7175 6965 7420 2428     f' --quiet $(
-00013ec0: 7b71 7565 7279 5f63 6d64 7d29 2729 0a20  {query_cmd})'). 
-00013ed0: 2020 2074 6573 7420 3d20 5465 7374 280a     test = Test(.
-00013ee0: 2020 2020 2020 2020 2773 706f 745f 7265          'spot_re
-00013ef0: 636f 7665 7279 5f6d 756c 7469 5f6e 6f64  covery_multi_nod
-00013f00: 655f 6763 7027 2c0a 2020 2020 2020 2020  e_gcp',.        
-00013f10: 5b0a 2020 2020 2020 2020 2020 2020 6627  [.            f'
-00013f20: 736b 7920 7370 6f74 206c 6175 6e63 6820  sky spot launch 
-00013f30: 2d2d 636c 6f75 6420 6763 7020 2d2d 7a6f  --cloud gcp --zo
-00013f40: 6e65 207b 7a6f 6e65 7d20 2d6e 207b 6e61  ne {zone} -n {na
-00013f50: 6d65 7d20 2d2d 6e75 6d2d 6e6f 6465 7320  me} --num-nodes 
-00013f60: 3220 2265 6368 6f20 534b 5950 494c 4f54  2 "echo SKYPILOT
-00013f70: 5f54 4153 4b5f 4944 3a20 5c24 534b 5950  _TASK_ID: \$SKYP
-00013f80: 494c 4f54 5f54 4153 4b5f 4944 3b20 736c  ILOT_TASK_ID; sl
-00013f90: 6565 7020 3138 3030 2220 202d 7920 2d64  eep 1800"  -y -d
-00013fa0: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-00013fb0: 736c 6565 7020 3430 3027 2c0a 2020 2020  sleep 400',.    
-00013fc0: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
-00013fd0: 5f51 5545 5545 5f57 4149 547d 7c20 6772  _QUEUE_WAIT}| gr
-00013fe0: 6570 207b 6e61 6d65 7d20 7c20 6865 6164  ep {name} | head
-00013ff0: 202d 6e31 207c 2067 7265 7020 2252 554e   -n1 | grep "RUN
-00014000: 4e49 4e47 2227 2c0a 2020 2020 2020 2020  NING"',.        
-00014010: 2020 2020 6627 5255 4e5f 4944 3d24 2873      f'RUN_ID=$(s
-00014020: 6b79 2073 706f 7420 6c6f 6773 202d 6e20  ky spot logs -n 
-00014030: 7b6e 616d 657d 202d 2d6e 6f2d 666f 6c6c  {name} --no-foll
-00014040: 6f77 207c 2067 7265 7020 534b 5950 494c  ow | grep SKYPIL
-00014050: 4f54 5f54 4153 4b5f 4944 207c 2063 7574  OT_TASK_ID | cut
-00014060: 202d 643a 202d 6632 293b 2065 6368 6f20   -d: -f2); echo 
-00014070: 2224 5255 4e5f 4944 2220 7c20 7465 6520  "$RUN_ID" | tee 
-00014080: 2f74 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d  /tmp/{name}-run-
-00014090: 6964 272c 0a20 2020 2020 2020 2020 2020  id',.           
-000140a0: 2023 2054 6572 6d69 6e61 7465 2074 6865   # Terminate the
-000140b0: 2077 6f72 6b65 7220 6d61 6e75 616c 6c79   worker manually
-000140c0: 2e0a 2020 2020 2020 2020 2020 2020 7465  ..            te
-000140d0: 726d 696e 6174 655f 636d 642c 0a20 2020  rminate_cmd,.   
-000140e0: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
-000140f0: 3530 272c 0a20 2020 2020 2020 2020 2020  50',.           
-00014100: 2066 277b 5f53 504f 545f 5155 4555 455f   f'{_SPOT_QUEUE_
-00014110: 5741 4954 7d7c 2067 7265 7020 7b6e 616d  WAIT}| grep {nam
-00014120: 657d 207c 2068 6561 6420 2d6e 3120 7c20  e} | head -n1 | 
-00014130: 6772 6570 2022 5245 434f 5645 5249 4e47  grep "RECOVERING
-00014140: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-00014150: 2773 6c65 6570 2034 3230 272c 0a20 2020  'sleep 420',.   
-00014160: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
-00014170: 545f 5155 4555 455f 5741 4954 7d7c 2067  T_QUEUE_WAIT}| g
-00014180: 7265 7020 7b6e 616d 657d 207c 2068 6561  rep {name} | hea
-00014190: 6420 2d6e 3120 7c20 6772 6570 2022 5255  d -n1 | grep "RU
-000141a0: 4e4e 494e 4722 272c 0a20 2020 2020 2020  NNING"',.       
-000141b0: 2020 2020 2066 2752 554e 5f49 443d 2428       f'RUN_ID=$(
-000141c0: 6361 7420 2f74 6d70 2f7b 6e61 6d65 7d2d  cat /tmp/{name}-
-000141d0: 7275 6e2d 6964 293b 2065 6368 6f20 2452  run-id); echo $R
-000141e0: 554e 5f49 443b 2073 6b79 2073 706f 7420  UN_ID; sky spot 
-000141f0: 6c6f 6773 202d 6e20 7b6e 616d 657d 202d  logs -n {name} -
-00014200: 2d6e 6f2d 666f 6c6c 6f77 207c 2067 7265  -no-follow | gre
-00014210: 7020 534b 5950 494c 4f54 5f54 4153 4b5f  p SKYPILOT_TASK_
-00014220: 4944 207c 2063 7574 202d 643a 202d 6632  ID | cut -d: -f2
-00014230: 207c 2067 7265 7020 2224 5255 4e5f 4944   | grep "$RUN_ID
-00014240: 2227 2c0a 2020 2020 2020 2020 5d2c 0a20  "',.        ],. 
-00014250: 2020 2020 2020 205f 5350 4f54 5f43 414e         _SPOT_CAN
-00014260: 4345 4c5f 5741 4954 2e66 6f72 6d61 7428  CEL_WAIT.format(
-00014270: 6a6f 625f 6e61 6d65 3d6e 616d 6529 2c0a  job_name=name),.
-00014280: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
-00014290: 3235 202a 2036 302c 0a20 2020 2029 0a20  25 * 60,.    ). 
-000142a0: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
-000142b0: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
-000142c0: 6d61 726b 2e61 7773 0a40 7079 7465 7374  mark.aws.@pytest
-000142d0: 2e6d 6172 6b2e 6d61 6e61 6765 645f 7370  .mark.managed_sp
-000142e0: 6f74 0a64 6566 2074 6573 745f 7370 6f74  ot.def test_spot
-000142f0: 5f63 616e 6365 6c6c 6174 696f 6e5f 6177  _cancellation_aw
-00014300: 7328 6177 735f 636f 6e66 6967 5f72 6567  s(aws_config_reg
-00014310: 696f 6e29 3a0a 2020 2020 6e61 6d65 203d  ion):.    name =
-00014320: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
-00014330: 6d65 2829 0a20 2020 2072 6567 696f 6e20  me().    region 
-00014340: 3d20 6177 735f 636f 6e66 6967 5f72 6567  = aws_config_reg
-00014350: 696f 6e0a 2020 2020 7465 7374 203d 2054  ion.    test = T
-00014360: 6573 7428 0a20 2020 2020 2020 2027 7370  est(.        'sp
-00014370: 6f74 5f63 616e 6365 6c6c 6174 696f 6e5f  ot_cancellation_
-00014380: 6177 7327 2c0a 2020 2020 2020 2020 5b0a  aws',.        [.
-00014390: 2020 2020 2020 2020 2020 2020 2320 5465              # Te
-000143a0: 7374 2063 616e 6365 6c6c 6174 696f 6e20  st cancellation 
-000143b0: 6475 7269 6e67 2073 706f 7420 636c 7573  during spot clus
-000143c0: 7465 7220 6265 696e 6720 6c61 756e 6368  ter being launch
-000143d0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-000143e0: 6627 736b 7920 7370 6f74 206c 6175 6e63  f'sky spot launc
-000143f0: 6820 2d2d 636c 6f75 6420 6177 7320 2d2d  h --cloud aws --
-00014400: 7265 6769 6f6e 207b 7265 6769 6f6e 7d20  region {region} 
-00014410: 2d6e 207b 6e61 6d65 7d20 2273 6c65 6570  -n {name} "sleep
-00014420: 2031 3030 3022 2020 2d79 202d 6427 2c0a   1000"  -y -d',.
-00014430: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
-00014440: 6570 2036 3027 2c0a 2020 2020 2020 2020  ep 60',.        
-00014450: 2020 2020 6627 7b5f 5350 4f54 5f51 5545      f'{_SPOT_QUE
-00014460: 5545 5f57 4149 547d 7c20 6772 6570 207b  UE_WAIT}| grep {
-00014470: 6e61 6d65 7d20 7c20 6865 6164 202d 6e31  name} | head -n1
-00014480: 207c 2067 7265 7020 2253 5441 5254 494e   | grep "STARTIN
-00014490: 4722 272c 0a20 2020 2020 2020 2020 2020  G"',.           
-000144a0: 205f 5350 4f54 5f43 414e 4345 4c5f 5741   _SPOT_CANCEL_WA
-000144b0: 4954 2e66 6f72 6d61 7428 6a6f 625f 6e61  IT.format(job_na
-000144c0: 6d65 3d6e 616d 6529 2c0a 2020 2020 2020  me=name),.      
-000144d0: 2020 2020 2020 2773 6c65 6570 2035 272c        'sleep 5',
-000144e0: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
-000144f0: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
-00014500: 7d7c 2067 7265 7020 7b6e 616d 657d 207c  }| grep {name} |
-00014510: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
-00014520: 2022 4341 4e43 454c 4c49 4e47 5c7c 4341   "CANCELLING\|CA
-00014530: 4e43 454c 4c45 4422 272c 0a20 2020 2020  NCELLED"',.     
-00014540: 2020 2020 2020 2027 736c 6565 7020 3132         'sleep 12
-00014550: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
-00014560: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
-00014570: 4149 547d 7c20 6772 6570 207b 6e61 6d65  AIT}| grep {name
-00014580: 7d20 7c20 6865 6164 202d 6e31 207c 2067  } | head -n1 | g
-00014590: 7265 7020 2243 414e 4345 4c4c 4544 2227  rep "CANCELLED"'
-000145a0: 2c0a 2020 2020 2020 2020 2020 2020 2866  ,.            (f
-000145b0: 2773 3d24 2861 7773 2065 6332 2064 6573  's=$(aws ec2 des
-000145c0: 6372 6962 652d 696e 7374 616e 6365 7320  cribe-instances 
-000145d0: 2d2d 7265 6769 6f6e 207b 7265 6769 6f6e  --region {region
-000145e0: 7d20 270a 2020 2020 2020 2020 2020 2020  } '.            
-000145f0: 2066 272d 2d66 696c 7465 7273 204e 616d   f'--filters Nam
-00014600: 653d 7461 673a 7261 792d 636c 7573 7465  e=tag:ray-cluste
-00014610: 722d 6e61 6d65 2c56 616c 7565 733d 7b6e  r-name,Values={n
-00014620: 616d 657d 2d2a 2027 0a20 2020 2020 2020  ame}-* '.       
-00014630: 2020 2020 2020 6627 2d2d 7175 6572 7920        f'--query 
-00014640: 5265 7365 7276 6174 696f 6e73 5b5d 2e49  Reservations[].I
-00014650: 6e73 7461 6e63 6573 5b5d 2e53 7461 7465  nstances[].State
-00014660: 5b5d 2e4e 616d 6520 270a 2020 2020 2020  [].Name '.      
-00014670: 2020 2020 2020 2027 2d2d 6f75 7470 7574         '--output
-00014680: 2074 6578 7429 2026 2620 6563 686f 2022   text) && echo "
-00014690: 2473 2220 2626 2065 6368 6f3b 205b 5b20  $s" && echo; [[ 
-000146a0: 2d7a 2022 2473 2220 5d5d 207c 7c20 5b5b  -z "$s" ]] || [[
-000146b0: 2022 2473 2220 3d20 2274 6572 6d69 6e61   "$s" = "termina
-000146c0: 7465 6422 205d 5d20 7c7c 205b 5b20 2224  ted" ]] || [[ "$
-000146d0: 7322 203d 2022 7368 7574 7469 6e67 2d64  s" = "shutting-d
-000146e0: 6f77 6e22 205d 5d27 0a20 2020 2020 2020  own" ]]'.       
-000146f0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-00014700: 2020 2020 2320 5465 7374 2063 616e 6365      # Test cance
-00014710: 6c6c 696e 6720 7468 6520 7370 6f74 2063  lling the spot c
-00014720: 6c75 7374 6572 2064 7572 696e 6720 7370  luster during sp
-00014730: 6f74 206a 6f62 2062 6569 6e67 2073 6574  ot job being set
-00014740: 7570 2e0a 2020 2020 2020 2020 2020 2020  up..            
-00014750: 6627 736b 7920 7370 6f74 206c 6175 6e63  f'sky spot launc
-00014760: 6820 2d2d 636c 6f75 6420 6177 7320 2d2d  h --cloud aws --
-00014770: 7265 6769 6f6e 207b 7265 6769 6f6e 7d20  region {region} 
-00014780: 2d6e 207b 6e61 6d65 7d2d 3220 7465 7374  -n {name}-2 test
-00014790: 732f 7465 7374 5f79 616d 6c73 2f74 6573  s/test_yamls/tes
-000147a0: 745f 6c6f 6e67 5f73 6574 7570 2e79 616d  t_long_setup.yam
-000147b0: 6c20 202d 7920 2d64 272c 0a20 2020 2020  l  -y -d',.     
-000147c0: 2020 2020 2020 2027 736c 6565 7020 3330         'sleep 30
-000147d0: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
-000147e0: 5f53 504f 545f 4341 4e43 454c 5f57 4149  _SPOT_CANCEL_WAI
-000147f0: 542e 666f 726d 6174 286a 6f62 5f6e 616d  T.format(job_nam
-00014800: 653d 6627 7b6e 616d 657d 2d32 2729 2c0a  e=f'{name}-2'),.
-00014810: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
-00014820: 6570 2035 272c 0a20 2020 2020 2020 2020  ep 5',.         
-00014830: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
-00014840: 455f 5741 4954 7d7c 2067 7265 7020 7b6e  E_WAIT}| grep {n
-00014850: 616d 657d 2d32 207c 2068 6561 6420 2d6e  ame}-2 | head -n
-00014860: 3120 7c20 6772 6570 2022 4341 4e43 454c  1 | grep "CANCEL
-00014870: 4c49 4e47 5c7c 4341 4e43 454c 4c45 4422  LING\|CANCELLED"
-00014880: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-00014890: 736c 6565 7020 3132 3027 2c0a 2020 2020  sleep 120',.    
-000148a0: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
-000148b0: 5f51 5545 5545 5f57 4149 547d 7c20 6772  _QUEUE_WAIT}| gr
-000148c0: 6570 207b 6e61 6d65 7d2d 3220 7c20 6865  ep {name}-2 | he
-000148d0: 6164 202d 6e31 207c 2067 7265 7020 2243  ad -n1 | grep "C
-000148e0: 414e 4345 4c4c 4544 2227 2c0a 2020 2020  ANCELLED"',.    
-000148f0: 2020 2020 2020 2020 2866 2773 3d24 2861          (f's=$(a
-00014900: 7773 2065 6332 2064 6573 6372 6962 652d  ws ec2 describe-
-00014910: 696e 7374 616e 6365 7320 2d2d 7265 6769  instances --regi
-00014920: 6f6e 207b 7265 6769 6f6e 7d20 270a 2020  on {region} '.  
-00014930: 2020 2020 2020 2020 2020 2066 272d 2d66             f'--f
-00014940: 696c 7465 7273 204e 616d 653d 7461 673a  ilters Name=tag:
-00014950: 7261 792d 636c 7573 7465 722d 6e61 6d65  ray-cluster-name
-00014960: 2c56 616c 7565 733d 7b6e 616d 657d 2d32  ,Values={name}-2
-00014970: 2d2a 2027 0a20 2020 2020 2020 2020 2020  -* '.           
-00014980: 2020 6627 2d2d 7175 6572 7920 5265 7365    f'--query Rese
-00014990: 7276 6174 696f 6e73 5b5d 2e49 6e73 7461  rvations[].Insta
-000149a0: 6e63 6573 5b5d 2e53 7461 7465 5b5d 2e4e  nces[].State[].N
-000149b0: 616d 6520 270a 2020 2020 2020 2020 2020  ame '.          
-000149c0: 2020 2027 2d2d 6f75 7470 7574 2074 6578     '--output tex
-000149d0: 7429 2026 2620 6563 686f 2022 2473 2220  t) && echo "$s" 
-000149e0: 2626 2065 6368 6f3b 205b 5b20 2d7a 2022  && echo; [[ -z "
-000149f0: 2473 2220 5d5d 207c 7c20 5b5b 2022 2473  $s" ]] || [[ "$s
-00014a00: 2220 3d20 2274 6572 6d69 6e61 7465 6422  " = "terminated"
-00014a10: 205d 5d20 7c7c 205b 5b20 2224 7322 203d   ]] || [[ "$s" =
-00014a20: 2022 7368 7574 7469 6e67 2d64 6f77 6e22   "shutting-down"
-00014a30: 205d 5d27 0a20 2020 2020 2020 2020 2020   ]]'.           
-00014a40: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00014a50: 2320 5465 7374 2063 616e 6365 6c6c 6174  # Test cancellat
-00014a60: 696f 6e20 6475 7269 6e67 2073 706f 7420  ion during spot 
-00014a70: 6a6f 6220 6973 2072 6563 6f76 6572 696e  job is recoverin
-00014a80: 672e 0a20 2020 2020 2020 2020 2020 2066  g..            f
-00014a90: 2773 6b79 2073 706f 7420 6c61 756e 6368  'sky spot launch
-00014aa0: 202d 2d63 6c6f 7564 2061 7773 202d 2d72   --cloud aws --r
-00014ab0: 6567 696f 6e20 7b72 6567 696f 6e7d 202d  egion {region} -
-00014ac0: 6e20 7b6e 616d 657d 2d33 2022 736c 6565  n {name}-3 "slee
-00014ad0: 7020 3130 3030 2220 202d 7920 2d64 272c  p 1000"  -y -d',
-00014ae0: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
-00014af0: 6565 7020 3330 3027 2c0a 2020 2020 2020  eep 300',.      
-00014b00: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
-00014b10: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
-00014b20: 207b 6e61 6d65 7d2d 3320 7c20 6865 6164   {name}-3 | head
-00014b30: 202d 6e31 207c 2067 7265 7020 2252 554e   -n1 | grep "RUN
-00014b40: 4e49 4e47 2227 2c0a 2020 2020 2020 2020  NING"',.        
-00014b50: 2020 2020 2320 5465 726d 696e 6174 6520      # Terminate 
-00014b60: 7468 6520 636c 7573 7465 7220 6d61 6e75  the cluster manu
-00014b70: 616c 6c79 2e0a 2020 2020 2020 2020 2020  ally..          
-00014b80: 2020 2866 2761 7773 2065 6332 2074 6572    (f'aws ec2 ter
-00014b90: 6d69 6e61 7465 2d69 6e73 7461 6e63 6573  minate-instances
-00014ba0: 202d 2d72 6567 696f 6e20 7b72 6567 696f   --region {regio
-00014bb0: 6e7d 202d 2d69 6e73 7461 6e63 652d 6964  n} --instance-id
-00014bc0: 7320 2428 270a 2020 2020 2020 2020 2020  s $('.          
-00014bd0: 2020 2066 2761 7773 2065 6332 2064 6573     f'aws ec2 des
-00014be0: 6372 6962 652d 696e 7374 616e 6365 7320  cribe-instances 
-00014bf0: 2d2d 7265 6769 6f6e 207b 7265 6769 6f6e  --region {region
-00014c00: 7d20 270a 2020 2020 2020 2020 2020 2020  } '.            
-00014c10: 2066 272d 2d66 696c 7465 7273 204e 616d   f'--filters Nam
-00014c20: 653d 7461 673a 7261 792d 636c 7573 7465  e=tag:ray-cluste
-00014c30: 722d 6e61 6d65 2c56 616c 7565 733d 7b6e  r-name,Values={n
-00014c40: 616d 657d 2d33 2d2a 2027 0a20 2020 2020  ame}-3-* '.     
-00014c50: 2020 2020 2020 2020 6627 2d2d 7175 6572          f'--quer
-00014c60: 7920 5265 7365 7276 6174 696f 6e73 5b5d  y Reservations[]
-00014c70: 2e49 6e73 7461 6e63 6573 5b5d 2e49 6e73  .Instances[].Ins
-00014c80: 7461 6e63 6549 6420 270a 2020 2020 2020  tanceId '.      
-00014c90: 2020 2020 2020 2027 2d2d 6f75 7470 7574         '--output
-00014ca0: 2074 6578 7429 2729 2c0a 2020 2020 2020   text)'),.      
-00014cb0: 2020 2020 2020 2773 6c65 6570 2031 3230        'sleep 120
-00014cc0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-00014cd0: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
-00014ce0: 4954 7d7c 2067 7265 7020 7b6e 616d 657d  IT}| grep {name}
-00014cf0: 2d33 207c 2068 6561 6420 2d6e 3120 7c20  -3 | head -n1 | 
-00014d00: 6772 6570 2022 5245 434f 5645 5249 4e47  grep "RECOVERING
-00014d10: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-00014d20: 5f53 504f 545f 4341 4e43 454c 5f57 4149  _SPOT_CANCEL_WAI
-00014d30: 542e 666f 726d 6174 286a 6f62 5f6e 616d  T.format(job_nam
-00014d40: 653d 6627 7b6e 616d 657d 2d33 2729 2c0a  e=f'{name}-3'),.
-00014d50: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
-00014d60: 6570 2035 272c 0a20 2020 2020 2020 2020  ep 5',.         
-00014d70: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
-00014d80: 455f 5741 4954 7d7c 2067 7265 7020 7b6e  E_WAIT}| grep {n
-00014d90: 616d 657d 2d33 207c 2068 6561 6420 2d6e  ame}-3 | head -n
-00014da0: 3120 7c20 6772 6570 2022 4341 4e43 454c  1 | grep "CANCEL
-00014db0: 4c49 4e47 5c7c 4341 4e43 454c 4c45 4422  LING\|CANCELLED"
-00014dc0: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-00014dd0: 736c 6565 7020 3132 3027 2c0a 2020 2020  sleep 120',.    
-00014de0: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
-00014df0: 5f51 5545 5545 5f57 4149 547d 7c20 6772  _QUEUE_WAIT}| gr
-00014e00: 6570 207b 6e61 6d65 7d2d 3320 7c20 6865  ep {name}-3 | he
-00014e10: 6164 202d 6e31 207c 2067 7265 7020 2243  ad -n1 | grep "C
-00014e20: 414e 4345 4c4c 4544 2227 2c0a 2020 2020  ANCELLED"',.    
-00014e30: 2020 2020 2020 2020 2320 5468 6520 636c          # The cl
-00014e40: 7573 7465 7220 7368 6f75 6c64 2062 6520  uster should be 
-00014e50: 7465 726d 696e 6174 6564 2028 7368 7574  terminated (shut
-00014e60: 7469 6e67 2d64 6f77 6e29 2061 6674 6572  ting-down) after
-00014e70: 2063 616e 6365 6c6c 6174 696f 6e2e 2057   cancellation. W
-00014e80: 6520 646f 6e27 7420 7573 6520 7468 6520  e don't use the 
-00014e90: 603d 6020 6f70 6572 6174 6f72 2068 6572  `=` operator her
-00014ea0: 6520 6265 6361 7573 650a 2020 2020 2020  e because.      
-00014eb0: 2020 2020 2020 2320 7468 6572 6520 6361        # there ca
-00014ec0: 6e20 6265 206d 756c 7469 706c 6520 564d  n be multiple VM
-00014ed0: 2077 6974 6820 7468 6520 7361 6d65 206e   with the same n
-00014ee0: 616d 6520 6475 6520 746f 2074 6865 2072  ame due to the r
-00014ef0: 6563 6f76 6572 792e 0a20 2020 2020 2020  ecovery..       
-00014f00: 2020 2020 2028 6627 733d 2428 6177 7320       (f's=$(aws 
-00014f10: 6563 3220 6465 7363 7269 6265 2d69 6e73  ec2 describe-ins
-00014f20: 7461 6e63 6573 202d 2d72 6567 696f 6e20  tances --region 
-00014f30: 7b72 6567 696f 6e7d 2027 0a20 2020 2020  {region} '.     
-00014f40: 2020 2020 2020 2020 6627 2d2d 6669 6c74          f'--filt
-00014f50: 6572 7320 4e61 6d65 3d74 6167 3a72 6179  ers Name=tag:ray
-00014f60: 2d63 6c75 7374 6572 2d6e 616d 652c 5661  -cluster-name,Va
-00014f70: 6c75 6573 3d7b 6e61 6d65 7d2d 332d 2a20  lues={name}-3-* 
-00014f80: 270a 2020 2020 2020 2020 2020 2020 2066  '.             f
-00014f90: 272d 2d71 7565 7279 2052 6573 6572 7661  '--query Reserva
-00014fa0: 7469 6f6e 735b 5d2e 496e 7374 616e 6365  tions[].Instance
-00014fb0: 735b 5d2e 5374 6174 655b 5d2e 4e61 6d65  s[].State[].Name
-00014fc0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-00014fd0: 272d 2d6f 7574 7075 7420 7465 7874 2920  '--output text) 
-00014fe0: 2626 2065 6368 6f20 2224 7322 2026 2620  && echo "$s" && 
-00014ff0: 6563 686f 3b20 5b5b 202d 7a20 2224 7322  echo; [[ -z "$s"
-00015000: 205d 5d20 7c7c 2065 6368 6f20 2224 7322   ]] || echo "$s"
-00015010: 207c 2067 7265 7020 2d76 202d 4520 2270   | grep -v -E "p
-00015020: 656e 6469 6e67 7c72 756e 6e69 6e67 7c73  ending|running|s
-00015030: 746f 7070 6564 7c73 746f 7070 696e 6722  topped|stopping"
-00015040: 270a 2020 2020 2020 2020 2020 2020 292c  '.            ),
-00015050: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
-00015060: 2020 2020 7469 6d65 6f75 743d 3235 202a      timeout=25 *
-00015070: 2036 3029 0a20 2020 2072 756e 5f6f 6e65   60).    run_one
-00015080: 5f74 6573 7428 7465 7374 290a 0a0a 4070  _test(test)...@p
-00015090: 7974 6573 742e 6d61 726b 2e67 6370 0a40  ytest.mark.gcp.@
-000150a0: 7079 7465 7374 2e6d 6172 6b2e 6d61 6e61  pytest.mark.mana
-000150b0: 6765 645f 7370 6f74 0a64 6566 2074 6573  ged_spot.def tes
-000150c0: 745f 7370 6f74 5f63 616e 6365 6c6c 6174  t_spot_cancellat
-000150d0: 696f 6e5f 6763 7028 293a 0a20 2020 206e  ion_gcp():.    n
-000150e0: 616d 6520 3d20 5f67 6574 5f63 6c75 7374  ame = _get_clust
-000150f0: 6572 5f6e 616d 6528 290a 2020 2020 7a6f  er_name().    zo
-00015100: 6e65 203d 2027 7573 2d77 6573 7433 2d62  ne = 'us-west3-b
-00015110: 270a 2020 2020 7175 6572 795f 7374 6174  '.    query_stat
-00015120: 655f 636d 6420 3d20 2827 6763 6c6f 7564  e_cmd = ('gcloud
-00015130: 2063 6f6d 7075 7465 2069 6e73 7461 6e63   compute instanc
-00015140: 6573 206c 6973 7420 270a 2020 2020 2020  es list '.      
-00015150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015160: 2066 272d 2d66 696c 7465 723d 2228 6c61   f'--filter="(la
-00015170: 6265 6c73 2e72 6179 2d63 6c75 7374 6572  bels.ray-cluster
-00015180: 2d6e 616d 653a 7b6e 616d 657d 2922 2027  -name:{name})" '
-00015190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000151a0: 2020 2020 2020 2020 272d 2d66 6f72 6d61          '--forma
-000151b0: 743d 2276 616c 7565 2873 7461 7475 7329  t="value(status)
-000151c0: 2227 290a 2020 2020 7175 6572 795f 636d  "').    query_cm
-000151d0: 6420 3d20 2866 2767 636c 6f75 6420 636f  d = (f'gcloud co
-000151e0: 6d70 7574 6520 696e 7374 616e 6365 7320  mpute instances 
-000151f0: 6c69 7374 202d 2d66 696c 7465 723d 270a  list --filter='.
-00015200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015210: 2066 2722 286c 6162 656c 732e 7261 792d   f'"(labels.ray-
-00015220: 636c 7573 7465 722d 6e61 6d65 3a7b 6e61  cluster-name:{na
-00015230: 6d65 7d29 2220 270a 2020 2020 2020 2020  me})" '.        
-00015240: 2020 2020 2020 2020 2066 272d 2d7a 6f6e           f'--zon
-00015250: 6573 3d7b 7a6f 6e65 7d20 2d2d 666f 726d  es={zone} --form
-00015260: 6174 3d22 7661 6c75 6528 6e61 6d65 2922  at="value(name)"
-00015270: 2729 0a20 2020 2074 6572 6d69 6e61 7465  ').    terminate
-00015280: 5f63 6d64 203d 2028 6627 6763 6c6f 7564  _cmd = (f'gcloud
-00015290: 2063 6f6d 7075 7465 2069 6e73 7461 6e63   compute instanc
-000152a0: 6573 2064 656c 6574 6520 2d2d 7a6f 6e65  es delete --zone
-000152b0: 3d7b 7a6f 6e65 7d27 0a20 2020 2020 2020  ={zone}'.       
-000152c0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-000152d0: 202d 2d71 7569 6574 2024 287b 7175 6572   --quiet $({quer
-000152e0: 795f 636d 647d 2927 290a 2020 2020 7465  y_cmd})').    te
-000152f0: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
-00015300: 2020 2027 7370 6f74 5f63 616e 6365 6c6c     'spot_cancell
-00015310: 6174 696f 6e5f 6763 7027 2c0a 2020 2020  ation_gcp',.    
-00015320: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-00015330: 2020 2320 5465 7374 2063 616e 6365 6c6c    # Test cancell
-00015340: 6174 696f 6e20 6475 7269 6e67 2073 706f  ation during spo
-00015350: 7420 636c 7573 7465 7220 6265 696e 6720  t cluster being 
-00015360: 6c61 756e 6368 6564 2e0a 2020 2020 2020  launched..      
-00015370: 2020 2020 2020 6627 736b 7920 7370 6f74        f'sky spot
-00015380: 206c 6175 6e63 6820 2d2d 636c 6f75 6420   launch --cloud 
-00015390: 6763 7020 2d2d 7a6f 6e65 207b 7a6f 6e65  gcp --zone {zone
-000153a0: 7d20 2d6e 207b 6e61 6d65 7d20 2273 6c65  } -n {name} "sle
-000153b0: 6570 2031 3030 3022 2020 2d79 202d 6427  ep 1000"  -y -d'
-000153c0: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
-000153d0: 6c65 6570 2036 3027 2c0a 2020 2020 2020  leep 60',.      
-000153e0: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
-000153f0: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
-00015400: 207b 6e61 6d65 7d20 7c20 6865 6164 202d   {name} | head -
-00015410: 6e31 207c 2067 7265 7020 2253 5441 5254  n1 | grep "START
-00015420: 494e 4722 272c 0a20 2020 2020 2020 2020  ING"',.         
-00015430: 2020 205f 5350 4f54 5f43 414e 4345 4c5f     _SPOT_CANCEL_
-00015440: 5741 4954 2e66 6f72 6d61 7428 6a6f 625f  WAIT.format(job_
-00015450: 6e61 6d65 3d6e 616d 6529 2c0a 2020 2020  name=name),.    
-00015460: 2020 2020 2020 2020 2773 6c65 6570 2035          'sleep 5
-00015470: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-00015480: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
-00015490: 4954 7d7c 2067 7265 7020 7b6e 616d 657d  IT}| grep {name}
-000154a0: 207c 2068 6561 6420 2d6e 3120 7c20 6772   | head -n1 | gr
-000154b0: 6570 2022 4341 4e43 454c 4c49 4e47 5c7c  ep "CANCELLING\|
-000154c0: 4341 4e43 454c 4c45 4422 272c 0a20 2020  CANCELLED"',.   
-000154d0: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
-000154e0: 3132 3027 2c0a 2020 2020 2020 2020 2020  120',.          
-000154f0: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
-00015500: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
-00015510: 6d65 7d20 7c20 6865 6164 202d 6e31 207c  me} | head -n1 |
-00015520: 2067 7265 7020 2243 414e 4345 4c4c 4544   grep "CANCELLED
-00015530: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-00015540: 2320 5465 7374 2063 616e 6365 6c6c 696e  # Test cancellin
-00015550: 6720 7468 6520 7370 6f74 2063 6c75 7374  g the spot clust
-00015560: 6572 2064 7572 696e 6720 7370 6f74 206a  er during spot j
-00015570: 6f62 2062 6569 6e67 2073 6574 7570 2e0a  ob being setup..
-00015580: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-00015590: 7920 7370 6f74 206c 6175 6e63 6820 2d2d  y spot launch --
-000155a0: 636c 6f75 6420 6763 7020 2d2d 7a6f 6e65  cloud gcp --zone
-000155b0: 207b 7a6f 6e65 7d20 2d6e 207b 6e61 6d65   {zone} -n {name
-000155c0: 7d2d 3220 7465 7374 732f 7465 7374 5f79  }-2 tests/test_y
-000155d0: 616d 6c73 2f74 6573 745f 6c6f 6e67 5f73  amls/test_long_s
-000155e0: 6574 7570 2e79 616d 6c20 202d 7920 2d64  etup.yaml  -y -d
-000155f0: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-00015600: 736c 6565 7020 3330 3027 2c0a 2020 2020  sleep 300',.    
-00015610: 2020 2020 2020 2020 5f53 504f 545f 4341          _SPOT_CA
-00015620: 4e43 454c 5f57 4149 542e 666f 726d 6174  NCEL_WAIT.format
-00015630: 286a 6f62 5f6e 616d 653d 6627 7b6e 616d  (job_name=f'{nam
-00015640: 657d 2d32 2729 2c0a 2020 2020 2020 2020  e}-2'),.        
-00015650: 2020 2020 2773 6c65 6570 2035 272c 0a20      'sleep 5',. 
-00015660: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
-00015670: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
-00015680: 2067 7265 7020 7b6e 616d 657d 2d32 207c   grep {name}-2 |
-00015690: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
-000156a0: 2022 4341 4e43 454c 4c49 4e47 5c7c 4341   "CANCELLING\|CA
-000156b0: 4e43 454c 4c45 4422 272c 0a20 2020 2020  NCELLED"',.     
-000156c0: 2020 2020 2020 2027 736c 6565 7020 3132         'sleep 12
-000156d0: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
-000156e0: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
-000156f0: 4149 547d 7c20 6772 6570 207b 6e61 6d65  AIT}| grep {name
-00015700: 7d2d 3220 7c20 6865 6164 202d 6e31 207c  }-2 | head -n1 |
-00015710: 2067 7265 7020 2243 414e 4345 4c4c 4544   grep "CANCELLED
-00015720: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-00015730: 2320 5465 7374 2063 616e 6365 6c6c 6174  # Test cancellat
-00015740: 696f 6e20 6475 7269 6e67 2073 706f 7420  ion during spot 
-00015750: 6a6f 6220 6973 2072 6563 6f76 6572 696e  job is recoverin
-00015760: 672e 0a20 2020 2020 2020 2020 2020 2066  g..            f
-00015770: 2773 6b79 2073 706f 7420 6c61 756e 6368  'sky spot launch
-00015780: 202d 2d63 6c6f 7564 2067 6370 202d 2d7a   --cloud gcp --z
-00015790: 6f6e 6520 7b7a 6f6e 657d 202d 6e20 7b6e  one {zone} -n {n
-000157a0: 616d 657d 2d33 2022 736c 6565 7020 3130  ame}-3 "sleep 10
-000157b0: 3030 2220 202d 7920 2d64 272c 0a20 2020  00"  -y -d',.   
-000157c0: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
-000157d0: 3330 3027 2c0a 2020 2020 2020 2020 2020  300',.          
-000157e0: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
-000157f0: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
-00015800: 6d65 7d2d 3320 7c20 6865 6164 202d 6e31  me}-3 | head -n1
-00015810: 207c 2067 7265 7020 2252 554e 4e49 4e47   | grep "RUNNING
-00015820: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-00015830: 2320 5465 726d 696e 6174 6520 7468 6520  # Terminate the 
-00015840: 636c 7573 7465 7220 6d61 6e75 616c 6c79  cluster manually
-00015850: 2e0a 2020 2020 2020 2020 2020 2020 7465  ..            te
-00015860: 726d 696e 6174 655f 636d 642c 0a20 2020  rminate_cmd,.   
-00015870: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
-00015880: 3130 3027 2c0a 2020 2020 2020 2020 2020  100',.          
-00015890: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
-000158a0: 5f57 4149 547d 7c20 6772 6570 207b 6e61  _WAIT}| grep {na
-000158b0: 6d65 7d2d 3320 7c20 6865 6164 202d 6e31  me}-3 | head -n1
-000158c0: 207c 2067 7265 7020 2252 4543 4f56 4552   | grep "RECOVER
-000158d0: 494e 4722 272c 0a20 2020 2020 2020 2020  ING"',.         
-000158e0: 2020 205f 5350 4f54 5f43 414e 4345 4c5f     _SPOT_CANCEL_
-000158f0: 5741 4954 2e66 6f72 6d61 7428 6a6f 625f  WAIT.format(job_
-00015900: 6e61 6d65 3d66 277b 6e61 6d65 7d2d 3327  name=f'{name}-3'
-00015910: 292c 0a20 2020 2020 2020 2020 2020 2027  ),.            '
-00015920: 736c 6565 7020 3527 2c0a 2020 2020 2020  sleep 5',.      
-00015930: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
-00015940: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
-00015950: 207b 6e61 6d65 7d2d 3320 7c20 6865 6164   {name}-3 | head
-00015960: 202d 6e31 207c 2067 7265 7020 2243 414e   -n1 | grep "CAN
-00015970: 4345 4c4c 494e 475c 7c43 414e 4345 4c4c  CELLING\|CANCELL
-00015980: 4544 2227 2c0a 2020 2020 2020 2020 2020  ED"',.          
-00015990: 2020 2773 6c65 6570 2031 3230 272c 0a20    'sleep 120',. 
-000159a0: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
-000159b0: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
-000159c0: 2067 7265 7020 7b6e 616d 657d 2d33 207c   grep {name}-3 |
-000159d0: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
-000159e0: 2022 4341 4e43 454c 4c45 4422 272c 0a20   "CANCELLED"',. 
-000159f0: 2020 2020 2020 2020 2020 2023 2054 6865             # The
-00015a00: 2063 6c75 7374 6572 2073 686f 756c 6420   cluster should 
-00015a10: 6265 2074 6572 6d69 6e61 7465 6420 2853  be terminated (S
-00015a20: 544f 5050 494e 4729 2061 6674 6572 2063  TOPPING) after c
-00015a30: 616e 6365 6c6c 6174 696f 6e2e 2057 6520  ancellation. We 
-00015a40: 646f 6e27 7420 7573 6520 7468 6520 603d  don't use the `=
-00015a50: 6020 6f70 6572 6174 6f72 2068 6572 6520  ` operator here 
-00015a60: 6265 6361 7573 650a 2020 2020 2020 2020  because.        
-00015a70: 2020 2020 2320 7468 6572 6520 6361 6e20      # there can 
-00015a80: 6265 206d 756c 7469 706c 6520 564d 2077  be multiple VM w
-00015a90: 6974 6820 7468 6520 7361 6d65 206e 616d  ith the same nam
-00015aa0: 6520 6475 6520 746f 2074 6865 2072 6563  e due to the rec
-00015ab0: 6f76 6572 792e 0a20 2020 2020 2020 2020  overy..         
-00015ac0: 2020 2028 6627 733d 2428 7b71 7565 7279     (f's=$({query
-00015ad0: 5f73 7461 7465 5f63 6d64 7d29 2026 2620  _state_cmd}) && 
-00015ae0: 6563 686f 2022 2473 2220 2626 2065 6368  echo "$s" && ech
-00015af0: 6f3b 205b 5b20 2d7a 2022 2473 2220 5d5d  o; [[ -z "$s" ]]
-00015b00: 207c 7c20 6563 686f 2022 2473 2220 7c20   || echo "$s" | 
-00015b10: 6772 6570 202d 7620 2d45 2022 5052 4f56  grep -v -E "PROV
-00015b20: 4953 494f 4e49 4e47 7c53 5441 4749 4e47  ISIONING|STAGING
-00015b30: 7c52 554e 4e49 4e47 7c52 4550 4149 5249  |RUNNING|REPAIRI
-00015b40: 4e47 7c54 4552 4d49 4e41 5445 447c 5355  NG|TERMINATED|SU
-00015b50: 5350 454e 4449 4e47 7c53 5553 5045 4e44  SPENDING|SUSPEND
-00015b60: 4544 7c53 5553 5045 4e44 4544 2227 0a20  ED|SUSPENDED"'. 
-00015b70: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00015b80: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-00015b90: 2074 696d 656f 7574 3d32 3520 2a20 3630   timeout=25 * 60
-00015ba0: 290a 2020 2020 7275 6e5f 6f6e 655f 7465  ).    run_one_te
-00015bb0: 7374 2874 6573 7429 0a0a 0a23 202d 2d2d  st(test)...# ---
-00015bc0: 2d2d 2d2d 2d2d 2d20 5465 7374 696e 6720  ------- Testing 
-00015bd0: 7374 6f72 6167 6520 666f 7220 6d61 6e61  storage for mana
-00015be0: 6765 6420 7370 6f74 202d 2d2d 2d2d 2d2d  ged spot -------
-00015bf0: 2d2d 2d0a 4070 7974 6573 742e 6d61 726b  ---.@pytest.mark
-00015c00: 2e6e 6f5f 6c61 6d62 6461 5f63 6c6f 7564  .no_lambda_cloud
-00015c10: 2020 2320 4c61 6d62 6461 2043 6c6f 7564    # Lambda Cloud
-00015c20: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
-00015c30: 7420 7370 6f74 2069 6e73 7461 6e63 6573  t spot instances
-00015c40: 0a40 7079 7465 7374 2e6d 6172 6b2e 6e6f  .@pytest.mark.no
-00015c50: 5f69 626d 2020 2320 4942 4d20 436c 6f75  _ibm  # IBM Clou
-00015c60: 6420 646f 6573 206e 6f74 2073 7570 706f  d does not suppo
-00015c70: 7274 2073 706f 7420 696e 7374 616e 6365  rt spot instance
-00015c80: 730a 4070 7974 6573 742e 6d61 726b 2e6e  s.@pytest.mark.n
-00015c90: 6f5f 7363 7020 2023 2053 4350 2064 6f65  o_scp  # SCP doe
-00015ca0: 7320 6e6f 7420 7375 7070 6f72 7420 7370  s not support sp
-00015cb0: 6f74 2069 6e73 7461 6e63 6573 0a40 7079  ot instances.@py
-00015cc0: 7465 7374 2e6d 6172 6b2e 6d61 6e61 6765  test.mark.manage
-00015cd0: 645f 7370 6f74 0a64 6566 2074 6573 745f  d_spot.def test_
-00015ce0: 7370 6f74 5f73 746f 7261 6765 2867 656e  spot_storage(gen
-00015cf0: 6572 6963 5f63 6c6f 7564 3a20 7374 7229  eric_cloud: str)
-00015d00: 3a0a 2020 2020 2222 2254 6573 7420 7374  :.    """Test st
-00015d10: 6f72 6167 6520 7769 7468 206d 616e 6167  orage with manag
-00015d20: 6564 2073 706f 7422 2222 0a20 2020 206e  ed spot""".    n
-00015d30: 616d 6520 3d20 5f67 6574 5f63 6c75 7374  ame = _get_clust
-00015d40: 6572 5f6e 616d 6528 290a 2020 2020 7961  er_name().    ya
-00015d50: 6d6c 5f73 7472 203d 2070 6174 686c 6962  ml_str = pathlib
-00015d60: 2e50 6174 6828 0a20 2020 2020 2020 2027  .Path(.        '
-00015d70: 6578 616d 706c 6573 2f6d 616e 6167 6564  examples/managed
-00015d80: 5f73 706f 745f 7769 7468 5f73 746f 7261  _spot_with_stora
-00015d90: 6765 2e79 616d 6c27 292e 7265 6164 5f74  ge.yaml').read_t
-00015da0: 6578 7428 290a 2020 2020 7374 6f72 6167  ext().    storag
-00015db0: 655f 6e61 6d65 203d 2066 2773 6b79 2d74  e_name = f'sky-t
-00015dc0: 6573 742d 7b69 6e74 2874 696d 652e 7469  est-{int(time.ti
-00015dd0: 6d65 2829 297d 270a 2020 2020 7961 6d6c  me())}'.    yaml
-00015de0: 5f73 7472 203d 2079 616d 6c5f 7374 722e  _str = yaml_str.
-00015df0: 7265 706c 6163 6528 2773 6b79 2d77 6f72  replace('sky-wor
-00015e00: 6b64 6972 2d7a 6877 7527 2c20 7374 6f72  kdir-zhwu', stor
-00015e10: 6167 655f 6e61 6d65 290a 2020 2020 7769  age_name).    wi
-00015e20: 7468 2074 656d 7066 696c 652e 4e61 6d65  th tempfile.Name
-00015e30: 6454 656d 706f 7261 7279 4669 6c65 2873  dTemporaryFile(s
-00015e40: 7566 6669 783d 272e 7961 6d6c 272c 206d  uffix='.yaml', m
-00015e50: 6f64 653d 2777 2729 2061 7320 663a 0a20  ode='w') as f:. 
-00015e60: 2020 2020 2020 2066 2e77 7269 7465 2879         f.write(y
-00015e70: 616d 6c5f 7374 7229 0a20 2020 2020 2020  aml_str).       
-00015e80: 2066 2e66 6c75 7368 2829 0a20 2020 2020   f.flush().     
-00015e90: 2020 2066 696c 655f 7061 7468 203d 2066     file_path = f
-00015ea0: 2e6e 616d 650a 2020 2020 2020 2020 7465  .name.        te
-00015eb0: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
-00015ec0: 2020 2020 2020 2027 7370 6f74 5f73 746f         'spot_sto
-00015ed0: 7261 6765 272c 0a20 2020 2020 2020 2020  rage',.         
-00015ee0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-00015ef0: 2020 2020 202a 7374 6f72 6167 655f 7365       *storage_se
-00015f00: 7475 705f 636f 6d6d 616e 6473 2c0a 2020  tup_commands,.  
-00015f10: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-00015f20: 736b 7920 7370 6f74 206c 6175 6e63 6820  sky spot launch 
-00015f30: 2d6e 207b 6e61 6d65 7d20 2d2d 636c 6f75  -n {name} --clou
-00015f40: 6420 7b67 656e 6572 6963 5f63 6c6f 7564  d {generic_cloud
-00015f50: 7d20 7b66 696c 655f 7061 7468 7d20 2d79  } {file_path} -y
-00015f60: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00015f70: 2020 2027 736c 6565 7020 3630 272c 2020     'sleep 60',  
-00015f80: 2320 5761 6974 2074 6865 2073 706f 7420  # Wait the spot 
-00015f90: 7175 6575 6520 746f 2062 6520 7570 6461  queue to be upda
-00015fa0: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
-00015fb0: 2020 2020 6627 7b5f 5350 4f54 5f51 5545      f'{_SPOT_QUE
-00015fc0: 5545 5f57 4149 547d 7c20 6772 6570 207b  UE_WAIT}| grep {
-00015fd0: 6e61 6d65 7d20 7c20 6772 6570 2053 5543  name} | grep SUC
-00015fe0: 4345 4544 4544 272c 0a20 2020 2020 2020  CEEDED',.       
-00015ff0: 2020 2020 2020 2020 2066 275b 2024 2861           f'[ $(a
-00016000: 7773 2073 3361 7069 206c 6973 742d 6275  ws s3api list-bu
-00016010: 636b 6574 7320 2d2d 7175 6572 7920 2242  ckets --query "B
-00016020: 7563 6b65 7473 5b3f 636f 6e74 6169 6e73  uckets[?contains
-00016030: 284e 616d 652c 205c 277b 7374 6f72 6167  (Name, \'{storag
-00016040: 655f 6e61 6d65 7d5c 2729 5d2e 4e61 6d65  e_name}\')].Name
-00016050: 2220 2d2d 6f75 7470 7574 2074 6578 7420  " --output text 
-00016060: 7c20 7763 202d 6c29 202d 6571 2030 205d  | wc -l) -eq 0 ]
-00016070: 270a 2020 2020 2020 2020 2020 2020 5d2c  '.            ],
-00016080: 0a20 2020 2020 2020 2020 2020 205f 5350  .            _SP
-00016090: 4f54 5f43 414e 4345 4c5f 5741 4954 2e66  OT_CANCEL_WAIT.f
-000160a0: 6f72 6d61 7428 6a6f 625f 6e61 6d65 3d6e  ormat(job_name=n
-000160b0: 616d 6529 2c0a 2020 2020 2020 2020 2020  ame),.          
-000160c0: 2020 2320 496e 6372 6561 7365 2074 696d    # Increase tim
-000160d0: 656f 7574 2073 696e 6365 2073 6b79 2073  eout since sky s
-000160e0: 706f 7420 7175 6575 6520 2d72 2063 616e  pot queue -r can
-000160f0: 2062 6520 626c 6f63 6b65 6420 6279 206f   be blocked by o
-00016100: 7468 6572 2073 706f 7420 7465 7374 732e  ther spot tests.
-00016110: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
-00016120: 656f 7574 3d32 3020 2a20 3630 2c0a 2020  eout=20 * 60,.  
-00016130: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00016140: 7275 6e5f 6f6e 655f 7465 7374 2874 6573  run_one_test(tes
-00016150: 7429 0a0a 0a23 202d 2d2d 2d2d 2d2d 2d2d  t)...# ---------
-00016160: 2d20 5465 7374 696e 6720 7370 6f74 2054  - Testing spot T
-00016170: 5055 202d 2d2d 2d2d 2d2d 2d2d 2d0a 4070  PU ----------.@p
-00016180: 7974 6573 742e 6d61 726b 2e67 6370 0a40  ytest.mark.gcp.@
-00016190: 7079 7465 7374 2e6d 6172 6b2e 6d61 6e61  pytest.mark.mana
-000161a0: 6765 645f 7370 6f74 0a64 6566 2074 6573  ged_spot.def tes
-000161b0: 745f 7370 6f74 5f74 7075 2829 3a0a 2020  t_spot_tpu():.  
-000161c0: 2020 2222 2254 6573 7420 6d61 6e61 6765    """Test manage
-000161d0: 6420 7370 6f74 206f 6e20 5450 552e 2222  d spot on TPU.""
-000161e0: 220a 2020 2020 6e61 6d65 203d 205f 6765  ".    name = _ge
-000161f0: 745f 636c 7573 7465 725f 6e61 6d65 2829  t_cluster_name()
-00016200: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
-00016210: 280a 2020 2020 2020 2020 2774 6573 742d  (.        'test-
-00016220: 7370 6f74 2d74 7075 272c 0a20 2020 2020  spot-tpu',.     
-00016230: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-00016240: 2066 2773 6b79 2073 706f 7420 6c61 756e   f'sky spot laun
-00016250: 6368 202d 6e20 7b6e 616d 657d 2065 7861  ch -n {name} exa
-00016260: 6d70 6c65 732f 7470 752f 7470 7576 6d5f  mples/tpu/tpuvm_
-00016270: 6d6e 6973 742e 7961 6d6c 202d 7920 2d64  mnist.yaml -y -d
-00016280: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-00016290: 736c 6565 7020 3527 2c0a 2020 2020 2020  sleep 5',.      
-000162a0: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
-000162b0: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
-000162c0: 207b 6e61 6d65 7d20 7c20 6865 6164 202d   {name} | head -
-000162d0: 6e31 207c 2067 7265 7020 5354 4152 5449  n1 | grep STARTI
-000162e0: 4e47 272c 0a20 2020 2020 2020 2020 2020  NG',.           
-000162f0: 2027 736c 6565 7020 3732 3027 2c20 2023   'sleep 720',  #
-00016300: 2054 5055 2074 616b 6573 2061 2077 6869   TPU takes a whi
-00016310: 6c65 2074 6f20 6c61 756e 6368 0a20 2020  le to launch.   
-00016320: 2020 2020 2020 2020 2066 277b 5f53 504f           f'{_SPO
-00016330: 545f 5155 4555 455f 5741 4954 7d7c 2067  T_QUEUE_WAIT}| g
-00016340: 7265 7020 7b6e 616d 657d 207c 2068 6561  rep {name} | hea
-00016350: 6420 2d6e 3120 7c20 6772 6570 2022 5255  d -n1 | grep "RU
-00016360: 4e4e 494e 475c 7c53 5543 4345 4544 4544  NNING\|SUCCEEDED
-00016370: 2227 2c0a 2020 2020 2020 2020 5d2c 0a20  "',.        ],. 
-00016380: 2020 2020 2020 205f 5350 4f54 5f43 414e         _SPOT_CAN
-00016390: 4345 4c5f 5741 4954 2e66 6f72 6d61 7428  CEL_WAIT.format(
-000163a0: 6a6f 625f 6e61 6d65 3d6e 616d 6529 2c0a  job_name=name),.
-000163b0: 2020 2020 2020 2020 2320 496e 6372 6561          # Increa
-000163c0: 7365 2074 696d 656f 7574 2073 696e 6365  se timeout since
-000163d0: 2073 6b79 2073 706f 7420 7175 6575 6520   sky spot queue 
-000163e0: 2d72 2063 616e 2062 6520 626c 6f63 6b65  -r can be blocke
-000163f0: 6420 6279 206f 7468 6572 2073 706f 7420  d by other spot 
-00016400: 7465 7374 732e 0a20 2020 2020 2020 2074  tests..        t
-00016410: 696d 656f 7574 3d32 3020 2a20 3630 2c0a  imeout=20 * 60,.
-00016420: 2020 2020 290a 2020 2020 7275 6e5f 6f6e      ).    run_on
-00016430: 655f 7465 7374 2874 6573 7429 0a0a 0a23  e_test(test)...#
-00016440: 202d 2d2d 2d2d 2d2d 2d2d 2d20 5465 7374   ---------- Test
-00016450: 696e 6720 656e 7620 666f 7220 7370 6f74  ing env for spot
-00016460: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 4070 7974   ----------.@pyt
-00016470: 6573 742e 6d61 726b 2e6e 6f5f 6c61 6d62  est.mark.no_lamb
-00016480: 6461 5f63 6c6f 7564 2020 2320 4c61 6d62  da_cloud  # Lamb
-00016490: 6461 2043 6c6f 7564 2064 6f65 7320 6e6f  da Cloud does no
-000164a0: 7420 7375 7070 6f72 7420 7370 6f74 2069  t support spot i
-000164b0: 6e73 7461 6e63 6573 0a40 7079 7465 7374  nstances.@pytest
-000164c0: 2e6d 6172 6b2e 6e6f 5f69 626d 2020 2320  .mark.no_ibm  # 
-000164d0: 4942 4d20 436c 6f75 6420 646f 6573 206e  IBM Cloud does n
-000164e0: 6f74 2073 7570 706f 7274 2073 706f 7420  ot support spot 
-000164f0: 696e 7374 616e 6365 730a 4070 7974 6573  instances.@pytes
-00016500: 742e 6d61 726b 2e6e 6f5f 7363 7020 2023  t.mark.no_scp  #
-00016510: 2053 4350 2064 6f65 7320 6e6f 7420 7375   SCP does not su
-00016520: 7070 6f72 7420 7370 6f74 2069 6e73 7461  pport spot insta
-00016530: 6e63 6573 0a40 7079 7465 7374 2e6d 6172  nces.@pytest.mar
-00016540: 6b2e 6d61 6e61 6765 645f 7370 6f74 0a64  k.managed_spot.d
-00016550: 6566 2074 6573 745f 7370 6f74 5f69 6e6c  ef test_spot_inl
-00016560: 696e 655f 656e 7628 6765 6e65 7269 635f  ine_env(generic_
-00016570: 636c 6f75 643a 2073 7472 293a 0a20 2020  cloud: str):.   
-00016580: 2022 2222 5465 7374 2073 706f 7420 656e   """Test spot en
-00016590: 7622 2222 0a20 2020 206e 616d 6520 3d20  v""".    name = 
-000165a0: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
-000165b0: 6528 290a 2020 2020 7465 7374 203d 2054  e().    test = T
-000165c0: 6573 7428 0a20 2020 2020 2020 2027 7465  est(.        'te
-000165d0: 7374 2d73 706f 742d 696e 6c69 6e65 2d65  st-spot-inline-e
-000165e0: 6e76 272c 0a20 2020 2020 2020 205b 0a20  nv',.        [. 
-000165f0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-00016600: 2073 706f 7420 6c61 756e 6368 202d 6e20   spot launch -n 
-00016610: 7b6e 616d 657d 202d 7920 2d2d 636c 6f75  {name} -y --clou
-00016620: 6420 7b67 656e 6572 6963 5f63 6c6f 7564  d {generic_cloud
-00016630: 7d20 2d2d 656e 7620 5445 5354 5f45 4e56  } --env TEST_ENV
-00016640: 3d22 6865 6c6c 6f20 776f 726c 6422 202d  ="hello world" -
-00016650: 2d20 2228 5b5b 2021 202d 7a20 5c5c 225c  - "([[ ! -z \\"\
-00016660: 2454 4553 545f 454e 565c 5c22 205d 5d20  $TEST_ENV\\" ]] 
-00016670: 2626 205b 5b20 2120 2d7a 205c 5c22 5c24  && [[ ! -z \\"\$
-00016680: 534b 5950 494c 4f54 5f4e 4f44 455f 4950  SKYPILOT_NODE_IP
-00016690: 535c 5c22 205d 5d20 2626 205b 5b20 2120  S\\" ]] && [[ ! 
-000166a0: 2d7a 205c 5c22 5c24 534b 5950 494c 4f54  -z \\"\$SKYPILOT
-000166b0: 5f4e 4f44 455f 5241 4e4b 5c5c 2220 5d5d  _NODE_RANK\\" ]]
-000166c0: 2920 7c7c 2065 7869 7420 3122 272c 0a20  ) || exit 1"',. 
-000166d0: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
-000166e0: 7020 3230 272c 0a20 2020 2020 2020 2020  p 20',.         
-000166f0: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
-00016700: 455f 5741 4954 7d20 7c20 6772 6570 207b  E_WAIT} | grep {
-00016710: 6e61 6d65 7d20 7c20 6772 6570 2053 5543  name} | grep SUC
-00016720: 4345 4544 4544 272c 0a20 2020 2020 2020  CEEDED',.       
-00016730: 205d 2c0a 2020 2020 2020 2020 5f53 504f   ],.        _SPO
-00016740: 545f 4341 4e43 454c 5f57 4149 542e 666f  T_CANCEL_WAIT.fo
-00016750: 726d 6174 286a 6f62 5f6e 616d 653d 6e61  rmat(job_name=na
-00016760: 6d65 292c 0a20 2020 2020 2020 2023 2049  me),.        # I
-00016770: 6e63 7265 6173 6520 7469 6d65 6f75 7420  ncrease timeout 
-00016780: 7369 6e63 6520 736b 7920 7370 6f74 2071  since sky spot q
-00016790: 7565 7565 202d 7220 6361 6e20 6265 2062  ueue -r can be b
-000167a0: 6c6f 636b 6564 2062 7920 6f74 6865 7220  locked by other 
-000167b0: 7370 6f74 2074 6573 7473 2e0a 2020 2020  spot tests..    
-000167c0: 2020 2020 7469 6d65 6f75 743d 3230 202a      timeout=20 *
-000167d0: 2036 302c 0a20 2020 2029 0a20 2020 2072   60,.    ).    r
-000167e0: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
-000167f0: 290a 0a0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  )...# ----------
-00016800: 2054 6573 7469 6e67 2065 6e76 202d 2d2d   Testing env ---
-00016810: 2d2d 2d2d 2d2d 2d0a 6465 6620 7465 7374  -------.def test
-00016820: 5f69 6e6c 696e 655f 656e 7628 6765 6e65  _inline_env(gene
-00016830: 7269 635f 636c 6f75 643a 2073 7472 293a  ric_cloud: str):
-00016840: 0a20 2020 2022 2222 5465 7374 2065 6e76  .    """Test env
-00016850: 2222 220a 2020 2020 6e61 6d65 203d 205f  """.    name = _
-00016860: 6765 745f 636c 7573 7465 725f 6e61 6d65  get_cluster_name
-00016870: 2829 0a20 2020 2074 6573 7420 3d20 5465  ().    test = Te
-00016880: 7374 280a 2020 2020 2020 2020 2774 6573  st(.        'tes
-00016890: 742d 696e 6c69 6e65 2d65 6e76 272c 0a20  t-inline-env',. 
-000168a0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-000168b0: 2020 2020 2066 2773 6b79 206c 6175 6e63       f'sky launc
-000168c0: 6820 2d63 207b 6e61 6d65 7d20 2d79 202d  h -c {name} -y -
-000168d0: 2d63 6c6f 7564 207b 6765 6e65 7269 635f  -cloud {generic_
-000168e0: 636c 6f75 647d 202d 2d65 6e76 2054 4553  cloud} --env TES
-000168f0: 545f 454e 563d 2268 656c 6c6f 2077 6f72  T_ENV="hello wor
-00016900: 6c64 2220 2d2d 2022 285b 5b20 2120 2d7a  ld" -- "([[ ! -z
-00016910: 205c 5c22 5c24 5445 5354 5f45 4e56 5c5c   \\"\$TEST_ENV\\
-00016920: 2220 5d5d 2026 2620 5b5b 2021 202d 7a20  " ]] && [[ ! -z 
-00016930: 5c5c 225c 2453 4b59 5049 4c4f 545f 4e4f  \\"\$SKYPILOT_NO
-00016940: 4445 5f49 5053 5c5c 2220 5d5d 2026 2620  DE_IPS\\" ]] && 
-00016950: 5b5b 2021 202d 7a20 5c5c 225c 2453 4b59  [[ ! -z \\"\$SKY
-00016960: 5049 4c4f 545f 4e4f 4445 5f52 414e 4b5c  PILOT_NODE_RANK\
-00016970: 5c22 205d 5d29 207c 7c20 6578 6974 2031  \" ]]) || exit 1
-00016980: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-00016990: 6627 736b 7920 6c6f 6773 207b 6e61 6d65  f'sky logs {name
-000169a0: 7d20 3120 2d2d 7374 6174 7573 272c 0a20  } 1 --status',. 
-000169b0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-000169c0: 2065 7865 6320 7b6e 616d 657d 202d 2d65   exec {name} --e
-000169d0: 6e76 2054 4553 545f 454e 5632 3d22 7375  nv TEST_ENV2="su
-000169e0: 6363 6573 7322 2022 285b 5b20 2120 2d7a  ccess" "([[ ! -z
-000169f0: 205c 5c22 5c24 5445 5354 5f45 4e56 325c   \\"\$TEST_ENV2\
-00016a00: 5c22 205d 5d20 2626 205b 5b20 2120 2d7a  \" ]] && [[ ! -z
-00016a10: 205c 5c22 5c24 534b 5950 494c 4f54 5f4e   \\"\$SKYPILOT_N
-00016a20: 4f44 455f 4950 535c 5c22 205d 5d20 2626  ODE_IPS\\" ]] &&
-00016a30: 205b 5b20 2120 2d7a 205c 5c22 5c24 534b   [[ ! -z \\"\$SK
-00016a40: 5950 494c 4f54 5f4e 4f44 455f 5241 4e4b  YPILOT_NODE_RANK
-00016a50: 5c5c 2220 5d5d 2920 7c7c 2065 7869 7420  \\" ]]) || exit 
-00016a60: 3122 272c 0a20 2020 2020 2020 2020 2020  1"',.           
-00016a70: 2066 2773 6b79 206c 6f67 7320 7b6e 616d   f'sky logs {nam
-00016a80: 657d 2032 202d 2d73 7461 7475 7327 2c0a  e} 2 --status',.
-00016a90: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00016aa0: 2020 2066 2773 6b79 2064 6f77 6e20 2d79     f'sky down -y
-00016ab0: 207b 6e61 6d65 7d27 2c0a 2020 2020 290a   {name}',.    ).
-00016ac0: 2020 2020 7275 6e5f 6f6e 655f 7465 7374      run_one_test
-00016ad0: 2874 6573 7429 0a0a 0a23 202d 2d2d 2d2d  (test)...# -----
-00016ae0: 2d2d 2d2d 2d20 5465 7374 696e 6720 6375  ----- Testing cu
-00016af0: 7374 6f6d 2069 6d61 6765 202d 2d2d 2d2d  stom image -----
-00016b00: 2d2d 2d2d 2d0a 4070 7974 6573 742e 6d61  -----.@pytest.ma
-00016b10: 726b 2e61 7773 0a64 6566 2074 6573 745f  rk.aws.def test_
-00016b20: 6375 7374 6f6d 5f69 6d61 6765 2829 3a0a  custom_image():.
-00016b30: 2020 2020 2222 2254 6573 7420 6375 7374      """Test cust
-00016b40: 6f6d 2069 6d61 6765 2222 220a 2020 2020  om image""".    
-00016b50: 6e61 6d65 203d 205f 6765 745f 636c 7573  name = _get_clus
-00016b60: 7465 725f 6e61 6d65 2829 0a20 2020 2074  ter_name().    t
-00016b70: 6573 7420 3d20 5465 7374 280a 2020 2020  est = Test(.    
-00016b80: 2020 2020 2774 6573 742d 6375 7374 6f6d      'test-custom
-00016b90: 2d69 6d61 6765 272c 0a20 2020 2020 2020  -image',.       
-00016ba0: 205b 0a20 2020 2020 2020 2020 2020 2066   [.            f
-00016bb0: 2773 6b79 206c 6175 6e63 6820 2d63 207b  'sky launch -c {
-00016bc0: 6e61 6d65 7d20 2d2d 7265 7472 792d 756e  name} --retry-un
-00016bd0: 7469 6c2d 7570 202d 7920 6578 616d 706c  til-up -y exampl
-00016be0: 6573 2f63 7573 746f 6d5f 696d 6167 652e  es/custom_image.
-00016bf0: 7961 6d6c 272c 0a20 2020 2020 2020 2020  yaml',.         
-00016c00: 2020 2066 2773 6b79 206c 6f67 7320 7b6e     f'sky logs {n
-00016c10: 616d 657d 2031 202d 2d73 7461 7475 7327  ame} 1 --status'
-00016c20: 2c0a 2020 2020 2020 2020 5d2c 0a20 2020  ,.        ],.   
-00016c30: 2020 2020 2066 2773 6b79 2064 6f77 6e20       f'sky down 
-00016c40: 2d79 207b 6e61 6d65 7d27 2c0a 2020 2020  -y {name}',.    
-00016c50: 2020 2020 7469 6d65 6f75 743d 3330 202a      timeout=30 *
-00016c60: 2036 302c 0a20 2020 2029 0a20 2020 2072   60,.    ).    r
-00016c70: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
-00016c80: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
-00016c90: 2e73 6c6f 770a 6465 6620 7465 7374 5f61  .slow.def test_a
-00016ca0: 7a75 7265 5f73 7461 7274 5f73 746f 705f  zure_start_stop_
-00016cb0: 7477 6f5f 6e6f 6465 7328 293a 0a20 2020  two_nodes():.   
-00016cc0: 206e 616d 6520 3d20 5f67 6574 5f63 6c75   name = _get_clu
-00016cd0: 7374 6572 5f6e 616d 6528 290a 2020 2020  ster_name().    
-00016ce0: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
-00016cf0: 2020 2020 2027 617a 7572 652d 7374 6172       'azure-star
-00016d00: 742d 7374 6f70 2d74 776f 2d6e 6f64 6573  t-stop-two-nodes
-00016d10: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
-00016d20: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
-00016d30: 6175 6e63 6820 2d2d 6e75 6d2d 6e6f 6465  aunch --num-node
-00016d40: 733d 3220 2d79 202d 6320 7b6e 616d 657d  s=2 -y -c {name}
-00016d50: 2065 7861 6d70 6c65 732f 617a 7572 655f   examples/azure_
-00016d60: 7374 6172 745f 7374 6f70 2e79 616d 6c27  start_stop.yaml'
-00016d70: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-00016d80: 736b 7920 6578 6563 202d 2d6e 756d 2d6e  sky exec --num-n
-00016d90: 6f64 6573 3d32 207b 6e61 6d65 7d20 6578  odes=2 {name} ex
-00016da0: 616d 706c 6573 2f61 7a75 7265 5f73 7461  amples/azure_sta
-00016db0: 7274 5f73 746f 702e 7961 6d6c 272c 0a20  rt_stop.yaml',. 
-00016dc0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-00016dd0: 206c 6f67 7320 7b6e 616d 657d 2031 202d   logs {name} 1 -
-00016de0: 2d73 7461 7475 7327 2c20 2023 2045 6e73  -status',  # Ens
-00016df0: 7572 6520 7468 6520 6a6f 6220 7375 6363  ure the job succ
-00016e00: 6565 6465 642e 0a20 2020 2020 2020 2020  eeded..         
-00016e10: 2020 2066 2773 6b79 2073 746f 7020 2d79     f'sky stop -y
-00016e20: 207b 6e61 6d65 7d27 2c0a 2020 2020 2020   {name}',.      
-00016e30: 2020 2020 2020 6627 736b 7920 7374 6172        f'sky star
-00016e40: 7420 2d79 207b 6e61 6d65 7d27 2c0a 2020  t -y {name}',.  
+0000b350: 7b6e 616d 657d 272c 0a20 2020 2020 2020  {name}',.       
+0000b360: 2074 696d 656f 7574 3d32 3020 2a20 3630   timeout=20 * 60
+0000b370: 2c20 2023 2032 3020 6d69 6e73 0a20 2020  ,  # 20 mins.   
+0000b380: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
+0000b390: 6573 7428 7465 7374 290a 0a0a 2320 2d2d  est(test)...# --
+0000b3a0: 2d2d 2d2d 2d2d 2d2d 2053 7562 6d69 7474  -------- Submitt
+0000b3b0: 696e 6720 6d75 6c74 6970 6c65 2074 6173  ing multiple tas
+0000b3c0: 6b73 2074 6f20 7468 6520 7361 6d65 2063  ks to the same c
+0000b3d0: 6c75 7374 6572 2e20 2d2d 2d2d 2d2d 2d2d  luster. --------
+0000b3e0: 2d2d 0a40 7079 7465 7374 2e6d 6172 6b2e  --.@pytest.mark.
+0000b3f0: 6e6f 5f6c 616d 6264 615f 636c 6f75 6420  no_lambda_cloud 
+0000b400: 2023 204c 616d 6264 6120 436c 6f75 6420   # Lambda Cloud 
+0000b410: 646f 6573 206e 6f74 2068 6176 6520 4b38  does not have K8
+0000b420: 3020 6770 7573 0a40 7079 7465 7374 2e6d  0 gpus.@pytest.m
+0000b430: 6172 6b2e 6e6f 5f69 626d 2020 2320 4942  ark.no_ibm  # IB
+0000b440: 4d20 436c 6f75 6420 646f 6573 206e 6f74  M Cloud does not
+0000b450: 2068 6176 6520 4b38 3020 6770 7573 0a40   have K80 gpus.@
+0000b460: 7079 7465 7374 2e6d 6172 6b2e 6e6f 5f73  pytest.mark.no_s
+0000b470: 6370 2020 2320 5343 5020 646f 6573 206e  cp  # SCP does n
+0000b480: 6f74 2073 7570 706f 7274 206e 756d 5f6e  ot support num_n
+0000b490: 6f64 6573 203e 2031 2079 6574 0a40 7079  odes > 1 yet.@py
+0000b4a0: 7465 7374 2e6d 6172 6b2e 6e6f 5f6f 6369  test.mark.no_oci
+0000b4b0: 2020 2320 4f43 4920 436c 6f75 6420 646f    # OCI Cloud do
+0000b4c0: 6573 206e 6f74 2068 6176 6520 4b38 3020  es not have K80 
+0000b4d0: 6770 7573 0a64 6566 2074 6573 745f 6d75  gpus.def test_mu
+0000b4e0: 6c74 695f 6563 686f 2867 656e 6572 6963  lti_echo(generic
+0000b4f0: 5f63 6c6f 7564 3a20 7374 7229 3a0a 2020  _cloud: str):.  
+0000b500: 2020 6e61 6d65 203d 205f 6765 745f 636c    name = _get_cl
+0000b510: 7573 7465 725f 6e61 6d65 2829 0a20 2020  uster_name().   
+0000b520: 2074 6573 7420 3d20 5465 7374 280a 2020   test = Test(.  
+0000b530: 2020 2020 2020 276d 756c 7469 5f65 6368        'multi_ech
+0000b540: 6f27 2c0a 2020 2020 2020 2020 5b0a 2020  o',.        [.  
+0000b550: 2020 2020 2020 2020 2020 6627 7079 7468            f'pyth
+0000b560: 6f6e 2065 7861 6d70 6c65 732f 6d75 6c74  on examples/mult
+0000b570: 695f 6563 686f 2e70 7920 7b6e 616d 657d  i_echo.py {name}
+0000b580: 207b 6765 6e65 7269 635f 636c 6f75 647d   {generic_cloud}
+0000b590: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+0000b5a0: 736c 6565 7020 3132 3027 2c0a 2020 2020  sleep 120',.    
+0000b5b0: 2020 2020 5d20 2b0a 2020 2020 2020 2020      ] +.        
+0000b5c0: 2320 456e 7375 7265 206a 6f62 7320 7375  # Ensure jobs su
+0000b5d0: 6363 6565 6465 642e 0a20 2020 2020 2020  cceeded..       
+0000b5e0: 205b 6627 736b 7920 6c6f 6773 207b 6e61   [f'sky logs {na
+0000b5f0: 6d65 7d20 7b69 202b 2031 7d20 2d2d 7374  me} {i + 1} --st
+0000b600: 6174 7573 2720 666f 7220 6920 696e 2072  atus' for i in r
+0000b610: 616e 6765 2833 3229 5d20 2b0a 2020 2020  ange(32)] +.    
+0000b620: 2020 2020 2320 456e 7375 7265 206d 6f6e      # Ensure mon
+0000b630: 6974 6f72 2f61 7574 6f73 6361 6c65 7220  itor/autoscaler 
+0000b640: 6469 646e 2774 2063 7261 7368 206f 6e20  didn't crash on 
+0000b650: 7468 6520 2761 7373 6572 7420 6e6f 740a  the 'assert not.
+0000b660: 2020 2020 2020 2020 2320 756e 6675 6c66          # unfulf
+0000b670: 696c 6c65 6427 2065 7272 6f72 2e20 2049  illed' error.  I
+0000b680: 6620 7072 6f63 6573 7320 6e6f 7420 666f  f process not fo
+0000b690: 756e 642c 2067 7265 702d 3e73 7368 2072  und, grep->ssh r
+0000b6a0: 6574 7572 6e73 2031 2e0a 2020 2020 2020  eturns 1..      
+0000b6b0: 2020 5b66 2773 7368 207b 6e61 6d65 7d20    [f'ssh {name} 
+0000b6c0: 5c27 7073 2061 7578 207c 2067 7265 7020  \'ps aux | grep 
+0000b6d0: 225b 2f5d 226d 6f6e 6974 6f72 2e70 795c  "[/]"monitor.py\
+0000b6e0: 2727 5d2c 0a20 2020 2020 2020 2066 2773  ''],.        f's
+0000b6f0: 6b79 2064 6f77 6e20 2d79 207b 6e61 6d65  ky down -y {name
+0000b700: 7d27 2c0a 2020 2020 2020 2020 7469 6d65  }',.        time
+0000b710: 6f75 743d 3230 202a 2036 302c 0a20 2020  out=20 * 60,.   
+0000b720: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
+0000b730: 6573 7428 7465 7374 290a 0a0a 2320 2d2d  est(test)...# --
+0000b740: 2d2d 2d2d 2d2d 2d2d 2054 6173 6b3a 2031  -------- Task: 1
+0000b750: 206e 6f64 6520 7472 6169 6e69 6e67 2e20   node training. 
+0000b760: 2d2d 2d2d 2d2d 2d2d 2d2d 0a40 7079 7465  ----------.@pyte
+0000b770: 7374 2e6d 6172 6b2e 6e6f 5f6c 616d 6264  st.mark.no_lambd
+0000b780: 615f 636c 6f75 6420 2023 204c 616d 6264  a_cloud  # Lambd
+0000b790: 6120 436c 6f75 6420 646f 6573 206e 6f74  a Cloud does not
+0000b7a0: 2068 6176 6520 5631 3030 2067 7075 730a   have V100 gpus.
+0000b7b0: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
+0000b7c0: 6962 6d20 2023 2049 424d 2063 6c6f 7564  ibm  # IBM cloud
+0000b7d0: 2063 7572 7265 6e74 6c79 2064 6f65 736e   currently doesn
+0000b7e0: 2774 2070 726f 7669 6465 2070 7562 6c69  't provide publi
+0000b7f0: 6320 696d 6167 6520 7769 7468 2043 5544  c image with CUD
+0000b800: 410a 4070 7974 6573 742e 6d61 726b 2e6e  A.@pytest.mark.n
+0000b810: 6f5f 7363 7020 2023 2053 4350 2064 6f65  o_scp  # SCP doe
+0000b820: 7320 6e6f 7420 6861 7665 2056 3130 3020  s not have V100 
+0000b830: 2831 3647 4229 2047 5055 732e 2052 756e  (16GB) GPUs. Run
+0000b840: 2074 6573 745f 7363 705f 6875 6767 696e   test_scp_huggin
+0000b850: 6766 6163 6520 696e 7374 6561 642e 0a64  gface instead..d
+0000b860: 6566 2074 6573 745f 6875 6767 696e 6766  ef test_huggingf
+0000b870: 6163 6528 6765 6e65 7269 635f 636c 6f75  ace(generic_clou
+0000b880: 643a 2073 7472 293a 0a20 2020 206e 616d  d: str):.    nam
+0000b890: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
+0000b8a0: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
+0000b8b0: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
+0000b8c0: 2027 6875 6767 696e 6766 6163 655f 676c   'huggingface_gl
+0000b8d0: 7565 5f69 6d64 625f 6170 7027 2c0a 2020  ue_imdb_app',.  
+0000b8e0: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+0000b8f0: 2020 2020 6627 736b 7920 6c61 756e 6368      f'sky launch
+0000b900: 202d 7920 2d63 207b 6e61 6d65 7d20 2d2d   -y -c {name} --
+0000b910: 636c 6f75 6420 7b67 656e 6572 6963 5f63  cloud {generic_c
+0000b920: 6c6f 7564 7d20 6578 616d 706c 6573 2f68  loud} examples/h
+0000b930: 7567 6769 6e67 6661 6365 5f67 6c75 655f  uggingface_glue_
+0000b940: 696d 6462 5f61 7070 2e79 616d 6c27 2c0a  imdb_app.yaml',.
+0000b950: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+0000b960: 7920 6c6f 6773 207b 6e61 6d65 7d20 3120  y logs {name} 1 
+0000b970: 2d2d 7374 6174 7573 272c 2020 2320 456e  --status',  # En
+0000b980: 7375 7265 2074 6865 206a 6f62 2073 7563  sure the job suc
+0000b990: 6365 6564 6564 2e0a 2020 2020 2020 2020  ceeded..        
+0000b9a0: 2020 2020 6627 736b 7920 6578 6563 207b      f'sky exec {
+0000b9b0: 6e61 6d65 7d20 6578 616d 706c 6573 2f68  name} examples/h
+0000b9c0: 7567 6769 6e67 6661 6365 5f67 6c75 655f  uggingface_glue_
+0000b9d0: 696d 6462 5f61 7070 2e79 616d 6c27 2c0a  imdb_app.yaml',.
+0000b9e0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+0000b9f0: 7920 6c6f 6773 207b 6e61 6d65 7d20 3220  y logs {name} 2 
+0000ba00: 2d2d 7374 6174 7573 272c 2020 2320 456e  --status',  # En
+0000ba10: 7375 7265 2074 6865 206a 6f62 2073 7563  sure the job suc
+0000ba20: 6365 6564 6564 2e0a 2020 2020 2020 2020  ceeded..        
+0000ba30: 5d2c 0a20 2020 2020 2020 2066 2773 6b79  ],.        f'sky
+0000ba40: 2064 6f77 6e20 2d79 207b 6e61 6d65 7d27   down -y {name}'
+0000ba50: 2c0a 2020 2020 290a 2020 2020 7275 6e5f  ,.    ).    run_
+0000ba60: 6f6e 655f 7465 7374 2874 6573 7429 0a0a  one_test(test)..
+0000ba70: 0a40 7079 7465 7374 2e6d 6172 6b2e 6c61  .@pytest.mark.la
+0000ba80: 6d62 6461 5f63 6c6f 7564 0a64 6566 2074  mbda_cloud.def t
+0000ba90: 6573 745f 6c61 6d62 6461 5f68 7567 6769  est_lambda_huggi
+0000baa0: 6e67 6661 6365 2867 656e 6572 6963 5f63  ngface(generic_c
+0000bab0: 6c6f 7564 3a20 7374 7229 3a0a 2020 2020  loud: str):.    
+0000bac0: 6e61 6d65 203d 205f 6765 745f 636c 7573  name = _get_clus
+0000bad0: 7465 725f 6e61 6d65 2829 0a20 2020 2074  ter_name().    t
+0000bae0: 6573 7420 3d20 5465 7374 280a 2020 2020  est = Test(.    
+0000baf0: 2020 2020 276c 616d 6264 615f 6875 6767      'lambda_hugg
+0000bb00: 696e 6766 6163 655f 676c 7565 5f69 6d64  ingface_glue_imd
+0000bb10: 625f 6170 7027 2c0a 2020 2020 2020 2020  b_app',.        
+0000bb20: 5b0a 2020 2020 2020 2020 2020 2020 6627  [.            f'
+0000bb30: 736b 7920 6c61 756e 6368 202d 7920 2d63  sky launch -y -c
+0000bb40: 207b 6e61 6d65 7d20 7b4c 414d 4244 415f   {name} {LAMBDA_
+0000bb50: 5459 5045 7d20 6578 616d 706c 6573 2f68  TYPE} examples/h
+0000bb60: 7567 6769 6e67 6661 6365 5f67 6c75 655f  uggingface_glue_
+0000bb70: 696d 6462 5f61 7070 2e79 616d 6c27 2c0a  imdb_app.yaml',.
+0000bb80: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+0000bb90: 7920 6c6f 6773 207b 6e61 6d65 7d20 3120  y logs {name} 1 
+0000bba0: 2d2d 7374 6174 7573 272c 2020 2320 456e  --status',  # En
+0000bbb0: 7375 7265 2074 6865 206a 6f62 2073 7563  sure the job suc
+0000bbc0: 6365 6564 6564 2e0a 2020 2020 2020 2020  ceeded..        
+0000bbd0: 2020 2020 6627 736b 7920 6578 6563 207b      f'sky exec {
+0000bbe0: 6e61 6d65 7d20 7b4c 414d 4244 415f 5459  name} {LAMBDA_TY
+0000bbf0: 5045 7d20 6578 616d 706c 6573 2f68 7567  PE} examples/hug
+0000bc00: 6769 6e67 6661 6365 5f67 6c75 655f 696d  gingface_glue_im
+0000bc10: 6462 5f61 7070 2e79 616d 6c27 2c0a 2020  db_app.yaml',.  
+0000bc20: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+0000bc30: 6c6f 6773 207b 6e61 6d65 7d20 3220 2d2d  logs {name} 2 --
+0000bc40: 7374 6174 7573 272c 2020 2320 456e 7375  status',  # Ensu
+0000bc50: 7265 2074 6865 206a 6f62 2073 7563 6365  re the job succe
+0000bc60: 6564 6564 2e0a 2020 2020 2020 2020 5d2c  eded..        ],
+0000bc70: 0a20 2020 2020 2020 2066 2773 6b79 2064  .        f'sky d
+0000bc80: 6f77 6e20 2d79 207b 6e61 6d65 7d27 2c0a  own -y {name}',.
+0000bc90: 2020 2020 290a 2020 2020 7275 6e5f 6f6e      ).    run_on
+0000bca0: 655f 7465 7374 2874 6573 7429 0a0a 0a40  e_test(test)...@
+0000bcb0: 7079 7465 7374 2e6d 6172 6b2e 7363 700a  pytest.mark.scp.
+0000bcc0: 6465 6620 7465 7374 5f73 6370 5f68 7567  def test_scp_hug
+0000bcd0: 6769 6e67 6661 6365 2867 656e 6572 6963  gingface(generic
+0000bce0: 5f63 6c6f 7564 3a20 7374 7229 3a0a 2020  _cloud: str):.  
+0000bcf0: 2020 6e61 6d65 203d 205f 6765 745f 636c    name = _get_cl
+0000bd00: 7573 7465 725f 6e61 6d65 2829 0a20 2020  uster_name().   
+0000bd10: 206e 756d 5f6f 665f 6770 755f 6c61 756e   num_of_gpu_laun
+0000bd20: 6368 203d 2031 0a20 2020 2074 6573 7420  ch = 1.    test 
+0000bd30: 3d20 5465 7374 280a 2020 2020 2020 2020  = Test(.        
+0000bd40: 2753 4350 5f68 7567 6769 6e67 6661 6365  'SCP_huggingface
+0000bd50: 5f67 6c75 655f 696d 6462 5f61 7070 272c  _glue_imdb_app',
+0000bd60: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
+0000bd70: 2020 2020 2020 2066 2773 6b79 206c 6175         f'sky lau
+0000bd80: 6e63 6820 2d79 202d 6320 7b6e 616d 657d  nch -y -c {name}
+0000bd90: 207b 5343 505f 5459 5045 7d20 7b53 4350   {SCP_TYPE} {SCP
+0000bda0: 5f47 5055 5f56 3130 307d 3a7b 6e75 6d5f  _GPU_V100}:{num_
+0000bdb0: 6f66 5f67 7075 5f6c 6175 6e63 687d 2065  of_gpu_launch} e
+0000bdc0: 7861 6d70 6c65 732f 6875 6767 696e 6766  xamples/huggingf
+0000bdd0: 6163 655f 676c 7565 5f69 6d64 625f 6170  ace_glue_imdb_ap
+0000bde0: 702e 7961 6d6c 272c 0a20 2020 2020 2020  p.yaml',.       
+0000bdf0: 2020 2020 2066 2773 6b79 206c 6f67 7320       f'sky logs 
+0000be00: 7b6e 616d 657d 2031 202d 2d73 7461 7475  {name} 1 --statu
+0000be10: 7327 2c20 2023 2045 6e73 7572 6520 7468  s',  # Ensure th
+0000be20: 6520 6a6f 6220 7375 6363 6565 6465 642e  e job succeeded.
+0000be30: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+0000be40: 6b79 2065 7865 6320 7b6e 616d 657d 207b  ky exec {name} {
+0000be50: 5343 505f 5459 5045 7d20 7b53 4350 5f47  SCP_TYPE} {SCP_G
+0000be60: 5055 5f56 3130 307d 3a7b 6e75 6d5f 6f66  PU_V100}:{num_of
+0000be70: 5f67 7075 5f6c 6175 6e63 687d 2065 7861  _gpu_launch} exa
+0000be80: 6d70 6c65 732f 6875 6767 696e 6766 6163  mples/huggingfac
+0000be90: 655f 676c 7565 5f69 6d64 625f 6170 702e  e_glue_imdb_app.
+0000bea0: 7961 6d6c 272c 0a20 2020 2020 2020 2020  yaml',.         
+0000beb0: 2020 2066 2773 6b79 206c 6f67 7320 7b6e     f'sky logs {n
+0000bec0: 616d 657d 2032 202d 2d73 7461 7475 7327  ame} 2 --status'
+0000bed0: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
+0000bee0: 6a6f 6220 7375 6363 6565 6465 642e 0a20  job succeeded.. 
+0000bef0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+0000bf00: 2020 6627 736b 7920 646f 776e 202d 7920    f'sky down -y 
+0000bf10: 7b6e 616d 657d 272c 0a20 2020 2029 0a20  {name}',.    ). 
+0000bf20: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+0000bf30: 7465 7374 290a 0a0a 2320 2d2d 2d2d 2d2d  test)...# ------
+0000bf40: 2d2d 2d2d 2054 5055 2e20 2d2d 2d2d 2d2d  ---- TPU. ------
+0000bf50: 2d2d 2d2d 0a40 7079 7465 7374 2e6d 6172  ----.@pytest.mar
+0000bf60: 6b2e 6763 700a 6465 6620 7465 7374 5f74  k.gcp.def test_t
+0000bf70: 7075 2829 3a0a 2020 2020 6e61 6d65 203d  pu():.    name =
+0000bf80: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
+0000bf90: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
+0000bfa0: 5465 7374 280a 2020 2020 2020 2020 2774  Test(.        't
+0000bfb0: 7075 5f61 7070 272c 0a20 2020 2020 2020  pu_app',.       
+0000bfc0: 205b 0a20 2020 2020 2020 2020 2020 2066   [.            f
+0000bfd0: 2773 6b79 206c 6175 6e63 6820 2d79 202d  'sky launch -y -
+0000bfe0: 6320 7b6e 616d 657d 2065 7861 6d70 6c65  c {name} example
+0000bff0: 732f 7470 752f 7470 755f 6170 702e 7961  s/tpu/tpu_app.ya
+0000c000: 6d6c 272c 0a20 2020 2020 2020 2020 2020  ml',.           
+0000c010: 2066 2773 6b79 206c 6f67 7320 7b6e 616d   f'sky logs {nam
+0000c020: 657d 2031 272c 2020 2320 456e 7375 7265  e} 1',  # Ensure
+0000c030: 2074 6865 206a 6f62 2066 696e 6973 6865   the job finishe
+0000c040: 642e 0a20 2020 2020 2020 2020 2020 2066  d..            f
+0000c050: 2773 6b79 206c 6f67 7320 7b6e 616d 657d  'sky logs {name}
+0000c060: 2031 202d 2d73 7461 7475 7327 2c20 2023   1 --status',  #
+0000c070: 2045 6e73 7572 6520 7468 6520 6a6f 6220   Ensure the job 
+0000c080: 7375 6363 6565 6465 642e 0a20 2020 2020  succeeded..     
+0000c090: 2020 2020 2020 2066 2773 6b79 206c 6175         f'sky lau
+0000c0a0: 6e63 6820 2d79 202d 6320 7b6e 616d 657d  nch -y -c {name}
+0000c0b0: 2065 7861 6d70 6c65 732f 7470 752f 7470   examples/tpu/tp
+0000c0c0: 755f 6170 702e 7961 6d6c 207c 2067 7265  u_app.yaml | gre
+0000c0d0: 7020 2254 5055 202e 2a20 616c 7265 6164  p "TPU .* alread
+0000c0e0: 7920 6578 6973 7473 2227 2c20 2023 2045  y exists"',  # E
+0000c0f0: 6e73 7572 6520 736b 7920 6c61 756e 6368  nsure sky launch
+0000c100: 2077 6f6e 2774 2063 7265 6174 6520 616e   won't create an
+0000c110: 6f74 6865 7220 5450 552e 0a20 2020 2020  other TPU..     
+0000c120: 2020 205d 2c0a 2020 2020 2020 2020 6627     ],.        f'
+0000c130: 736b 7920 646f 776e 202d 7920 7b6e 616d  sky down -y {nam
+0000c140: 657d 272c 0a20 2020 2020 2020 2074 696d  e}',.        tim
+0000c150: 656f 7574 3d33 3020 2a20 3630 2c20 2023  eout=30 * 60,  #
+0000c160: 2063 616e 2074 616b 6520 3e32 3020 6d69   can take >20 mi
+0000c170: 6e73 0a20 2020 2029 0a20 2020 2072 756e  ns.    ).    run
+0000c180: 5f6f 6e65 5f74 6573 7428 7465 7374 290a  _one_test(test).
+0000c190: 0a0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2054  ..# ---------- T
+0000c1a0: 5055 2056 4d2e 202d 2d2d 2d2d 2d2d 2d2d  PU VM. ---------
+0000c1b0: 2d0a 4070 7974 6573 742e 6d61 726b 2e67  -.@pytest.mark.g
+0000c1c0: 6370 0a64 6566 2074 6573 745f 7470 755f  cp.def test_tpu_
+0000c1d0: 766d 2829 3a0a 2020 2020 6e61 6d65 203d  vm():.    name =
+0000c1e0: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
+0000c1f0: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
+0000c200: 5465 7374 280a 2020 2020 2020 2020 2774  Test(.        't
+0000c210: 7075 5f76 6d5f 6170 7027 2c0a 2020 2020  pu_vm_app',.    
+0000c220: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+0000c230: 2020 6627 736b 7920 6c61 756e 6368 202d    f'sky launch -
+0000c240: 7920 2d63 207b 6e61 6d65 7d20 6578 616d  y -c {name} exam
+0000c250: 706c 6573 2f74 7075 2f74 7075 766d 5f6d  ples/tpu/tpuvm_m
+0000c260: 6e69 7374 2e79 616d 6c27 2c0a 2020 2020  nist.yaml',.    
+0000c270: 2020 2020 2020 2020 6627 736b 7920 6c6f          f'sky lo
+0000c280: 6773 207b 6e61 6d65 7d20 3127 2c20 2023  gs {name} 1',  #
+0000c290: 2045 6e73 7572 6520 7468 6520 6a6f 6220   Ensure the job 
+0000c2a0: 6669 6e69 7368 6564 2e0a 2020 2020 2020  finished..      
+0000c2b0: 2020 2020 2020 6627 736b 7920 6c6f 6773        f'sky logs
+0000c2c0: 207b 6e61 6d65 7d20 3120 2d2d 7374 6174   {name} 1 --stat
+0000c2d0: 7573 272c 2020 2320 456e 7375 7265 2074  us',  # Ensure t
+0000c2e0: 6865 206a 6f62 2073 7563 6365 6564 6564  he job succeeded
+0000c2f0: 2e0a 2020 2020 2020 2020 2020 2020 6627  ..            f'
+0000c300: 736b 7920 7374 6f70 202d 7920 7b6e 616d  sky stop -y {nam
+0000c310: 657d 272c 0a20 2020 2020 2020 2020 2020  e}',.           
+0000c320: 2066 2773 3d24 2873 6b79 2073 7461 7475   f's=$(sky statu
+0000c330: 7320 7b6e 616d 657d 202d 2d72 6566 7265  s {name} --refre
+0000c340: 7368 293b 2065 6368 6f20 2224 7322 3b20  sh); echo "$s"; 
+0000c350: 6563 686f 3b20 6563 686f 3b20 6563 686f  echo; echo; echo
+0000c360: 2022 2473 2220 207c 2067 7265 7020 7b6e   "$s"  | grep {n
+0000c370: 616d 657d 207c 2067 7265 7020 5354 4f50  ame} | grep STOP
+0000c380: 5045 4427 2c20 2023 2045 6e73 7572 6520  PED',  # Ensure 
+0000c390: 7468 6520 636c 7573 7465 7220 6973 2053  the cluster is S
+0000c3a0: 544f 5050 4544 2e0a 2020 2020 2020 2020  TOPPED..        
+0000c3b0: 2020 2020 2320 5573 6520 7265 7472 793a      # Use retry:
+0000c3c0: 2067 7561 7264 2061 6761 696e 7374 2074   guard against t
+0000c3d0: 7261 6e73 6965 6e74 2065 7272 6f72 7320  ransient errors 
+0000c3e0: 6f62 7365 7276 6564 2066 6f72 0a20 2020  observed for.   
+0000c3f0: 2020 2020 2020 2020 2023 206a 7573 742d           # just-
+0000c400: 7374 6f70 7065 6420 5450 5520 564d 7320  stopped TPU VMs 
+0000c410: 2823 3936 3229 2e0a 2020 2020 2020 2020  (#962)..        
+0000c420: 2020 2020 6627 736b 7920 7374 6172 7420      f'sky start 
+0000c430: 2d2d 7265 7472 792d 756e 7469 6c2d 7570  --retry-until-up
+0000c440: 202d 7920 7b6e 616d 657d 272c 0a20 2020   -y {name}',.   
+0000c450: 2020 2020 2020 2020 2066 2773 6b79 2065           f'sky e
+0000c460: 7865 6320 7b6e 616d 657d 2065 7861 6d70  xec {name} examp
+0000c470: 6c65 732f 7470 752f 7470 7576 6d5f 6d6e  les/tpu/tpuvm_mn
+0000c480: 6973 742e 7961 6d6c 272c 0a20 2020 2020  ist.yaml',.     
+0000c490: 2020 2020 2020 2066 2773 6b79 206c 6f67         f'sky log
+0000c4a0: 7320 7b6e 616d 657d 2032 202d 2d73 7461  s {name} 2 --sta
+0000c4b0: 7475 7327 2c20 2023 2045 6e73 7572 6520  tus',  # Ensure 
+0000c4c0: 7468 6520 6a6f 6220 7375 6363 6565 6465  the job succeede
+0000c4d0: 642e 0a20 2020 2020 2020 2020 2020 2066  d..            f
+0000c4e0: 2773 6b79 2073 746f 7020 2d79 207b 6e61  'sky stop -y {na
+0000c4f0: 6d65 7d27 2c0a 2020 2020 2020 2020 5d2c  me}',.        ],
+0000c500: 0a20 2020 2020 2020 2066 2773 6b79 2064  .        f'sky d
+0000c510: 6f77 6e20 2d79 207b 6e61 6d65 7d27 2c0a  own -y {name}',.
+0000c520: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
+0000c530: 3330 202a 2036 302c 2020 2320 6361 6e20  30 * 60,  # can 
+0000c540: 7461 6b65 2033 3020 6d69 6e73 0a20 2020  take 30 mins.   
+0000c550: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
+0000c560: 6573 7428 7465 7374 290a 0a0a 2320 2d2d  est(test)...# --
+0000c570: 2d2d 2d2d 2d2d 2d2d 2054 5055 2056 4d20  -------- TPU VM 
+0000c580: 506f 642e 202d 2d2d 2d2d 2d2d 2d2d 2d0a  Pod. ----------.
+0000c590: 4070 7974 6573 742e 6d61 726b 2e67 6370  @pytest.mark.gcp
+0000c5a0: 0a64 6566 2074 6573 745f 7470 755f 766d  .def test_tpu_vm
+0000c5b0: 5f70 6f64 2829 3a0a 2020 2020 6e61 6d65  _pod():.    name
+0000c5c0: 203d 205f 6765 745f 636c 7573 7465 725f   = _get_cluster_
+0000c5d0: 6e61 6d65 2829 0a20 2020 2074 6573 7420  name().    test 
+0000c5e0: 3d20 5465 7374 280a 2020 2020 2020 2020  = Test(.        
+0000c5f0: 2774 7075 5f70 6f64 272c 0a20 2020 2020  'tpu_pod',.     
+0000c600: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+0000c610: 2066 2773 6b79 206c 6175 6e63 6820 2d79   f'sky launch -y
+0000c620: 202d 6320 7b6e 616d 657d 2065 7861 6d70   -c {name} examp
+0000c630: 6c65 732f 7470 752f 7470 7576 6d5f 6d6e  les/tpu/tpuvm_mn
+0000c640: 6973 742e 7961 6d6c 202d 2d67 7075 7320  ist.yaml --gpus 
+0000c650: 7470 752d 7632 2d33 3220 2d2d 7573 652d  tpu-v2-32 --use-
+0000c660: 7370 6f74 202d 2d7a 6f6e 6520 6575 726f  spot --zone euro
+0000c670: 7065 2d77 6573 7434 2d61 272c 0a20 2020  pe-west4-a',.   
+0000c680: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
+0000c690: 6f67 7320 7b6e 616d 657d 2031 272c 2020  ogs {name} 1',  
+0000c6a0: 2320 456e 7375 7265 2074 6865 206a 6f62  # Ensure the job
+0000c6b0: 2066 696e 6973 6865 642e 0a20 2020 2020   finished..     
+0000c6c0: 2020 2020 2020 2066 2773 6b79 206c 6f67         f'sky log
+0000c6d0: 7320 7b6e 616d 657d 2031 202d 2d73 7461  s {name} 1 --sta
+0000c6e0: 7475 7327 2c20 2023 2045 6e73 7572 6520  tus',  # Ensure 
+0000c6f0: 7468 6520 6a6f 6220 7375 6363 6565 6465  the job succeede
+0000c700: 642e 0a20 2020 2020 2020 205d 2c0a 2020  d..        ],.  
+0000c710: 2020 2020 2020 6627 736b 7920 646f 776e        f'sky down
+0000c720: 202d 7920 7b6e 616d 657d 272c 0a20 2020   -y {name}',.   
+0000c730: 2020 2020 2074 696d 656f 7574 3d33 3020       timeout=30 
+0000c740: 2a20 3630 2c20 2023 2063 616e 2074 616b  * 60,  # can tak
+0000c750: 6520 3330 206d 696e 730a 2020 2020 290a  e 30 mins.    ).
+0000c760: 2020 2020 7275 6e5f 6f6e 655f 7465 7374      run_one_test
+0000c770: 2874 6573 7429 0a0a 0a23 202d 2d2d 2d2d  (test)...# -----
+0000c780: 2d2d 2d2d 2d20 5369 6d70 6c65 2061 7070  ----- Simple app
+0000c790: 732e 202d 2d2d 2d2d 2d2d 2d2d 2d0a 4070  s. ----------.@p
+0000c7a0: 7974 6573 742e 6d61 726b 2e6e 6f5f 7363  ytest.mark.no_sc
+0000c7b0: 7020 2023 2053 4350 2064 6f65 7320 6e6f  p  # SCP does no
+0000c7c0: 7420 7375 7070 6f72 7420 6e75 6d5f 6e6f  t support num_no
+0000c7d0: 6465 7320 3e20 3120 7965 740a 6465 6620  des > 1 yet.def 
+0000c7e0: 7465 7374 5f6d 756c 7469 5f68 6f73 746e  test_multi_hostn
+0000c7f0: 616d 6528 6765 6e65 7269 635f 636c 6f75  ame(generic_clou
+0000c800: 643a 2073 7472 293a 0a20 2020 206e 616d  d: str):.    nam
+0000c810: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
+0000c820: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
+0000c830: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
+0000c840: 2027 6d75 6c74 695f 686f 7374 6e61 6d65   'multi_hostname
+0000c850: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
+0000c860: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
+0000c870: 6175 6e63 6820 2d79 202d 6320 7b6e 616d  aunch -y -c {nam
+0000c880: 657d 202d 2d63 6c6f 7564 207b 6765 6e65  e} --cloud {gene
+0000c890: 7269 635f 636c 6f75 647d 2065 7861 6d70  ric_cloud} examp
+0000c8a0: 6c65 732f 6d75 6c74 695f 686f 7374 6e61  les/multi_hostna
+0000c8b0: 6d65 2e79 616d 6c27 2c0a 2020 2020 2020  me.yaml',.      
+0000c8c0: 2020 2020 2020 6627 736b 7920 6c6f 6773        f'sky logs
+0000c8d0: 207b 6e61 6d65 7d20 3120 2d2d 7374 6174   {name} 1 --stat
+0000c8e0: 7573 272c 2020 2320 456e 7375 7265 2074  us',  # Ensure t
+0000c8f0: 6865 206a 6f62 2073 7563 6365 6564 6564  he job succeeded
+0000c900: 2e0a 2020 2020 2020 2020 2020 2020 6627  ..            f'
+0000c910: 736b 7920 6c6f 6773 207b 6e61 6d65 7d20  sky logs {name} 
+0000c920: 3120 7c20 6772 6570 2022 4d79 2068 6f73  1 | grep "My hos
+0000c930: 746e 616d 653a 2220 7c20 7763 202d 6c20  tname:" | wc -l 
+0000c940: 7c20 6772 6570 2032 272c 2020 2320 456e  | grep 2',  # En
+0000c950: 7375 7265 2074 6865 7265 2061 7265 2032  sure there are 2
+0000c960: 2068 6f73 7473 2e0a 2020 2020 2020 2020   hosts..        
+0000c970: 2020 2020 6627 736b 7920 6578 6563 207b      f'sky exec {
+0000c980: 6e61 6d65 7d20 6578 616d 706c 6573 2f6d  name} examples/m
+0000c990: 756c 7469 5f68 6f73 746e 616d 652e 7961  ulti_hostname.ya
+0000c9a0: 6d6c 272c 0a20 2020 2020 2020 2020 2020  ml',.           
+0000c9b0: 2066 2773 6b79 206c 6f67 7320 7b6e 616d   f'sky logs {nam
+0000c9c0: 657d 2032 202d 2d73 7461 7475 7327 2c20  e} 2 --status', 
+0000c9d0: 2023 2045 6e73 7572 6520 7468 6520 6a6f   # Ensure the jo
+0000c9e0: 6220 7375 6363 6565 6465 642e 0a20 2020  b succeeded..   
+0000c9f0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+0000ca00: 6627 736b 7920 646f 776e 202d 7920 7b6e  f'sky down -y {n
+0000ca10: 616d 657d 272c 0a20 2020 2029 0a20 2020  ame}',.    ).   
+0000ca20: 2072 756e 5f6f 6e65 5f74 6573 7428 7465   run_one_test(te
+0000ca30: 7374 290a 0a0a 2320 2d2d 2d2d 2d2d 2d2d  st)...# --------
+0000ca40: 2d2d 2054 6173 6b3a 206e 3d32 206e 6f64  -- Task: n=2 nod
+0000ca50: 6573 2077 6974 6820 7365 7475 7073 2e20  es with setups. 
+0000ca60: 2d2d 2d2d 2d2d 2d2d 2d2d 0a40 7079 7465  ----------.@pyte
+0000ca70: 7374 2e6d 6172 6b2e 6e6f 5f6c 616d 6264  st.mark.no_lambd
+0000ca80: 615f 636c 6f75 6420 2023 204c 616d 6264  a_cloud  # Lambd
+0000ca90: 6120 436c 6f75 6420 646f 6573 206e 6f74  a Cloud does not
+0000caa0: 2068 6176 6520 5631 3030 2067 7075 730a   have V100 gpus.
+0000cab0: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
+0000cac0: 6962 6d20 2023 2049 424d 2063 6c6f 7564  ibm  # IBM cloud
+0000cad0: 2063 7572 7265 6e74 6c79 2064 6f65 736e   currently doesn
+0000cae0: 2774 2070 726f 7669 6465 2070 7562 6c69  't provide publi
+0000caf0: 6320 696d 6167 6520 7769 7468 2043 5544  c image with CUD
+0000cb00: 410a 4070 7974 6573 742e 6d61 726b 2e6e  A.@pytest.mark.n
+0000cb10: 6f5f 7363 7020 2023 2053 4350 2064 6f65  o_scp  # SCP doe
+0000cb20: 7320 6e6f 7420 7375 7070 6f72 7420 6e75  s not support nu
+0000cb30: 6d5f 6e6f 6465 7320 3e20 3120 7965 740a  m_nodes > 1 yet.
+0000cb40: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+0000cb50: 7028 0a20 2020 2072 6561 736f 6e3d 0a20  p(.    reason=. 
+0000cb60: 2020 2027 5468 6520 7265 736e 6574 5f64     'The resnet_d
+0000cb70: 6973 7472 6962 7574 6564 5f74 665f 6170  istributed_tf_ap
+0000cb80: 7020 6973 2066 6c61 6b79 2c20 6475 6520  p is flaky, due 
+0000cb90: 746f 2069 7420 6661 696c 696e 6720 746f  to it failing to
+0000cba0: 2064 6574 6563 7420 4750 5573 2e27 290a   detect GPUs.').
+0000cbb0: 6465 6620 7465 7374 5f64 6973 7472 6962  def test_distrib
+0000cbc0: 7574 6564 5f74 6628 6765 6e65 7269 635f  uted_tf(generic_
+0000cbd0: 636c 6f75 643a 2073 7472 293a 0a20 2020  cloud: str):.   
+0000cbe0: 206e 616d 6520 3d20 5f67 6574 5f63 6c75   name = _get_clu
+0000cbf0: 7374 6572 5f6e 616d 6528 290a 2020 2020  ster_name().    
+0000cc00: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
+0000cc10: 2020 2020 2027 7265 736e 6574 5f64 6973       'resnet_dis
+0000cc20: 7472 6962 7574 6564 5f74 665f 6170 7027  tributed_tf_app'
+0000cc30: 2c0a 2020 2020 2020 2020 5b0a 2020 2020  ,.        [.    
+0000cc40: 2020 2020 2020 2020 2320 4e4f 5445 3a20          # NOTE: 
+0000cc50: 7275 6e6e 696e 6720 6974 2074 7769 6365  running it twice
+0000cc60: 2077 696c 6c20 6861 6e67 2028 736f 6d65   will hang (some
+0000cc70: 7469 6d65 733f 2920 2d20 616e 2061 7070  times?) - an app
+0000cc80: 2d6c 6576 656c 2062 7567 2e0a 2020 2020  -level bug..    
+0000cc90: 2020 2020 2020 2020 6627 7079 7468 6f6e          f'python
+0000cca0: 2065 7861 6d70 6c65 732f 7265 736e 6574   examples/resnet
+0000ccb0: 5f64 6973 7472 6962 7574 6564 5f74 665f  _distributed_tf_
+0000ccc0: 6170 702e 7079 207b 6e61 6d65 7d20 7b67  app.py {name} {g
+0000ccd0: 656e 6572 6963 5f63 6c6f 7564 7d27 2c0a  eneric_cloud}',.
+0000cce0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+0000ccf0: 7920 6c6f 6773 207b 6e61 6d65 7d20 3120  y logs {name} 1 
+0000cd00: 2d2d 7374 6174 7573 272c 2020 2320 456e  --status',  # En
+0000cd10: 7375 7265 2074 6865 206a 6f62 2073 7563  sure the job suc
+0000cd20: 6365 6564 6564 2e0a 2020 2020 2020 2020  ceeded..        
+0000cd30: 5d2c 0a20 2020 2020 2020 2066 2773 6b79  ],.        f'sky
+0000cd40: 2064 6f77 6e20 2d79 207b 6e61 6d65 7d27   down -y {name}'
+0000cd50: 2c0a 2020 2020 2020 2020 7469 6d65 6f75  ,.        timeou
+0000cd60: 743d 3235 202a 2036 302c 2020 2320 3235  t=25 * 60,  # 25
+0000cd70: 206d 696e 7320 2869 7420 7461 6b65 7320   mins (it takes 
+0000cd80: 6172 6f75 6e64 207e 3139 206d 696e 7329  around ~19 mins)
+0000cd90: 0a20 2020 2029 0a20 2020 2072 756e 5f6f  .    ).    run_o
+0000cda0: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
+0000cdb0: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2054 6573  # ---------- Tes
+0000cdc0: 7469 6e67 2047 4350 2073 7461 7274 2061  ting GCP start a
+0000cdd0: 6e64 2073 746f 7020 696e 7374 616e 6365  nd stop instance
+0000cde0: 7320 2d2d 2d2d 2d2d 2d2d 2d2d 0a40 7079  s ----------.@py
+0000cdf0: 7465 7374 2e6d 6172 6b2e 6763 700a 6465  test.mark.gcp.de
+0000ce00: 6620 7465 7374 5f67 6370 5f73 7461 7274  f test_gcp_start
+0000ce10: 5f73 746f 7028 293a 0a20 2020 206e 616d  _stop():.    nam
+0000ce20: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
+0000ce30: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
+0000ce40: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
+0000ce50: 2027 6763 702d 7374 6172 742d 7374 6f70   'gcp-start-stop
+0000ce60: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
+0000ce70: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
+0000ce80: 6175 6e63 6820 2d79 202d 6320 7b6e 616d  aunch -y -c {nam
+0000ce90: 657d 2065 7861 6d70 6c65 732f 6763 705f  e} examples/gcp_
+0000cea0: 7374 6172 745f 7374 6f70 2e79 616d 6c27  start_stop.yaml'
+0000ceb0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+0000cec0: 736b 7920 6c6f 6773 207b 6e61 6d65 7d20  sky logs {name} 
+0000ced0: 3120 2d2d 7374 6174 7573 272c 2020 2320  1 --status',  # 
+0000cee0: 456e 7375 7265 2074 6865 206a 6f62 2073  Ensure the job s
+0000cef0: 7563 6365 6564 6564 2e0a 2020 2020 2020  ucceeded..      
+0000cf00: 2020 2020 2020 6627 736b 7920 6578 6563        f'sky exec
+0000cf10: 207b 6e61 6d65 7d20 6578 616d 706c 6573   {name} examples
+0000cf20: 2f67 6370 5f73 7461 7274 5f73 746f 702e  /gcp_start_stop.
+0000cf30: 7961 6d6c 272c 0a20 2020 2020 2020 2020  yaml',.         
+0000cf40: 2020 2066 2773 6b79 206c 6f67 7320 7b6e     f'sky logs {n
+0000cf50: 616d 657d 2032 202d 2d73 7461 7475 7327  ame} 2 --status'
+0000cf60: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
+0000cf70: 6a6f 6220 7375 6363 6565 6465 642e 0a20  job succeeded.. 
+0000cf80: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+0000cf90: 2065 7865 6320 7b6e 616d 657d 2022 7072   exec {name} "pr
+0000cfa0: 6c69 6d69 7420 2d6e 202d 2d70 6964 3d5c  limit -n --pid=\
+0000cfb0: 2428 7067 7265 7020 2d66 205c 2772 6179  $(pgrep -f \'ray
+0000cfc0: 6c65 742f 7261 796c 6574 202d 2d72 6179  let/raylet --ray
+0000cfd0: 6c65 745f 736f 636b 6574 5f6e 616d 655c  let_socket_name\
+0000cfe0: 2729 207c 2067 7265 7020 5c27 225c 2731  ') | grep \'"\'1
+0000cff0: 3034 3835 3736 2031 3034 3835 3736 5c27  048576 1048576\'
+0000d000: 225c 2722 272c 2020 2320 456e 7375 7265  "\'"',  # Ensure
+0000d010: 2074 6865 2072 6179 6c65 7420 7072 6f63   the raylet proc
+0000d020: 6573 7320 6861 7320 7468 6520 636f 7272  ess has the corr
+0000d030: 6563 7420 6669 6c65 2064 6573 6372 6970  ect file descrip
+0000d040: 746f 7220 6c69 6d69 742e 0a20 2020 2020  tor limit..     
+0000d050: 2020 2020 2020 2066 2773 6b79 206c 6f67         f'sky log
+0000d060: 7320 7b6e 616d 657d 2033 202d 2d73 7461  s {name} 3 --sta
+0000d070: 7475 7327 2c20 2023 2045 6e73 7572 6520  tus',  # Ensure 
+0000d080: 7468 6520 6a6f 6220 7375 6363 6565 6465  the job succeede
+0000d090: 642e 0a20 2020 2020 2020 2020 2020 2066  d..            f
+0000d0a0: 2773 6b79 2073 746f 7020 2d79 207b 6e61  'sky stop -y {na
+0000d0b0: 6d65 7d27 2c0a 2020 2020 2020 2020 2020  me}',.          
+0000d0c0: 2020 6627 736c 6565 7020 3230 272c 0a20    f'sleep 20',. 
+0000d0d0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+0000d0e0: 2073 7461 7274 202d 7920 7b6e 616d 657d   start -y {name}
+0000d0f0: 202d 6920 3127 2c0a 2020 2020 2020 2020   -i 1',.        
+0000d100: 2020 2020 6627 736b 7920 6578 6563 207b      f'sky exec {
+0000d110: 6e61 6d65 7d20 6578 616d 706c 6573 2f67  name} examples/g
+0000d120: 6370 5f73 7461 7274 5f73 746f 702e 7961  cp_start_stop.ya
+0000d130: 6d6c 272c 0a20 2020 2020 2020 2020 2020  ml',.           
+0000d140: 2066 2773 6b79 206c 6f67 7320 7b6e 616d   f'sky logs {nam
+0000d150: 657d 2034 202d 2d73 7461 7475 7327 2c20  e} 4 --status', 
+0000d160: 2023 2045 6e73 7572 6520 7468 6520 6a6f   # Ensure the jo
+0000d170: 6220 7375 6363 6565 6465 642e 0a20 2020  b succeeded..   
+0000d180: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
+0000d190: 3138 3027 2c0a 2020 2020 2020 2020 2020  180',.          
+0000d1a0: 2020 6627 736b 7920 7374 6174 7573 202d    f'sky status -
+0000d1b0: 7220 7b6e 616d 657d 207c 2067 7265 7020  r {name} | grep 
+0000d1c0: 2249 4e49 545c 7c53 544f 5050 4544 2227  "INIT\|STOPPED"'
+0000d1d0: 2c0a 2020 2020 2020 2020 5d2c 0a20 2020  ,.        ],.   
+0000d1e0: 2020 2020 2066 2773 6b79 2064 6f77 6e20       f'sky down 
+0000d1f0: 2d79 207b 6e61 6d65 7d27 2c0a 2020 2020  -y {name}',.    
+0000d200: 290a 2020 2020 7275 6e5f 6f6e 655f 7465  ).    run_one_te
+0000d210: 7374 2874 6573 7429 0a0a 0a23 202d 2d2d  st(test)...# ---
+0000d220: 2d2d 2d2d 2d2d 2d20 5465 7374 696e 6720  ------- Testing 
+0000d230: 417a 7572 6520 7374 6172 7420 616e 6420  Azure start and 
+0000d240: 7374 6f70 2069 6e73 7461 6e63 6573 202d  stop instances -
+0000d250: 2d2d 2d2d 2d2d 2d2d 2d0a 4070 7974 6573  ---------.@pytes
+0000d260: 742e 6d61 726b 2e61 7a75 7265 0a64 6566  t.mark.azure.def
+0000d270: 2074 6573 745f 617a 7572 655f 7374 6172   test_azure_star
+0000d280: 745f 7374 6f70 2829 3a0a 2020 2020 6e61  t_stop():.    na
+0000d290: 6d65 203d 205f 6765 745f 636c 7573 7465  me = _get_cluste
+0000d2a0: 725f 6e61 6d65 2829 0a20 2020 2074 6573  r_name().    tes
+0000d2b0: 7420 3d20 5465 7374 280a 2020 2020 2020  t = Test(.      
+0000d2c0: 2020 2761 7a75 7265 2d73 7461 7274 2d73    'azure-start-s
+0000d2d0: 746f 7027 2c0a 2020 2020 2020 2020 5b0a  top',.        [.
+0000d2e0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+0000d2f0: 7920 6c61 756e 6368 202d 7920 2d63 207b  y launch -y -c {
+0000d300: 6e61 6d65 7d20 6578 616d 706c 6573 2f61  name} examples/a
+0000d310: 7a75 7265 5f73 7461 7274 5f73 746f 702e  zure_start_stop.
+0000d320: 7961 6d6c 272c 0a20 2020 2020 2020 2020  yaml',.         
+0000d330: 2020 2066 2773 6b79 2065 7865 6320 7b6e     f'sky exec {n
+0000d340: 616d 657d 2065 7861 6d70 6c65 732f 617a  ame} examples/az
+0000d350: 7572 655f 7374 6172 745f 7374 6f70 2e79  ure_start_stop.y
+0000d360: 616d 6c27 2c0a 2020 2020 2020 2020 2020  aml',.          
+0000d370: 2020 6627 736b 7920 6c6f 6773 207b 6e61    f'sky logs {na
+0000d380: 6d65 7d20 3120 2d2d 7374 6174 7573 272c  me} 1 --status',
+0000d390: 2020 2320 456e 7375 7265 2074 6865 206a    # Ensure the j
+0000d3a0: 6f62 2073 7563 6365 6564 6564 2e0a 2020  ob succeeded..  
+0000d3b0: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+0000d3c0: 6578 6563 207b 6e61 6d65 7d20 2270 726c  exec {name} "prl
+0000d3d0: 696d 6974 202d 6e20 2d2d 7069 643d 5c24  imit -n --pid=\$
+0000d3e0: 2870 6772 6570 202d 6620 5c27 7261 796c  (pgrep -f \'rayl
+0000d3f0: 6574 2f72 6179 6c65 7420 2d2d 7261 796c  et/raylet --rayl
+0000d400: 6574 5f73 6f63 6b65 745f 6e61 6d65 5c27  et_socket_name\'
+0000d410: 2920 7c20 6772 6570 205c 2722 5c27 3130  ) | grep \'"\'10
+0000d420: 3438 3537 3620 3130 3438 3537 365c 2722  48576 1048576\'"
+0000d430: 5c27 2227 2c20 2023 2045 6e73 7572 6520  \'"',  # Ensure 
+0000d440: 7468 6520 7261 796c 6574 2070 726f 6365  the raylet proce
+0000d450: 7373 2068 6173 2074 6865 2063 6f72 7265  ss has the corre
+0000d460: 6374 2066 696c 6520 6465 7363 7269 7074  ct file descript
+0000d470: 6f72 206c 696d 6974 2e0a 2020 2020 2020  or limit..      
+0000d480: 2020 2020 2020 6627 736b 7920 6c6f 6773        f'sky logs
+0000d490: 207b 6e61 6d65 7d20 3220 2d2d 7374 6174   {name} 2 --stat
+0000d4a0: 7573 272c 2020 2320 456e 7375 7265 2074  us',  # Ensure t
+0000d4b0: 6865 206a 6f62 2073 7563 6365 6564 6564  he job succeeded
+0000d4c0: 2e0a 2020 2020 2020 2020 2020 2020 6627  ..            f'
+0000d4d0: 736b 7920 7374 6f70 202d 7920 7b6e 616d  sky stop -y {nam
+0000d4e0: 657d 272c 0a20 2020 2020 2020 2020 2020  e}',.           
+0000d4f0: 2066 2773 6b79 2073 7461 7274 202d 7920   f'sky start -y 
+0000d500: 7b6e 616d 657d 202d 6920 3127 2c0a 2020  {name} -i 1',.  
+0000d510: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+0000d520: 6578 6563 207b 6e61 6d65 7d20 6578 616d  exec {name} exam
+0000d530: 706c 6573 2f61 7a75 7265 5f73 7461 7274  ples/azure_start
+0000d540: 5f73 746f 702e 7961 6d6c 272c 0a20 2020  _stop.yaml',.   
+0000d550: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
+0000d560: 6f67 7320 7b6e 616d 657d 2033 202d 2d73  ogs {name} 3 --s
+0000d570: 7461 7475 7327 2c20 2023 2045 6e73 7572  tatus',  # Ensur
+0000d580: 6520 7468 6520 6a6f 6220 7375 6363 6565  e the job succee
+0000d590: 6465 642e 0a20 2020 2020 2020 2020 2020  ded..           
+0000d5a0: 2027 736c 6565 7020 3230 3027 2c0a 2020   'sleep 200',.  
+0000d5b0: 2020 2020 2020 2020 2020 6627 733d 2428            f's=$(
+0000d5c0: 736b 7920 7374 6174 7573 202d 7220 7b6e  sky status -r {n
+0000d5d0: 616d 657d 2920 2626 2065 6368 6f20 2473  ame}) && echo $s
+0000d5e0: 2026 2620 6563 686f 2024 7320 7c20 6772   && echo $s | gr
+0000d5f0: 6570 2022 494e 4954 5c7c 5354 4f50 5045  ep "INIT\|STOPPE
+0000d600: 4422 270a 2020 2020 2020 2020 5d2c 0a20  D"'.        ],. 
+0000d610: 2020 2020 2020 2066 2773 6b79 2064 6f77         f'sky dow
+0000d620: 6e20 2d79 207b 6e61 6d65 7d27 2c0a 2020  n -y {name}',.  
+0000d630: 2020 2020 2020 7469 6d65 6f75 743d 3330        timeout=30
+0000d640: 202a 2036 302c 2020 2320 3330 206d 696e   * 60,  # 30 min
+0000d650: 730a 2020 2020 290a 2020 2020 7275 6e5f  s.    ).    run_
+0000d660: 6f6e 655f 7465 7374 2874 6573 7429 0a0a  one_test(test)..
+0000d670: 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d20 5465  .# ---------- Te
+0000d680: 7374 696e 6720 4175 746f 7374 6f70 7069  sting Autostoppi
+0000d690: 6e67 202d 2d2d 2d2d 2d2d 2d2d 2d0a 4070  ng ----------.@p
+0000d6a0: 7974 6573 742e 6d61 726b 2e6e 6f5f 6c61  ytest.mark.no_la
+0000d6b0: 6d62 6461 5f63 6c6f 7564 2020 2320 4c61  mbda_cloud  # La
+0000d6c0: 6d62 6461 2043 6c6f 7564 2064 6f65 7320  mbda Cloud does 
+0000d6d0: 6e6f 7420 7375 7070 6f72 7420 7374 6f70  not support stop
+0000d6e0: 7069 6e67 2069 6e73 7461 6e63 6573 0a40  ping instances.@
+0000d6f0: 7079 7465 7374 2e6d 6172 6b2e 6e6f 5f69  pytest.mark.no_i
+0000d700: 626d 2020 2320 4649 5828 4942 4d29 2073  bm  # FIX(IBM) s
+0000d710: 706f 7261 6469 6361 6c6c 7920 6661 696c  poradically fail
+0000d720: 732c 2061 7320 7265 7374 6172 7465 6420  s, as restarted 
+0000d730: 776f 726b 6572 7320 7374 6179 2075 6e69  workers stay uni
+0000d740: 6e69 7469 616c 697a 6564 2069 6e64 6566  nitialized indef
+0000d750: 696e 6974 656c 790a 4070 7974 6573 742e  initely.@pytest.
+0000d760: 6d61 726b 2e6e 6f5f 7363 7020 2023 2053  mark.no_scp  # S
+0000d770: 4350 2064 6f65 7320 6e6f 7420 7375 7070  CP does not supp
+0000d780: 6f72 7420 6e75 6d5f 6e6f 6465 7320 3e20  ort num_nodes > 
+0000d790: 3120 7965 740a 6465 6620 7465 7374 5f61  1 yet.def test_a
+0000d7a0: 7574 6f73 746f 7028 6765 6e65 7269 635f  utostop(generic_
+0000d7b0: 636c 6f75 643a 2073 7472 293a 0a20 2020  cloud: str):.   
+0000d7c0: 206e 616d 6520 3d20 5f67 6574 5f63 6c75   name = _get_clu
+0000d7d0: 7374 6572 5f6e 616d 6528 290a 2020 2020  ster_name().    
+0000d7e0: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
+0000d7f0: 2020 2020 2027 6175 746f 7374 6f70 272c       'autostop',
+0000d800: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
+0000d810: 2020 2020 2020 2066 2773 6b79 206c 6175         f'sky lau
+0000d820: 6e63 6820 2d79 202d 6420 2d63 207b 6e61  nch -y -d -c {na
+0000d830: 6d65 7d20 2d2d 6e75 6d2d 6e6f 6465 7320  me} --num-nodes 
+0000d840: 3220 2d2d 636c 6f75 6420 7b67 656e 6572  2 --cloud {gener
+0000d850: 6963 5f63 6c6f 7564 7d20 7465 7374 732f  ic_cloud} tests/
+0000d860: 7465 7374 5f79 616d 6c73 2f6d 696e 696d  test_yamls/minim
+0000d870: 616c 2e79 616d 6c27 2c0a 2020 2020 2020  al.yaml',.      
+0000d880: 2020 2020 2020 6627 736b 7920 6175 746f        f'sky auto
+0000d890: 7374 6f70 202d 7920 7b6e 616d 657d 202d  stop -y {name} -
+0000d8a0: 6920 3127 2c0a 0a20 2020 2020 2020 2020  i 1',..         
+0000d8b0: 2020 2023 2045 6e73 7572 6520 6175 746f     # Ensure auto
+0000d8c0: 7374 6f70 2069 7320 7365 742e 0a20 2020  stop is set..   
+0000d8d0: 2020 2020 2020 2020 2066 2773 6b79 2073           f'sky s
+0000d8e0: 7461 7475 7320 7c20 6772 6570 207b 6e61  tatus | grep {na
+0000d8f0: 6d65 7d20 7c20 6772 6570 2022 316d 2227  me} | grep "1m"'
+0000d900: 2c0a 0a20 2020 2020 2020 2020 2020 2023  ,..            #
+0000d910: 2045 6e73 7572 6520 7468 6520 636c 7573   Ensure the clus
+0000d920: 7465 7220 6973 206e 6f74 2073 746f 7070  ter is not stopp
+0000d930: 6564 2065 6172 6c79 2e0a 2020 2020 2020  ed early..      
+0000d940: 2020 2020 2020 2773 6c65 6570 2034 3527        'sleep 45'
+0000d950: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+0000d960: 733d 2428 736b 7920 7374 6174 7573 207b  s=$(sky status {
+0000d970: 6e61 6d65 7d20 2d2d 7265 6672 6573 6829  name} --refresh)
+0000d980: 3b20 6563 686f 2022 2473 223b 2065 6368  ; echo "$s"; ech
+0000d990: 6f3b 2065 6368 6f3b 2065 6368 6f20 2224  o; echo; echo "$
+0000d9a0: 7322 2020 7c20 6772 6570 207b 6e61 6d65  s"  | grep {name
+0000d9b0: 7d20 7c20 6772 6570 2055 5027 2c0a 0a20  } | grep UP',.. 
+0000d9c0: 2020 2020 2020 2020 2020 2023 2045 6e73             # Ens
+0000d9d0: 7572 6520 7468 6520 636c 7573 7465 7220  ure the cluster 
+0000d9e0: 6973 2053 544f 5050 4544 2e0a 2020 2020  is STOPPED..    
+0000d9f0: 2020 2020 2020 2020 2773 6c65 6570 2032          'sleep 2
+0000da00: 3530 272c 0a20 2020 2020 2020 2020 2020  50',.           
+0000da10: 2066 2773 3d24 2873 6b79 2073 7461 7475   f's=$(sky statu
+0000da20: 7320 7b6e 616d 657d 202d 2d72 6566 7265  s {name} --refre
+0000da30: 7368 293b 2065 6368 6f20 2224 7322 3b20  sh); echo "$s"; 
+0000da40: 6563 686f 3b20 6563 686f 3b20 6563 686f  echo; echo; echo
+0000da50: 2022 2473 2220 207c 2067 7265 7020 7b6e   "$s"  | grep {n
+0000da60: 616d 657d 207c 2067 7265 7020 5354 4f50  ame} | grep STOP
+0000da70: 5045 4427 2c0a 0a20 2020 2020 2020 2020  PED',..         
+0000da80: 2020 2023 2045 6e73 7572 6520 7468 6520     # Ensure the 
+0000da90: 636c 7573 7465 7220 6973 2055 5020 616e  cluster is UP an
+0000daa0: 6420 7468 6520 6175 746f 7374 6f70 2073  d the autostop s
+0000dab0: 6574 7469 6e67 2069 7320 7265 7365 7420  etting is reset 
+0000dac0: 2827 2d27 292e 0a20 2020 2020 2020 2020  ('-')..         
+0000dad0: 2020 2066 2773 6b79 2073 7461 7274 202d     f'sky start -
+0000dae0: 7920 7b6e 616d 657d 272c 0a20 2020 2020  y {name}',.     
+0000daf0: 2020 2020 2020 2066 2773 6b79 2073 7461         f'sky sta
+0000db00: 7475 7320 7c20 6772 6570 207b 6e61 6d65  tus | grep {name
+0000db10: 7d20 7c20 6772 6570 202d 4520 2255 505c  } | grep -E "UP\
+0000db20: 732b 2d22 272c 0a0a 2020 2020 2020 2020  s+-"',..        
+0000db30: 2020 2020 2320 456e 7375 7265 2074 6865      # Ensure the
+0000db40: 206a 6f62 2073 7563 6365 6564 6564 2e0a   job succeeded..
+0000db50: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+0000db60: 7920 6578 6563 207b 6e61 6d65 7d20 7465  y exec {name} te
+0000db70: 7374 732f 7465 7374 5f79 616d 6c73 2f6d  sts/test_yamls/m
+0000db80: 696e 696d 616c 2e79 616d 6c27 2c0a 2020  inimal.yaml',.  
+0000db90: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+0000dba0: 6c6f 6773 207b 6e61 6d65 7d20 3220 2d2d  logs {name} 2 --
+0000dbb0: 7374 6174 7573 272c 0a0a 2020 2020 2020  status',..      
+0000dbc0: 2020 2020 2020 2320 5465 7374 2072 6573        # Test res
+0000dbd0: 7461 7274 696e 6720 7468 6520 6964 6c65  tarting the idle
+0000dbe0: 6e65 7373 2074 696d 6572 2076 6961 2063  ness timer via c
+0000dbf0: 616e 6365 6c20 2b20 7265 7365 743a 0a20  ancel + reset:. 
+0000dc00: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+0000dc10: 2061 7574 6f73 746f 7020 2d79 207b 6e61   autostop -y {na
+0000dc20: 6d65 7d20 2d69 2031 272c 2020 2320 4964  me} -i 1',  # Id
+0000dc30: 6c65 6e65 7373 2073 7461 7274 7320 636f  leness starts co
+0000dc40: 756e 7469 6e67 2e0a 2020 2020 2020 2020  unting..        
+0000dc50: 2020 2020 2773 6c65 6570 2034 3527 2c20      'sleep 45', 
+0000dc60: 2023 2041 6c6d 6f73 7420 7265 6163 6865   # Almost reache
+0000dc70: 6420 7468 6520 7468 7265 7368 6f6c 642e  d the threshold.
+0000dc80: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+0000dc90: 6b79 2061 7574 6f73 746f 7020 2d79 207b  ky autostop -y {
+0000dca0: 6e61 6d65 7d20 2d2d 6361 6e63 656c 272c  name} --cancel',
+0000dcb0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+0000dcc0: 6b79 2061 7574 6f73 746f 7020 2d79 207b  ky autostop -y {
+0000dcd0: 6e61 6d65 7d20 2d69 2031 272c 2020 2320  name} -i 1',  # 
+0000dce0: 5368 6f75 6c64 2072 6573 7461 7274 2074  Should restart t
+0000dcf0: 6865 2074 696d 6572 2e0a 2020 2020 2020  he timer..      
+0000dd00: 2020 2020 2020 2773 6c65 6570 2034 3527        'sleep 45'
+0000dd10: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+0000dd20: 733d 2428 736b 7920 7374 6174 7573 207b  s=$(sky status {
+0000dd30: 6e61 6d65 7d20 2d2d 7265 6672 6573 6829  name} --refresh)
+0000dd40: 3b20 6563 686f 2022 2473 223b 2065 6368  ; echo "$s"; ech
+0000dd50: 6f3b 2065 6368 6f3b 2065 6368 6f20 2224  o; echo; echo "$
+0000dd60: 7322 207c 2067 7265 7020 7b6e 616d 657d  s" | grep {name}
+0000dd70: 207c 2067 7265 7020 5550 272c 0a20 2020   | grep UP',.   
+0000dd80: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
+0000dd90: 3235 3027 2c0a 2020 2020 2020 2020 2020  250',.          
+0000dda0: 2020 6627 733d 2428 736b 7920 7374 6174    f's=$(sky stat
+0000ddb0: 7573 207b 6e61 6d65 7d20 2d2d 7265 6672  us {name} --refr
+0000ddc0: 6573 6829 3b20 6563 686f 2022 2473 223b  esh); echo "$s";
+0000ddd0: 2065 6368 6f3b 2065 6368 6f3b 2065 6368   echo; echo; ech
+0000dde0: 6f20 2224 7322 2020 7c20 6772 6570 207b  o "$s"  | grep {
+0000ddf0: 6e61 6d65 7d20 7c20 6772 6570 2053 544f  name} | grep STO
+0000de00: 5050 4544 272c 0a0a 2020 2020 2020 2020  PPED',..        
+0000de10: 2020 2020 2320 5465 7374 2072 6573 7461      # Test resta
+0000de20: 7274 696e 6720 7468 6520 6964 6c65 6e65  rting the idlene
+0000de30: 7373 2074 696d 6572 2076 6961 2065 7865  ss timer via exe
+0000de40: 633a 0a20 2020 2020 2020 2020 2020 2066  c:.            f
+0000de50: 2773 6b79 2073 7461 7274 202d 7920 7b6e  'sky start -y {n
+0000de60: 616d 657d 272c 0a20 2020 2020 2020 2020  ame}',.         
+0000de70: 2020 2066 2773 6b79 2073 7461 7475 7320     f'sky status 
+0000de80: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
+0000de90: 6772 6570 202d 4520 2255 505c 732b 2d22  grep -E "UP\s+-"
+0000dea0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+0000deb0: 2773 6b79 2061 7574 6f73 746f 7020 2d79  'sky autostop -y
+0000dec0: 207b 6e61 6d65 7d20 2d69 2031 272c 2020   {name} -i 1',  
+0000ded0: 2320 4964 6c65 6e65 7373 2073 7461 7274  # Idleness start
+0000dee0: 7320 636f 756e 7469 6e67 2e0a 2020 2020  s counting..    
+0000def0: 2020 2020 2020 2020 2773 6c65 6570 2034          'sleep 4
+0000df00: 3527 2c20 2023 2041 6c6d 6f73 7420 7265  5',  # Almost re
+0000df10: 6163 6865 6420 7468 6520 7468 7265 7368  ached the thresh
+0000df20: 6f6c 642e 0a20 2020 2020 2020 2020 2020  old..           
+0000df30: 2066 2773 6b79 2065 7865 6320 7b6e 616d   f'sky exec {nam
+0000df40: 657d 2065 6368 6f20 6869 272c 2020 2320  e} echo hi',  # 
+0000df50: 5368 6f75 6c64 2072 6573 7461 7274 2074  Should restart t
+0000df60: 6865 2074 696d 6572 2e0a 2020 2020 2020  he timer..      
+0000df70: 2020 2020 2020 2773 6c65 6570 2034 3527        'sleep 45'
+0000df80: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+0000df90: 733d 2428 736b 7920 7374 6174 7573 207b  s=$(sky status {
+0000dfa0: 6e61 6d65 7d20 2d2d 7265 6672 6573 6829  name} --refresh)
+0000dfb0: 3b20 6563 686f 2022 2473 223b 2065 6368  ; echo "$s"; ech
+0000dfc0: 6f3b 2065 6368 6f3b 2065 6368 6f20 2224  o; echo; echo "$
+0000dfd0: 7322 2020 7c20 6772 6570 207b 6e61 6d65  s"  | grep {name
+0000dfe0: 7d20 7c20 6772 6570 2055 5027 2c0a 2020  } | grep UP',.  
+0000dff0: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
+0000e000: 2032 3530 272c 0a20 2020 2020 2020 2020   250',.         
+0000e010: 2020 2066 2773 3d24 2873 6b79 2073 7461     f's=$(sky sta
+0000e020: 7475 7320 7b6e 616d 657d 202d 2d72 6566  tus {name} --ref
+0000e030: 7265 7368 293b 2065 6368 6f20 2224 7322  resh); echo "$s"
+0000e040: 3b20 6563 686f 3b20 6563 686f 3b20 6563  ; echo; echo; ec
+0000e050: 686f 2022 2473 2220 207c 2067 7265 7020  ho "$s"  | grep 
+0000e060: 7b6e 616d 657d 207c 2067 7265 7020 5354  {name} | grep ST
+0000e070: 4f50 5045 4427 2c0a 2020 2020 2020 2020  OPPED',.        
+0000e080: 5d2c 0a20 2020 2020 2020 2066 2773 6b79  ],.        f'sky
+0000e090: 2064 6f77 6e20 2d79 207b 6e61 6d65 7d27   down -y {name}'
+0000e0a0: 2c0a 2020 2020 2020 2020 7469 6d65 6f75  ,.        timeou
+0000e0b0: 743d 3230 202a 2036 302c 0a20 2020 2029  t=20 * 60,.    )
+0000e0c0: 0a20 2020 2072 756e 5f6f 6e65 5f74 6573  .    run_one_tes
+0000e0d0: 7428 7465 7374 290a 0a0a 2320 2d2d 2d2d  t(test)...# ----
+0000e0e0: 2d2d 2d2d 2d2d 2054 6573 7469 6e67 2041  ------ Testing A
+0000e0f0: 7574 6f64 6f77 6e69 6e67 202d 2d2d 2d2d  utodowning -----
+0000e100: 2d2d 2d2d 2d0a 4070 7974 6573 742e 6d61  -----.@pytest.ma
+0000e110: 726b 2e6e 6f5f 7363 7020 2023 2053 4350  rk.no_scp  # SCP
+0000e120: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
+0000e130: 7420 6e75 6d5f 6e6f 6465 7320 3e20 3120  t num_nodes > 1 
+0000e140: 7965 742e 2052 756e 2074 6573 745f 7363  yet. Run test_sc
+0000e150: 705f 6175 746f 646f 776e 2069 6e73 7465  p_autodown inste
+0000e160: 6164 2e0a 6465 6620 7465 7374 5f61 7574  ad..def test_aut
+0000e170: 6f64 6f77 6e28 6765 6e65 7269 635f 636c  odown(generic_cl
+0000e180: 6f75 643a 2073 7472 293a 0a20 2020 206e  oud: str):.    n
+0000e190: 616d 6520 3d20 5f67 6574 5f63 6c75 7374  ame = _get_clust
+0000e1a0: 6572 5f6e 616d 6528 290a 2020 2020 7465  er_name().    te
+0000e1b0: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
+0000e1c0: 2020 2027 6175 746f 646f 776e 272c 0a20     'autodown',. 
+0000e1d0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+0000e1e0: 2020 2020 2066 2773 6b79 206c 6175 6e63       f'sky launc
+0000e1f0: 6820 2d79 202d 6420 2d63 207b 6e61 6d65  h -y -d -c {name
+0000e200: 7d20 2d2d 6e75 6d2d 6e6f 6465 7320 3220  } --num-nodes 2 
+0000e210: 2d2d 636c 6f75 6420 7b67 656e 6572 6963  --cloud {generic
+0000e220: 5f63 6c6f 7564 7d20 7465 7374 732f 7465  _cloud} tests/te
+0000e230: 7374 5f79 616d 6c73 2f6d 696e 696d 616c  st_yamls/minimal
+0000e240: 2e79 616d 6c27 2c0a 2020 2020 2020 2020  .yaml',.        
+0000e250: 2020 2020 6627 736b 7920 6175 746f 7374      f'sky autost
+0000e260: 6f70 202d 7920 7b6e 616d 657d 202d 2d64  op -y {name} --d
+0000e270: 6f77 6e20 2d69 2031 272c 0a20 2020 2020  own -i 1',.     
+0000e280: 2020 2020 2020 2023 2045 6e73 7572 6520         # Ensure 
+0000e290: 6175 746f 7374 6f70 2069 7320 7365 742e  autostop is set.
+0000e2a0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+0000e2b0: 6b79 2073 7461 7475 7320 7c20 6772 6570  ky status | grep
+0000e2c0: 207b 6e61 6d65 7d20 7c20 6772 6570 2022   {name} | grep "
+0000e2d0: 316d 2028 646f 776e 2922 272c 0a20 2020  1m (down)"',.   
+0000e2e0: 2020 2020 2020 2020 2023 2045 6e73 7572           # Ensur
+0000e2f0: 6520 7468 6520 636c 7573 7465 7220 6973  e the cluster is
+0000e300: 206e 6f74 2074 6572 6d69 6e61 7465 6420   not terminated 
+0000e310: 6561 726c 792e 0a20 2020 2020 2020 2020  early..         
+0000e320: 2020 2027 736c 6565 7020 3435 272c 0a20     'sleep 45',. 
+0000e330: 2020 2020 2020 2020 2020 2066 2773 3d24             f's=$
+0000e340: 2873 6b79 2073 7461 7475 7320 7b6e 616d  (sky status {nam
+0000e350: 657d 202d 2d72 6566 7265 7368 293b 2065  e} --refresh); e
+0000e360: 6368 6f20 2224 7322 3b20 6563 686f 3b20  cho "$s"; echo; 
+0000e370: 6563 686f 3b20 6563 686f 2022 2473 2220  echo; echo "$s" 
+0000e380: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
+0000e390: 2067 7265 7020 5550 272c 0a20 2020 2020   grep UP',.     
+0000e3a0: 2020 2020 2020 2023 2045 6e73 7572 6520         # Ensure 
+0000e3b0: 7468 6520 636c 7573 7465 7220 6973 2074  the cluster is t
+0000e3c0: 6572 6d69 6e61 7465 642e 0a20 2020 2020  erminated..     
+0000e3d0: 2020 2020 2020 2027 736c 6565 7020 3230         'sleep 20
+0000e3e0: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
+0000e3f0: 6627 733d 2428 534b 5950 494c 4f54 5f44  f's=$(SKYPILOT_D
+0000e400: 4542 5547 3d30 2073 6b79 2073 7461 7475  EBUG=0 sky statu
+0000e410: 7320 7b6e 616d 657d 202d 2d72 6566 7265  s {name} --refre
+0000e420: 7368 2920 2626 2065 6368 6f20 2224 7322  sh) && echo "$s"
+0000e430: 2026 2620 7b7b 2065 6368 6f20 2224 7322   && {{ echo "$s"
+0000e440: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
+0000e450: 2067 7265 7020 2241 7574 6f64 6f77 6e65   grep "Autodowne
+0000e460: 6420 636c 7573 7465 725c 7c74 6572 6d69  d cluster\|termi
+0000e470: 6e61 7465 6420 6f6e 2074 6865 2063 6c6f  nated on the clo
+0000e480: 7564 223b 207d 7d20 7c7c 207b 7b20 6563  ud"; }} || {{ ec
+0000e490: 686f 2022 2473 2220 7c20 6772 6570 207b  ho "$s" | grep {
+0000e4a0: 6e61 6d65 7d20 2626 2065 7869 7420 3120  name} && exit 1 
+0000e4b0: 7c7c 2065 7869 7420 303b 207d 7d27 2c0a  || exit 0; }}',.
+0000e4c0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+0000e4d0: 7920 6c61 756e 6368 202d 7920 2d64 202d  y launch -y -d -
+0000e4e0: 6320 7b6e 616d 657d 202d 2d63 6c6f 7564  c {name} --cloud
+0000e4f0: 207b 6765 6e65 7269 635f 636c 6f75 647d   {generic_cloud}
+0000e500: 202d 2d6e 756d 2d6e 6f64 6573 2032 202d   --num-nodes 2 -
+0000e510: 2d64 6f77 6e20 7465 7374 732f 7465 7374  -down tests/test
+0000e520: 5f79 616d 6c73 2f6d 696e 696d 616c 2e79  _yamls/minimal.y
+0000e530: 616d 6c27 2c0a 2020 2020 2020 2020 2020  aml',.          
+0000e540: 2020 6627 736b 7920 7374 6174 7573 207c    f'sky status |
+0000e550: 2067 7265 7020 7b6e 616d 657d 207c 2067   grep {name} | g
+0000e560: 7265 7020 5550 272c 2020 2320 456e 7375  rep UP',  # Ensu
+0000e570: 7265 2074 6865 2063 6c75 7374 6572 2069  re the cluster i
+0000e580: 7320 5550 2e0a 2020 2020 2020 2020 2020  s UP..          
+0000e590: 2020 6627 736b 7920 6578 6563 207b 6e61    f'sky exec {na
+0000e5a0: 6d65 7d20 2d2d 636c 6f75 6420 7b67 656e  me} --cloud {gen
+0000e5b0: 6572 6963 5f63 6c6f 7564 7d20 7465 7374  eric_cloud} test
+0000e5c0: 732f 7465 7374 5f79 616d 6c73 2f6d 696e  s/test_yamls/min
+0000e5d0: 696d 616c 2e79 616d 6c27 2c0a 2020 2020  imal.yaml',.    
+0000e5e0: 2020 2020 2020 2020 6627 736b 7920 7374          f'sky st
+0000e5f0: 6174 7573 207c 2067 7265 7020 7b6e 616d  atus | grep {nam
+0000e600: 657d 207c 2067 7265 7020 2231 6d20 2864  e} | grep "1m (d
+0000e610: 6f77 6e29 2227 2c0a 2020 2020 2020 2020  own)"',.        
+0000e620: 2020 2020 2773 6c65 6570 2032 3430 272c      'sleep 240',
+0000e630: 0a20 2020 2020 2020 2020 2020 2023 2045  .            # E
+0000e640: 6e73 7572 6520 7468 6520 636c 7573 7465  nsure the cluste
+0000e650: 7220 6973 2074 6572 6d69 6e61 7465 642e  r is terminated.
+0000e660: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+0000e670: 3d24 2853 4b59 5049 4c4f 545f 4445 4255  =$(SKYPILOT_DEBU
+0000e680: 473d 3020 736b 7920 7374 6174 7573 207b  G=0 sky status {
+0000e690: 6e61 6d65 7d20 2d2d 7265 6672 6573 6829  name} --refresh)
+0000e6a0: 2026 2620 6563 686f 2022 2473 2220 2626   && echo "$s" &&
+0000e6b0: 207b 7b20 6563 686f 2022 2473 2220 7c20   {{ echo "$s" | 
+0000e6c0: 6772 6570 207b 6e61 6d65 7d20 7c20 6772  grep {name} | gr
+0000e6d0: 6570 2022 4175 746f 646f 776e 6564 2063  ep "Autodowned c
+0000e6e0: 6c75 7374 6572 5c7c 7465 726d 696e 6174  luster\|terminat
+0000e6f0: 6564 206f 6e20 7468 6520 636c 6f75 6422  ed on the cloud"
+0000e700: 3b20 7d7d 207c 7c20 7b7b 2065 6368 6f20  ; }} || {{ echo 
+0000e710: 2224 7322 207c 2067 7265 7020 7b6e 616d  "$s" | grep {nam
+0000e720: 657d 2026 2620 6578 6974 2031 207c 7c20  e} && exit 1 || 
+0000e730: 6578 6974 2030 3b20 7d7d 272c 0a20 2020  exit 0; }}',.   
+0000e740: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
+0000e750: 6175 6e63 6820 2d79 202d 6420 2d63 207b  aunch -y -d -c {
+0000e760: 6e61 6d65 7d20 2d2d 636c 6f75 6420 7b67  name} --cloud {g
+0000e770: 656e 6572 6963 5f63 6c6f 7564 7d20 2d2d  eneric_cloud} --
+0000e780: 6e75 6d2d 6e6f 6465 7320 3220 2d2d 646f  num-nodes 2 --do
+0000e790: 776e 2074 6573 7473 2f74 6573 745f 7961  wn tests/test_ya
+0000e7a0: 6d6c 732f 6d69 6e69 6d61 6c2e 7961 6d6c  mls/minimal.yaml
+0000e7b0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+0000e7c0: 2773 6b79 2061 7574 6f73 746f 7020 2d79  'sky autostop -y
+0000e7d0: 207b 6e61 6d65 7d20 2d2d 6361 6e63 656c   {name} --cancel
+0000e7e0: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+0000e7f0: 736c 6565 7020 3234 3027 2c0a 2020 2020  sleep 240',.    
+0000e800: 2020 2020 2020 2020 2320 456e 7375 7265          # Ensure
+0000e810: 2074 6865 2063 6c75 7374 6572 2069 7320   the cluster is 
+0000e820: 7374 696c 6c20 5550 2e0a 2020 2020 2020  still UP..      
+0000e830: 2020 2020 2020 6627 733d 2428 534b 5950        f's=$(SKYP
+0000e840: 494c 4f54 5f44 4542 5547 3d30 2073 6b79  ILOT_DEBUG=0 sky
+0000e850: 2073 7461 7475 7320 7b6e 616d 657d 202d   status {name} -
+0000e860: 2d72 6566 7265 7368 2920 2626 2065 6368  -refresh) && ech
+0000e870: 6f20 2224 7322 2026 2620 6563 686f 2022  o "$s" && echo "
+0000e880: 2473 2220 7c20 6772 6570 207b 6e61 6d65  $s" | grep {name
+0000e890: 7d20 7c20 6772 6570 2055 5027 2c0a 2020  } | grep UP',.  
+0000e8a0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+0000e8b0: 2066 2773 6b79 2064 6f77 6e20 2d79 207b   f'sky down -y {
+0000e8c0: 6e61 6d65 7d27 2c0a 2020 2020 2020 2020  name}',.        
+0000e8d0: 7469 6d65 6f75 743d 3230 202a 2036 302c  timeout=20 * 60,
+0000e8e0: 0a20 2020 2029 0a20 2020 2072 756e 5f6f  .    ).    run_o
+0000e8f0: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
+0000e900: 4070 7974 6573 742e 6d61 726b 2e73 6370  @pytest.mark.scp
+0000e910: 0a64 6566 2074 6573 745f 7363 705f 6175  .def test_scp_au
+0000e920: 746f 646f 776e 2829 3a0a 2020 2020 6e61  todown():.    na
+0000e930: 6d65 203d 205f 6765 745f 636c 7573 7465  me = _get_cluste
+0000e940: 725f 6e61 6d65 2829 0a20 2020 2074 6573  r_name().    tes
+0000e950: 7420 3d20 5465 7374 280a 2020 2020 2020  t = Test(.      
+0000e960: 2020 2753 4350 5f61 7574 6f64 6f77 6e27    'SCP_autodown'
+0000e970: 2c0a 2020 2020 2020 2020 5b0a 2020 2020  ,.        [.    
+0000e980: 2020 2020 2020 2020 6627 736b 7920 6c61          f'sky la
+0000e990: 756e 6368 202d 7920 2d64 202d 6320 7b6e  unch -y -d -c {n
+0000e9a0: 616d 657d 207b 5343 505f 5459 5045 7d20  ame} {SCP_TYPE} 
+0000e9b0: 7465 7374 732f 7465 7374 5f79 616d 6c73  tests/test_yamls
+0000e9c0: 2f6d 696e 696d 616c 2e79 616d 6c27 2c0a  /minimal.yaml',.
+0000e9d0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+0000e9e0: 7920 6175 746f 7374 6f70 202d 7920 7b6e  y autostop -y {n
+0000e9f0: 616d 657d 202d 2d64 6f77 6e20 2d69 2031  ame} --down -i 1
+0000ea00: 272c 0a20 2020 2020 2020 2020 2020 2023  ',.            #
+0000ea10: 2045 6e73 7572 6520 6175 746f 7374 6f70   Ensure autostop
+0000ea20: 2069 7320 7365 742e 0a20 2020 2020 2020   is set..       
+0000ea30: 2020 2020 2066 2773 6b79 2073 7461 7475       f'sky statu
+0000ea40: 7320 7c20 6772 6570 207b 6e61 6d65 7d20  s | grep {name} 
+0000ea50: 7c20 6772 6570 2022 316d 2028 646f 776e  | grep "1m (down
+0000ea60: 2922 272c 0a20 2020 2020 2020 2020 2020  )"',.           
+0000ea70: 2023 2045 6e73 7572 6520 7468 6520 636c   # Ensure the cl
+0000ea80: 7573 7465 7220 6973 206e 6f74 2074 6572  uster is not ter
+0000ea90: 6d69 6e61 7465 6420 6561 726c 792e 0a20  minated early.. 
+0000eaa0: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
+0000eab0: 7020 3435 272c 0a20 2020 2020 2020 2020  p 45',.         
+0000eac0: 2020 2066 2773 6b79 2073 7461 7475 7320     f'sky status 
+0000ead0: 2d2d 7265 6672 6573 6820 7c20 6772 6570  --refresh | grep
+0000eae0: 207b 6e61 6d65 7d20 7c20 6772 6570 2055   {name} | grep U
+0000eaf0: 5027 2c0a 2020 2020 2020 2020 2020 2020  P',.            
+0000eb00: 2320 456e 7375 7265 2074 6865 2063 6c75  # Ensure the clu
+0000eb10: 7374 6572 2069 7320 7465 726d 696e 6174  ster is terminat
+0000eb20: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+0000eb30: 2773 6c65 6570 2032 3030 272c 0a20 2020  'sleep 200',.   
+0000eb40: 2020 2020 2020 2020 2066 2773 3d24 2853           f's=$(S
+0000eb50: 4b59 5049 4c4f 545f 4445 4255 473d 3020  KYPILOT_DEBUG=0 
+0000eb60: 736b 7920 7374 6174 7573 202d 2d72 6566  sky status --ref
+0000eb70: 7265 7368 2920 2626 2070 7269 6e74 6620  resh) && printf 
+0000eb80: 2224 7322 2026 2620 7b7b 2065 6368 6f20  "$s" && {{ echo 
+0000eb90: 2224 7322 207c 2067 7265 7020 7b6e 616d  "$s" | grep {nam
+0000eba0: 657d 207c 2067 7265 7020 2241 7574 6f64  e} | grep "Autod
+0000ebb0: 6f77 6e65 6420 636c 7573 7465 725c 7c74  owned cluster\|t
+0000ebc0: 6572 6d69 6e61 7465 6420 6f6e 2074 6865  erminated on the
+0000ebd0: 2063 6c6f 7564 223b 207d 7d20 7c7c 207b   cloud"; }} || {
+0000ebe0: 7b20 6563 686f 2022 2473 2220 7c20 6772  { echo "$s" | gr
+0000ebf0: 6570 207b 6e61 6d65 7d20 2626 2065 7869  ep {name} && exi
+0000ec00: 7420 3120 7c7c 2065 7869 7420 303b 207d  t 1 || exit 0; }
+0000ec10: 7d27 2c0a 2020 2020 2020 2020 2020 2020  }',.            
+0000ec20: 6627 736b 7920 6c61 756e 6368 202d 7920  f'sky launch -y 
+0000ec30: 2d64 202d 6320 7b6e 616d 657d 207b 5343  -d -c {name} {SC
+0000ec40: 505f 5459 5045 7d20 2d2d 646f 776e 2074  P_TYPE} --down t
+0000ec50: 6573 7473 2f74 6573 745f 7961 6d6c 732f  ests/test_yamls/
+0000ec60: 6d69 6e69 6d61 6c2e 7961 6d6c 272c 0a20  minimal.yaml',. 
+0000ec70: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+0000ec80: 2073 7461 7475 7320 7c20 6772 6570 207b   status | grep {
+0000ec90: 6e61 6d65 7d20 7c20 6772 6570 2055 5027  name} | grep UP'
+0000eca0: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
+0000ecb0: 636c 7573 7465 7220 6973 2055 502e 0a20  cluster is UP.. 
+0000ecc0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+0000ecd0: 2065 7865 6320 7b6e 616d 657d 207b 5343   exec {name} {SC
+0000ece0: 505f 5459 5045 7d20 7465 7374 732f 7465  P_TYPE} tests/te
+0000ecf0: 7374 5f79 616d 6c73 2f6d 696e 696d 616c  st_yamls/minimal
+0000ed00: 2e79 616d 6c27 2c0a 2020 2020 2020 2020  .yaml',.        
+0000ed10: 2020 2020 6627 736b 7920 7374 6174 7573      f'sky status
+0000ed20: 207c 2067 7265 7020 7b6e 616d 657d 207c   | grep {name} |
+0000ed30: 2067 7265 7020 2231 6d20 2864 6f77 6e29   grep "1m (down)
+0000ed40: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+0000ed50: 2773 6c65 6570 2032 3030 272c 0a20 2020  'sleep 200',.   
+0000ed60: 2020 2020 2020 2020 2023 2045 6e73 7572           # Ensur
+0000ed70: 6520 7468 6520 636c 7573 7465 7220 6973  e the cluster is
+0000ed80: 2074 6572 6d69 6e61 7465 642e 0a20 2020   terminated..   
+0000ed90: 2020 2020 2020 2020 2066 2773 3d24 2853           f's=$(S
+0000eda0: 4b59 5049 4c4f 545f 4445 4255 473d 3020  KYPILOT_DEBUG=0 
+0000edb0: 736b 7920 7374 6174 7573 202d 2d72 6566  sky status --ref
+0000edc0: 7265 7368 2920 2626 2070 7269 6e74 6620  resh) && printf 
+0000edd0: 2224 7322 2026 2620 7b7b 2065 6368 6f20  "$s" && {{ echo 
+0000ede0: 2224 7322 207c 2067 7265 7020 7b6e 616d  "$s" | grep {nam
+0000edf0: 657d 207c 2067 7265 7020 2241 7574 6f64  e} | grep "Autod
+0000ee00: 6f77 6e65 6420 636c 7573 7465 725c 7c74  owned cluster\|t
+0000ee10: 6572 6d69 6e61 7465 6420 6f6e 2074 6865  erminated on the
+0000ee20: 2063 6c6f 7564 223b 207d 7d20 7c7c 207b   cloud"; }} || {
+0000ee30: 7b20 6563 686f 2022 2473 2220 7c20 6772  { echo "$s" | gr
+0000ee40: 6570 207b 6e61 6d65 7d20 2626 2065 7869  ep {name} && exi
+0000ee50: 7420 3120 7c7c 2065 7869 7420 303b 207d  t 1 || exit 0; }
+0000ee60: 7d27 2c0a 2020 2020 2020 2020 2020 2020  }',.            
+0000ee70: 6627 736b 7920 6c61 756e 6368 202d 7920  f'sky launch -y 
+0000ee80: 2d64 202d 6320 7b6e 616d 657d 207b 5343  -d -c {name} {SC
+0000ee90: 505f 5459 5045 7d20 2d2d 646f 776e 2074  P_TYPE} --down t
+0000eea0: 6573 7473 2f74 6573 745f 7961 6d6c 732f  ests/test_yamls/
+0000eeb0: 6d69 6e69 6d61 6c2e 7961 6d6c 272c 0a20  minimal.yaml',. 
+0000eec0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+0000eed0: 2061 7574 6f73 746f 7020 2d79 207b 6e61   autostop -y {na
+0000eee0: 6d65 7d20 2d2d 6361 6e63 656c 272c 0a20  me} --cancel',. 
+0000eef0: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
+0000ef00: 7020 3230 3027 2c0a 2020 2020 2020 2020  p 200',.        
+0000ef10: 2020 2020 2320 456e 7375 7265 2074 6865      # Ensure the
+0000ef20: 2063 6c75 7374 6572 2069 7320 7374 696c   cluster is stil
+0000ef30: 6c20 5550 2e0a 2020 2020 2020 2020 2020  l UP..          
+0000ef40: 2020 6627 733d 2428 534b 5950 494c 4f54    f's=$(SKYPILOT
+0000ef50: 5f44 4542 5547 3d30 2073 6b79 2073 7461  _DEBUG=0 sky sta
+0000ef60: 7475 7320 2d2d 7265 6672 6573 6829 2026  tus --refresh) &
+0000ef70: 2620 7072 696e 7466 2022 2473 2220 2626  & printf "$s" &&
+0000ef80: 2065 6368 6f20 2224 7322 207c 2067 7265   echo "$s" | gre
+0000ef90: 7020 7b6e 616d 657d 207c 2067 7265 7020  p {name} | grep 
+0000efa0: 5550 272c 0a20 2020 2020 2020 205d 2c0a  UP',.        ],.
+0000efb0: 2020 2020 2020 2020 6627 736b 7920 646f          f'sky do
+0000efc0: 776e 202d 7920 7b6e 616d 657d 272c 0a20  wn -y {name}',. 
+0000efd0: 2020 2020 2020 2074 696d 656f 7574 3d32         timeout=2
+0000efe0: 3520 2a20 3630 2c0a 2020 2020 290a 2020  5 * 60,.    ).  
+0000eff0: 2020 7275 6e5f 6f6e 655f 7465 7374 2874    run_one_test(t
+0000f000: 6573 7429 0a0a 0a64 6566 205f 6765 745f  est)...def _get_
+0000f010: 6361 6e63 656c 5f74 6173 6b5f 7769 7468  cancel_task_with
+0000f020: 5f63 6c6f 7564 286e 616d 652c 2063 6c6f  _cloud(name, clo
+0000f030: 7564 2c20 7469 6d65 6f75 743d 3135 202a  ud, timeout=15 *
+0000f040: 2036 3029 3a0a 2020 2020 7465 7374 203d   60):.    test =
+0000f050: 2054 6573 7428 0a20 2020 2020 2020 2066   Test(.        f
+0000f060: 277b 636c 6f75 647d 2d63 616e 6365 6c2d  '{cloud}-cancel-
+0000f070: 7461 736b 272c 0a20 2020 2020 2020 205b  task',.        [
+0000f080: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+0000f090: 6b79 206c 6175 6e63 6820 2d63 207b 6e61  ky launch -c {na
+0000f0a0: 6d65 7d20 6578 616d 706c 6573 2f72 6573  me} examples/res
+0000f0b0: 6e65 745f 6170 702e 7961 6d6c 202d 2d63  net_app.yaml --c
+0000f0c0: 6c6f 7564 207b 636c 6f75 647d 202d 7920  loud {cloud} -y 
+0000f0d0: 2d64 272c 0a20 2020 2020 2020 2020 2020  -d',.           
+0000f0e0: 2023 2057 6169 7420 7468 6520 4750 5520   # Wait the GPU 
+0000f0f0: 7072 6f63 6573 7320 746f 2073 7461 7274  process to start
+0000f100: 2e0a 2020 2020 2020 2020 2020 2020 2773  ..            's
+0000f110: 6c65 6570 2036 3027 2c0a 2020 2020 2020  leep 60',.      
+0000f120: 2020 2020 2020 6627 736b 7920 6578 6563        f'sky exec
+0000f130: 207b 6e61 6d65 7d20 226e 7669 6469 612d   {name} "nvidia-
+0000f140: 736d 6920 7c20 6772 6570 2070 7974 686f  smi | grep pytho
+0000f150: 6e22 272c 0a20 2020 2020 2020 2020 2020  n"',.           
+0000f160: 2066 2773 6b79 206c 6f67 7320 7b6e 616d   f'sky logs {nam
+0000f170: 657d 2032 202d 2d73 7461 7475 7327 2c20  e} 2 --status', 
+0000f180: 2023 2045 6e73 7572 6520 7468 6520 6a6f   # Ensure the jo
+0000f190: 6220 7375 6363 6565 6465 642e 0a20 2020  b succeeded..   
+0000f1a0: 2020 2020 2020 2020 2066 2773 6b79 2063           f'sky c
+0000f1b0: 616e 6365 6c20 2d79 207b 6e61 6d65 7d20  ancel -y {name} 
+0000f1c0: 3127 2c0a 2020 2020 2020 2020 2020 2020  1',.            
+0000f1d0: 2773 6c65 6570 2036 3027 2c0a 2020 2020  'sleep 60',.    
+0000f1e0: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
+0000f1f0: 6966 2074 6865 2070 7974 686f 6e20 6a6f  if the python jo
+0000f200: 6220 6973 2067 6f6e 652e 0a20 2020 2020  b is gone..     
+0000f210: 2020 2020 2020 2066 2773 6b79 2065 7865         f'sky exe
+0000f220: 6320 7b6e 616d 657d 2022 2120 6e76 6964  c {name} "! nvid
+0000f230: 6961 2d73 6d69 207c 2067 7265 7020 7079  ia-smi | grep py
+0000f240: 7468 6f6e 2227 2c0a 2020 2020 2020 2020  thon"',.        
+0000f250: 2020 2020 6627 736b 7920 6c6f 6773 207b      f'sky logs {
+0000f260: 6e61 6d65 7d20 3320 2d2d 7374 6174 7573  name} 3 --status
+0000f270: 272c 2020 2320 456e 7375 7265 2074 6865  ',  # Ensure the
+0000f280: 206a 6f62 2073 7563 6365 6564 6564 2e0a   job succeeded..
+0000f290: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+0000f2a0: 2020 2066 2773 6b79 2064 6f77 6e20 2d79     f'sky down -y
+0000f2b0: 207b 6e61 6d65 7d27 2c0a 2020 2020 2020   {name}',.      
+0000f2c0: 2020 7469 6d65 6f75 743d 7469 6d65 6f75    timeout=timeou
+0000f2d0: 742c 0a20 2020 2029 0a20 2020 2072 6574  t,.    ).    ret
+0000f2e0: 7572 6e20 7465 7374 0a0a 0a23 202d 2d2d  urn test...# ---
+0000f2f0: 2d2d 2d2d 2d2d 2d20 5465 7374 696e 6720  ------- Testing 
+0000f300: 6073 6b79 2063 616e 6365 6c60 202d 2d2d  `sky cancel` ---
+0000f310: 2d2d 2d2d 2d2d 2d0a 4070 7974 6573 742e  -------.@pytest.
+0000f320: 6d61 726b 2e61 7773 0a40 7079 7465 7374  mark.aws.@pytest
+0000f330: 2e6d 6172 6b2e 736b 6970 280a 2020 2020  .mark.skip(.    
+0000f340: 7265 6173 6f6e 3d27 5468 6520 7265 736e  reason='The resn
+0000f350: 6574 5f61 7070 2069 7320 666c 616b 792c  et_app is flaky,
+0000f360: 2064 7565 2074 6f20 5446 2066 6169 6c69   due to TF faili
+0000f370: 6e67 2074 6f20 6465 7465 6374 2047 5055  ng to detect GPU
+0000f380: 732e 2729 0a64 6566 2074 6573 745f 6361  s.').def test_ca
+0000f390: 6e63 656c 5f61 7773 2829 3a0a 2020 2020  ncel_aws():.    
+0000f3a0: 6e61 6d65 203d 205f 6765 745f 636c 7573  name = _get_clus
+0000f3b0: 7465 725f 6e61 6d65 2829 0a20 2020 2074  ter_name().    t
+0000f3c0: 6573 7420 3d20 5f67 6574 5f63 616e 6365  est = _get_cance
+0000f3d0: 6c5f 7461 736b 5f77 6974 685f 636c 6f75  l_task_with_clou
+0000f3e0: 6428 6e61 6d65 2c20 2761 7773 2729 0a20  d(name, 'aws'). 
+0000f3f0: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+0000f400: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
+0000f410: 6d61 726b 2e67 6370 0a40 7079 7465 7374  mark.gcp.@pytest
+0000f420: 2e6d 6172 6b2e 736b 6970 280a 2020 2020  .mark.skip(.    
+0000f430: 7265 6173 6f6e 3d27 5468 6520 7265 736e  reason='The resn
+0000f440: 6574 5f61 7070 2069 7320 666c 616b 792c  et_app is flaky,
+0000f450: 2064 7565 2074 6f20 5446 2066 6169 6c69   due to TF faili
+0000f460: 6e67 2074 6f20 6465 7465 6374 2047 5055  ng to detect GPU
+0000f470: 732e 2729 0a64 6566 2074 6573 745f 6361  s.').def test_ca
+0000f480: 6e63 656c 5f67 6370 2829 3a0a 2020 2020  ncel_gcp():.    
+0000f490: 6e61 6d65 203d 205f 6765 745f 636c 7573  name = _get_clus
+0000f4a0: 7465 725f 6e61 6d65 2829 0a20 2020 2074  ter_name().    t
+0000f4b0: 6573 7420 3d20 5f67 6574 5f63 616e 6365  est = _get_cance
+0000f4c0: 6c5f 7461 736b 5f77 6974 685f 636c 6f75  l_task_with_clou
+0000f4d0: 6428 6e61 6d65 2c20 2767 6370 2729 0a20  d(name, 'gcp'). 
+0000f4e0: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+0000f4f0: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
+0000f500: 6d61 726b 2e61 7a75 7265 0a40 7079 7465  mark.azure.@pyte
+0000f510: 7374 2e6d 6172 6b2e 736b 6970 280a 2020  st.mark.skip(.  
+0000f520: 2020 7265 6173 6f6e 3d27 5468 6520 7265    reason='The re
+0000f530: 736e 6574 5f61 7070 2069 7320 666c 616b  snet_app is flak
+0000f540: 792c 2064 7565 2074 6f20 5446 2066 6169  y, due to TF fai
+0000f550: 6c69 6e67 2074 6f20 6465 7465 6374 2047  ling to detect G
+0000f560: 5055 732e 2729 0a64 6566 2074 6573 745f  PUs.').def test_
+0000f570: 6361 6e63 656c 5f61 7a75 7265 2829 3a0a  cancel_azure():.
+0000f580: 2020 2020 6e61 6d65 203d 205f 6765 745f      name = _get_
+0000f590: 636c 7573 7465 725f 6e61 6d65 2829 0a20  cluster_name(). 
+0000f5a0: 2020 2074 6573 7420 3d20 5f67 6574 5f63     test = _get_c
+0000f5b0: 616e 6365 6c5f 7461 736b 5f77 6974 685f  ancel_task_with_
+0000f5c0: 636c 6f75 6428 6e61 6d65 2c20 2761 7a75  cloud(name, 'azu
+0000f5d0: 7265 272c 2074 696d 656f 7574 3d33 3020  re', timeout=30 
+0000f5e0: 2a20 3630 290a 2020 2020 7275 6e5f 6f6e  * 60).    run_on
+0000f5f0: 655f 7465 7374 2874 6573 7429 0a0a 0a40  e_test(test)...@
+0000f600: 7079 7465 7374 2e6d 6172 6b2e 6e6f 5f6c  pytest.mark.no_l
+0000f610: 616d 6264 615f 636c 6f75 6420 2023 204c  ambda_cloud  # L
+0000f620: 616d 6264 6120 436c 6f75 6420 646f 6573  ambda Cloud does
+0000f630: 206e 6f74 2068 6176 6520 5631 3030 2067   not have V100 g
+0000f640: 7075 730a 4070 7974 6573 742e 6d61 726b  pus.@pytest.mark
+0000f650: 2e6e 6f5f 6962 6d20 2023 2049 424d 2063  .no_ibm  # IBM c
+0000f660: 6c6f 7564 2063 7572 7265 6e74 6c79 2064  loud currently d
+0000f670: 6f65 736e 2774 2070 726f 7669 6465 2070  oesn't provide p
+0000f680: 7562 6c69 6320 696d 6167 6520 7769 7468  ublic image with
+0000f690: 2043 5544 410a 4070 7974 6573 742e 6d61   CUDA.@pytest.ma
+0000f6a0: 726b 2e6e 6f5f 7363 7020 2023 2053 4350  rk.no_scp  # SCP
+0000f6b0: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
+0000f6c0: 7420 6e75 6d5f 6e6f 6465 7320 3e20 3120  t num_nodes > 1 
+0000f6d0: 7965 740a 6465 6620 7465 7374 5f63 616e  yet.def test_can
+0000f6e0: 6365 6c5f 7079 746f 7263 6828 6765 6e65  cel_pytorch(gene
+0000f6f0: 7269 635f 636c 6f75 643a 2073 7472 293a  ric_cloud: str):
+0000f700: 0a20 2020 206e 616d 6520 3d20 5f67 6574  .    name = _get
+0000f710: 5f63 6c75 7374 6572 5f6e 616d 6528 290a  _cluster_name().
+0000f720: 2020 2020 7465 7374 203d 2054 6573 7428      test = Test(
+0000f730: 0a20 2020 2020 2020 2027 6361 6e63 656c  .        'cancel
+0000f740: 2d70 7974 6f72 6368 272c 0a20 2020 2020  -pytorch',.     
+0000f750: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+0000f760: 2066 2773 6b79 206c 6175 6e63 6820 2d63   f'sky launch -c
+0000f770: 207b 6e61 6d65 7d20 2d2d 636c 6f75 6420   {name} --cloud 
+0000f780: 7b67 656e 6572 6963 5f63 6c6f 7564 7d20  {generic_cloud} 
+0000f790: 6578 616d 706c 6573 2f72 6573 6e65 745f  examples/resnet_
+0000f7a0: 6469 7374 7269 6275 7465 645f 746f 7263  distributed_torc
+0000f7b0: 682e 7961 6d6c 202d 7920 2d64 272c 0a20  h.yaml -y -d',. 
+0000f7c0: 2020 2020 2020 2020 2020 2023 2057 6169             # Wai
+0000f7d0: 7420 7468 6520 4750 5520 7072 6f63 6573  t the GPU proces
+0000f7e0: 7320 746f 2073 7461 7274 2e0a 2020 2020  s to start..    
+0000f7f0: 2020 2020 2020 2020 2773 6c65 6570 2039          'sleep 9
+0000f800: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
+0000f810: 6627 736b 7920 6578 6563 207b 6e61 6d65  f'sky exec {name
+0000f820: 7d20 226e 7669 6469 612d 736d 6920 7c20  } "nvidia-smi | 
+0000f830: 6772 6570 2070 7974 686f 6e22 272c 0a20  grep python"',. 
+0000f840: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+0000f850: 206c 6f67 7320 7b6e 616d 657d 2032 202d   logs {name} 2 -
+0000f860: 2d73 7461 7475 7327 2c20 2023 2045 6e73  -status',  # Ens
+0000f870: 7572 6520 7468 6520 6a6f 6220 7375 6363  ure the job succ
+0000f880: 6565 6465 642e 0a20 2020 2020 2020 2020  eeded..         
+0000f890: 2020 2066 2773 6b79 2063 616e 6365 6c20     f'sky cancel 
+0000f8a0: 2d79 207b 6e61 6d65 7d20 3127 2c0a 2020  -y {name} 1',.  
+0000f8b0: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
+0000f8c0: 2036 3027 2c0a 2020 2020 2020 2020 2020   60',.          
+0000f8d0: 2020 6627 736b 7920 6578 6563 207b 6e61    f'sky exec {na
+0000f8e0: 6d65 7d20 2228 6e76 6964 6961 2d73 6d69  me} "(nvidia-smi
+0000f8f0: 207c 2067 7265 7020 5c27 4e6f 2072 756e   | grep \'No run
+0000f900: 6e69 6e67 2070 726f 6365 7373 5c27 2920  ning process\') 
+0000f910: 7c7c 2027 0a20 2020 2020 2020 2020 2020  || '.           
+0000f920: 2023 2045 6e73 7572 6520 586f 7267 2069   # Ensure Xorg i
+0000f930: 7320 7468 6520 6f6e 6c79 2070 726f 6365  s the only proce
+0000f940: 7373 2072 756e 6e69 6e67 2e0a 2020 2020  ss running..    
+0000f950: 2020 2020 2020 2020 275b 205c 2428 6e76          '[ \$(nv
+0000f960: 6964 6961 2d73 6d69 207c 2067 7265 7020  idia-smi | grep 
+0000f970: 2d41 2031 3020 5072 6f63 6573 7365 7320  -A 10 Processes 
+0000f980: 7c20 6772 6570 202d 4120 3130 203d 3d3d  | grep -A 10 ===
+0000f990: 207c 2067 7265 7020 2d76 2058 6f72 6729   | grep -v Xorg)
+0000f9a0: 202d 6571 2032 205d 2227 2c0a 2020 2020   -eq 2 ]"',.    
+0000f9b0: 2020 2020 2020 2020 6627 736b 7920 6c6f          f'sky lo
+0000f9c0: 6773 207b 6e61 6d65 7d20 3320 2d2d 7374  gs {name} 3 --st
+0000f9d0: 6174 7573 272c 2020 2320 456e 7375 7265  atus',  # Ensure
+0000f9e0: 2074 6865 206a 6f62 2073 7563 6365 6564   the job succeed
+0000f9f0: 6564 2e0a 2020 2020 2020 2020 5d2c 0a20  ed..        ],. 
+0000fa00: 2020 2020 2020 2066 2773 6b79 2064 6f77         f'sky dow
+0000fa10: 6e20 2d79 207b 6e61 6d65 7d27 2c0a 2020  n -y {name}',.  
+0000fa20: 2020 2020 2020 7469 6d65 6f75 743d 3230        timeout=20
+0000fa30: 202a 2036 302c 0a20 2020 2029 0a20 2020   * 60,.    ).   
+0000fa40: 2072 756e 5f6f 6e65 5f74 6573 7428 7465   run_one_test(te
+0000fa50: 7374 290a 0a0a 2320 6361 6e27 7420 7573  st)...# can't us
+0000fa60: 6520 605f 6765 745f 6361 6e63 656c 5f74  e `_get_cancel_t
+0000fa70: 6173 6b5f 7769 7468 5f63 6c6f 7564 2829  ask_with_cloud()
+0000fa80: 602c 2061 7320 636f 6d6d 616e 6420 606e  `, as command `n
+0000fa90: 7669 6469 612d 736d 6960 0a23 2072 6571  vidia-smi`.# req
+0000faa0: 7569 7265 7320 6120 4355 4441 2070 7562  uires a CUDA pub
+0000fab0: 6c69 6320 696d 6167 652c 2077 6869 6368  lic image, which
+0000fac0: 2049 424d 2064 6f65 736e 2774 206f 6666   IBM doesn't off
+0000fad0: 6572 0a40 7079 7465 7374 2e6d 6172 6b2e  er.@pytest.mark.
+0000fae0: 6962 6d0a 6465 6620 7465 7374 5f63 616e  ibm.def test_can
+0000faf0: 6365 6c5f 6962 6d28 293a 0a20 2020 206e  cel_ibm():.    n
+0000fb00: 616d 6520 3d20 5f67 6574 5f63 6c75 7374  ame = _get_clust
+0000fb10: 6572 5f6e 616d 6528 290a 2020 2020 7465  er_name().    te
+0000fb20: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
+0000fb30: 2020 2027 6962 6d2d 6361 6e63 656c 2d74     'ibm-cancel-t
+0000fb40: 6173 6b27 2c0a 2020 2020 2020 2020 5b0a  ask',.        [.
+0000fb50: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+0000fb60: 7920 6c61 756e 6368 202d 7920 2d63 207b  y launch -y -c {
+0000fb70: 6e61 6d65 7d20 2d2d 636c 6f75 6420 6962  name} --cloud ib
+0000fb80: 6d20 6578 616d 706c 6573 2f6d 696e 696d  m examples/minim
+0000fb90: 616c 2e79 616d 6c27 2c0a 2020 2020 2020  al.yaml',.      
+0000fba0: 2020 2020 2020 6627 736b 7920 6578 6563        f'sky exec
+0000fbb0: 207b 6e61 6d65 7d20 2d6e 207b 6e61 6d65   {name} -n {name
+0000fbc0: 7d2d 3120 2d64 2020 2277 6869 6c65 2074  }-1 -d  "while t
+0000fbd0: 7275 653b 2064 6f20 6563 686f 205c 2748  rue; do echo \'H
+0000fbe0: 656c 6c6f 2053 6b79 5069 6c6f 745c 273b  ello SkyPilot\';
+0000fbf0: 2073 6c65 6570 2032 3b20 646f 6e65 2227   sleep 2; done"'
+0000fc00: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
+0000fc10: 6c65 6570 2032 3027 2c0a 2020 2020 2020  leep 20',.      
+0000fc20: 2020 2020 2020 6627 736b 7920 7175 6575        f'sky queu
+0000fc30: 6520 7b6e 616d 657d 207c 2067 7265 7020  e {name} | grep 
+0000fc40: 7b6e 616d 657d 2d31 207c 2067 7265 7020  {name}-1 | grep 
+0000fc50: 5255 4e4e 494e 4727 2c0a 2020 2020 2020  RUNNING',.      
+0000fc60: 2020 2020 2020 6627 736b 7920 6361 6e63        f'sky canc
+0000fc70: 656c 202d 7920 7b6e 616d 657d 2032 272c  el -y {name} 2',
+0000fc80: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+0000fc90: 6c65 6570 2035 272c 0a20 2020 2020 2020  leep 5',.       
+0000fca0: 2020 2020 2066 2773 6b79 2071 7565 7565       f'sky queue
+0000fcb0: 207b 6e61 6d65 7d20 7c20 6772 6570 207b   {name} | grep {
+0000fcc0: 6e61 6d65 7d2d 3120 7c20 6772 6570 2043  name}-1 | grep C
+0000fcd0: 414e 4345 4c4c 4544 272c 0a20 2020 2020  ANCELLED',.     
+0000fce0: 2020 205d 2c0a 2020 2020 2020 2020 6627     ],.        f'
+0000fcf0: 736b 7920 646f 776e 202d 7920 7b6e 616d  sky down -y {nam
+0000fd00: 657d 272c 0a20 2020 2029 0a20 2020 2072  e}',.    ).    r
+0000fd10: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
+0000fd20: 290a 0a0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  )...# ----------
+0000fd30: 2054 6573 7469 6e67 2075 7365 2d73 706f   Testing use-spo
+0000fd40: 7420 6f70 7469 6f6e 202d 2d2d 2d2d 2d2d  t option -------
+0000fd50: 2d2d 2d0a 4070 7974 6573 742e 6d61 726b  ---.@pytest.mark
+0000fd60: 2e6e 6f5f 6c61 6d62 6461 5f63 6c6f 7564  .no_lambda_cloud
+0000fd70: 2020 2320 4c61 6d62 6461 2043 6c6f 7564    # Lambda Cloud
+0000fd80: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
+0000fd90: 7420 7370 6f74 2069 6e73 7461 6e63 6573  t spot instances
+0000fda0: 0a40 7079 7465 7374 2e6d 6172 6b2e 6e6f  .@pytest.mark.no
+0000fdb0: 5f69 626d 2020 2320 4942 4d20 436c 6f75  _ibm  # IBM Clou
+0000fdc0: 6420 646f 6573 206e 6f74 2073 7570 706f  d does not suppo
+0000fdd0: 7274 2073 706f 7420 696e 7374 616e 6365  rt spot instance
+0000fde0: 730a 4070 7974 6573 742e 6d61 726b 2e6e  s.@pytest.mark.n
+0000fdf0: 6f5f 7363 7020 2023 2053 4350 2064 6f65  o_scp  # SCP doe
+0000fe00: 7320 6e6f 7420 7375 7070 6f72 7420 7370  s not support sp
+0000fe10: 6f74 2069 6e73 7461 6e63 6573 0a64 6566  ot instances.def
+0000fe20: 2074 6573 745f 7573 655f 7370 6f74 2867   test_use_spot(g
+0000fe30: 656e 6572 6963 5f63 6c6f 7564 3a20 7374  eneric_cloud: st
+0000fe40: 7229 3a0a 2020 2020 2222 2254 6573 7420  r):.    """Test 
+0000fe50: 7573 652d 7370 6f74 2061 6e64 2073 6b79  use-spot and sky
+0000fe60: 2065 7865 632e 2222 220a 2020 2020 6e61   exec.""".    na
+0000fe70: 6d65 203d 205f 6765 745f 636c 7573 7465  me = _get_cluste
+0000fe80: 725f 6e61 6d65 2829 0a20 2020 2074 6573  r_name().    tes
+0000fe90: 7420 3d20 5465 7374 280a 2020 2020 2020  t = Test(.      
+0000fea0: 2020 2775 7365 2d73 706f 7427 2c0a 2020    'use-spot',.  
+0000feb0: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+0000fec0: 2020 2020 6627 736b 7920 6c61 756e 6368      f'sky launch
+0000fed0: 202d 6320 7b6e 616d 657d 202d 2d63 6c6f   -c {name} --clo
+0000fee0: 7564 207b 6765 6e65 7269 635f 636c 6f75  ud {generic_clou
+0000fef0: 647d 2074 6573 7473 2f74 6573 745f 7961  d} tests/test_ya
+0000ff00: 6d6c 732f 6d69 6e69 6d61 6c2e 7961 6d6c  mls/minimal.yaml
+0000ff10: 202d 2d75 7365 2d73 706f 7420 2d79 272c   --use-spot -y',
+0000ff20: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+0000ff30: 6b79 206c 6f67 7320 7b6e 616d 657d 2031  ky logs {name} 1
+0000ff40: 202d 2d73 7461 7475 7327 2c0a 2020 2020   --status',.    
+0000ff50: 2020 2020 2020 2020 6627 736b 7920 6578          f'sky ex
+0000ff60: 6563 207b 6e61 6d65 7d20 6563 686f 2068  ec {name} echo h
+0000ff70: 6927 2c0a 2020 2020 2020 2020 2020 2020  i',.            
+0000ff80: 6627 736b 7920 6c6f 6773 207b 6e61 6d65  f'sky logs {name
+0000ff90: 7d20 3220 2d2d 7374 6174 7573 272c 0a20  } 2 --status',. 
+0000ffa0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+0000ffb0: 2020 6627 736b 7920 646f 776e 202d 7920    f'sky down -y 
+0000ffc0: 7b6e 616d 657d 272c 0a20 2020 2029 0a20  {name}',.    ). 
+0000ffd0: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+0000ffe0: 7465 7374 290a 0a0a 2320 2d2d 2d2d 2d2d  test)...# ------
+0000fff0: 2d2d 2d2d 2054 6573 7469 6e67 206d 616e  ---- Testing man
+00010000: 6167 6564 2073 706f 7420 2d2d 2d2d 2d2d  aged spot ------
+00010010: 2d2d 2d2d 0a40 7079 7465 7374 2e6d 6172  ----.@pytest.mar
+00010020: 6b2e 6e6f 5f6c 616d 6264 615f 636c 6f75  k.no_lambda_clou
+00010030: 6420 2023 204c 616d 6264 6120 436c 6f75  d  # Lambda Clou
+00010040: 6420 646f 6573 206e 6f74 2073 7570 706f  d does not suppo
+00010050: 7274 2073 706f 7420 696e 7374 616e 6365  rt spot instance
+00010060: 730a 4070 7974 6573 742e 6d61 726b 2e6e  s.@pytest.mark.n
+00010070: 6f5f 6962 6d20 2023 2049 424d 2043 6c6f  o_ibm  # IBM Clo
+00010080: 7564 2064 6f65 7320 6e6f 7420 7375 7070  ud does not supp
+00010090: 6f72 7420 7370 6f74 2069 6e73 7461 6e63  ort spot instanc
+000100a0: 6573 0a40 7079 7465 7374 2e6d 6172 6b2e  es.@pytest.mark.
+000100b0: 6e6f 5f73 6370 2020 2320 5343 5020 646f  no_scp  # SCP do
+000100c0: 6573 206e 6f74 2073 7570 706f 7274 2073  es not support s
+000100d0: 706f 7420 696e 7374 616e 6365 730a 4070  pot instances.@p
+000100e0: 7974 6573 742e 6d61 726b 2e6d 616e 6167  ytest.mark.manag
+000100f0: 6564 5f73 706f 740a 6465 6620 7465 7374  ed_spot.def test
+00010100: 5f73 706f 7428 6765 6e65 7269 635f 636c  _spot(generic_cl
+00010110: 6f75 643a 2073 7472 293a 0a20 2020 2022  oud: str):.    "
+00010120: 2222 5465 7374 2074 6865 2073 706f 7420  ""Test the spot 
+00010130: 7961 6d6c 2e22 2222 0a20 2020 206e 616d  yaml.""".    nam
+00010140: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
+00010150: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
+00010160: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
+00010170: 2027 6d61 6e61 6765 642d 7370 6f74 272c   'managed-spot',
+00010180: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
+00010190: 2020 2020 2020 2066 2773 6b79 2073 706f         f'sky spo
+000101a0: 7420 6c61 756e 6368 202d 6e20 7b6e 616d  t launch -n {nam
+000101b0: 657d 2d31 202d 2d63 6c6f 7564 207b 6765  e}-1 --cloud {ge
+000101c0: 6e65 7269 635f 636c 6f75 647d 2065 7861  neric_cloud} exa
+000101d0: 6d70 6c65 732f 6d61 6e61 6765 645f 7370  mples/managed_sp
+000101e0: 6f74 2e79 616d 6c20 2d79 202d 6427 2c0a  ot.yaml -y -d',.
+000101f0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+00010200: 7920 7370 6f74 206c 6175 6e63 6820 2d6e  y spot launch -n
+00010210: 207b 6e61 6d65 7d2d 3220 2d2d 636c 6f75   {name}-2 --clou
+00010220: 6420 7b67 656e 6572 6963 5f63 6c6f 7564  d {generic_cloud
+00010230: 7d20 6578 616d 706c 6573 2f6d 616e 6167  } examples/manag
+00010240: 6564 5f73 706f 742e 7961 6d6c 202d 7920  ed_spot.yaml -y 
+00010250: 2d64 272c 0a20 2020 2020 2020 2020 2020  -d',.           
+00010260: 2027 736c 6565 7020 3527 2c0a 2020 2020   'sleep 5',.    
+00010270: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
+00010280: 5f51 5545 5545 5f57 4149 547d 7c20 6772  _QUEUE_WAIT}| gr
+00010290: 6570 207b 6e61 6d65 7d2d 3120 7c20 6865  ep {name}-1 | he
+000102a0: 6164 202d 6e31 207c 2067 7265 7020 2253  ad -n1 | grep "S
+000102b0: 5441 5254 494e 475c 7c52 554e 4e49 4e47  TARTING\|RUNNING
+000102c0: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+000102d0: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
+000102e0: 4149 547d 7c20 6772 6570 207b 6e61 6d65  AIT}| grep {name
+000102f0: 7d2d 3220 7c20 6865 6164 202d 6e31 207c  }-2 | head -n1 |
+00010300: 2067 7265 7020 2253 5441 5254 494e 475c   grep "STARTING\
+00010310: 7c52 554e 4e49 4e47 2227 2c0a 2020 2020  |RUNNING"',.    
+00010320: 2020 2020 2020 2020 5f53 504f 545f 4341          _SPOT_CA
+00010330: 4e43 454c 5f57 4149 542e 666f 726d 6174  NCEL_WAIT.format
+00010340: 286a 6f62 5f6e 616d 653d 6627 7b6e 616d  (job_name=f'{nam
+00010350: 657d 2d31 2729 2c0a 2020 2020 2020 2020  e}-1'),.        
+00010360: 2020 2020 2773 6c65 6570 2035 272c 0a20      'sleep 5',. 
+00010370: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
+00010380: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
+00010390: 2067 7265 7020 7b6e 616d 657d 2d31 207c   grep {name}-1 |
+000103a0: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
+000103b0: 2022 4341 4e43 454c 4c49 4e47 5c7c 4341   "CANCELLING\|CA
+000103c0: 4e43 454c 4c45 4422 272c 0a20 2020 2020  NCELLED"',.     
+000103d0: 2020 2020 2020 2027 736c 6565 7020 3230         'sleep 20
+000103e0: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
+000103f0: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
+00010400: 4149 547d 7c20 6772 6570 207b 6e61 6d65  AIT}| grep {name
+00010410: 7d2d 3120 7c20 6865 6164 202d 6e31 207c  }-1 | head -n1 |
+00010420: 2067 7265 7020 4341 4e43 454c 4c45 4427   grep CANCELLED'
+00010430: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+00010440: 7b5f 5350 4f54 5f51 5545 5545 5f57 4149  {_SPOT_QUEUE_WAI
+00010450: 547d 7c20 6772 6570 207b 6e61 6d65 7d2d  T}| grep {name}-
+00010460: 3220 7c20 6865 6164 202d 6e31 207c 2067  2 | head -n1 | g
+00010470: 7265 7020 2252 554e 4e49 4e47 5c7c 5355  rep "RUNNING\|SU
+00010480: 4343 4545 4445 4422 272c 0a20 2020 2020  CCEEDED"',.     
+00010490: 2020 205d 2c0a 2020 2020 2020 2020 2320     ],.        # 
+000104a0: 544f 444f 287a 6877 7529 3a20 4368 616e  TODO(zhwu): Chan
+000104b0: 6765 2074 6f20 5f53 504f 545f 4341 4e43  ge to _SPOT_CANC
+000104c0: 454c 5f57 4149 542e 666f 726d 6174 286a  EL_WAIT.format(j
+000104d0: 6f62 5f6e 616d 653d 6627 7b6e 616d 657d  ob_name=f'{name}
+000104e0: 2d31 202d 6e20 7b6e 616d 657d 2d32 2729  -1 -n {name}-2')
+000104f0: 2077 6865 6e0a 2020 2020 2020 2020 2320   when.        # 
+00010500: 6361 6e63 656c 696e 6720 6d75 6c74 6970  canceling multip
+00010510: 6c65 206a 6f62 206e 616d 6573 2069 7320  le job names is 
+00010520: 7375 7070 6f72 7465 642e 0a20 2020 2020  supported..     
+00010530: 2020 2028 5f53 504f 545f 4341 4e43 454c     (_SPOT_CANCEL
+00010540: 5f57 4149 542e 666f 726d 6174 286a 6f62  _WAIT.format(job
+00010550: 5f6e 616d 653d 6627 7b6e 616d 657d 2d31  _name=f'{name}-1
+00010560: 2729 202b 2027 3b20 2720 2b0a 2020 2020  ') + '; ' +.    
+00010570: 2020 2020 205f 5350 4f54 5f43 414e 4345       _SPOT_CANCE
+00010580: 4c5f 5741 4954 2e66 6f72 6d61 7428 6a6f  L_WAIT.format(jo
+00010590: 625f 6e61 6d65 3d66 277b 6e61 6d65 7d2d  b_name=f'{name}-
+000105a0: 3227 2929 2c0a 2020 2020 2020 2020 2320  2')),.        # 
+000105b0: 496e 6372 6561 7365 2074 696d 656f 7574  Increase timeout
+000105c0: 2073 696e 6365 2073 6b79 2073 706f 7420   since sky spot 
+000105d0: 7175 6575 6520 2d72 2063 616e 2062 6520  queue -r can be 
+000105e0: 626c 6f63 6b65 6420 6279 206f 7468 6572  blocked by other
+000105f0: 2073 706f 7420 7465 7374 732e 0a20 2020   spot tests..   
+00010600: 2020 2020 2074 696d 656f 7574 3d32 3020       timeout=20 
+00010610: 2a20 3630 2c0a 2020 2020 290a 2020 2020  * 60,.    ).    
+00010620: 7275 6e5f 6f6e 655f 7465 7374 2874 6573  run_one_test(tes
+00010630: 7429 0a0a 0a40 7079 7465 7374 2e6d 6172  t)...@pytest.mar
+00010640: 6b2e 6e6f 5f6c 616d 6264 615f 636c 6f75  k.no_lambda_clou
+00010650: 6420 2023 204c 616d 6264 6120 436c 6f75  d  # Lambda Clou
+00010660: 6420 646f 6573 206e 6f74 2073 7570 706f  d does not suppo
+00010670: 7274 2073 706f 7420 696e 7374 616e 6365  rt spot instance
+00010680: 730a 4070 7974 6573 742e 6d61 726b 2e6e  s.@pytest.mark.n
+00010690: 6f5f 6962 6d20 2023 2049 424d 2043 6c6f  o_ibm  # IBM Clo
+000106a0: 7564 2064 6f65 7320 6e6f 7420 7375 7070  ud does not supp
+000106b0: 6f72 7420 7370 6f74 2069 6e73 7461 6e63  ort spot instanc
+000106c0: 6573 0a40 7079 7465 7374 2e6d 6172 6b2e  es.@pytest.mark.
+000106d0: 6e6f 5f73 6370 2020 2320 5343 5020 646f  no_scp  # SCP do
+000106e0: 6573 206e 6f74 2073 7570 706f 7274 2073  es not support s
+000106f0: 706f 7420 696e 7374 616e 6365 730a 4070  pot instances.@p
+00010700: 7974 6573 742e 6d61 726b 2e6d 616e 6167  ytest.mark.manag
+00010710: 6564 5f73 706f 740a 6465 6620 7465 7374  ed_spot.def test
+00010720: 5f73 706f 745f 7069 7065 6c69 6e65 2867  _spot_pipeline(g
+00010730: 656e 6572 6963 5f63 6c6f 7564 3a20 7374  eneric_cloud: st
+00010740: 7229 3a0a 2020 2020 2222 2254 6573 7420  r):.    """Test 
+00010750: 6120 7370 6f74 c2a0 7069 7065 6c69 6e65  a spot..pipeline
+00010760: 2e22 2222 0a20 2020 206e 616d 6520 3d20  .""".    name = 
+00010770: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
+00010780: 6528 290a 2020 2020 7465 7374 203d 2054  e().    test = T
+00010790: 6573 7428 0a20 2020 2020 2020 2027 7370  est(.        'sp
+000107a0: 6f74 2d70 6970 656c 696e 6527 2c0a 2020  ot-pipeline',.  
+000107b0: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+000107c0: 2020 2020 6627 736b 7920 7370 6f74 206c      f'sky spot l
+000107d0: 6175 6e63 6820 2d6e 207b 6e61 6d65 7d20  aunch -n {name} 
+000107e0: 7465 7374 732f 7465 7374 5f79 616d 6c73  tests/test_yamls
+000107f0: 2f70 6970 656c 696e 652e 7961 6d6c 202d  /pipeline.yaml -
+00010800: 7920 2d64 272c 0a20 2020 2020 2020 2020  y -d',.         
+00010810: 2020 2027 736c 6565 7020 3527 2c0a 2020     'sleep 5',.  
+00010820: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
+00010830: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
+00010840: 6772 6570 207b 6e61 6d65 7d20 7c20 6865  grep {name} | he
+00010850: 6164 202d 6e31 207c 2067 7265 7020 2253  ad -n1 | grep "S
+00010860: 5441 5254 494e 475c 7c52 554e 4e49 4e47  TARTING\|RUNNING
+00010870: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+00010880: 2320 6067 7265 7020 2d41 2034 207b 6e61  # `grep -A 4 {na
+00010890: 6d65 7d60 2066 696e 6473 2074 6865 206a  me}` finds the j
+000108a0: 6f62 2077 6974 6820 7b6e 616d 657d 2061  ob with {name} a
+000108b0: 6e64 2074 6865 2034 206c 696e 6573 0a20  nd the 4 lines. 
+000108c0: 2020 2020 2020 2020 2020 2023 2061 6674             # aft
+000108d0: 6572 2069 742c 2069 2e65 2e20 7468 6520  er it, i.e. the 
+000108e0: 3420 7461 736b 7320 7769 7468 696e 2074  4 tasks within t
+000108f0: 6865 206a 6f62 2e0a 2020 2020 2020 2020  he job..        
+00010900: 2020 2020 2320 6073 6564 202d 6e20 3270      # `sed -n 2p
+00010910: 6020 6765 7473 2074 6865 2073 6563 6f6e  ` gets the secon
+00010920: 6420 6c69 6e65 206f 6620 7468 6520 3420  d line of the 4 
+00010930: 6c69 6e65 732c 2069 2e65 2e20 7468 6520  lines, i.e. the 
+00010940: 6669 7273 740a 2020 2020 2020 2020 2020  first.          
+00010950: 2020 2320 7461 736b 2077 6974 6869 6e20    # task within 
+00010960: 7468 6520 6a6f 622e 0a20 2020 2020 2020  the job..       
+00010970: 2020 2020 2066 277b 5f53 504f 545f 5155       f'{_SPOT_QU
+00010980: 4555 455f 5741 4954 7d7c 2067 7265 7020  EUE_WAIT}| grep 
+00010990: 2d41 2034 207b 6e61 6d65 7d7c 2073 6564  -A 4 {name}| sed
+000109a0: 202d 6e20 3270 207c 2067 7265 7020 2253   -n 2p | grep "S
+000109b0: 5441 5254 494e 475c 7c52 554e 4e49 4e47  TARTING\|RUNNING
+000109c0: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+000109d0: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
+000109e0: 4149 547d 7c20 6772 6570 202d 4120 3420  AIT}| grep -A 4 
+000109f0: 7b6e 616d 657d 7c20 7365 6420 2d6e 2033  {name}| sed -n 3
+00010a00: 7020 7c20 6772 6570 2022 5045 4e44 494e  p | grep "PENDIN
+00010a10: 4722 272c 0a20 2020 2020 2020 2020 2020  G"',.           
+00010a20: 205f 5350 4f54 5f43 414e 4345 4c5f 5741   _SPOT_CANCEL_WA
+00010a30: 4954 2e66 6f72 6d61 7428 6a6f 625f 6e61  IT.format(job_na
+00010a40: 6d65 3d66 277b 6e61 6d65 7d27 292c 0a20  me=f'{name}'),. 
+00010a50: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
+00010a60: 7020 3527 2c0a 2020 2020 2020 2020 2020  p 5',.          
+00010a70: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
+00010a80: 5f57 4149 547d 7c20 6772 6570 202d 4120  _WAIT}| grep -A 
+00010a90: 3420 7b6e 616d 657d 7c20 7365 6420 2d6e  4 {name}| sed -n
+00010aa0: 2032 7020 7c20 6772 6570 2022 4341 4e43   2p | grep "CANC
+00010ab0: 454c 4c49 4e47 5c7c 4341 4e43 454c 4c45  ELLING\|CANCELLE
+00010ac0: 4422 272c 0a20 2020 2020 2020 2020 2020  D"',.           
+00010ad0: 2066 277b 5f53 504f 545f 5155 4555 455f   f'{_SPOT_QUEUE_
+00010ae0: 5741 4954 7d7c 2067 7265 7020 2d41 2034  WAIT}| grep -A 4
+00010af0: 207b 6e61 6d65 7d7c 2073 6564 202d 6e20   {name}| sed -n 
+00010b00: 3370 207c 2067 7265 7020 2243 414e 4345  3p | grep "CANCE
+00010b10: 4c4c 494e 475c 7c43 414e 4345 4c4c 4544  LLING\|CANCELLED
+00010b20: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+00010b30: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
+00010b40: 4149 547d 7c20 6772 6570 202d 4120 3420  AIT}| grep -A 4 
+00010b50: 7b6e 616d 657d 7c20 7365 6420 2d6e 2034  {name}| sed -n 4
+00010b60: 7020 7c20 6772 6570 2022 4341 4e43 454c  p | grep "CANCEL
+00010b70: 4c49 4e47 5c7c 4341 4e43 454c 4c45 4422  LING\|CANCELLED"
+00010b80: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+00010b90: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
+00010ba0: 4954 7d7c 2067 7265 7020 2d41 2034 207b  IT}| grep -A 4 {
+00010bb0: 6e61 6d65 7d7c 2073 6564 202d 6e20 3570  name}| sed -n 5p
+00010bc0: 207c 2067 7265 7020 2243 414e 4345 4c4c   | grep "CANCELL
+00010bd0: 494e 475c 7c43 414e 4345 4c4c 4544 2227  ING\|CANCELLED"'
+00010be0: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
+00010bf0: 6c65 6570 2032 3030 272c 0a20 2020 2020  leep 200',.     
+00010c00: 2020 2020 2020 2066 277b 5f53 504f 545f         f'{_SPOT_
+00010c10: 5155 4555 455f 5741 4954 7d7c 2067 7265  QUEUE_WAIT}| gre
+00010c20: 7020 2d41 2034 207b 6e61 6d65 7d7c 2073  p -A 4 {name}| s
+00010c30: 6564 202d 6e20 3270 207c 2067 7265 7020  ed -n 2p | grep 
+00010c40: 2243 414e 4345 4c4c 4544 2227 2c0a 2020  "CANCELLED"',.  
+00010c50: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
+00010c60: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
+00010c70: 6772 6570 202d 4120 3420 7b6e 616d 657d  grep -A 4 {name}
+00010c80: 7c20 7365 6420 2d6e 2033 7020 7c20 6772  | sed -n 3p | gr
+00010c90: 6570 2022 4341 4e43 454c 4c45 4422 272c  ep "CANCELLED"',
+00010ca0: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
+00010cb0: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
+00010cc0: 7d7c 2067 7265 7020 2d41 2034 207b 6e61  }| grep -A 4 {na
+00010cd0: 6d65 7d7c 2073 6564 202d 6e20 3470 207c  me}| sed -n 4p |
+00010ce0: 2067 7265 7020 2243 414e 4345 4c4c 4544   grep "CANCELLED
+00010cf0: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+00010d00: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
+00010d10: 4149 547d 7c20 6772 6570 202d 4120 3420  AIT}| grep -A 4 
+00010d20: 7b6e 616d 657d 7c20 7365 6420 2d6e 2035  {name}| sed -n 5
+00010d30: 7020 7c20 6772 6570 2022 4341 4e43 454c  p | grep "CANCEL
+00010d40: 4c45 4422 272c 0a20 2020 2020 2020 205d  LED"',.        ]
+00010d50: 2c0a 2020 2020 2020 2020 5f53 504f 545f  ,.        _SPOT_
+00010d60: 4341 4e43 454c 5f57 4149 542e 666f 726d  CANCEL_WAIT.form
+00010d70: 6174 286a 6f62 5f6e 616d 653d 6627 7b6e  at(job_name=f'{n
+00010d80: 616d 657d 2729 2c0a 2020 2020 2020 2020  ame}'),.        
+00010d90: 2320 496e 6372 6561 7365 2074 696d 656f  # Increase timeo
+00010da0: 7574 2073 696e 6365 2073 6b79 2073 706f  ut since sky spo
+00010db0: 7420 7175 6575 6520 2d72 2063 616e 2062  t queue -r can b
+00010dc0: 6520 626c 6f63 6b65 6420 6279 206f 7468  e blocked by oth
+00010dd0: 6572 2073 706f 7420 7465 7374 732e 0a20  er spot tests.. 
+00010de0: 2020 2020 2020 2074 696d 656f 7574 3d33         timeout=3
+00010df0: 3020 2a20 3630 2c0a 2020 2020 290a 2020  0 * 60,.    ).  
+00010e00: 2020 7275 6e5f 6f6e 655f 7465 7374 2874    run_one_test(t
+00010e10: 6573 7429 0a0a 0a40 7079 7465 7374 2e6d  est)...@pytest.m
+00010e20: 6172 6b2e 6e6f 5f6c 616d 6264 615f 636c  ark.no_lambda_cl
+00010e30: 6f75 6420 2023 204c 616d 6264 6120 436c  oud  # Lambda Cl
+00010e40: 6f75 6420 646f 6573 206e 6f74 2073 7570  oud does not sup
+00010e50: 706f 7274 2073 706f 7420 696e 7374 616e  port spot instan
+00010e60: 6365 730a 4070 7974 6573 742e 6d61 726b  ces.@pytest.mark
+00010e70: 2e6e 6f5f 6962 6d20 2023 2049 424d 2043  .no_ibm  # IBM C
+00010e80: 6c6f 7564 2064 6f65 7320 6e6f 7420 7375  loud does not su
+00010e90: 7070 6f72 7420 7370 6f74 2069 6e73 7461  pport spot insta
+00010ea0: 6e63 6573 0a40 7079 7465 7374 2e6d 6172  nces.@pytest.mar
+00010eb0: 6b2e 6e6f 5f73 6370 2020 2320 5343 5020  k.no_scp  # SCP 
+00010ec0: 646f 6573 206e 6f74 2073 7570 706f 7274  does not support
+00010ed0: 2073 706f 7420 696e 7374 616e 6365 730a   spot instances.
+00010ee0: 4070 7974 6573 742e 6d61 726b 2e6d 616e  @pytest.mark.man
+00010ef0: 6167 6564 5f73 706f 740a 6465 6620 7465  aged_spot.def te
+00010f00: 7374 5f73 706f 745f 6661 696c 6564 5f73  st_spot_failed_s
+00010f10: 6574 7570 2867 656e 6572 6963 5f63 6c6f  etup(generic_clo
+00010f20: 7564 3a20 7374 7229 3a0a 2020 2020 2222  ud: str):.    ""
+00010f30: 2254 6573 7420 6d61 6e61 6765 6420 7370  "Test managed sp
+00010f40: 6f74 206a 6f62 2077 6974 6820 6661 696c  ot job with fail
+00010f50: 6564 2073 6574 7570 2e22 2222 0a20 2020  ed setup.""".   
+00010f60: 206e 616d 6520 3d20 5f67 6574 5f63 6c75   name = _get_clu
+00010f70: 7374 6572 5f6e 616d 6528 290a 2020 2020  ster_name().    
+00010f80: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
+00010f90: 2020 2020 2027 7370 6f74 5f66 6169 6c65       'spot_faile
+00010fa0: 645f 7365 7475 7027 2c0a 2020 2020 2020  d_setup',.      
+00010fb0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
+00010fc0: 6627 736b 7920 7370 6f74 206c 6175 6e63  f'sky spot launc
+00010fd0: 6820 2d6e 207b 6e61 6d65 7d20 2d2d 636c  h -n {name} --cl
+00010fe0: 6f75 6420 7b67 656e 6572 6963 5f63 6c6f  oud {generic_clo
+00010ff0: 7564 7d20 2d79 202d 6420 7465 7374 732f  ud} -y -d tests/
+00011000: 7465 7374 5f79 616d 6c73 2f66 6169 6c65  test_yamls/faile
+00011010: 645f 7365 7475 702e 7961 6d6c 272c 0a20  d_setup.yaml',. 
+00011020: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
+00011030: 7020 3333 3027 2c0a 2020 2020 2020 2020  p 330',.        
+00011040: 2020 2020 2320 4d61 6b65 2073 7572 6520      # Make sure 
+00011050: 7468 6520 6a6f 6220 6661 696c 6564 2071  the job failed q
+00011060: 7569 636b 6c79 2e0a 2020 2020 2020 2020  uickly..        
+00011070: 2020 2020 6627 7b5f 5350 4f54 5f51 5545      f'{_SPOT_QUE
+00011080: 5545 5f57 4149 547d 207c 2067 7265 7020  UE_WAIT} | grep 
+00011090: 7b6e 616d 657d 207c 2068 6561 6420 2d6e  {name} | head -n
+000110a0: 3120 7c20 6772 6570 2022 4641 494c 4544  1 | grep "FAILED
+000110b0: 5f53 4554 5550 2227 2c0a 2020 2020 2020  _SETUP"',.      
+000110c0: 2020 5d2c 0a20 2020 2020 2020 205f 5350    ],.        _SP
+000110d0: 4f54 5f43 414e 4345 4c5f 5741 4954 2e66  OT_CANCEL_WAIT.f
+000110e0: 6f72 6d61 7428 6a6f 625f 6e61 6d65 3d6e  ormat(job_name=n
+000110f0: 616d 6529 2c0a 2020 2020 2020 2020 2320  ame),.        # 
+00011100: 496e 6372 6561 7365 2074 696d 656f 7574  Increase timeout
+00011110: 2073 696e 6365 2073 6b79 2073 706f 7420   since sky spot 
+00011120: 7175 6575 6520 2d72 2063 616e 2062 6520  queue -r can be 
+00011130: 626c 6f63 6b65 6420 6279 206f 7468 6572  blocked by other
+00011140: 2073 706f 7420 7465 7374 732e 0a20 2020   spot tests..   
+00011150: 2020 2020 2074 696d 656f 7574 3d32 3020       timeout=20 
+00011160: 2a20 3630 2c0a 2020 2020 290a 2020 2020  * 60,.    ).    
+00011170: 7275 6e5f 6f6e 655f 7465 7374 2874 6573  run_one_test(tes
+00011180: 7429 0a0a 0a40 7079 7465 7374 2e6d 6172  t)...@pytest.mar
+00011190: 6b2e 6e6f 5f6c 616d 6264 615f 636c 6f75  k.no_lambda_clou
+000111a0: 6420 2023 204c 616d 6264 6120 436c 6f75  d  # Lambda Clou
+000111b0: 6420 646f 6573 206e 6f74 2073 7570 706f  d does not suppo
+000111c0: 7274 2073 706f 7420 696e 7374 616e 6365  rt spot instance
+000111d0: 730a 4070 7974 6573 742e 6d61 726b 2e6e  s.@pytest.mark.n
+000111e0: 6f5f 6962 6d20 2023 2049 424d 2043 6c6f  o_ibm  # IBM Clo
+000111f0: 7564 2064 6f65 7320 6e6f 7420 7375 7070  ud does not supp
+00011200: 6f72 7420 7370 6f74 2069 6e73 7461 6e63  ort spot instanc
+00011210: 6573 0a40 7079 7465 7374 2e6d 6172 6b2e  es.@pytest.mark.
+00011220: 6e6f 5f73 6370 2020 2320 5343 5020 646f  no_scp  # SCP do
+00011230: 6573 206e 6f74 2073 7570 706f 7274 2073  es not support s
+00011240: 706f 7420 696e 7374 616e 6365 730a 4070  pot instances.@p
+00011250: 7974 6573 742e 6d61 726b 2e6d 616e 6167  ytest.mark.manag
+00011260: 6564 5f73 706f 740a 6465 6620 7465 7374  ed_spot.def test
+00011270: 5f73 706f 745f 7069 7065 6c69 6e65 5f66  _spot_pipeline_f
+00011280: 6169 6c65 645f 7365 7475 7028 6765 6e65  ailed_setup(gene
+00011290: 7269 635f 636c 6f75 643a 2073 7472 293a  ric_cloud: str):
+000112a0: 0a20 2020 2022 2222 5465 7374 206d 616e  .    """Test man
+000112b0: 6167 6564 2073 706f 7420 6a6f 6220 7769  aged spot job wi
+000112c0: 7468 2066 6169 6c65 6420 7365 7475 7020  th failed setup 
+000112d0: 666f 7220 6120 7069 7065 6c69 6e65 2e22  for a pipeline."
+000112e0: 2222 0a20 2020 206e 616d 6520 3d20 5f67  "".    name = _g
+000112f0: 6574 5f63 6c75 7374 6572 5f6e 616d 6528  et_cluster_name(
+00011300: 290a 2020 2020 7465 7374 203d 2054 6573  ).    test = Tes
+00011310: 7428 0a20 2020 2020 2020 2027 7370 6f74  t(.        'spot
+00011320: 5f70 6970 656c 696e 655f 6661 696c 6564  _pipeline_failed
+00011330: 5f73 6574 7570 272c 0a20 2020 2020 2020  _setup',.       
+00011340: 205b 0a20 2020 2020 2020 2020 2020 2066   [.            f
+00011350: 2773 6b79 2073 706f 7420 6c61 756e 6368  'sky spot launch
+00011360: 202d 6e20 7b6e 616d 657d 202d 7920 2d64   -n {name} -y -d
+00011370: 2074 6573 7473 2f74 6573 745f 7961 6d6c   tests/test_yaml
+00011380: 732f 6661 696c 6564 5f73 6574 7570 5f70  s/failed_setup_p
+00011390: 6970 656c 696e 652e 7961 6d6c 272c 0a20  ipeline.yaml',. 
+000113a0: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
+000113b0: 7020 3830 3027 2c0a 2020 2020 2020 2020  p 800',.        
+000113c0: 2020 2020 2320 4d61 6b65 2073 7572 6520      # Make sure 
+000113d0: 7468 6520 6a6f 6220 6661 696c 6564 2071  the job failed q
+000113e0: 7569 636b 6c79 2e0a 2020 2020 2020 2020  uickly..        
+000113f0: 2020 2020 6627 7b5f 5350 4f54 5f51 5545      f'{_SPOT_QUE
+00011400: 5545 5f57 4149 547d 207c 2067 7265 7020  UE_WAIT} | grep 
+00011410: 7b6e 616d 657d 207c 2068 6561 6420 2d6e  {name} | head -n
+00011420: 3120 7c20 6772 6570 2022 4641 494c 4544  1 | grep "FAILED
+00011430: 5f53 4554 5550 2227 2c0a 2020 2020 2020  _SETUP"',.      
+00011440: 2020 2020 2020 2320 5461 736b 2030 2073        # Task 0 s
+00011450: 686f 756c 6420 6265 2053 5543 4345 4544  hould be SUCCEED
+00011460: 4544 2e0a 2020 2020 2020 2020 2020 2020  ED..            
+00011470: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
+00011480: 4149 547d 207c 2067 7265 7020 2d41 2034  AIT} | grep -A 4
+00011490: 207b 6e61 6d65 7d7c 2073 6564 202d 6e20   {name}| sed -n 
+000114a0: 3270 207c 2067 7265 7020 2253 5543 4345  2p | grep "SUCCE
+000114b0: 4544 4544 2227 2c0a 2020 2020 2020 2020  EDED"',.        
+000114c0: 2020 2020 2320 5461 736b 2031 2073 686f      # Task 1 sho
+000114d0: 756c 6420 6265 2046 4149 4c45 445f 5345  uld be FAILED_SE
+000114e0: 5455 502e 0a20 2020 2020 2020 2020 2020  TUP..           
+000114f0: 2066 277b 5f53 504f 545f 5155 4555 455f   f'{_SPOT_QUEUE_
+00011500: 5741 4954 7d20 7c20 6772 6570 202d 4120  WAIT} | grep -A 
+00011510: 3420 7b6e 616d 657d 7c20 7365 6420 2d6e  4 {name}| sed -n
+00011520: 2033 7020 7c20 6772 6570 2022 4641 494c   3p | grep "FAIL
+00011530: 4544 5f53 4554 5550 2227 2c0a 2020 2020  ED_SETUP"',.    
+00011540: 2020 2020 2020 2020 2320 5461 736b 2032          # Task 2
+00011550: 2073 686f 756c 6420 6265 2043 414e 4345   should be CANCE
+00011560: 4c4c 4544 2e0a 2020 2020 2020 2020 2020  LLED..          
+00011570: 2020 6627 7b5f 5350 4f54 5f51 5545 5545    f'{_SPOT_QUEUE
+00011580: 5f57 4149 547d 207c 2067 7265 7020 2d41  _WAIT} | grep -A
+00011590: 2034 207b 6e61 6d65 7d7c 2073 6564 202d   4 {name}| sed -
+000115a0: 6e20 3470 207c 2067 7265 7020 2243 414e  n 4p | grep "CAN
+000115b0: 4345 4c4c 4544 2227 2c0a 2020 2020 2020  CELLED"',.      
+000115c0: 2020 2020 2020 2320 5461 736b 2033 2073        # Task 3 s
+000115d0: 686f 756c 6420 6265 2043 414e 4345 4c4c  hould be CANCELL
+000115e0: 4544 2e0a 2020 2020 2020 2020 2020 2020  ED..            
+000115f0: 6627 7b5f 5350 4f54 5f51 5545 5545 5f57  f'{_SPOT_QUEUE_W
+00011600: 4149 547d 207c 2067 7265 7020 2d41 2034  AIT} | grep -A 4
+00011610: 207b 6e61 6d65 7d7c 2073 6564 202d 6e20   {name}| sed -n 
+00011620: 3570 207c 2067 7265 7020 2243 414e 4345  5p | grep "CANCE
+00011630: 4c4c 4544 2227 2c0a 2020 2020 2020 2020  LLED"',.        
+00011640: 5d2c 0a20 2020 2020 2020 205f 5350 4f54  ],.        _SPOT
+00011650: 5f43 414e 4345 4c5f 5741 4954 2e66 6f72  _CANCEL_WAIT.for
+00011660: 6d61 7428 6a6f 625f 6e61 6d65 3d6e 616d  mat(job_name=nam
+00011670: 6529 2c0a 2020 2020 2020 2020 2320 496e  e),.        # In
+00011680: 6372 6561 7365 2074 696d 656f 7574 2073  crease timeout s
+00011690: 696e 6365 2073 6b79 2073 706f 7420 7175  ince sky spot qu
+000116a0: 6575 6520 2d72 2063 616e 2062 6520 626c  eue -r can be bl
+000116b0: 6f63 6b65 6420 6279 206f 7468 6572 2073  ocked by other s
+000116c0: 706f 7420 7465 7374 732e 0a20 2020 2020  pot tests..     
+000116d0: 2020 2074 696d 656f 7574 3d33 3020 2a20     timeout=30 * 
+000116e0: 3630 2c0a 2020 2020 290a 2020 2020 7275  60,.    ).    ru
+000116f0: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
+00011700: 0a0a 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d20  ...# ---------- 
+00011710: 5465 7374 696e 6720 6d61 6e61 6765 6420  Testing managed 
+00011720: 7370 6f74 2072 6563 6f76 6572 7920 2d2d  spot recovery --
+00011730: 2d2d 2d2d 2d2d 2d2d 0a0a 0a40 7079 7465  --------...@pyte
+00011740: 7374 2e6d 6172 6b2e 6177 730a 4070 7974  st.mark.aws.@pyt
+00011750: 6573 742e 6d61 726b 2e6d 616e 6167 6564  est.mark.managed
+00011760: 5f73 706f 740a 6465 6620 7465 7374 5f73  _spot.def test_s
+00011770: 706f 745f 7265 636f 7665 7279 5f61 7773  pot_recovery_aws
+00011780: 2861 7773 5f63 6f6e 6669 675f 7265 6769  (aws_config_regi
+00011790: 6f6e 293a 0a20 2020 2022 2222 5465 7374  on):.    """Test
+000117a0: 206d 616e 6167 6564 2073 706f 7420 7265   managed spot re
+000117b0: 636f 7665 7279 2e22 2222 0a20 2020 206e  covery.""".    n
+000117c0: 616d 6520 3d20 5f67 6574 5f63 6c75 7374  ame = _get_clust
+000117d0: 6572 5f6e 616d 6528 290a 2020 2020 7265  er_name().    re
+000117e0: 6769 6f6e 203d 2061 7773 5f63 6f6e 6669  gion = aws_confi
+000117f0: 675f 7265 6769 6f6e 0a20 2020 2074 6573  g_region.    tes
+00011800: 7420 3d20 5465 7374 280a 2020 2020 2020  t = Test(.      
+00011810: 2020 2773 706f 745f 7265 636f 7665 7279    'spot_recovery
+00011820: 5f61 7773 272c 0a20 2020 2020 2020 205b  _aws',.        [
+00011830: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+00011840: 6b79 2073 706f 7420 6c61 756e 6368 202d  ky spot launch -
+00011850: 2d63 6c6f 7564 2061 7773 202d 2d72 6567  -cloud aws --reg
+00011860: 696f 6e20 7b72 6567 696f 6e7d 202d 6e20  ion {region} -n 
+00011870: 7b6e 616d 657d 2022 6563 686f 2053 4b59  {name} "echo SKY
+00011880: 5049 4c4f 545f 5441 534b 5f49 443a 205c  PILOT_TASK_ID: \
+00011890: 2453 4b59 5049 4c4f 545f 5441 534b 5f49  $SKYPILOT_TASK_I
+000118a0: 443b 2073 6c65 6570 2031 3830 3022 2020  D; sleep 1800"  
+000118b0: 2d79 202d 6427 2c0a 2020 2020 2020 2020  -y -d',.        
+000118c0: 2020 2020 2773 6c65 6570 2033 3630 272c      'sleep 360',
+000118d0: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
+000118e0: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
+000118f0: 7d7c 2067 7265 7020 7b6e 616d 657d 207c  }| grep {name} |
+00011900: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
+00011910: 2022 5255 4e4e 494e 4722 272c 0a20 2020   "RUNNING"',.   
+00011920: 2020 2020 2020 2020 2066 2752 554e 5f49           f'RUN_I
+00011930: 443d 2428 736b 7920 7370 6f74 206c 6f67  D=$(sky spot log
+00011940: 7320 2d6e 207b 6e61 6d65 7d20 2d2d 6e6f  s -n {name} --no
+00011950: 2d66 6f6c 6c6f 7720 7c20 6772 6570 2053  -follow | grep S
+00011960: 4b59 5049 4c4f 545f 5441 534b 5f49 4420  KYPILOT_TASK_ID 
+00011970: 7c20 6375 7420 2d64 3a20 2d66 3229 3b20  | cut -d: -f2); 
+00011980: 6563 686f 2022 2452 554e 5f49 4422 207c  echo "$RUN_ID" |
+00011990: 2074 6565 202f 746d 702f 7b6e 616d 657d   tee /tmp/{name}
+000119a0: 2d72 756e 2d69 6427 2c0a 2020 2020 2020  -run-id',.      
+000119b0: 2020 2020 2020 2320 5465 726d 696e 6174        # Terminat
+000119c0: 6520 7468 6520 636c 7573 7465 7220 6d61  e the cluster ma
+000119d0: 6e75 616c 6c79 2e0a 2020 2020 2020 2020  nually..        
+000119e0: 2020 2020 2866 2761 7773 2065 6332 2074      (f'aws ec2 t
+000119f0: 6572 6d69 6e61 7465 2d69 6e73 7461 6e63  erminate-instanc
+00011a00: 6573 202d 2d72 6567 696f 6e20 7b72 6567  es --region {reg
+00011a10: 696f 6e7d 202d 2d69 6e73 7461 6e63 652d  ion} --instance-
+00011a20: 6964 7320 2428 270a 2020 2020 2020 2020  ids $('.        
+00011a30: 2020 2020 2066 2761 7773 2065 6332 2064       f'aws ec2 d
+00011a40: 6573 6372 6962 652d 696e 7374 616e 6365  escribe-instance
+00011a50: 7320 2d2d 7265 6769 6f6e 207b 7265 6769  s --region {regi
+00011a60: 6f6e 7d20 270a 2020 2020 2020 2020 2020  on} '.          
+00011a70: 2020 2066 272d 2d66 696c 7465 7273 204e     f'--filters N
+00011a80: 616d 653d 7461 673a 7261 792d 636c 7573  ame=tag:ray-clus
+00011a90: 7465 722d 6e61 6d65 2c56 616c 7565 733d  ter-name,Values=
+00011aa0: 7b6e 616d 657d 2a20 270a 2020 2020 2020  {name}* '.      
+00011ab0: 2020 2020 2020 2066 272d 2d71 7565 7279         f'--query
+00011ac0: 2052 6573 6572 7661 7469 6f6e 735b 5d2e   Reservations[].
+00011ad0: 496e 7374 616e 6365 735b 5d2e 496e 7374  Instances[].Inst
+00011ae0: 616e 6365 4964 2027 0a20 2020 2020 2020  anceId '.       
+00011af0: 2020 2020 2020 272d 2d6f 7574 7075 7420        '--output 
+00011b00: 7465 7874 2927 292c 0a20 2020 2020 2020  text)'),.       
+00011b10: 2020 2020 2027 736c 6565 7020 3130 3027       'sleep 100'
+00011b20: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+00011b30: 7b5f 5350 4f54 5f51 5545 5545 5f57 4149  {_SPOT_QUEUE_WAI
+00011b40: 547d 7c20 6772 6570 207b 6e61 6d65 7d20  T}| grep {name} 
+00011b50: 7c20 6865 6164 202d 6e31 207c 2067 7265  | head -n1 | gre
+00011b60: 7020 2252 4543 4f56 4552 494e 4722 272c  p "RECOVERING"',
+00011b70: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
+00011b80: 6565 7020 3230 3027 2c0a 2020 2020 2020  eep 200',.      
+00011b90: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
+00011ba0: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
+00011bb0: 207b 6e61 6d65 7d20 7c20 6865 6164 202d   {name} | head -
+00011bc0: 6e31 207c 2067 7265 7020 2252 554e 4e49  n1 | grep "RUNNI
+00011bd0: 4e47 2227 2c0a 2020 2020 2020 2020 2020  NG"',.          
+00011be0: 2020 6627 5255 4e5f 4944 3d24 2863 6174    f'RUN_ID=$(cat
+00011bf0: 202f 746d 702f 7b6e 616d 657d 2d72 756e   /tmp/{name}-run
+00011c00: 2d69 6429 3b20 6563 686f 2024 5255 4e5f  -id); echo $RUN_
+00011c10: 4944 3b20 736b 7920 7370 6f74 206c 6f67  ID; sky spot log
+00011c20: 7320 2d6e 207b 6e61 6d65 7d20 2d2d 6e6f  s -n {name} --no
+00011c30: 2d66 6f6c 6c6f 7720 7c20 6772 6570 2053  -follow | grep S
+00011c40: 4b59 5049 4c4f 545f 5441 534b 5f49 4420  KYPILOT_TASK_ID 
+00011c50: 7c20 6772 6570 2022 2452 554e 5f49 4422  | grep "$RUN_ID"
+00011c60: 272c 0a20 2020 2020 2020 205d 2c0a 2020  ',.        ],.  
+00011c70: 2020 2020 2020 5f53 504f 545f 4341 4e43        _SPOT_CANC
+00011c80: 454c 5f57 4149 542e 666f 726d 6174 286a  EL_WAIT.format(j
+00011c90: 6f62 5f6e 616d 653d 6e61 6d65 292c 0a20  ob_name=name),. 
+00011ca0: 2020 2020 2020 2074 696d 656f 7574 3d32         timeout=2
+00011cb0: 3520 2a20 3630 2c0a 2020 2020 290a 2020  5 * 60,.    ).  
+00011cc0: 2020 7275 6e5f 6f6e 655f 7465 7374 2874    run_one_test(t
+00011cd0: 6573 7429 0a0a 0a40 7079 7465 7374 2e6d  est)...@pytest.m
+00011ce0: 6172 6b2e 6763 700a 4070 7974 6573 742e  ark.gcp.@pytest.
+00011cf0: 6d61 726b 2e6d 616e 6167 6564 5f73 706f  mark.managed_spo
+00011d00: 740a 6465 6620 7465 7374 5f73 706f 745f  t.def test_spot_
+00011d10: 7265 636f 7665 7279 5f67 6370 2829 3a0a  recovery_gcp():.
+00011d20: 2020 2020 2222 2254 6573 7420 6d61 6e61      """Test mana
+00011d30: 6765 6420 7370 6f74 2072 6563 6f76 6572  ged spot recover
+00011d40: 792e 2222 220a 2020 2020 6e61 6d65 203d  y.""".    name =
+00011d50: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
+00011d60: 6d65 2829 0a20 2020 207a 6f6e 6520 3d20  me().    zone = 
+00011d70: 2775 732d 6561 7374 342d 6227 0a20 2020  'us-east4-b'.   
+00011d80: 2071 7565 7279 5f63 6d64 203d 2028 6627   query_cmd = (f'
+00011d90: 6763 6c6f 7564 2063 6f6d 7075 7465 2069  gcloud compute i
+00011da0: 6e73 7461 6e63 6573 206c 6973 7420 2d2d  nstances list --
+00011db0: 6669 6c74 6572 3d27 0a20 2020 2020 2020  filter='.       
+00011dc0: 2020 2020 2020 2020 2020 6627 2228 6c61            f'"(la
+00011dd0: 6265 6c73 2e72 6179 2d63 6c75 7374 6572  bels.ray-cluster
+00011de0: 2d6e 616d 653a 7b6e 616d 657d 2922 2027  -name:{name})" '
+00011df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011e00: 2020 6627 2d2d 7a6f 6e65 733d 7b7a 6f6e    f'--zones={zon
+00011e10: 657d 202d 2d66 6f72 6d61 743d 2276 616c  e} --format="val
+00011e20: 7565 286e 616d 6529 2227 290a 2020 2020  ue(name)"').    
+00011e30: 7465 726d 696e 6174 655f 636d 6420 3d20  terminate_cmd = 
+00011e40: 2866 2767 636c 6f75 6420 636f 6d70 7574  (f'gcloud comput
+00011e50: 6520 696e 7374 616e 6365 7320 6465 6c65  e instances dele
+00011e60: 7465 202d 2d7a 6f6e 653d 7b7a 6f6e 657d  te --zone={zone}
+00011e70: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00011e80: 2020 2020 2020 2066 2720 2d2d 7175 6965         f' --quie
+00011e90: 7420 2428 7b71 7565 7279 5f63 6d64 7d29  t $({query_cmd})
+00011ea0: 2729 0a20 2020 2074 6573 7420 3d20 5465  ').    test = Te
+00011eb0: 7374 280a 2020 2020 2020 2020 2773 706f  st(.        'spo
+00011ec0: 745f 7265 636f 7665 7279 5f67 6370 272c  t_recovery_gcp',
+00011ed0: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
+00011ee0: 2020 2020 2020 2066 2773 6b79 2073 706f         f'sky spo
+00011ef0: 7420 6c61 756e 6368 202d 2d63 6c6f 7564  t launch --cloud
+00011f00: 2067 6370 202d 2d7a 6f6e 6520 7b7a 6f6e   gcp --zone {zon
+00011f10: 657d 202d 6e20 7b6e 616d 657d 2022 6563  e} -n {name} "ec
+00011f20: 686f 2053 4b59 5049 4c4f 545f 5441 534b  ho SKYPILOT_TASK
+00011f30: 5f49 443a 205c 2453 4b59 5049 4c4f 545f  _ID: \$SKYPILOT_
+00011f40: 5441 534b 5f49 443b 2073 6c65 6570 2031  TASK_ID; sleep 1
+00011f50: 3830 3022 2020 2d79 202d 6427 2c0a 2020  800"  -y -d',.  
+00011f60: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
+00011f70: 2033 3630 272c 0a20 2020 2020 2020 2020   360',.         
+00011f80: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
+00011f90: 455f 5741 4954 7d7c 2067 7265 7020 7b6e  E_WAIT}| grep {n
+00011fa0: 616d 657d 207c 2068 6561 6420 2d6e 3120  ame} | head -n1 
+00011fb0: 7c20 6772 6570 2022 5255 4e4e 494e 4722  | grep "RUNNING"
+00011fc0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+00011fd0: 2752 554e 5f49 443d 2428 736b 7920 7370  'RUN_ID=$(sky sp
+00011fe0: 6f74 206c 6f67 7320 2d6e 207b 6e61 6d65  ot logs -n {name
+00011ff0: 7d20 2d2d 6e6f 2d66 6f6c 6c6f 7720 7c20  } --no-follow | 
+00012000: 6772 6570 2053 4b59 5049 4c4f 545f 5441  grep SKYPILOT_TA
+00012010: 534b 5f49 4420 7c20 6375 7420 2d64 3a20  SK_ID | cut -d: 
+00012020: 2d66 3229 3b20 6563 686f 2022 2452 554e  -f2); echo "$RUN
+00012030: 5f49 4422 207c 2074 6565 202f 746d 702f  _ID" | tee /tmp/
+00012040: 7b6e 616d 657d 2d72 756e 2d69 6427 2c0a  {name}-run-id',.
+00012050: 2020 2020 2020 2020 2020 2020 2320 5465              # Te
+00012060: 726d 696e 6174 6520 7468 6520 636c 7573  rminate the clus
+00012070: 7465 7220 6d61 6e75 616c 6c79 2e0a 2020  ter manually..  
+00012080: 2020 2020 2020 2020 2020 7465 726d 696e            termin
+00012090: 6174 655f 636d 642c 0a20 2020 2020 2020  ate_cmd,.       
+000120a0: 2020 2020 2027 736c 6565 7020 3130 3027       'sleep 100'
+000120b0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+000120c0: 7b5f 5350 4f54 5f51 5545 5545 5f57 4149  {_SPOT_QUEUE_WAI
+000120d0: 547d 7c20 6772 6570 207b 6e61 6d65 7d20  T}| grep {name} 
+000120e0: 7c20 6865 6164 202d 6e31 207c 2067 7265  | head -n1 | gre
+000120f0: 7020 2252 4543 4f56 4552 494e 4722 272c  p "RECOVERING"',
+00012100: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
+00012110: 6565 7020 3230 3027 2c0a 2020 2020 2020  eep 200',.      
+00012120: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
+00012130: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
+00012140: 207b 6e61 6d65 7d20 7c20 6865 6164 202d   {name} | head -
+00012150: 6e31 207c 2067 7265 7020 2252 554e 4e49  n1 | grep "RUNNI
+00012160: 4e47 2227 2c0a 2020 2020 2020 2020 2020  NG"',.          
+00012170: 2020 6627 5255 4e5f 4944 3d24 2863 6174    f'RUN_ID=$(cat
+00012180: 202f 746d 702f 7b6e 616d 657d 2d72 756e   /tmp/{name}-run
+00012190: 2d69 6429 3b20 6563 686f 2024 5255 4e5f  -id); echo $RUN_
+000121a0: 4944 3b20 736b 7920 7370 6f74 206c 6f67  ID; sky spot log
+000121b0: 7320 2d6e 207b 6e61 6d65 7d20 2d2d 6e6f  s -n {name} --no
+000121c0: 2d66 6f6c 6c6f 7720 7c20 6772 6570 2053  -follow | grep S
+000121d0: 4b59 5049 4c4f 545f 5441 534b 5f49 443a  KYPILOT_TASK_ID:
+000121e0: 207c 2067 7265 7020 2224 5255 4e5f 4944   | grep "$RUN_ID
+000121f0: 2227 2c0a 2020 2020 2020 2020 5d2c 0a20  "',.        ],. 
+00012200: 2020 2020 2020 205f 5350 4f54 5f43 414e         _SPOT_CAN
+00012210: 4345 4c5f 5741 4954 2e66 6f72 6d61 7428  CEL_WAIT.format(
+00012220: 6a6f 625f 6e61 6d65 3d6e 616d 6529 2c0a  job_name=name),.
+00012230: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
+00012240: 3235 202a 2036 302c 0a20 2020 2029 0a20  25 * 60,.    ). 
+00012250: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+00012260: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
+00012270: 6d61 726b 2e61 7773 0a40 7079 7465 7374  mark.aws.@pytest
+00012280: 2e6d 6172 6b2e 6d61 6e61 6765 645f 7370  .mark.managed_sp
+00012290: 6f74 0a64 6566 2074 6573 745f 7370 6f74  ot.def test_spot
+000122a0: 5f70 6970 656c 696e 655f 7265 636f 7665  _pipeline_recove
+000122b0: 7279 5f61 7773 2861 7773 5f63 6f6e 6669  ry_aws(aws_confi
+000122c0: 675f 7265 6769 6f6e 293a 0a20 2020 2022  g_region):.    "
+000122d0: 2222 5465 7374 206d 616e 6167 6564 2073  ""Test managed s
+000122e0: 706f 7420 7265 636f 7665 7279 2066 6f72  pot recovery for
+000122f0: 2061 2070 6970 656c 696e 652e 2222 220a   a pipeline.""".
+00012300: 2020 2020 6e61 6d65 203d 205f 6765 745f      name = _get_
+00012310: 636c 7573 7465 725f 6e61 6d65 2829 0a20  cluster_name(). 
+00012320: 2020 2072 6567 696f 6e20 3d20 6177 735f     region = aws_
+00012330: 636f 6e66 6967 5f72 6567 696f 6e0a 2020  config_region.  
+00012340: 2020 6966 2072 6567 696f 6e20 213d 2027    if region != '
+00012350: 7573 2d77 6573 742d 3227 3a0a 2020 2020  us-west-2':.    
+00012360: 2020 2020 7079 7465 7374 2e73 6b69 7028      pytest.skip(
+00012370: 274f 6e6c 7920 7275 6e20 7370 6f74 2070  'Only run spot p
+00012380: 6970 656c 696e 6520 7265 636f 7665 7279  ipeline recovery
+00012390: 2074 6573 7420 696e 2075 732d 7765 7374   test in us-west
+000123a0: 2d32 2729 0a20 2020 2074 6573 7420 3d20  -2').    test = 
+000123b0: 5465 7374 280a 2020 2020 2020 2020 2773  Test(.        's
+000123c0: 706f 745f 7069 7065 6c69 6e65 5f72 6563  pot_pipeline_rec
+000123d0: 6f76 6572 795f 6177 7327 2c0a 2020 2020  overy_aws',.    
+000123e0: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+000123f0: 2020 6627 736b 7920 7370 6f74 206c 6175    f'sky spot lau
+00012400: 6e63 6820 2d6e 207b 6e61 6d65 7d20 7465  nch -n {name} te
+00012410: 7374 732f 7465 7374 5f79 616d 6c73 2f70  sts/test_yamls/p
+00012420: 6970 656c 696e 655f 6177 732e 7961 6d6c  ipeline_aws.yaml
+00012430: 2020 2d79 202d 6427 2c0a 2020 2020 2020    -y -d',.      
+00012440: 2020 2020 2020 2773 6c65 6570 2034 3030        'sleep 400
+00012450: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+00012460: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
+00012470: 4954 7d7c 2067 7265 7020 7b6e 616d 657d  IT}| grep {name}
+00012480: 207c 2068 6561 6420 2d6e 3120 7c20 6772   | head -n1 | gr
+00012490: 6570 2022 5255 4e4e 494e 4722 272c 0a20  ep "RUNNING"',. 
+000124a0: 2020 2020 2020 2020 2020 2066 2752 554e             f'RUN
+000124b0: 5f49 443d 2428 736b 7920 7370 6f74 206c  _ID=$(sky spot l
+000124c0: 6f67 7320 2d6e 207b 6e61 6d65 7d20 2d2d  ogs -n {name} --
+000124d0: 6e6f 2d66 6f6c 6c6f 7720 7c20 6772 6570  no-follow | grep
+000124e0: 2053 4b59 5049 4c4f 545f 5441 534b 5f49   SKYPILOT_TASK_I
+000124f0: 443a 207c 2063 7574 202d 643a 202d 6632  D: | cut -d: -f2
+00012500: 293b 2065 6368 6f20 2224 5255 4e5f 4944  ); echo "$RUN_ID
+00012510: 2220 7c20 7465 6520 2f74 6d70 2f7b 6e61  " | tee /tmp/{na
+00012520: 6d65 7d2d 7275 6e2d 6964 272c 0a20 2020  me}-run-id',.   
+00012530: 2020 2020 2020 2020 2066 2752 554e 5f49           f'RUN_I
+00012540: 4453 3d24 2873 6b79 2073 706f 7420 6c6f  DS=$(sky spot lo
+00012550: 6773 202d 6e20 7b6e 616d 657d 202d 2d6e  gs -n {name} --n
+00012560: 6f2d 666f 6c6c 6f77 207c 2067 7265 7020  o-follow | grep 
+00012570: 2d41 2034 2053 4b59 5049 4c4f 545f 5441  -A 4 SKYPILOT_TA
+00012580: 534b 5f49 4453 207c 2063 7574 202d 6422  SK_IDS | cut -d"
+00012590: 2922 202d 6632 293b 2065 6368 6f20 2224  )" -f2); echo "$
+000125a0: 5255 4e5f 4944 5322 207c 2074 6565 202f  RUN_IDS" | tee /
+000125b0: 746d 702f 7b6e 616d 657d 2d72 756e 2d69  tmp/{name}-run-i
+000125c0: 6473 272c 0a20 2020 2020 2020 2020 2020  ds',.           
+000125d0: 2023 2054 6572 6d69 6e61 7465 2074 6865   # Terminate the
+000125e0: 2063 6c75 7374 6572 206d 616e 7561 6c6c   cluster manuall
+000125f0: 792e 0a20 2020 2020 2020 2020 2020 2023  y..            #
+00012600: 2054 6865 2060 6361 7420 2e2e 2e7c 2072   The `cat ...| r
+00012610: 6576 6020 6973 2074 6f20 7265 7472 6965  ev` is to retrie
+00012620: 7665 2074 6865 206a 6f62 5f69 6420 6672  ve the job_id fr
+00012630: 6f6d 2074 6865 0a20 2020 2020 2020 2020  om the.         
+00012640: 2020 2023 2053 4b59 5049 4c4f 545f 5441     # SKYPILOT_TA
+00012650: 534b 5f49 442c 2077 6869 6368 2067 6574  SK_ID, which get
+00012660: 7320 7468 6520 7365 636f 6e64 2074 6f20  s the second to 
+00012670: 6c61 7374 2066 6965 6c64 0a20 2020 2020  last field.     
+00012680: 2020 2020 2020 2023 2073 6570 6172 6174         # separat
+00012690: 6564 2062 7920 602d 602e 0a20 2020 2020  ed by `-`..     
+000126a0: 2020 2020 2020 2028 6627 5350 4f54 5f4a         (f'SPOT_J
+000126b0: 4f42 5f49 443d 6063 6174 202f 746d 702f  OB_ID=`cat /tmp/
+000126c0: 7b6e 616d 657d 2d72 756e 2d69 6420 7c20  {name}-run-id | 
+000126d0: 7265 7620 7c20 270a 2020 2020 2020 2020  rev | '.        
+000126e0: 2020 2020 2027 6375 7420 2d64 5c27 2d5c       'cut -d\'-\
+000126f0: 2720 2d66 3220 7c20 7265 7660 3b27 0a20  ' -f2 | rev`;'. 
+00012700: 2020 2020 2020 2020 2020 2020 6627 6177              f'aw
+00012710: 7320 6563 3220 7465 726d 696e 6174 652d  s ec2 terminate-
+00012720: 696e 7374 616e 6365 7320 2d2d 7265 6769  instances --regi
+00012730: 6f6e 207b 7265 6769 6f6e 7d20 2d2d 696e  on {region} --in
+00012740: 7374 616e 6365 2d69 6473 2024 2827 0a20  stance-ids $('. 
+00012750: 2020 2020 2020 2020 2020 2020 6627 6177              f'aw
+00012760: 7320 6563 3220 6465 7363 7269 6265 2d69  s ec2 describe-i
+00012770: 6e73 7461 6e63 6573 202d 2d72 6567 696f  nstances --regio
+00012780: 6e20 7b72 6567 696f 6e7d 2027 0a20 2020  n {region} '.   
+00012790: 2020 2020 2020 2020 2020 272d 2d66 696c            '--fil
+000127a0: 7465 7273 204e 616d 653d 7461 673a 7261  ters Name=tag:ra
+000127b0: 792d 636c 7573 7465 722d 6e61 6d65 2c56  y-cluster-name,V
+000127c0: 616c 7565 733d 2a2d 247b 5350 4f54 5f4a  alues=*-${SPOT_J
+000127d0: 4f42 5f49 447d 2027 0a20 2020 2020 2020  OB_ID} '.       
+000127e0: 2020 2020 2020 6627 2d2d 7175 6572 7920        f'--query 
+000127f0: 5265 7365 7276 6174 696f 6e73 5b5d 2e49  Reservations[].I
+00012800: 6e73 7461 6e63 6573 5b5d 2e49 6e73 7461  nstances[].Insta
+00012810: 6e63 6549 6420 270a 2020 2020 2020 2020  nceId '.        
+00012820: 2020 2020 2027 2d2d 6f75 7470 7574 2074       '--output t
+00012830: 6578 7429 2729 2c0a 2020 2020 2020 2020  ext)'),.        
+00012840: 2020 2020 2773 6c65 6570 2031 3030 272c      'sleep 100',
+00012850: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
+00012860: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
+00012870: 7d7c 2067 7265 7020 7b6e 616d 657d 207c  }| grep {name} |
+00012880: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
+00012890: 2022 5245 434f 5645 5249 4e47 2227 2c0a   "RECOVERING"',.
+000128a0: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
+000128b0: 6570 2032 3030 272c 0a20 2020 2020 2020  ep 200',.       
+000128c0: 2020 2020 2066 277b 5f53 504f 545f 5155       f'{_SPOT_QU
+000128d0: 4555 455f 5741 4954 7d7c 2067 7265 7020  EUE_WAIT}| grep 
+000128e0: 7b6e 616d 657d 207c 2068 6561 6420 2d6e  {name} | head -n
+000128f0: 3120 7c20 6772 6570 2022 5255 4e4e 494e  1 | grep "RUNNIN
+00012900: 4722 272c 0a20 2020 2020 2020 2020 2020  G"',.           
+00012910: 2066 2752 554e 5f49 443d 2428 6361 7420   f'RUN_ID=$(cat 
+00012920: 2f74 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d  /tmp/{name}-run-
+00012930: 6964 293b 2065 6368 6f20 2452 554e 5f49  id); echo $RUN_I
+00012940: 443b 2073 6b79 2073 706f 7420 6c6f 6773  D; sky spot logs
+00012950: 202d 6e20 7b6e 616d 657d 202d 2d6e 6f2d   -n {name} --no-
+00012960: 666f 6c6c 6f77 207c 2067 7265 7020 534b  follow | grep SK
+00012970: 5950 494c 4f54 5f54 4153 4b5f 4944 3a20  YPILOT_TASK_ID: 
+00012980: 7c20 6772 6570 2022 2452 554e 5f49 4422  | grep "$RUN_ID"
+00012990: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+000129a0: 2752 554e 5f49 4453 3d24 2873 6b79 2073  'RUN_IDS=$(sky s
+000129b0: 706f 7420 6c6f 6773 202d 6e20 7b6e 616d  pot logs -n {nam
+000129c0: 657d 202d 2d6e 6f2d 666f 6c6c 6f77 207c  e} --no-follow |
+000129d0: 2067 7265 7020 2d41 2034 2053 4b59 5049   grep -A 4 SKYPI
+000129e0: 4c4f 545f 5441 534b 5f49 4453 207c 2063  LOT_TASK_IDS | c
+000129f0: 7574 202d 6422 2922 202d 6632 293b 2065  ut -d")" -f2); e
+00012a00: 6368 6f20 2224 5255 4e5f 4944 5322 207c  cho "$RUN_IDS" |
+00012a10: 2074 6565 202f 746d 702f 7b6e 616d 657d   tee /tmp/{name}
+00012a20: 2d72 756e 2d69 6473 2d6e 6577 272c 0a20  -run-ids-new',. 
+00012a30: 2020 2020 2020 2020 2020 2066 2764 6966             f'dif
+00012a40: 6620 2f74 6d70 2f7b 6e61 6d65 7d2d 7275  f /tmp/{name}-ru
+00012a50: 6e2d 6964 7320 2f74 6d70 2f7b 6e61 6d65  n-ids /tmp/{name
+00012a60: 7d2d 7275 6e2d 6964 732d 6e65 7727 2c0a  }-run-ids-new',.
+00012a70: 2020 2020 2020 2020 2020 2020 6627 6361              f'ca
+00012a80: 7420 2f74 6d70 2f7b 6e61 6d65 7d2d 7275  t /tmp/{name}-ru
+00012a90: 6e2d 6964 7320 7c20 7365 6420 2d6e 2032  n-ids | sed -n 2
+00012aa0: 7020 7c20 6772 6570 2060 6361 7420 2f74  p | grep `cat /t
+00012ab0: 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d 6964  mp/{name}-run-id
+00012ac0: 6027 2c0a 2020 2020 2020 2020 5d2c 0a20  `',.        ],. 
+00012ad0: 2020 2020 2020 205f 5350 4f54 5f43 414e         _SPOT_CAN
+00012ae0: 4345 4c5f 5741 4954 2e66 6f72 6d61 7428  CEL_WAIT.format(
+00012af0: 6a6f 625f 6e61 6d65 3d6e 616d 6529 2c0a  job_name=name),.
+00012b00: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
+00012b10: 3235 202a 2036 302c 0a20 2020 2029 0a20  25 * 60,.    ). 
+00012b20: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+00012b30: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
+00012b40: 6d61 726b 2e67 6370 0a40 7079 7465 7374  mark.gcp.@pytest
+00012b50: 2e6d 6172 6b2e 6d61 6e61 6765 645f 7370  .mark.managed_sp
+00012b60: 6f74 0a64 6566 2074 6573 745f 7370 6f74  ot.def test_spot
+00012b70: 5f70 6970 656c 696e 655f 7265 636f 7665  _pipeline_recove
+00012b80: 7279 5f67 6370 2829 3a0a 2020 2020 2222  ry_gcp():.    ""
+00012b90: 2254 6573 7420 6d61 6e61 6765 6420 7370  "Test managed sp
+00012ba0: 6f74 2072 6563 6f76 6572 7920 666f 7220  ot recovery for 
+00012bb0: 6120 7069 7065 6c69 6e65 2e22 2222 0a20  a pipeline.""". 
+00012bc0: 2020 206e 616d 6520 3d20 5f67 6574 5f63     name = _get_c
+00012bd0: 6c75 7374 6572 5f6e 616d 6528 290a 2020  luster_name().  
+00012be0: 2020 7a6f 6e65 203d 2027 7573 2d65 6173    zone = 'us-eas
+00012bf0: 7434 2d62 270a 2020 2020 7175 6572 795f  t4-b'.    query_
+00012c00: 636d 6420 3d20 2827 6763 6c6f 7564 2063  cmd = ('gcloud c
+00012c10: 6f6d 7075 7465 2069 6e73 7461 6e63 6573  ompute instances
+00012c20: 206c 6973 7420 2d2d 6669 6c74 6572 3d27   list --filter='
+00012c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012c40: 2020 2722 286c 6162 656c 732e 7261 792d    '"(labels.ray-
+00012c50: 636c 7573 7465 722d 6e61 6d65 3a2a 2d24  cluster-name:*-$
+00012c60: 7b53 504f 545f 4a4f 425f 4944 7d29 2220  {SPOT_JOB_ID})" 
+00012c70: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00012c80: 2020 2066 272d 2d7a 6f6e 6573 3d7b 7a6f     f'--zones={zo
+00012c90: 6e65 7d20 2d2d 666f 726d 6174 3d22 7661  ne} --format="va
+00012ca0: 6c75 6528 6e61 6d65 2922 2729 0a20 2020  lue(name)"').   
+00012cb0: 2074 6572 6d69 6e61 7465 5f63 6d64 203d   terminate_cmd =
+00012cc0: 2028 6627 6763 6c6f 7564 2063 6f6d 7075   (f'gcloud compu
+00012cd0: 7465 2069 6e73 7461 6e63 6573 2064 656c  te instances del
+00012ce0: 6574 6520 2d2d 7a6f 6e65 3d7b 7a6f 6e65  ete --zone={zone
+00012cf0: 7d27 0a20 2020 2020 2020 2020 2020 2020  }'.             
+00012d00: 2020 2020 2020 2020 6627 202d 2d71 7569          f' --qui
+00012d10: 6574 2024 287b 7175 6572 795f 636d 647d  et $({query_cmd}
+00012d20: 2927 290a 2020 2020 7465 7374 203d 2054  )').    test = T
+00012d30: 6573 7428 0a20 2020 2020 2020 2027 7370  est(.        'sp
+00012d40: 6f74 5f70 6970 656c 696e 655f 7265 636f  ot_pipeline_reco
+00012d50: 7665 7279 5f67 6370 272c 0a20 2020 2020  very_gcp',.     
+00012d60: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+00012d70: 2066 2773 6b79 2073 706f 7420 6c61 756e   f'sky spot laun
+00012d80: 6368 202d 6e20 7b6e 616d 657d 2074 6573  ch -n {name} tes
+00012d90: 7473 2f74 6573 745f 7961 6d6c 732f 7069  ts/test_yamls/pi
+00012da0: 7065 6c69 6e65 5f67 6370 2e79 616d 6c20  peline_gcp.yaml 
+00012db0: 202d 7920 2d64 272c 0a20 2020 2020 2020   -y -d',.       
+00012dc0: 2020 2020 2027 736c 6565 7020 3430 3027       'sleep 400'
+00012dd0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+00012de0: 7b5f 5350 4f54 5f51 5545 5545 5f57 4149  {_SPOT_QUEUE_WAI
+00012df0: 547d 7c20 6772 6570 207b 6e61 6d65 7d20  T}| grep {name} 
+00012e00: 7c20 6865 6164 202d 6e31 207c 2067 7265  | head -n1 | gre
+00012e10: 7020 2252 554e 4e49 4e47 2227 2c0a 2020  p "RUNNING"',.  
+00012e20: 2020 2020 2020 2020 2020 6627 5255 4e5f            f'RUN_
+00012e30: 4944 3d24 2873 6b79 2073 706f 7420 6c6f  ID=$(sky spot lo
+00012e40: 6773 202d 6e20 7b6e 616d 657d 202d 2d6e  gs -n {name} --n
+00012e50: 6f2d 666f 6c6c 6f77 207c 2067 7265 7020  o-follow | grep 
+00012e60: 534b 5950 494c 4f54 5f54 4153 4b5f 4944  SKYPILOT_TASK_ID
+00012e70: 3a20 7c20 6375 7420 2d64 3a20 2d66 3229  : | cut -d: -f2)
+00012e80: 3b20 6563 686f 2022 2452 554e 5f49 4422  ; echo "$RUN_ID"
+00012e90: 207c 2074 6565 202f 746d 702f 7b6e 616d   | tee /tmp/{nam
+00012ea0: 657d 2d72 756e 2d69 6427 2c0a 2020 2020  e}-run-id',.    
+00012eb0: 2020 2020 2020 2020 6627 5255 4e5f 4944          f'RUN_ID
+00012ec0: 533d 2428 736b 7920 7370 6f74 206c 6f67  S=$(sky spot log
+00012ed0: 7320 2d6e 207b 6e61 6d65 7d20 2d2d 6e6f  s -n {name} --no
+00012ee0: 2d66 6f6c 6c6f 7720 7c20 6772 6570 202d  -follow | grep -
+00012ef0: 4120 3420 534b 5950 494c 4f54 5f54 4153  A 4 SKYPILOT_TAS
+00012f00: 4b5f 4944 5320 7c20 6375 7420 2d64 2229  K_IDS | cut -d")
+00012f10: 2220 2d66 3229 3b20 6563 686f 2022 2452  " -f2); echo "$R
+00012f20: 554e 5f49 4453 2220 7c20 7465 6520 2f74  UN_IDS" | tee /t
+00012f30: 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d 6964  mp/{name}-run-id
+00012f40: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
+00012f50: 2320 5465 726d 696e 6174 6520 7468 6520  # Terminate the 
+00012f60: 636c 7573 7465 7220 6d61 6e75 616c 6c79  cluster manually
+00012f70: 2e0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00012f80: 5468 6520 6063 6174 202e 2e2e 7c20 7265  The `cat ...| re
+00012f90: 7660 2069 7320 746f 2072 6574 7269 6576  v` is to retriev
+00012fa0: 6520 7468 6520 6a6f 625f 6964 2066 726f  e the job_id fro
+00012fb0: 6d20 7468 650a 2020 2020 2020 2020 2020  m the.          
+00012fc0: 2020 2320 534b 5950 494c 4f54 5f54 4153    # SKYPILOT_TAS
+00012fd0: 4b5f 4944 2c20 7768 6963 6820 6765 7473  K_ID, which gets
+00012fe0: 2074 6865 2073 6563 6f6e 6420 746f 206c   the second to l
+00012ff0: 6173 7420 6669 656c 640a 2020 2020 2020  ast field.      
+00013000: 2020 2020 2020 2320 7365 7061 7261 7465        # separate
+00013010: 6420 6279 2060 2d60 2e0a 2020 2020 2020  d by `-`..      
+00013020: 2020 2020 2020 2866 2753 504f 545f 4a4f        (f'SPOT_JO
+00013030: 425f 4944 3d60 6361 7420 2f74 6d70 2f7b  B_ID=`cat /tmp/{
+00013040: 6e61 6d65 7d2d 7275 6e2d 6964 207c 2072  name}-run-id | r
+00013050: 6576 207c 2027 0a20 2020 2020 2020 2020  ev | '.         
+00013060: 2020 2020 6627 6375 7420 2d64 5c27 2d5c      f'cut -d\'-\
+00013070: 2720 2d66 3220 7c20 7265 7660 3b7b 7465  ' -f2 | rev`;{te
+00013080: 726d 696e 6174 655f 636d 647d 2729 2c0a  rminate_cmd}'),.
+00013090: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
+000130a0: 6570 2031 3030 272c 0a20 2020 2020 2020  ep 100',.       
+000130b0: 2020 2020 2066 277b 5f53 504f 545f 5155       f'{_SPOT_QU
+000130c0: 4555 455f 5741 4954 7d7c 2067 7265 7020  EUE_WAIT}| grep 
+000130d0: 7b6e 616d 657d 207c 2068 6561 6420 2d6e  {name} | head -n
+000130e0: 3120 7c20 6772 6570 2022 5245 434f 5645  1 | grep "RECOVE
+000130f0: 5249 4e47 2227 2c0a 2020 2020 2020 2020  RING"',.        
+00013100: 2020 2020 2773 6c65 6570 2032 3030 272c      'sleep 200',
+00013110: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
+00013120: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
+00013130: 7d7c 2067 7265 7020 7b6e 616d 657d 207c  }| grep {name} |
+00013140: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
+00013150: 2022 5255 4e4e 494e 4722 272c 0a20 2020   "RUNNING"',.   
+00013160: 2020 2020 2020 2020 2066 2752 554e 5f49           f'RUN_I
+00013170: 443d 2428 6361 7420 2f74 6d70 2f7b 6e61  D=$(cat /tmp/{na
+00013180: 6d65 7d2d 7275 6e2d 6964 293b 2065 6368  me}-run-id); ech
+00013190: 6f20 2452 554e 5f49 443b 2073 6b79 2073  o $RUN_ID; sky s
+000131a0: 706f 7420 6c6f 6773 202d 6e20 7b6e 616d  pot logs -n {nam
+000131b0: 657d 202d 2d6e 6f2d 666f 6c6c 6f77 207c  e} --no-follow |
+000131c0: 2067 7265 7020 534b 5950 494c 4f54 5f54   grep SKYPILOT_T
+000131d0: 4153 4b5f 4944 3a20 7c20 6772 6570 2022  ASK_ID: | grep "
+000131e0: 2452 554e 5f49 4422 272c 0a20 2020 2020  $RUN_ID"',.     
+000131f0: 2020 2020 2020 2066 2752 554e 5f49 4453         f'RUN_IDS
+00013200: 3d24 2873 6b79 2073 706f 7420 6c6f 6773  =$(sky spot logs
+00013210: 202d 6e20 7b6e 616d 657d 202d 2d6e 6f2d   -n {name} --no-
+00013220: 666f 6c6c 6f77 207c 2067 7265 7020 2d41  follow | grep -A
+00013230: 2034 2053 4b59 5049 4c4f 545f 5441 534b   4 SKYPILOT_TASK
+00013240: 5f49 4453 207c 2063 7574 202d 6422 2922  _IDS | cut -d")"
+00013250: 202d 6632 293b 2065 6368 6f20 2224 5255   -f2); echo "$RU
+00013260: 4e5f 4944 5322 207c 2074 6565 202f 746d  N_IDS" | tee /tm
+00013270: 702f 7b6e 616d 657d 2d72 756e 2d69 6473  p/{name}-run-ids
+00013280: 2d6e 6577 272c 0a20 2020 2020 2020 2020  -new',.         
+00013290: 2020 2066 2764 6966 6620 2f74 6d70 2f7b     f'diff /tmp/{
+000132a0: 6e61 6d65 7d2d 7275 6e2d 6964 7320 2f74  name}-run-ids /t
+000132b0: 6d70 2f7b 6e61 6d65 7d2d 7275 6e2d 6964  mp/{name}-run-id
+000132c0: 732d 6e65 7727 2c0a 2020 2020 2020 2020  s-new',.        
+000132d0: 2020 2020 6627 6361 7420 2f74 6d70 2f7b      f'cat /tmp/{
+000132e0: 6e61 6d65 7d2d 7275 6e2d 6964 7320 7c20  name}-run-ids | 
+000132f0: 7365 6420 2d6e 2032 7020 7c20 6772 6570  sed -n 2p | grep
+00013300: 2060 6361 7420 2f74 6d70 2f7b 6e61 6d65   `cat /tmp/{name
+00013310: 7d2d 7275 6e2d 6964 6027 2c0a 2020 2020  }-run-id`',.    
+00013320: 2020 2020 5d2c 0a20 2020 2020 2020 205f      ],.        _
+00013330: 5350 4f54 5f43 414e 4345 4c5f 5741 4954  SPOT_CANCEL_WAIT
+00013340: 2e66 6f72 6d61 7428 6a6f 625f 6e61 6d65  .format(job_name
+00013350: 3d6e 616d 6529 2c0a 2020 2020 2020 2020  =name),.        
+00013360: 7469 6d65 6f75 743d 3235 202a 2036 302c  timeout=25 * 60,
+00013370: 0a20 2020 2029 0a20 2020 2072 756e 5f6f  .    ).    run_o
+00013380: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
+00013390: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
+000133a0: 6c61 6d62 6461 5f63 6c6f 7564 2020 2320  lambda_cloud  # 
+000133b0: 4c61 6d62 6461 2043 6c6f 7564 2064 6f65  Lambda Cloud doe
+000133c0: 7320 6e6f 7420 7375 7070 6f72 7420 7370  s not support sp
+000133d0: 6f74 2069 6e73 7461 6e63 6573 0a40 7079  ot instances.@py
+000133e0: 7465 7374 2e6d 6172 6b2e 6e6f 5f69 626d  test.mark.no_ibm
+000133f0: 2020 2320 4942 4d20 436c 6f75 6420 646f    # IBM Cloud do
+00013400: 6573 206e 6f74 2073 7570 706f 7274 2073  es not support s
+00013410: 706f 7420 696e 7374 616e 6365 730a 4070  pot instances.@p
+00013420: 7974 6573 742e 6d61 726b 2e6e 6f5f 7363  ytest.mark.no_sc
+00013430: 7020 2023 2053 4350 2064 6f65 7320 6e6f  p  # SCP does no
+00013440: 7420 7375 7070 6f72 7420 7370 6f74 2069  t support spot i
+00013450: 6e73 7461 6e63 6573 0a40 7079 7465 7374  nstances.@pytest
+00013460: 2e6d 6172 6b2e 6d61 6e61 6765 645f 7370  .mark.managed_sp
+00013470: 6f74 0a64 6566 2074 6573 745f 7370 6f74  ot.def test_spot
+00013480: 5f72 6563 6f76 6572 795f 6465 6661 756c  _recovery_defaul
+00013490: 745f 7265 736f 7572 6365 7328 6765 6e65  t_resources(gene
+000134a0: 7269 635f 636c 6f75 643a 2073 7472 293a  ric_cloud: str):
+000134b0: 0a20 2020 2022 2222 5465 7374 206d 616e  .    """Test man
+000134c0: 6167 6564 2073 706f 7420 7265 636f 7665  aged spot recove
+000134d0: 7279 2066 6f72 2064 6566 6175 6c74 2072  ry for default r
+000134e0: 6573 6f75 7263 6573 2e22 2222 0a20 2020  esources.""".   
+000134f0: 206e 616d 6520 3d20 5f67 6574 5f63 6c75   name = _get_clu
+00013500: 7374 6572 5f6e 616d 6528 290a 2020 2020  ster_name().    
+00013510: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
+00013520: 2020 2020 2027 6d61 6e61 6765 642d 7370       'managed-sp
+00013530: 6f74 2d72 6563 6f76 6572 792d 6465 6661  ot-recovery-defa
+00013540: 756c 742d 7265 736f 7572 6365 7327 2c0a  ult-resources',.
+00013550: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
+00013560: 2020 2020 2020 6627 736b 7920 7370 6f74        f'sky spot
+00013570: 206c 6175 6e63 6820 2d6e 207b 6e61 6d65   launch -n {name
+00013580: 7d20 2d2d 636c 6f75 6420 7b67 656e 6572  } --cloud {gener
+00013590: 6963 5f63 6c6f 7564 7d20 2273 6c65 6570  ic_cloud} "sleep
+000135a0: 2033 3020 2626 2073 7564 6f20 7368 7574   30 && sudo shut
+000135b0: 646f 776e 206e 6f77 2026 2620 736c 6565  down now && slee
+000135c0: 7020 3130 3030 2220 2d79 202d 6427 2c0a  p 1000" -y -d',.
+000135d0: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
+000135e0: 6570 2033 3630 272c 0a20 2020 2020 2020  ep 360',.       
+000135f0: 2020 2020 2066 277b 5f53 504f 545f 5155       f'{_SPOT_QU
+00013600: 4555 455f 5741 4954 7d7c 2067 7265 7020  EUE_WAIT}| grep 
+00013610: 7b6e 616d 657d 207c 2068 6561 6420 2d6e  {name} | head -n
+00013620: 3120 7c20 6772 6570 2022 5255 4e4e 494e  1 | grep "RUNNIN
+00013630: 475c 7c52 4543 4f56 4552 494e 4722 272c  G\|RECOVERING"',
+00013640: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
+00013650: 2020 2020 5f53 504f 545f 4341 4e43 454c      _SPOT_CANCEL
+00013660: 5f57 4149 542e 666f 726d 6174 286a 6f62  _WAIT.format(job
+00013670: 5f6e 616d 653d 6e61 6d65 292c 0a20 2020  _name=name),.   
+00013680: 2020 2020 2074 696d 656f 7574 3d32 3520       timeout=25 
+00013690: 2a20 3630 2c0a 2020 2020 290a 2020 2020  * 60,.    ).    
+000136a0: 7275 6e5f 6f6e 655f 7465 7374 2874 6573  run_one_test(tes
+000136b0: 7429 0a0a 0a40 7079 7465 7374 2e6d 6172  t)...@pytest.mar
+000136c0: 6b2e 6177 730a 4070 7974 6573 742e 6d61  k.aws.@pytest.ma
+000136d0: 726b 2e6d 616e 6167 6564 5f73 706f 740a  rk.managed_spot.
+000136e0: 6465 6620 7465 7374 5f73 706f 745f 7265  def test_spot_re
+000136f0: 636f 7665 7279 5f6d 756c 7469 5f6e 6f64  covery_multi_nod
+00013700: 655f 6177 7328 6177 735f 636f 6e66 6967  e_aws(aws_config
+00013710: 5f72 6567 696f 6e29 3a0a 2020 2020 2222  _region):.    ""
+00013720: 2254 6573 7420 6d61 6e61 6765 6420 7370  "Test managed sp
+00013730: 6f74 2072 6563 6f76 6572 792e 2222 220a  ot recovery.""".
+00013740: 2020 2020 6e61 6d65 203d 205f 6765 745f      name = _get_
+00013750: 636c 7573 7465 725f 6e61 6d65 2829 0a20  cluster_name(). 
+00013760: 2020 2072 6567 696f 6e20 3d20 6177 735f     region = aws_
+00013770: 636f 6e66 6967 5f72 6567 696f 6e0a 2020  config_region.  
+00013780: 2020 7465 7374 203d 2054 6573 7428 0a20    test = Test(. 
+00013790: 2020 2020 2020 2027 7370 6f74 5f72 6563         'spot_rec
+000137a0: 6f76 6572 795f 6d75 6c74 695f 6e6f 6465  overy_multi_node
+000137b0: 5f61 7773 272c 0a20 2020 2020 2020 205b  _aws',.        [
+000137c0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+000137d0: 6b79 2073 706f 7420 6c61 756e 6368 202d  ky spot launch -
+000137e0: 2d63 6c6f 7564 2061 7773 202d 2d72 6567  -cloud aws --reg
+000137f0: 696f 6e20 7b72 6567 696f 6e7d 202d 6e20  ion {region} -n 
+00013800: 7b6e 616d 657d 202d 2d6e 756d 2d6e 6f64  {name} --num-nod
+00013810: 6573 2032 2022 6563 686f 2053 4b59 5049  es 2 "echo SKYPI
+00013820: 4c4f 545f 5441 534b 5f49 443a 205c 2453  LOT_TASK_ID: \$S
+00013830: 4b59 5049 4c4f 545f 5441 534b 5f49 443b  KYPILOT_TASK_ID;
+00013840: 2073 6c65 6570 2031 3830 3022 2020 2d79   sleep 1800"  -y
+00013850: 202d 6427 2c0a 2020 2020 2020 2020 2020   -d',.          
+00013860: 2020 2773 6c65 6570 2034 3530 272c 0a20    'sleep 450',. 
+00013870: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
+00013880: 504f 545f 5155 4555 455f 5741 4954 7d7c  POT_QUEUE_WAIT}|
+00013890: 2067 7265 7020 7b6e 616d 657d 207c 2068   grep {name} | h
+000138a0: 6561 6420 2d6e 3120 7c20 6772 6570 2022  ead -n1 | grep "
+000138b0: 5255 4e4e 494e 4722 272c 0a20 2020 2020  RUNNING"',.     
+000138c0: 2020 2020 2020 2066 2752 554e 5f49 443d         f'RUN_ID=
+000138d0: 2428 736b 7920 7370 6f74 206c 6f67 7320  $(sky spot logs 
+000138e0: 2d6e 207b 6e61 6d65 7d20 2d2d 6e6f 2d66  -n {name} --no-f
+000138f0: 6f6c 6c6f 7720 7c20 6772 6570 2053 4b59  ollow | grep SKY
+00013900: 5049 4c4f 545f 5441 534b 5f49 4420 7c20  PILOT_TASK_ID | 
+00013910: 6375 7420 2d64 3a20 2d66 3229 3b20 6563  cut -d: -f2); ec
+00013920: 686f 2022 2452 554e 5f49 4422 207c 2074  ho "$RUN_ID" | t
+00013930: 6565 202f 746d 702f 7b6e 616d 657d 2d72  ee /tmp/{name}-r
+00013940: 756e 2d69 6427 2c0a 2020 2020 2020 2020  un-id',.        
+00013950: 2020 2020 2320 5465 726d 696e 6174 6520      # Terminate 
+00013960: 7468 6520 776f 726b 6572 206d 616e 7561  the worker manua
+00013970: 6c6c 792e 0a20 2020 2020 2020 2020 2020  lly..           
+00013980: 2028 6627 6177 7320 6563 3220 7465 726d   (f'aws ec2 term
+00013990: 696e 6174 652d 696e 7374 616e 6365 7320  inate-instances 
+000139a0: 2d2d 7265 6769 6f6e 207b 7265 6769 6f6e  --region {region
+000139b0: 7d20 2d2d 696e 7374 616e 6365 2d69 6473  } --instance-ids
+000139c0: 2024 2827 0a20 2020 2020 2020 2020 2020   $('.           
+000139d0: 2020 6627 6177 7320 6563 3220 6465 7363    f'aws ec2 desc
+000139e0: 7269 6265 2d69 6e73 7461 6e63 6573 202d  ribe-instances -
+000139f0: 2d72 6567 696f 6e20 7b72 6567 696f 6e7d  -region {region}
+00013a00: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+00013a10: 6627 2d2d 6669 6c74 6572 7320 4e61 6d65  f'--filters Name
+00013a20: 3d74 6167 3a72 6179 2d63 6c75 7374 6572  =tag:ray-cluster
+00013a30: 2d6e 616d 652c 5661 6c75 6573 3d7b 6e61  -name,Values={na
+00013a40: 6d65 7d2a 2027 0a20 2020 2020 2020 2020  me}* '.         
+00013a50: 2020 2020 274e 616d 653d 7461 673a 7261      'Name=tag:ra
+00013a60: 792d 6e6f 6465 2d74 7970 652c 5661 6c75  y-node-type,Valu
+00013a70: 6573 3d77 6f72 6b65 7220 270a 2020 2020  es=worker '.    
+00013a80: 2020 2020 2020 2020 2066 272d 2d71 7565           f'--que
+00013a90: 7279 2052 6573 6572 7661 7469 6f6e 735b  ry Reservations[
+00013aa0: 5d2e 496e 7374 616e 6365 735b 5d2e 496e  ].Instances[].In
+00013ab0: 7374 616e 6365 4964 2027 0a20 2020 2020  stanceId '.     
+00013ac0: 2020 2020 2020 2020 272d 2d6f 7574 7075          '--outpu
+00013ad0: 7420 7465 7874 2927 292c 0a20 2020 2020  t text)'),.     
+00013ae0: 2020 2020 2020 2027 736c 6565 7020 3530         'sleep 50
+00013af0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+00013b00: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
+00013b10: 4954 7d7c 2067 7265 7020 7b6e 616d 657d  IT}| grep {name}
+00013b20: 207c 2068 6561 6420 2d6e 3120 7c20 6772   | head -n1 | gr
+00013b30: 6570 2022 5245 434f 5645 5249 4e47 2227  ep "RECOVERING"'
+00013b40: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
+00013b50: 6c65 6570 2035 3630 272c 0a20 2020 2020  leep 560',.     
+00013b60: 2020 2020 2020 2066 277b 5f53 504f 545f         f'{_SPOT_
+00013b70: 5155 4555 455f 5741 4954 7d7c 2067 7265  QUEUE_WAIT}| gre
+00013b80: 7020 7b6e 616d 657d 207c 2068 6561 6420  p {name} | head 
+00013b90: 2d6e 3120 7c20 6772 6570 2022 5255 4e4e  -n1 | grep "RUNN
+00013ba0: 494e 4722 272c 0a20 2020 2020 2020 2020  ING"',.         
+00013bb0: 2020 2066 2752 554e 5f49 443d 2428 6361     f'RUN_ID=$(ca
+00013bc0: 7420 2f74 6d70 2f7b 6e61 6d65 7d2d 7275  t /tmp/{name}-ru
+00013bd0: 6e2d 6964 293b 2065 6368 6f20 2452 554e  n-id); echo $RUN
+00013be0: 5f49 443b 2073 6b79 2073 706f 7420 6c6f  _ID; sky spot lo
+00013bf0: 6773 202d 6e20 7b6e 616d 657d 202d 2d6e  gs -n {name} --n
+00013c00: 6f2d 666f 6c6c 6f77 207c 2067 7265 7020  o-follow | grep 
+00013c10: 534b 5950 494c 4f54 5f54 4153 4b5f 4944  SKYPILOT_TASK_ID
+00013c20: 207c 2063 7574 202d 643a 202d 6632 207c   | cut -d: -f2 |
+00013c30: 2067 7265 7020 2224 5255 4e5f 4944 2227   grep "$RUN_ID"'
+00013c40: 2c0a 2020 2020 2020 2020 5d2c 0a20 2020  ,.        ],.   
+00013c50: 2020 2020 205f 5350 4f54 5f43 414e 4345       _SPOT_CANCE
+00013c60: 4c5f 5741 4954 2e66 6f72 6d61 7428 6a6f  L_WAIT.format(jo
+00013c70: 625f 6e61 6d65 3d6e 616d 6529 2c0a 2020  b_name=name),.  
+00013c80: 2020 2020 2020 7469 6d65 6f75 743d 3330        timeout=30
+00013c90: 202a 2036 302c 0a20 2020 2029 0a20 2020   * 60,.    ).   
+00013ca0: 2072 756e 5f6f 6e65 5f74 6573 7428 7465   run_one_test(te
+00013cb0: 7374 290a 0a0a 4070 7974 6573 742e 6d61  st)...@pytest.ma
+00013cc0: 726b 2e67 6370 0a40 7079 7465 7374 2e6d  rk.gcp.@pytest.m
+00013cd0: 6172 6b2e 6d61 6e61 6765 645f 7370 6f74  ark.managed_spot
+00013ce0: 0a64 6566 2074 6573 745f 7370 6f74 5f72  .def test_spot_r
+00013cf0: 6563 6f76 6572 795f 6d75 6c74 695f 6e6f  ecovery_multi_no
+00013d00: 6465 5f67 6370 2829 3a0a 2020 2020 2222  de_gcp():.    ""
+00013d10: 2254 6573 7420 6d61 6e61 6765 6420 7370  "Test managed sp
+00013d20: 6f74 2072 6563 6f76 6572 792e 2222 220a  ot recovery.""".
+00013d30: 2020 2020 6e61 6d65 203d 205f 6765 745f      name = _get_
+00013d40: 636c 7573 7465 725f 6e61 6d65 2829 0a20  cluster_name(). 
+00013d50: 2020 207a 6f6e 6520 3d20 2775 732d 7765     zone = 'us-we
+00013d60: 7374 322d 6127 0a20 2020 2023 2055 7365  st2-a'.    # Use
+00013d70: 2027 3a27 2074 6f20 6d61 7463 6820 6173   ':' to match as
+00013d80: 2074 6865 2063 6c75 7374 6572 206e 616d   the cluster nam
+00013d90: 6520 7769 6c6c 2063 6f6e 7461 696e 2074  e will contain t
+00013da0: 6865 2073 7566 6669 7820 7769 7468 206a  he suffix with j
+00013db0: 6f62 2069 640a 2020 2020 7175 6572 795f  ob id.    query_
+00013dc0: 636d 6420 3d20 280a 2020 2020 2020 2020  cmd = (.        
+00013dd0: 6627 6763 6c6f 7564 2063 6f6d 7075 7465  f'gcloud compute
+00013de0: 2069 6e73 7461 6e63 6573 206c 6973 7420   instances list 
+00013df0: 2d2d 6669 6c74 6572 3d27 0a20 2020 2020  --filter='.     
+00013e00: 2020 2066 2722 286c 6162 656c 732e 7261     f'"(labels.ra
+00013e10: 792d 636c 7573 7465 722d 6e61 6d65 3a7b  y-cluster-name:{
+00013e20: 6e61 6d65 7d20 414e 4420 6c61 6265 6c73  name} AND labels
+00013e30: 2e72 6179 2d6e 6f64 652d 7479 7065 3d77  .ray-node-type=w
+00013e40: 6f72 6b65 7229 2220 270a 2020 2020 2020  orker)" '.      
+00013e50: 2020 6627 2d2d 7a6f 6e65 733d 7b7a 6f6e    f'--zones={zon
+00013e60: 657d 202d 2d66 6f72 6d61 743d 2276 616c  e} --format="val
+00013e70: 7565 286e 616d 6529 2227 290a 2020 2020  ue(name)"').    
+00013e80: 7465 726d 696e 6174 655f 636d 6420 3d20  terminate_cmd = 
+00013e90: 2866 2767 636c 6f75 6420 636f 6d70 7574  (f'gcloud comput
+00013ea0: 6520 696e 7374 616e 6365 7320 6465 6c65  e instances dele
+00013eb0: 7465 202d 2d7a 6f6e 653d 7b7a 6f6e 657d  te --zone={zone}
+00013ec0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00013ed0: 2020 2020 2020 2066 2720 2d2d 7175 6965         f' --quie
+00013ee0: 7420 2428 7b71 7565 7279 5f63 6d64 7d29  t $({query_cmd})
+00013ef0: 2729 0a20 2020 2074 6573 7420 3d20 5465  ').    test = Te
+00013f00: 7374 280a 2020 2020 2020 2020 2773 706f  st(.        'spo
+00013f10: 745f 7265 636f 7665 7279 5f6d 756c 7469  t_recovery_multi
+00013f20: 5f6e 6f64 655f 6763 7027 2c0a 2020 2020  _node_gcp',.    
+00013f30: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00013f40: 2020 6627 736b 7920 7370 6f74 206c 6175    f'sky spot lau
+00013f50: 6e63 6820 2d2d 636c 6f75 6420 6763 7020  nch --cloud gcp 
+00013f60: 2d2d 7a6f 6e65 207b 7a6f 6e65 7d20 2d6e  --zone {zone} -n
+00013f70: 207b 6e61 6d65 7d20 2d2d 6e75 6d2d 6e6f   {name} --num-no
+00013f80: 6465 7320 3220 2265 6368 6f20 534b 5950  des 2 "echo SKYP
+00013f90: 494c 4f54 5f54 4153 4b5f 4944 3a20 5c24  ILOT_TASK_ID: \$
+00013fa0: 534b 5950 494c 4f54 5f54 4153 4b5f 4944  SKYPILOT_TASK_ID
+00013fb0: 3b20 736c 6565 7020 3138 3030 2220 202d  ; sleep 1800"  -
+00013fc0: 7920 2d64 272c 0a20 2020 2020 2020 2020  y -d',.         
+00013fd0: 2020 2027 736c 6565 7020 3430 3027 2c0a     'sleep 400',.
+00013fe0: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+00013ff0: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
+00014000: 7c20 6772 6570 207b 6e61 6d65 7d20 7c20  | grep {name} | 
+00014010: 6865 6164 202d 6e31 207c 2067 7265 7020  head -n1 | grep 
+00014020: 2252 554e 4e49 4e47 2227 2c0a 2020 2020  "RUNNING"',.    
+00014030: 2020 2020 2020 2020 6627 5255 4e5f 4944          f'RUN_ID
+00014040: 3d24 2873 6b79 2073 706f 7420 6c6f 6773  =$(sky spot logs
+00014050: 202d 6e20 7b6e 616d 657d 202d 2d6e 6f2d   -n {name} --no-
+00014060: 666f 6c6c 6f77 207c 2067 7265 7020 534b  follow | grep SK
+00014070: 5950 494c 4f54 5f54 4153 4b5f 4944 207c  YPILOT_TASK_ID |
+00014080: 2063 7574 202d 643a 202d 6632 293b 2065   cut -d: -f2); e
+00014090: 6368 6f20 2224 5255 4e5f 4944 2220 7c20  cho "$RUN_ID" | 
+000140a0: 7465 6520 2f74 6d70 2f7b 6e61 6d65 7d2d  tee /tmp/{name}-
+000140b0: 7275 6e2d 6964 272c 0a20 2020 2020 2020  run-id',.       
+000140c0: 2020 2020 2023 2054 6572 6d69 6e61 7465       # Terminate
+000140d0: 2074 6865 2077 6f72 6b65 7220 6d61 6e75   the worker manu
+000140e0: 616c 6c79 2e0a 2020 2020 2020 2020 2020  ally..          
+000140f0: 2020 7465 726d 696e 6174 655f 636d 642c    terminate_cmd,
+00014100: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
+00014110: 6565 7020 3530 272c 0a20 2020 2020 2020  eep 50',.       
+00014120: 2020 2020 2066 277b 5f53 504f 545f 5155       f'{_SPOT_QU
+00014130: 4555 455f 5741 4954 7d7c 2067 7265 7020  EUE_WAIT}| grep 
+00014140: 7b6e 616d 657d 207c 2068 6561 6420 2d6e  {name} | head -n
+00014150: 3120 7c20 6772 6570 2022 5245 434f 5645  1 | grep "RECOVE
+00014160: 5249 4e47 2227 2c0a 2020 2020 2020 2020  RING"',.        
+00014170: 2020 2020 2773 6c65 6570 2034 3230 272c      'sleep 420',
+00014180: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
+00014190: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
+000141a0: 7d7c 2067 7265 7020 7b6e 616d 657d 207c  }| grep {name} |
+000141b0: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
+000141c0: 2022 5255 4e4e 494e 4722 272c 0a20 2020   "RUNNING"',.   
+000141d0: 2020 2020 2020 2020 2066 2752 554e 5f49           f'RUN_I
+000141e0: 443d 2428 6361 7420 2f74 6d70 2f7b 6e61  D=$(cat /tmp/{na
+000141f0: 6d65 7d2d 7275 6e2d 6964 293b 2065 6368  me}-run-id); ech
+00014200: 6f20 2452 554e 5f49 443b 2073 6b79 2073  o $RUN_ID; sky s
+00014210: 706f 7420 6c6f 6773 202d 6e20 7b6e 616d  pot logs -n {nam
+00014220: 657d 202d 2d6e 6f2d 666f 6c6c 6f77 207c  e} --no-follow |
+00014230: 2067 7265 7020 534b 5950 494c 4f54 5f54   grep SKYPILOT_T
+00014240: 4153 4b5f 4944 207c 2063 7574 202d 643a  ASK_ID | cut -d:
+00014250: 202d 6632 207c 2067 7265 7020 2224 5255   -f2 | grep "$RU
+00014260: 4e5f 4944 2227 2c0a 2020 2020 2020 2020  N_ID"',.        
+00014270: 5d2c 0a20 2020 2020 2020 205f 5350 4f54  ],.        _SPOT
+00014280: 5f43 414e 4345 4c5f 5741 4954 2e66 6f72  _CANCEL_WAIT.for
+00014290: 6d61 7428 6a6f 625f 6e61 6d65 3d6e 616d  mat(job_name=nam
+000142a0: 6529 2c0a 2020 2020 2020 2020 7469 6d65  e),.        time
+000142b0: 6f75 743d 3235 202a 2036 302c 0a20 2020  out=25 * 60,.   
+000142c0: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
+000142d0: 6573 7428 7465 7374 290a 0a0a 4070 7974  est(test)...@pyt
+000142e0: 6573 742e 6d61 726b 2e61 7773 0a40 7079  est.mark.aws.@py
+000142f0: 7465 7374 2e6d 6172 6b2e 6d61 6e61 6765  test.mark.manage
+00014300: 645f 7370 6f74 0a64 6566 2074 6573 745f  d_spot.def test_
+00014310: 7370 6f74 5f63 616e 6365 6c6c 6174 696f  spot_cancellatio
+00014320: 6e5f 6177 7328 6177 735f 636f 6e66 6967  n_aws(aws_config
+00014330: 5f72 6567 696f 6e29 3a0a 2020 2020 6e61  _region):.    na
+00014340: 6d65 203d 205f 6765 745f 636c 7573 7465  me = _get_cluste
+00014350: 725f 6e61 6d65 2829 0a20 2020 2072 6567  r_name().    reg
+00014360: 696f 6e20 3d20 6177 735f 636f 6e66 6967  ion = aws_config
+00014370: 5f72 6567 696f 6e0a 2020 2020 7465 7374  _region.    test
+00014380: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
+00014390: 2027 7370 6f74 5f63 616e 6365 6c6c 6174   'spot_cancellat
+000143a0: 696f 6e5f 6177 7327 2c0a 2020 2020 2020  ion_aws',.      
+000143b0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
+000143c0: 2320 5465 7374 2063 616e 6365 6c6c 6174  # Test cancellat
+000143d0: 696f 6e20 6475 7269 6e67 2073 706f 7420  ion during spot 
+000143e0: 636c 7573 7465 7220 6265 696e 6720 6c61  cluster being la
+000143f0: 756e 6368 6564 2e0a 2020 2020 2020 2020  unched..        
+00014400: 2020 2020 6627 736b 7920 7370 6f74 206c      f'sky spot l
+00014410: 6175 6e63 6820 2d2d 636c 6f75 6420 6177  aunch --cloud aw
+00014420: 7320 2d2d 7265 6769 6f6e 207b 7265 6769  s --region {regi
+00014430: 6f6e 7d20 2d6e 207b 6e61 6d65 7d20 2273  on} -n {name} "s
+00014440: 6c65 6570 2031 3030 3022 2020 2d79 202d  leep 1000"  -y -
+00014450: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
+00014460: 2773 6c65 6570 2036 3027 2c0a 2020 2020  'sleep 60',.    
+00014470: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
+00014480: 5f51 5545 5545 5f57 4149 547d 7c20 6772  _QUEUE_WAIT}| gr
+00014490: 6570 207b 6e61 6d65 7d20 7c20 6865 6164  ep {name} | head
+000144a0: 202d 6e31 207c 2067 7265 7020 2253 5441   -n1 | grep "STA
+000144b0: 5254 494e 4722 272c 0a20 2020 2020 2020  RTING"',.       
+000144c0: 2020 2020 205f 5350 4f54 5f43 414e 4345       _SPOT_CANCE
+000144d0: 4c5f 5741 4954 2e66 6f72 6d61 7428 6a6f  L_WAIT.format(jo
+000144e0: 625f 6e61 6d65 3d6e 616d 6529 2c0a 2020  b_name=name),.  
+000144f0: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
+00014500: 2035 272c 0a20 2020 2020 2020 2020 2020   5',.           
+00014510: 2066 277b 5f53 504f 545f 5155 4555 455f   f'{_SPOT_QUEUE_
+00014520: 5741 4954 7d7c 2067 7265 7020 7b6e 616d  WAIT}| grep {nam
+00014530: 657d 207c 2068 6561 6420 2d6e 3120 7c20  e} | head -n1 | 
+00014540: 6772 6570 2022 4341 4e43 454c 4c49 4e47  grep "CANCELLING
+00014550: 5c7c 4341 4e43 454c 4c45 4422 272c 0a20  \|CANCELLED"',. 
+00014560: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
+00014570: 7020 3132 3027 2c0a 2020 2020 2020 2020  p 120',.        
+00014580: 2020 2020 6627 7b5f 5350 4f54 5f51 5545      f'{_SPOT_QUE
+00014590: 5545 5f57 4149 547d 7c20 6772 6570 207b  UE_WAIT}| grep {
+000145a0: 6e61 6d65 7d20 7c20 6865 6164 202d 6e31  name} | head -n1
+000145b0: 207c 2067 7265 7020 2243 414e 4345 4c4c   | grep "CANCELL
+000145c0: 4544 2227 2c0a 2020 2020 2020 2020 2020  ED"',.          
+000145d0: 2020 2866 2773 3d24 2861 7773 2065 6332    (f's=$(aws ec2
+000145e0: 2064 6573 6372 6962 652d 696e 7374 616e   describe-instan
+000145f0: 6365 7320 2d2d 7265 6769 6f6e 207b 7265  ces --region {re
+00014600: 6769 6f6e 7d20 270a 2020 2020 2020 2020  gion} '.        
+00014610: 2020 2020 2066 272d 2d66 696c 7465 7273       f'--filters
+00014620: 204e 616d 653d 7461 673a 7261 792d 636c   Name=tag:ray-cl
+00014630: 7573 7465 722d 6e61 6d65 2c56 616c 7565  uster-name,Value
+00014640: 733d 7b6e 616d 657d 2d2a 2027 0a20 2020  s={name}-* '.   
+00014650: 2020 2020 2020 2020 2020 6627 2d2d 7175            f'--qu
+00014660: 6572 7920 5265 7365 7276 6174 696f 6e73  ery Reservations
+00014670: 5b5d 2e49 6e73 7461 6e63 6573 5b5d 2e53  [].Instances[].S
+00014680: 7461 7465 5b5d 2e4e 616d 6520 270a 2020  tate[].Name '.  
+00014690: 2020 2020 2020 2020 2020 2027 2d2d 6f75             '--ou
+000146a0: 7470 7574 2074 6578 7429 2026 2620 6563  tput text) && ec
+000146b0: 686f 2022 2473 2220 2626 2065 6368 6f3b  ho "$s" && echo;
+000146c0: 205b 5b20 2d7a 2022 2473 2220 5d5d 207c   [[ -z "$s" ]] |
+000146d0: 7c20 5b5b 2022 2473 2220 3d20 2274 6572  | [[ "$s" = "ter
+000146e0: 6d69 6e61 7465 6422 205d 5d20 7c7c 205b  minated" ]] || [
+000146f0: 5b20 2224 7322 203d 2022 7368 7574 7469  [ "$s" = "shutti
+00014700: 6e67 2d64 6f77 6e22 205d 5d27 0a20 2020  ng-down" ]]'.   
+00014710: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+00014720: 2020 2020 2020 2020 2320 5465 7374 2063          # Test c
+00014730: 616e 6365 6c6c 696e 6720 7468 6520 7370  ancelling the sp
+00014740: 6f74 2063 6c75 7374 6572 2064 7572 696e  ot cluster durin
+00014750: 6720 7370 6f74 206a 6f62 2062 6569 6e67  g spot job being
+00014760: 2073 6574 7570 2e0a 2020 2020 2020 2020   setup..        
+00014770: 2020 2020 6627 736b 7920 7370 6f74 206c      f'sky spot l
+00014780: 6175 6e63 6820 2d2d 636c 6f75 6420 6177  aunch --cloud aw
+00014790: 7320 2d2d 7265 6769 6f6e 207b 7265 6769  s --region {regi
+000147a0: 6f6e 7d20 2d6e 207b 6e61 6d65 7d2d 3220  on} -n {name}-2 
+000147b0: 7465 7374 732f 7465 7374 5f79 616d 6c73  tests/test_yamls
+000147c0: 2f74 6573 745f 6c6f 6e67 5f73 6574 7570  /test_long_setup
+000147d0: 2e79 616d 6c20 202d 7920 2d64 272c 0a20  .yaml  -y -d',. 
+000147e0: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
+000147f0: 7020 3330 3027 2c0a 2020 2020 2020 2020  p 300',.        
+00014800: 2020 2020 5f53 504f 545f 4341 4e43 454c      _SPOT_CANCEL
+00014810: 5f57 4149 542e 666f 726d 6174 286a 6f62  _WAIT.format(job
+00014820: 5f6e 616d 653d 6627 7b6e 616d 657d 2d32  _name=f'{name}-2
+00014830: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+00014840: 2773 6c65 6570 2035 272c 0a20 2020 2020  'sleep 5',.     
+00014850: 2020 2020 2020 2066 277b 5f53 504f 545f         f'{_SPOT_
+00014860: 5155 4555 455f 5741 4954 7d7c 2067 7265  QUEUE_WAIT}| gre
+00014870: 7020 7b6e 616d 657d 2d32 207c 2068 6561  p {name}-2 | hea
+00014880: 6420 2d6e 3120 7c20 6772 6570 2022 4341  d -n1 | grep "CA
+00014890: 4e43 454c 4c49 4e47 5c7c 4341 4e43 454c  NCELLING\|CANCEL
+000148a0: 4c45 4422 272c 0a20 2020 2020 2020 2020  LED"',.         
+000148b0: 2020 2027 736c 6565 7020 3132 3027 2c0a     'sleep 120',.
+000148c0: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+000148d0: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
+000148e0: 7c20 6772 6570 207b 6e61 6d65 7d2d 3220  | grep {name}-2 
+000148f0: 7c20 6865 6164 202d 6e31 207c 2067 7265  | head -n1 | gre
+00014900: 7020 2243 414e 4345 4c4c 4544 2227 2c0a  p "CANCELLED"',.
+00014910: 2020 2020 2020 2020 2020 2020 2866 2773              (f's
+00014920: 3d24 2861 7773 2065 6332 2064 6573 6372  =$(aws ec2 descr
+00014930: 6962 652d 696e 7374 616e 6365 7320 2d2d  ibe-instances --
+00014940: 7265 6769 6f6e 207b 7265 6769 6f6e 7d20  region {region} 
+00014950: 270a 2020 2020 2020 2020 2020 2020 2066  '.             f
+00014960: 272d 2d66 696c 7465 7273 204e 616d 653d  '--filters Name=
+00014970: 7461 673a 7261 792d 636c 7573 7465 722d  tag:ray-cluster-
+00014980: 6e61 6d65 2c56 616c 7565 733d 7b6e 616d  name,Values={nam
+00014990: 657d 2d32 2d2a 2027 0a20 2020 2020 2020  e}-2-* '.       
+000149a0: 2020 2020 2020 6627 2d2d 7175 6572 7920        f'--query 
+000149b0: 5265 7365 7276 6174 696f 6e73 5b5d 2e49  Reservations[].I
+000149c0: 6e73 7461 6e63 6573 5b5d 2e53 7461 7465  nstances[].State
+000149d0: 5b5d 2e4e 616d 6520 270a 2020 2020 2020  [].Name '.      
+000149e0: 2020 2020 2020 2027 2d2d 6f75 7470 7574         '--output
+000149f0: 2074 6578 7429 2026 2620 6563 686f 2022   text) && echo "
+00014a00: 2473 2220 2626 2065 6368 6f3b 205b 5b20  $s" && echo; [[ 
+00014a10: 2d7a 2022 2473 2220 5d5d 207c 7c20 5b5b  -z "$s" ]] || [[
+00014a20: 2022 2473 2220 3d20 2274 6572 6d69 6e61   "$s" = "termina
+00014a30: 7465 6422 205d 5d20 7c7c 205b 5b20 2224  ted" ]] || [[ "$
+00014a40: 7322 203d 2022 7368 7574 7469 6e67 2d64  s" = "shutting-d
+00014a50: 6f77 6e22 205d 5d27 0a20 2020 2020 2020  own" ]]'.       
+00014a60: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+00014a70: 2020 2020 2320 5465 7374 2063 616e 6365      # Test cance
+00014a80: 6c6c 6174 696f 6e20 6475 7269 6e67 2073  llation during s
+00014a90: 706f 7420 6a6f 6220 6973 2072 6563 6f76  pot job is recov
+00014aa0: 6572 696e 672e 0a20 2020 2020 2020 2020  ering..         
+00014ab0: 2020 2066 2773 6b79 2073 706f 7420 6c61     f'sky spot la
+00014ac0: 756e 6368 202d 2d63 6c6f 7564 2061 7773  unch --cloud aws
+00014ad0: 202d 2d72 6567 696f 6e20 7b72 6567 696f   --region {regio
+00014ae0: 6e7d 202d 6e20 7b6e 616d 657d 2d33 2022  n} -n {name}-3 "
+00014af0: 736c 6565 7020 3130 3030 2220 202d 7920  sleep 1000"  -y 
+00014b00: 2d64 272c 0a20 2020 2020 2020 2020 2020  -d',.           
+00014b10: 2027 736c 6565 7020 3330 3027 2c0a 2020   'sleep 300',.  
+00014b20: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
+00014b30: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
+00014b40: 6772 6570 207b 6e61 6d65 7d2d 3320 7c20  grep {name}-3 | 
+00014b50: 6865 6164 202d 6e31 207c 2067 7265 7020  head -n1 | grep 
+00014b60: 2252 554e 4e49 4e47 2227 2c0a 2020 2020  "RUNNING"',.    
+00014b70: 2020 2020 2020 2020 2320 5465 726d 696e          # Termin
+00014b80: 6174 6520 7468 6520 636c 7573 7465 7220  ate the cluster 
+00014b90: 6d61 6e75 616c 6c79 2e0a 2020 2020 2020  manually..      
+00014ba0: 2020 2020 2020 2866 2761 7773 2065 6332        (f'aws ec2
+00014bb0: 2074 6572 6d69 6e61 7465 2d69 6e73 7461   terminate-insta
+00014bc0: 6e63 6573 202d 2d72 6567 696f 6e20 7b72  nces --region {r
+00014bd0: 6567 696f 6e7d 202d 2d69 6e73 7461 6e63  egion} --instanc
+00014be0: 652d 6964 7320 2428 270a 2020 2020 2020  e-ids $('.      
+00014bf0: 2020 2020 2020 2066 2761 7773 2065 6332         f'aws ec2
+00014c00: 2064 6573 6372 6962 652d 696e 7374 616e   describe-instan
+00014c10: 6365 7320 2d2d 7265 6769 6f6e 207b 7265  ces --region {re
+00014c20: 6769 6f6e 7d20 270a 2020 2020 2020 2020  gion} '.        
+00014c30: 2020 2020 2066 272d 2d66 696c 7465 7273       f'--filters
+00014c40: 204e 616d 653d 7461 673a 7261 792d 636c   Name=tag:ray-cl
+00014c50: 7573 7465 722d 6e61 6d65 2c56 616c 7565  uster-name,Value
+00014c60: 733d 7b6e 616d 657d 2d33 2d2a 2027 0a20  s={name}-3-* '. 
+00014c70: 2020 2020 2020 2020 2020 2020 6627 2d2d              f'--
+00014c80: 7175 6572 7920 5265 7365 7276 6174 696f  query Reservatio
+00014c90: 6e73 5b5d 2e49 6e73 7461 6e63 6573 5b5d  ns[].Instances[]
+00014ca0: 2e49 6e73 7461 6e63 6549 6420 270a 2020  .InstanceId '.  
+00014cb0: 2020 2020 2020 2020 2020 2027 2d2d 6f75             '--ou
+00014cc0: 7470 7574 2074 6578 7429 2729 2c0a 2020  tput text)'),.  
+00014cd0: 2020 2020 2020 2020 2020 2773 6c65 6570            'sleep
+00014ce0: 2031 3230 272c 0a20 2020 2020 2020 2020   120',.         
+00014cf0: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
+00014d00: 455f 5741 4954 7d7c 2067 7265 7020 7b6e  E_WAIT}| grep {n
+00014d10: 616d 657d 2d33 207c 2068 6561 6420 2d6e  ame}-3 | head -n
+00014d20: 3120 7c20 6772 6570 2022 5245 434f 5645  1 | grep "RECOVE
+00014d30: 5249 4e47 2227 2c0a 2020 2020 2020 2020  RING"',.        
+00014d40: 2020 2020 5f53 504f 545f 4341 4e43 454c      _SPOT_CANCEL
+00014d50: 5f57 4149 542e 666f 726d 6174 286a 6f62  _WAIT.format(job
+00014d60: 5f6e 616d 653d 6627 7b6e 616d 657d 2d33  _name=f'{name}-3
+00014d70: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+00014d80: 2773 6c65 6570 2035 272c 0a20 2020 2020  'sleep 5',.     
+00014d90: 2020 2020 2020 2066 277b 5f53 504f 545f         f'{_SPOT_
+00014da0: 5155 4555 455f 5741 4954 7d7c 2067 7265  QUEUE_WAIT}| gre
+00014db0: 7020 7b6e 616d 657d 2d33 207c 2068 6561  p {name}-3 | hea
+00014dc0: 6420 2d6e 3120 7c20 6772 6570 2022 4341  d -n1 | grep "CA
+00014dd0: 4e43 454c 4c49 4e47 5c7c 4341 4e43 454c  NCELLING\|CANCEL
+00014de0: 4c45 4422 272c 0a20 2020 2020 2020 2020  LED"',.         
+00014df0: 2020 2027 736c 6565 7020 3132 3027 2c0a     'sleep 120',.
+00014e00: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+00014e10: 5350 4f54 5f51 5545 5545 5f57 4149 547d  SPOT_QUEUE_WAIT}
+00014e20: 7c20 6772 6570 207b 6e61 6d65 7d2d 3320  | grep {name}-3 
+00014e30: 7c20 6865 6164 202d 6e31 207c 2067 7265  | head -n1 | gre
+00014e40: 7020 2243 414e 4345 4c4c 4544 2227 2c0a  p "CANCELLED"',.
+00014e50: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
+00014e60: 6520 636c 7573 7465 7220 7368 6f75 6c64  e cluster should
+00014e70: 2062 6520 7465 726d 696e 6174 6564 2028   be terminated (
+00014e80: 7368 7574 7469 6e67 2d64 6f77 6e29 2061  shutting-down) a
+00014e90: 6674 6572 2063 616e 6365 6c6c 6174 696f  fter cancellatio
+00014ea0: 6e2e 2057 6520 646f 6e27 7420 7573 6520  n. We don't use 
+00014eb0: 7468 6520 603d 6020 6f70 6572 6174 6f72  the `=` operator
+00014ec0: 2068 6572 6520 6265 6361 7573 650a 2020   here because.  
+00014ed0: 2020 2020 2020 2020 2020 2320 7468 6572            # ther
+00014ee0: 6520 6361 6e20 6265 206d 756c 7469 706c  e can be multipl
+00014ef0: 6520 564d 2077 6974 6820 7468 6520 7361  e VM with the sa
+00014f00: 6d65 206e 616d 6520 6475 6520 746f 2074  me name due to t
+00014f10: 6865 2072 6563 6f76 6572 792e 0a20 2020  he recovery..   
+00014f20: 2020 2020 2020 2020 2028 6627 733d 2428           (f's=$(
+00014f30: 6177 7320 6563 3220 6465 7363 7269 6265  aws ec2 describe
+00014f40: 2d69 6e73 7461 6e63 6573 202d 2d72 6567  -instances --reg
+00014f50: 696f 6e20 7b72 6567 696f 6e7d 2027 0a20  ion {region} '. 
+00014f60: 2020 2020 2020 2020 2020 2020 6627 2d2d              f'--
+00014f70: 6669 6c74 6572 7320 4e61 6d65 3d74 6167  filters Name=tag
+00014f80: 3a72 6179 2d63 6c75 7374 6572 2d6e 616d  :ray-cluster-nam
+00014f90: 652c 5661 6c75 6573 3d7b 6e61 6d65 7d2d  e,Values={name}-
+00014fa0: 332d 2a20 270a 2020 2020 2020 2020 2020  3-* '.          
+00014fb0: 2020 2066 272d 2d71 7565 7279 2052 6573     f'--query Res
+00014fc0: 6572 7661 7469 6f6e 735b 5d2e 496e 7374  ervations[].Inst
+00014fd0: 616e 6365 735b 5d2e 5374 6174 655b 5d2e  ances[].State[].
+00014fe0: 4e61 6d65 2027 0a20 2020 2020 2020 2020  Name '.         
+00014ff0: 2020 2020 272d 2d6f 7574 7075 7420 7465      '--output te
+00015000: 7874 2920 2626 2065 6368 6f20 2224 7322  xt) && echo "$s"
+00015010: 2026 2620 6563 686f 3b20 5b5b 202d 7a20   && echo; [[ -z 
+00015020: 2224 7322 205d 5d20 7c7c 2065 6368 6f20  "$s" ]] || echo 
+00015030: 2224 7322 207c 2067 7265 7020 2d76 202d  "$s" | grep -v -
+00015040: 4520 2270 656e 6469 6e67 7c72 756e 6e69  E "pending|runni
+00015050: 6e67 7c73 746f 7070 6564 7c73 746f 7070  ng|stopped|stopp
+00015060: 696e 6722 270a 2020 2020 2020 2020 2020  ing"'.          
+00015070: 2020 292c 0a20 2020 2020 2020 205d 2c0a    ),.        ],.
+00015080: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
+00015090: 3235 202a 2036 3029 0a20 2020 2072 756e  25 * 60).    run
+000150a0: 5f6f 6e65 5f74 6573 7428 7465 7374 290a  _one_test(test).
+000150b0: 0a0a 4070 7974 6573 742e 6d61 726b 2e67  ..@pytest.mark.g
+000150c0: 6370 0a40 7079 7465 7374 2e6d 6172 6b2e  cp.@pytest.mark.
+000150d0: 6d61 6e61 6765 645f 7370 6f74 0a64 6566  managed_spot.def
+000150e0: 2074 6573 745f 7370 6f74 5f63 616e 6365   test_spot_cance
+000150f0: 6c6c 6174 696f 6e5f 6763 7028 293a 0a20  llation_gcp():. 
+00015100: 2020 206e 616d 6520 3d20 5f67 6574 5f63     name = _get_c
+00015110: 6c75 7374 6572 5f6e 616d 6528 290a 2020  luster_name().  
+00015120: 2020 7a6f 6e65 203d 2027 7573 2d77 6573    zone = 'us-wes
+00015130: 7433 2d62 270a 2020 2020 7175 6572 795f  t3-b'.    query_
+00015140: 7374 6174 655f 636d 6420 3d20 2827 6763  state_cmd = ('gc
+00015150: 6c6f 7564 2063 6f6d 7075 7465 2069 6e73  loud compute ins
+00015160: 7461 6e63 6573 206c 6973 7420 270a 2020  tances list '.  
+00015170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015180: 2020 2020 2066 272d 2d66 696c 7465 723d       f'--filter=
+00015190: 2228 6c61 6265 6c73 2e72 6179 2d63 6c75  "(labels.ray-clu
+000151a0: 7374 6572 2d6e 616d 653a 7b6e 616d 657d  ster-name:{name}
+000151b0: 2922 2027 0a20 2020 2020 2020 2020 2020  )" '.           
+000151c0: 2020 2020 2020 2020 2020 2020 272d 2d66              '--f
+000151d0: 6f72 6d61 743d 2276 616c 7565 2873 7461  ormat="value(sta
+000151e0: 7475 7329 2227 290a 2020 2020 7175 6572  tus)"').    quer
+000151f0: 795f 636d 6420 3d20 2866 2767 636c 6f75  y_cmd = (f'gclou
+00015200: 6420 636f 6d70 7574 6520 696e 7374 616e  d compute instan
+00015210: 6365 7320 6c69 7374 202d 2d66 696c 7465  ces list --filte
+00015220: 723d 270a 2020 2020 2020 2020 2020 2020  r='.            
+00015230: 2020 2020 2066 2722 286c 6162 656c 732e       f'"(labels.
+00015240: 7261 792d 636c 7573 7465 722d 6e61 6d65  ray-cluster-name
+00015250: 3a7b 6e61 6d65 7d29 2220 270a 2020 2020  :{name})" '.    
+00015260: 2020 2020 2020 2020 2020 2020 2066 272d               f'-
+00015270: 2d7a 6f6e 6573 3d7b 7a6f 6e65 7d20 2d2d  -zones={zone} --
+00015280: 666f 726d 6174 3d22 7661 6c75 6528 6e61  format="value(na
+00015290: 6d65 2922 2729 0a20 2020 2074 6572 6d69  me)"').    termi
+000152a0: 6e61 7465 5f63 6d64 203d 2028 6627 6763  nate_cmd = (f'gc
+000152b0: 6c6f 7564 2063 6f6d 7075 7465 2069 6e73  loud compute ins
+000152c0: 7461 6e63 6573 2064 656c 6574 6520 2d2d  tances delete --
+000152d0: 7a6f 6e65 3d7b 7a6f 6e65 7d27 0a20 2020  zone={zone}'.   
+000152e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152f0: 2020 6627 202d 2d71 7569 6574 2024 287b    f' --quiet $({
+00015300: 7175 6572 795f 636d 647d 2927 290a 2020  query_cmd})').  
+00015310: 2020 7465 7374 203d 2054 6573 7428 0a20    test = Test(. 
+00015320: 2020 2020 2020 2027 7370 6f74 5f63 616e         'spot_can
+00015330: 6365 6c6c 6174 696f 6e5f 6763 7027 2c0a  cellation_gcp',.
+00015340: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
+00015350: 2020 2020 2020 2320 5465 7374 2063 616e        # Test can
+00015360: 6365 6c6c 6174 696f 6e20 6475 7269 6e67  cellation during
+00015370: 2073 706f 7420 636c 7573 7465 7220 6265   spot cluster be
+00015380: 696e 6720 6c61 756e 6368 6564 2e0a 2020  ing launched..  
+00015390: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+000153a0: 7370 6f74 206c 6175 6e63 6820 2d2d 636c  spot launch --cl
+000153b0: 6f75 6420 6763 7020 2d2d 7a6f 6e65 207b  oud gcp --zone {
+000153c0: 7a6f 6e65 7d20 2d6e 207b 6e61 6d65 7d20  zone} -n {name} 
+000153d0: 2273 6c65 6570 2031 3030 3022 2020 2d79  "sleep 1000"  -y
+000153e0: 202d 6427 2c0a 2020 2020 2020 2020 2020   -d',.          
+000153f0: 2020 2773 6c65 6570 2036 3027 2c0a 2020    'sleep 60',.  
+00015400: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
+00015410: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
+00015420: 6772 6570 207b 6e61 6d65 7d20 7c20 6865  grep {name} | he
+00015430: 6164 202d 6e31 207c 2067 7265 7020 2253  ad -n1 | grep "S
+00015440: 5441 5254 494e 4722 272c 0a20 2020 2020  TARTING"',.     
+00015450: 2020 2020 2020 205f 5350 4f54 5f43 414e         _SPOT_CAN
+00015460: 4345 4c5f 5741 4954 2e66 6f72 6d61 7428  CEL_WAIT.format(
+00015470: 6a6f 625f 6e61 6d65 3d6e 616d 6529 2c0a  job_name=name),.
+00015480: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
+00015490: 6570 2035 272c 0a20 2020 2020 2020 2020  ep 5',.         
+000154a0: 2020 2066 277b 5f53 504f 545f 5155 4555     f'{_SPOT_QUEU
+000154b0: 455f 5741 4954 7d7c 2067 7265 7020 7b6e  E_WAIT}| grep {n
+000154c0: 616d 657d 207c 2068 6561 6420 2d6e 3120  ame} | head -n1 
+000154d0: 7c20 6772 6570 2022 4341 4e43 454c 4c49  | grep "CANCELLI
+000154e0: 4e47 5c7c 4341 4e43 454c 4c45 4422 272c  NG\|CANCELLED"',
+000154f0: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
+00015500: 6565 7020 3132 3027 2c0a 2020 2020 2020  eep 120',.      
+00015510: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
+00015520: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
+00015530: 207b 6e61 6d65 7d20 7c20 6865 6164 202d   {name} | head -
+00015540: 6e31 207c 2067 7265 7020 2243 414e 4345  n1 | grep "CANCE
+00015550: 4c4c 4544 2227 2c0a 2020 2020 2020 2020  LLED"',.        
+00015560: 2020 2020 2320 5465 7374 2063 616e 6365      # Test cance
+00015570: 6c6c 696e 6720 7468 6520 7370 6f74 2063  lling the spot c
+00015580: 6c75 7374 6572 2064 7572 696e 6720 7370  luster during sp
+00015590: 6f74 206a 6f62 2062 6569 6e67 2073 6574  ot job being set
+000155a0: 7570 2e0a 2020 2020 2020 2020 2020 2020  up..            
+000155b0: 6627 736b 7920 7370 6f74 206c 6175 6e63  f'sky spot launc
+000155c0: 6820 2d2d 636c 6f75 6420 6763 7020 2d2d  h --cloud gcp --
+000155d0: 7a6f 6e65 207b 7a6f 6e65 7d20 2d6e 207b  zone {zone} -n {
+000155e0: 6e61 6d65 7d2d 3220 7465 7374 732f 7465  name}-2 tests/te
+000155f0: 7374 5f79 616d 6c73 2f74 6573 745f 6c6f  st_yamls/test_lo
+00015600: 6e67 5f73 6574 7570 2e79 616d 6c20 202d  ng_setup.yaml  -
+00015610: 7920 2d64 272c 0a20 2020 2020 2020 2020  y -d',.         
+00015620: 2020 2027 736c 6565 7020 3330 3027 2c0a     'sleep 300',.
+00015630: 2020 2020 2020 2020 2020 2020 5f53 504f              _SPO
+00015640: 545f 4341 4e43 454c 5f57 4149 542e 666f  T_CANCEL_WAIT.fo
+00015650: 726d 6174 286a 6f62 5f6e 616d 653d 6627  rmat(job_name=f'
+00015660: 7b6e 616d 657d 2d32 2729 2c0a 2020 2020  {name}-2'),.    
+00015670: 2020 2020 2020 2020 2773 6c65 6570 2035          'sleep 5
+00015680: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+00015690: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
+000156a0: 4954 7d7c 2067 7265 7020 7b6e 616d 657d  IT}| grep {name}
+000156b0: 2d32 207c 2068 6561 6420 2d6e 3120 7c20  -2 | head -n1 | 
+000156c0: 6772 6570 2022 4341 4e43 454c 4c49 4e47  grep "CANCELLING
+000156d0: 5c7c 4341 4e43 454c 4c45 4422 272c 0a20  \|CANCELLED"',. 
+000156e0: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
+000156f0: 7020 3132 3027 2c0a 2020 2020 2020 2020  p 120',.        
+00015700: 2020 2020 6627 7b5f 5350 4f54 5f51 5545      f'{_SPOT_QUE
+00015710: 5545 5f57 4149 547d 7c20 6772 6570 207b  UE_WAIT}| grep {
+00015720: 6e61 6d65 7d2d 3220 7c20 6865 6164 202d  name}-2 | head -
+00015730: 6e31 207c 2067 7265 7020 2243 414e 4345  n1 | grep "CANCE
+00015740: 4c4c 4544 2227 2c0a 2020 2020 2020 2020  LLED"',.        
+00015750: 2020 2020 2320 5465 7374 2063 616e 6365      # Test cance
+00015760: 6c6c 6174 696f 6e20 6475 7269 6e67 2073  llation during s
+00015770: 706f 7420 6a6f 6220 6973 2072 6563 6f76  pot job is recov
+00015780: 6572 696e 672e 0a20 2020 2020 2020 2020  ering..         
+00015790: 2020 2066 2773 6b79 2073 706f 7420 6c61     f'sky spot la
+000157a0: 756e 6368 202d 2d63 6c6f 7564 2067 6370  unch --cloud gcp
+000157b0: 202d 2d7a 6f6e 6520 7b7a 6f6e 657d 202d   --zone {zone} -
+000157c0: 6e20 7b6e 616d 657d 2d33 2022 736c 6565  n {name}-3 "slee
+000157d0: 7020 3130 3030 2220 202d 7920 2d64 272c  p 1000"  -y -d',
+000157e0: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
+000157f0: 6565 7020 3330 3027 2c0a 2020 2020 2020  eep 300',.      
+00015800: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
+00015810: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
+00015820: 207b 6e61 6d65 7d2d 3320 7c20 6865 6164   {name}-3 | head
+00015830: 202d 6e31 207c 2067 7265 7020 2252 554e   -n1 | grep "RUN
+00015840: 4e49 4e47 2227 2c0a 2020 2020 2020 2020  NING"',.        
+00015850: 2020 2020 2320 5465 726d 696e 6174 6520      # Terminate 
+00015860: 7468 6520 636c 7573 7465 7220 6d61 6e75  the cluster manu
+00015870: 616c 6c79 2e0a 2020 2020 2020 2020 2020  ally..          
+00015880: 2020 7465 726d 696e 6174 655f 636d 642c    terminate_cmd,
+00015890: 0a20 2020 2020 2020 2020 2020 2027 736c  .            'sl
+000158a0: 6565 7020 3130 3027 2c0a 2020 2020 2020  eep 100',.      
+000158b0: 2020 2020 2020 6627 7b5f 5350 4f54 5f51        f'{_SPOT_Q
+000158c0: 5545 5545 5f57 4149 547d 7c20 6772 6570  UEUE_WAIT}| grep
+000158d0: 207b 6e61 6d65 7d2d 3320 7c20 6865 6164   {name}-3 | head
+000158e0: 202d 6e31 207c 2067 7265 7020 2252 4543   -n1 | grep "REC
+000158f0: 4f56 4552 494e 4722 272c 0a20 2020 2020  OVERING"',.     
+00015900: 2020 2020 2020 205f 5350 4f54 5f43 414e         _SPOT_CAN
+00015910: 4345 4c5f 5741 4954 2e66 6f72 6d61 7428  CEL_WAIT.format(
+00015920: 6a6f 625f 6e61 6d65 3d66 277b 6e61 6d65  job_name=f'{name
+00015930: 7d2d 3327 292c 0a20 2020 2020 2020 2020  }-3'),.         
+00015940: 2020 2027 736c 6565 7020 3527 2c0a 2020     'sleep 5',.  
+00015950: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
+00015960: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
+00015970: 6772 6570 207b 6e61 6d65 7d2d 3320 7c20  grep {name}-3 | 
+00015980: 6865 6164 202d 6e31 207c 2067 7265 7020  head -n1 | grep 
+00015990: 2243 414e 4345 4c4c 494e 475c 7c43 414e  "CANCELLING\|CAN
+000159a0: 4345 4c4c 4544 2227 2c0a 2020 2020 2020  CELLED"',.      
+000159b0: 2020 2020 2020 2773 6c65 6570 2031 3230        'sleep 120
+000159c0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+000159d0: 277b 5f53 504f 545f 5155 4555 455f 5741  '{_SPOT_QUEUE_WA
+000159e0: 4954 7d7c 2067 7265 7020 7b6e 616d 657d  IT}| grep {name}
+000159f0: 2d33 207c 2068 6561 6420 2d6e 3120 7c20  -3 | head -n1 | 
+00015a00: 6772 6570 2022 4341 4e43 454c 4c45 4422  grep "CANCELLED"
+00015a10: 272c 0a20 2020 2020 2020 2020 2020 2023  ',.            #
+00015a20: 2054 6865 2063 6c75 7374 6572 2073 686f   The cluster sho
+00015a30: 756c 6420 6265 2074 6572 6d69 6e61 7465  uld be terminate
+00015a40: 6420 2853 544f 5050 494e 4729 2061 6674  d (STOPPING) aft
+00015a50: 6572 2063 616e 6365 6c6c 6174 696f 6e2e  er cancellation.
+00015a60: 2057 6520 646f 6e27 7420 7573 6520 7468   We don't use th
+00015a70: 6520 603d 6020 6f70 6572 6174 6f72 2068  e `=` operator h
+00015a80: 6572 6520 6265 6361 7573 650a 2020 2020  ere because.    
+00015a90: 2020 2020 2020 2020 2320 7468 6572 6520          # there 
+00015aa0: 6361 6e20 6265 206d 756c 7469 706c 6520  can be multiple 
+00015ab0: 564d 2077 6974 6820 7468 6520 7361 6d65  VM with the same
+00015ac0: 206e 616d 6520 6475 6520 746f 2074 6865   name due to the
+00015ad0: 2072 6563 6f76 6572 792e 0a20 2020 2020   recovery..     
+00015ae0: 2020 2020 2020 2028 6627 733d 2428 7b71         (f's=$({q
+00015af0: 7565 7279 5f73 7461 7465 5f63 6d64 7d29  uery_state_cmd})
+00015b00: 2026 2620 6563 686f 2022 2473 2220 2626   && echo "$s" &&
+00015b10: 2065 6368 6f3b 205b 5b20 2d7a 2022 2473   echo; [[ -z "$s
+00015b20: 2220 5d5d 207c 7c20 6563 686f 2022 2473  " ]] || echo "$s
+00015b30: 2220 7c20 6772 6570 202d 7620 2d45 2022  " | grep -v -E "
+00015b40: 5052 4f56 4953 494f 4e49 4e47 7c53 5441  PROVISIONING|STA
+00015b50: 4749 4e47 7c52 554e 4e49 4e47 7c52 4550  GING|RUNNING|REP
+00015b60: 4149 5249 4e47 7c54 4552 4d49 4e41 5445  AIRING|TERMINATE
+00015b70: 447c 5355 5350 454e 4449 4e47 7c53 5553  D|SUSPENDING|SUS
+00015b80: 5045 4e44 4544 7c53 5553 5045 4e44 4544  PENDED|SUSPENDED
+00015b90: 2227 0a20 2020 2020 2020 2020 2020 2029  "'.            )
+00015ba0: 2c0a 2020 2020 2020 2020 5d2c 0a20 2020  ,.        ],.   
+00015bb0: 2020 2020 2074 696d 656f 7574 3d32 3520       timeout=25 
+00015bc0: 2a20 3630 290a 2020 2020 7275 6e5f 6f6e  * 60).    run_on
+00015bd0: 655f 7465 7374 2874 6573 7429 0a0a 0a23  e_test(test)...#
+00015be0: 202d 2d2d 2d2d 2d2d 2d2d 2d20 5465 7374   ---------- Test
+00015bf0: 696e 6720 7374 6f72 6167 6520 666f 7220  ing storage for 
+00015c00: 6d61 6e61 6765 6420 7370 6f74 202d 2d2d  managed spot ---
+00015c10: 2d2d 2d2d 2d2d 2d0a 4070 7974 6573 742e  -------.@pytest.
+00015c20: 6d61 726b 2e6e 6f5f 6c61 6d62 6461 5f63  mark.no_lambda_c
+00015c30: 6c6f 7564 2020 2320 4c61 6d62 6461 2043  loud  # Lambda C
+00015c40: 6c6f 7564 2064 6f65 7320 6e6f 7420 7375  loud does not su
+00015c50: 7070 6f72 7420 7370 6f74 2069 6e73 7461  pport spot insta
+00015c60: 6e63 6573 0a40 7079 7465 7374 2e6d 6172  nces.@pytest.mar
+00015c70: 6b2e 6e6f 5f69 626d 2020 2320 4942 4d20  k.no_ibm  # IBM 
+00015c80: 436c 6f75 6420 646f 6573 206e 6f74 2073  Cloud does not s
+00015c90: 7570 706f 7274 2073 706f 7420 696e 7374  upport spot inst
+00015ca0: 616e 6365 730a 4070 7974 6573 742e 6d61  ances.@pytest.ma
+00015cb0: 726b 2e6e 6f5f 7363 7020 2023 2053 4350  rk.no_scp  # SCP
+00015cc0: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
+00015cd0: 7420 7370 6f74 2069 6e73 7461 6e63 6573  t spot instances
+00015ce0: 0a40 7079 7465 7374 2e6d 6172 6b2e 6d61  .@pytest.mark.ma
+00015cf0: 6e61 6765 645f 7370 6f74 0a64 6566 2074  naged_spot.def t
+00015d00: 6573 745f 7370 6f74 5f73 746f 7261 6765  est_spot_storage
+00015d10: 2867 656e 6572 6963 5f63 6c6f 7564 3a20  (generic_cloud: 
+00015d20: 7374 7229 3a0a 2020 2020 2222 2254 6573  str):.    """Tes
+00015d30: 7420 7374 6f72 6167 6520 7769 7468 206d  t storage with m
+00015d40: 616e 6167 6564 2073 706f 7422 2222 0a20  anaged spot""". 
+00015d50: 2020 206e 616d 6520 3d20 5f67 6574 5f63     name = _get_c
+00015d60: 6c75 7374 6572 5f6e 616d 6528 290a 2020  luster_name().  
+00015d70: 2020 7961 6d6c 5f73 7472 203d 2070 6174    yaml_str = pat
+00015d80: 686c 6962 2e50 6174 6828 0a20 2020 2020  hlib.Path(.     
+00015d90: 2020 2027 6578 616d 706c 6573 2f6d 616e     'examples/man
+00015da0: 6167 6564 5f73 706f 745f 7769 7468 5f73  aged_spot_with_s
+00015db0: 746f 7261 6765 2e79 616d 6c27 292e 7265  torage.yaml').re
+00015dc0: 6164 5f74 6578 7428 290a 2020 2020 7374  ad_text().    st
+00015dd0: 6f72 6167 655f 6e61 6d65 203d 2066 2773  orage_name = f's
+00015de0: 6b79 2d74 6573 742d 7b69 6e74 2874 696d  ky-test-{int(tim
+00015df0: 652e 7469 6d65 2829 297d 270a 2020 2020  e.time())}'.    
+00015e00: 7961 6d6c 5f73 7472 203d 2079 616d 6c5f  yaml_str = yaml_
+00015e10: 7374 722e 7265 706c 6163 6528 2773 6b79  str.replace('sky
+00015e20: 2d77 6f72 6b64 6972 2d7a 6877 7527 2c20  -workdir-zhwu', 
+00015e30: 7374 6f72 6167 655f 6e61 6d65 290a 2020  storage_name).  
+00015e40: 2020 7769 7468 2074 656d 7066 696c 652e    with tempfile.
+00015e50: 4e61 6d65 6454 656d 706f 7261 7279 4669  NamedTemporaryFi
+00015e60: 6c65 2873 7566 6669 783d 272e 7961 6d6c  le(suffix='.yaml
+00015e70: 272c 206d 6f64 653d 2777 2729 2061 7320  ', mode='w') as 
+00015e80: 663a 0a20 2020 2020 2020 2066 2e77 7269  f:.        f.wri
+00015e90: 7465 2879 616d 6c5f 7374 7229 0a20 2020  te(yaml_str).   
+00015ea0: 2020 2020 2066 2e66 6c75 7368 2829 0a20       f.flush(). 
+00015eb0: 2020 2020 2020 2066 696c 655f 7061 7468         file_path
+00015ec0: 203d 2066 2e6e 616d 650a 2020 2020 2020   = f.name.      
+00015ed0: 2020 7465 7374 203d 2054 6573 7428 0a20    test = Test(. 
+00015ee0: 2020 2020 2020 2020 2020 2027 7370 6f74             'spot
+00015ef0: 5f73 746f 7261 6765 272c 0a20 2020 2020  _storage',.     
+00015f00: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00015f10: 2020 2020 2020 2020 202a 7374 6f72 6167           *storag
+00015f20: 655f 7365 7475 705f 636f 6d6d 616e 6473  e_setup_commands
+00015f30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00015f40: 2020 6627 736b 7920 7370 6f74 206c 6175    f'sky spot lau
+00015f50: 6e63 6820 2d6e 207b 6e61 6d65 7d20 2d2d  nch -n {name} --
+00015f60: 636c 6f75 6420 7b67 656e 6572 6963 5f63  cloud {generic_c
+00015f70: 6c6f 7564 7d20 7b66 696c 655f 7061 7468  loud} {file_path
+00015f80: 7d20 2d79 272c 0a20 2020 2020 2020 2020  } -y',.         
+00015f90: 2020 2020 2020 2027 736c 6565 7020 3630         'sleep 60
+00015fa0: 272c 2020 2320 5761 6974 2074 6865 2073  ',  # Wait the s
+00015fb0: 706f 7420 7175 6575 6520 746f 2062 6520  pot queue to be 
+00015fc0: 7570 6461 7465 640a 2020 2020 2020 2020  updated.        
+00015fd0: 2020 2020 2020 2020 6627 7b5f 5350 4f54          f'{_SPOT
+00015fe0: 5f51 5545 5545 5f57 4149 547d 7c20 6772  _QUEUE_WAIT}| gr
+00015ff0: 6570 207b 6e61 6d65 7d20 7c20 6772 6570  ep {name} | grep
+00016000: 2053 5543 4345 4544 4544 272c 0a20 2020   SUCCEEDED',.   
+00016010: 2020 2020 2020 2020 2020 2020 2066 275b               f'[
+00016020: 2024 2861 7773 2073 3361 7069 206c 6973   $(aws s3api lis
+00016030: 742d 6275 636b 6574 7320 2d2d 7175 6572  t-buckets --quer
+00016040: 7920 2242 7563 6b65 7473 5b3f 636f 6e74  y "Buckets[?cont
+00016050: 6169 6e73 284e 616d 652c 205c 277b 7374  ains(Name, \'{st
+00016060: 6f72 6167 655f 6e61 6d65 7d5c 2729 5d2e  orage_name}\')].
+00016070: 4e61 6d65 2220 2d2d 6f75 7470 7574 2074  Name" --output t
+00016080: 6578 7420 7c20 7763 202d 6c29 202d 6571  ext | wc -l) -eq
+00016090: 2030 205d 270a 2020 2020 2020 2020 2020   0 ]'.          
+000160a0: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
+000160b0: 205f 5350 4f54 5f43 414e 4345 4c5f 5741   _SPOT_CANCEL_WA
+000160c0: 4954 2e66 6f72 6d61 7428 6a6f 625f 6e61  IT.format(job_na
+000160d0: 6d65 3d6e 616d 6529 2c0a 2020 2020 2020  me=name),.      
+000160e0: 2020 2020 2020 2320 496e 6372 6561 7365        # Increase
+000160f0: 2074 696d 656f 7574 2073 696e 6365 2073   timeout since s
+00016100: 6b79 2073 706f 7420 7175 6575 6520 2d72  ky spot queue -r
+00016110: 2063 616e 2062 6520 626c 6f63 6b65 6420   can be blocked 
+00016120: 6279 206f 7468 6572 2073 706f 7420 7465  by other spot te
+00016130: 7374 732e 0a20 2020 2020 2020 2020 2020  sts..           
+00016140: 2074 696d 656f 7574 3d32 3020 2a20 3630   timeout=20 * 60
+00016150: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00016160: 2020 2020 7275 6e5f 6f6e 655f 7465 7374      run_one_test
+00016170: 2874 6573 7429 0a0a 0a23 202d 2d2d 2d2d  (test)...# -----
+00016180: 2d2d 2d2d 2d20 5465 7374 696e 6720 7370  ----- Testing sp
+00016190: 6f74 2054 5055 202d 2d2d 2d2d 2d2d 2d2d  ot TPU ---------
+000161a0: 2d0a 4070 7974 6573 742e 6d61 726b 2e67  -.@pytest.mark.g
+000161b0: 6370 0a40 7079 7465 7374 2e6d 6172 6b2e  cp.@pytest.mark.
+000161c0: 6d61 6e61 6765 645f 7370 6f74 0a64 6566  managed_spot.def
+000161d0: 2074 6573 745f 7370 6f74 5f74 7075 2829   test_spot_tpu()
+000161e0: 3a0a 2020 2020 2222 2254 6573 7420 6d61  :.    """Test ma
+000161f0: 6e61 6765 6420 7370 6f74 206f 6e20 5450  naged spot on TP
+00016200: 552e 2222 220a 2020 2020 6e61 6d65 203d  U.""".    name =
+00016210: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
+00016220: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
+00016230: 5465 7374 280a 2020 2020 2020 2020 2774  Test(.        't
+00016240: 6573 742d 7370 6f74 2d74 7075 272c 0a20  est-spot-tpu',. 
+00016250: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00016260: 2020 2020 2066 2773 6b79 2073 706f 7420       f'sky spot 
+00016270: 6c61 756e 6368 202d 6e20 7b6e 616d 657d  launch -n {name}
+00016280: 2065 7861 6d70 6c65 732f 7470 752f 7470   examples/tpu/tp
+00016290: 7576 6d5f 6d6e 6973 742e 7961 6d6c 202d  uvm_mnist.yaml -
+000162a0: 7920 2d64 272c 0a20 2020 2020 2020 2020  y -d',.         
+000162b0: 2020 2027 736c 6565 7020 3527 2c0a 2020     'sleep 5',.  
+000162c0: 2020 2020 2020 2020 2020 6627 7b5f 5350            f'{_SP
+000162d0: 4f54 5f51 5545 5545 5f57 4149 547d 7c20  OT_QUEUE_WAIT}| 
+000162e0: 6772 6570 207b 6e61 6d65 7d20 7c20 6865  grep {name} | he
+000162f0: 6164 202d 6e31 207c 2067 7265 7020 5354  ad -n1 | grep ST
+00016300: 4152 5449 4e47 272c 0a20 2020 2020 2020  ARTING',.       
+00016310: 2020 2020 2027 736c 6565 7020 3732 3027       'sleep 720'
+00016320: 2c20 2023 2054 5055 2074 616b 6573 2061  ,  # TPU takes a
+00016330: 2077 6869 6c65 2074 6f20 6c61 756e 6368   while to launch
+00016340: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
+00016350: 5f53 504f 545f 5155 4555 455f 5741 4954  _SPOT_QUEUE_WAIT
+00016360: 7d7c 2067 7265 7020 7b6e 616d 657d 207c  }| grep {name} |
+00016370: 2068 6561 6420 2d6e 3120 7c20 6772 6570   head -n1 | grep
+00016380: 2022 5255 4e4e 494e 475c 7c53 5543 4345   "RUNNING\|SUCCE
+00016390: 4544 4544 2227 2c0a 2020 2020 2020 2020  EDED"',.        
+000163a0: 5d2c 0a20 2020 2020 2020 205f 5350 4f54  ],.        _SPOT
+000163b0: 5f43 414e 4345 4c5f 5741 4954 2e66 6f72  _CANCEL_WAIT.for
+000163c0: 6d61 7428 6a6f 625f 6e61 6d65 3d6e 616d  mat(job_name=nam
+000163d0: 6529 2c0a 2020 2020 2020 2020 2320 496e  e),.        # In
+000163e0: 6372 6561 7365 2074 696d 656f 7574 2073  crease timeout s
+000163f0: 696e 6365 2073 6b79 2073 706f 7420 7175  ince sky spot qu
+00016400: 6575 6520 2d72 2063 616e 2062 6520 626c  eue -r can be bl
+00016410: 6f63 6b65 6420 6279 206f 7468 6572 2073  ocked by other s
+00016420: 706f 7420 7465 7374 732e 0a20 2020 2020  pot tests..     
+00016430: 2020 2074 696d 656f 7574 3d32 3020 2a20     timeout=20 * 
+00016440: 3630 2c0a 2020 2020 290a 2020 2020 7275  60,.    ).    ru
+00016450: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
+00016460: 0a0a 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d20  ...# ---------- 
+00016470: 5465 7374 696e 6720 656e 7620 666f 7220  Testing env for 
+00016480: 7370 6f74 202d 2d2d 2d2d 2d2d 2d2d 2d0a  spot ----------.
+00016490: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
+000164a0: 6c61 6d62 6461 5f63 6c6f 7564 2020 2320  lambda_cloud  # 
+000164b0: 4c61 6d62 6461 2043 6c6f 7564 2064 6f65  Lambda Cloud doe
+000164c0: 7320 6e6f 7420 7375 7070 6f72 7420 7370  s not support sp
+000164d0: 6f74 2069 6e73 7461 6e63 6573 0a40 7079  ot instances.@py
+000164e0: 7465 7374 2e6d 6172 6b2e 6e6f 5f69 626d  test.mark.no_ibm
+000164f0: 2020 2320 4942 4d20 436c 6f75 6420 646f    # IBM Cloud do
+00016500: 6573 206e 6f74 2073 7570 706f 7274 2073  es not support s
+00016510: 706f 7420 696e 7374 616e 6365 730a 4070  pot instances.@p
+00016520: 7974 6573 742e 6d61 726b 2e6e 6f5f 7363  ytest.mark.no_sc
+00016530: 7020 2023 2053 4350 2064 6f65 7320 6e6f  p  # SCP does no
+00016540: 7420 7375 7070 6f72 7420 7370 6f74 2069  t support spot i
+00016550: 6e73 7461 6e63 6573 0a40 7079 7465 7374  nstances.@pytest
+00016560: 2e6d 6172 6b2e 6d61 6e61 6765 645f 7370  .mark.managed_sp
+00016570: 6f74 0a64 6566 2074 6573 745f 7370 6f74  ot.def test_spot
+00016580: 5f69 6e6c 696e 655f 656e 7628 6765 6e65  _inline_env(gene
+00016590: 7269 635f 636c 6f75 643a 2073 7472 293a  ric_cloud: str):
+000165a0: 0a20 2020 2022 2222 5465 7374 2073 706f  .    """Test spo
+000165b0: 7420 656e 7622 2222 0a20 2020 206e 616d  t env""".    nam
+000165c0: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
+000165d0: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
+000165e0: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
+000165f0: 2027 7465 7374 2d73 706f 742d 696e 6c69   'test-spot-inli
+00016600: 6e65 2d65 6e76 272c 0a20 2020 2020 2020  ne-env',.       
+00016610: 205b 0a20 2020 2020 2020 2020 2020 2066   [.            f
+00016620: 2773 6b79 2073 706f 7420 6c61 756e 6368  'sky spot launch
+00016630: 202d 6e20 7b6e 616d 657d 202d 7920 2d2d   -n {name} -y --
+00016640: 636c 6f75 6420 7b67 656e 6572 6963 5f63  cloud {generic_c
+00016650: 6c6f 7564 7d20 2d2d 656e 7620 5445 5354  loud} --env TEST
+00016660: 5f45 4e56 3d22 6865 6c6c 6f20 776f 726c  _ENV="hello worl
+00016670: 6422 202d 2d20 2228 5b5b 2021 202d 7a20  d" -- "([[ ! -z 
+00016680: 5c5c 225c 2454 4553 545f 454e 565c 5c22  \\"\$TEST_ENV\\"
+00016690: 205d 5d20 2626 205b 5b20 2120 2d7a 205c   ]] && [[ ! -z \
+000166a0: 5c22 5c24 534b 5950 494c 4f54 5f4e 4f44  \"\$SKYPILOT_NOD
+000166b0: 455f 4950 535c 5c22 205d 5d20 2626 205b  E_IPS\\" ]] && [
+000166c0: 5b20 2120 2d7a 205c 5c22 5c24 534b 5950  [ ! -z \\"\$SKYP
+000166d0: 494c 4f54 5f4e 4f44 455f 5241 4e4b 5c5c  ILOT_NODE_RANK\\
+000166e0: 2220 5d5d 2920 7c7c 2065 7869 7420 3122  " ]]) || exit 1"
+000166f0: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+00016700: 736c 6565 7020 3230 272c 0a20 2020 2020  sleep 20',.     
+00016710: 2020 2020 2020 2066 277b 5f53 504f 545f         f'{_SPOT_
+00016720: 5155 4555 455f 5741 4954 7d20 7c20 6772  QUEUE_WAIT} | gr
+00016730: 6570 207b 6e61 6d65 7d20 7c20 6772 6570  ep {name} | grep
+00016740: 2053 5543 4345 4544 4544 272c 0a20 2020   SUCCEEDED',.   
+00016750: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00016760: 5f53 504f 545f 4341 4e43 454c 5f57 4149  _SPOT_CANCEL_WAI
+00016770: 542e 666f 726d 6174 286a 6f62 5f6e 616d  T.format(job_nam
+00016780: 653d 6e61 6d65 292c 0a20 2020 2020 2020  e=name),.       
+00016790: 2023 2049 6e63 7265 6173 6520 7469 6d65   # Increase time
+000167a0: 6f75 7420 7369 6e63 6520 736b 7920 7370  out since sky sp
+000167b0: 6f74 2071 7565 7565 202d 7220 6361 6e20  ot queue -r can 
+000167c0: 6265 2062 6c6f 636b 6564 2062 7920 6f74  be blocked by ot
+000167d0: 6865 7220 7370 6f74 2074 6573 7473 2e0a  her spot tests..
+000167e0: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
+000167f0: 3230 202a 2036 302c 0a20 2020 2029 0a20  20 * 60,.    ). 
+00016800: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+00016810: 7465 7374 290a 0a0a 2320 2d2d 2d2d 2d2d  test)...# ------
+00016820: 2d2d 2d2d 2054 6573 7469 6e67 2065 6e76  ---- Testing env
+00016830: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 6465 6620   ----------.def 
+00016840: 7465 7374 5f69 6e6c 696e 655f 656e 7628  test_inline_env(
+00016850: 6765 6e65 7269 635f 636c 6f75 643a 2073  generic_cloud: s
+00016860: 7472 293a 0a20 2020 2022 2222 5465 7374  tr):.    """Test
+00016870: 2065 6e76 2222 220a 2020 2020 6e61 6d65   env""".    name
+00016880: 203d 205f 6765 745f 636c 7573 7465 725f   = _get_cluster_
+00016890: 6e61 6d65 2829 0a20 2020 2074 6573 7420  name().    test 
+000168a0: 3d20 5465 7374 280a 2020 2020 2020 2020  = Test(.        
+000168b0: 2774 6573 742d 696e 6c69 6e65 2d65 6e76  'test-inline-env
+000168c0: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
+000168d0: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
+000168e0: 6175 6e63 6820 2d63 207b 6e61 6d65 7d20  aunch -c {name} 
+000168f0: 2d79 202d 2d63 6c6f 7564 207b 6765 6e65  -y --cloud {gene
+00016900: 7269 635f 636c 6f75 647d 202d 2d65 6e76  ric_cloud} --env
+00016910: 2054 4553 545f 454e 563d 2268 656c 6c6f   TEST_ENV="hello
+00016920: 2077 6f72 6c64 2220 2d2d 2022 285b 5b20   world" -- "([[ 
+00016930: 2120 2d7a 205c 5c22 5c24 5445 5354 5f45  ! -z \\"\$TEST_E
+00016940: 4e56 5c5c 2220 5d5d 2026 2620 5b5b 2021  NV\\" ]] && [[ !
+00016950: 202d 7a20 5c5c 225c 2453 4b59 5049 4c4f   -z \\"\$SKYPILO
+00016960: 545f 4e4f 4445 5f49 5053 5c5c 2220 5d5d  T_NODE_IPS\\" ]]
+00016970: 2026 2620 5b5b 2021 202d 7a20 5c5c 225c   && [[ ! -z \\"\
+00016980: 2453 4b59 5049 4c4f 545f 4e4f 4445 5f52  $SKYPILOT_NODE_R
+00016990: 414e 4b5c 5c22 205d 5d29 207c 7c20 6578  ANK\\" ]]) || ex
+000169a0: 6974 2031 2227 2c0a 2020 2020 2020 2020  it 1"',.        
+000169b0: 2020 2020 6627 736b 7920 6c6f 6773 207b      f'sky logs {
+000169c0: 6e61 6d65 7d20 3120 2d2d 7374 6174 7573  name} 1 --status
+000169d0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+000169e0: 2773 6b79 2065 7865 6320 7b6e 616d 657d  'sky exec {name}
+000169f0: 202d 2d65 6e76 2054 4553 545f 454e 5632   --env TEST_ENV2
+00016a00: 3d22 7375 6363 6573 7322 2022 285b 5b20  ="success" "([[ 
+00016a10: 2120 2d7a 205c 5c22 5c24 5445 5354 5f45  ! -z \\"\$TEST_E
+00016a20: 4e56 325c 5c22 205d 5d20 2626 205b 5b20  NV2\\" ]] && [[ 
+00016a30: 2120 2d7a 205c 5c22 5c24 534b 5950 494c  ! -z \\"\$SKYPIL
+00016a40: 4f54 5f4e 4f44 455f 4950 535c 5c22 205d  OT_NODE_IPS\\" ]
+00016a50: 5d20 2626 205b 5b20 2120 2d7a 205c 5c22  ] && [[ ! -z \\"
+00016a60: 5c24 534b 5950 494c 4f54 5f4e 4f44 455f  \$SKYPILOT_NODE_
+00016a70: 5241 4e4b 5c5c 2220 5d5d 2920 7c7c 2065  RANK\\" ]]) || e
+00016a80: 7869 7420 3122 272c 0a20 2020 2020 2020  xit 1"',.       
+00016a90: 2020 2020 2066 2773 6b79 206c 6f67 7320       f'sky logs 
+00016aa0: 7b6e 616d 657d 2032 202d 2d73 7461 7475  {name} 2 --statu
+00016ab0: 7327 2c0a 2020 2020 2020 2020 5d2c 0a20  s',.        ],. 
+00016ac0: 2020 2020 2020 2066 2773 6b79 2064 6f77         f'sky dow
+00016ad0: 6e20 2d79 207b 6e61 6d65 7d27 2c0a 2020  n -y {name}',.  
+00016ae0: 2020 290a 2020 2020 7275 6e5f 6f6e 655f    ).    run_one_
+00016af0: 7465 7374 2874 6573 7429 0a0a 0a23 202d  test(test)...# -
+00016b00: 2d2d 2d2d 2d2d 2d2d 2d20 5465 7374 696e  --------- Testin
+00016b10: 6720 6375 7374 6f6d 2069 6d61 6765 202d  g custom image -
+00016b20: 2d2d 2d2d 2d2d 2d2d 2d0a 4070 7974 6573  ---------.@pytes
+00016b30: 742e 6d61 726b 2e61 7773 0a64 6566 2074  t.mark.aws.def t
+00016b40: 6573 745f 6375 7374 6f6d 5f69 6d61 6765  est_custom_image
+00016b50: 2829 3a0a 2020 2020 2222 2254 6573 7420  ():.    """Test 
+00016b60: 6375 7374 6f6d 2069 6d61 6765 2222 220a  custom image""".
+00016b70: 2020 2020 6e61 6d65 203d 205f 6765 745f      name = _get_
+00016b80: 636c 7573 7465 725f 6e61 6d65 2829 0a20  cluster_name(). 
+00016b90: 2020 2074 6573 7420 3d20 5465 7374 280a     test = Test(.
+00016ba0: 2020 2020 2020 2020 2774 6573 742d 6375          'test-cu
+00016bb0: 7374 6f6d 2d69 6d61 6765 272c 0a20 2020  stom-image',.   
+00016bc0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+00016bd0: 2020 2066 2773 6b79 206c 6175 6e63 6820     f'sky launch 
+00016be0: 2d63 207b 6e61 6d65 7d20 2d2d 7265 7472  -c {name} --retr
+00016bf0: 792d 756e 7469 6c2d 7570 202d 7920 6578  y-until-up -y ex
+00016c00: 616d 706c 6573 2f63 7573 746f 6d5f 696d  amples/custom_im
+00016c10: 6167 652e 7961 6d6c 272c 0a20 2020 2020  age.yaml',.     
+00016c20: 2020 2020 2020 2066 2773 6b79 206c 6f67         f'sky log
+00016c30: 7320 7b6e 616d 657d 2031 202d 2d73 7461  s {name} 1 --sta
+00016c40: 7475 7327 2c0a 2020 2020 2020 2020 5d2c  tus',.        ],
+00016c50: 0a20 2020 2020 2020 2066 2773 6b79 2064  .        f'sky d
+00016c60: 6f77 6e20 2d79 207b 6e61 6d65 7d27 2c0a  own -y {name}',.
+00016c70: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
+00016c80: 3330 202a 2036 302c 0a20 2020 2029 0a20  30 * 60,.    ). 
+00016c90: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+00016ca0: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
+00016cb0: 6d61 726b 2e73 6c6f 770a 6465 6620 7465  mark.slow.def te
+00016cc0: 7374 5f61 7a75 7265 5f73 7461 7274 5f73  st_azure_start_s
+00016cd0: 746f 705f 7477 6f5f 6e6f 6465 7328 293a  top_two_nodes():
+00016ce0: 0a20 2020 206e 616d 6520 3d20 5f67 6574  .    name = _get
+00016cf0: 5f63 6c75 7374 6572 5f6e 616d 6528 290a  _cluster_name().
+00016d00: 2020 2020 7465 7374 203d 2054 6573 7428      test = Test(
+00016d10: 0a20 2020 2020 2020 2027 617a 7572 652d  .        'azure-
+00016d20: 7374 6172 742d 7374 6f70 2d74 776f 2d6e  start-stop-two-n
+00016d30: 6f64 6573 272c 0a20 2020 2020 2020 205b  odes',.        [
+00016d40: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+00016d50: 6b79 206c 6175 6e63 6820 2d2d 6e75 6d2d  ky launch --num-
+00016d60: 6e6f 6465 733d 3220 2d79 202d 6320 7b6e  nodes=2 -y -c {n
+00016d70: 616d 657d 2065 7861 6d70 6c65 732f 617a  ame} examples/az
+00016d80: 7572 655f 7374 6172 745f 7374 6f70 2e79  ure_start_stop.y
+00016d90: 616d 6c27 2c0a 2020 2020 2020 2020 2020  aml',.          
+00016da0: 2020 6627 736b 7920 6578 6563 202d 2d6e    f'sky exec --n
+00016db0: 756d 2d6e 6f64 6573 3d32 207b 6e61 6d65  um-nodes=2 {name
+00016dc0: 7d20 6578 616d 706c 6573 2f61 7a75 7265  } examples/azure
+00016dd0: 5f73 7461 7274 5f73 746f 702e 7961 6d6c  _start_stop.yaml
+00016de0: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+00016df0: 2773 6b79 206c 6f67 7320 7b6e 616d 657d  'sky logs {name}
+00016e00: 2031 202d 2d73 7461 7475 7327 2c20 2023   1 --status',  #
+00016e10: 2045 6e73 7572 6520 7468 6520 6a6f 6220   Ensure the job 
+00016e20: 7375 6363 6565 6465 642e 0a20 2020 2020  succeeded..     
+00016e30: 2020 2020 2020 2066 2773 6b79 2073 746f         f'sky sto
+00016e40: 7020 2d79 207b 6e61 6d65 7d27 2c0a 2020  p -y {name}',.  
 00016e50: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-00016e60: 6578 6563 202d 2d6e 756d 2d6e 6f64 6573  exec --num-nodes
-00016e70: 3d32 207b 6e61 6d65 7d20 6578 616d 706c  =2 {name} exampl
-00016e80: 6573 2f61 7a75 7265 5f73 7461 7274 5f73  es/azure_start_s
-00016e90: 746f 702e 7961 6d6c 272c 0a20 2020 2020  top.yaml',.     
-00016ea0: 2020 2020 2020 2066 2773 6b79 206c 6f67         f'sky log
-00016eb0: 7320 7b6e 616d 657d 2032 202d 2d73 7461  s {name} 2 --sta
-00016ec0: 7475 7327 2c20 2023 2045 6e73 7572 6520  tus',  # Ensure 
-00016ed0: 7468 6520 6a6f 6220 7375 6363 6565 6465  the job succeede
-00016ee0: 642e 0a20 2020 2020 2020 205d 2c0a 2020  d..        ],.  
-00016ef0: 2020 2020 2020 6627 736b 7920 646f 776e        f'sky down
-00016f00: 202d 7920 7b6e 616d 657d 272c 0a20 2020   -y {name}',.   
-00016f10: 2020 2020 2074 696d 656f 7574 3d33 3020       timeout=30 
-00016f20: 2a20 3630 2c20 2023 2033 3020 6d69 6e73  * 60,  # 30 mins
-00016f30: 2020 2869 7420 7461 6b65 7320 6172 6f75    (it takes arou
-00016f40: 6e64 207e 3233 206d 696e 7329 0a20 2020  nd ~23 mins).   
-00016f50: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
-00016f60: 6573 7428 7465 7374 290a 0a0a 2320 2d2d  est(test)...# --
-00016f70: 2d2d 2d2d 2d2d 2d2d 2054 6573 7469 6e67  -------- Testing
-00016f80: 2065 6e76 2066 6f72 2064 6973 6b20 7469   env for disk ti
-00016f90: 6572 202d 2d2d 2d2d 2d2d 2d2d 2d0a 4070  er ----------.@p
-00016fa0: 7974 6573 742e 6d61 726b 2e61 7773 0a64  ytest.mark.aws.d
-00016fb0: 6566 2074 6573 745f 6177 735f 6469 736b  ef test_aws_disk
-00016fc0: 5f74 6965 7228 293a 0a0a 2020 2020 6465  _tier():..    de
-00016fd0: 6620 5f67 6574 5f61 7773 5f71 7565 7279  f _get_aws_query
-00016fe0: 5f63 6f6d 6d61 6e64 2872 6567 696f 6e2c  _command(region,
-00016ff0: 2069 6e73 7461 6e63 655f 6964 2c20 6669   instance_id, fi
-00017000: 656c 642c 2065 7870 6563 7465 6429 3a0a  eld, expected):.
-00017010: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-00017020: 6627 6177 7320 6563 3220 6465 7363 7269  f'aws ec2 descri
-00017030: 6265 2d76 6f6c 756d 6573 202d 2d72 6567  be-volumes --reg
-00017040: 696f 6e20 7b72 6567 696f 6e7d 2027 0a20  ion {region} '. 
-00017050: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00017060: 272d 2d66 696c 7465 7273 204e 616d 653d  '--filters Name=
-00017070: 6174 7461 6368 6d65 6e74 2e69 6e73 7461  attachment.insta
-00017080: 6e63 652d 6964 2c56 616c 7565 733d 7b69  nce-id,Values={i
-00017090: 6e73 7461 6e63 655f 6964 7d20 270a 2020  nstance_id} '.  
-000170a0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-000170b0: 2d2d 7175 6572 7920 566f 6c75 6d65 735b  --query Volumes[
-000170c0: 2a5d 2e7b 6669 656c 647d 207c 2067 7265  *].{field} | gre
-000170d0: 7020 7b65 7870 6563 7465 647d 203b 2027  p {expected} ; '
-000170e0: 290a 0a20 2020 2066 6f72 2064 6973 6b5f  )..    for disk_
-000170f0: 7469 6572 2069 6e20 5b27 6c6f 7727 2c20  tier in ['low', 
-00017100: 276d 6564 6975 6d27 2c20 2768 6967 6827  'medium', 'high'
-00017110: 5d3a 0a20 2020 2020 2020 2073 7065 6373  ]:.        specs
-00017120: 203d 2041 5753 2e5f 6765 745f 6469 736b   = AWS._get_disk
-00017130: 5f73 7065 6373 2864 6973 6b5f 7469 6572  _specs(disk_tier
-00017140: 290a 2020 2020 2020 2020 6e61 6d65 203d  ).        name =
-00017150: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
-00017160: 6d65 2829 202b 2027 2d27 202b 2064 6973  me() + '-' + dis
-00017170: 6b5f 7469 6572 0a20 2020 2020 2020 2072  k_tier.        r
-00017180: 6567 696f 6e20 3d20 2775 732d 7765 7374  egion = 'us-west
-00017190: 2d32 270a 2020 2020 2020 2020 7465 7374  -2'.        test
-000171a0: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
-000171b0: 2020 2020 2027 6177 732d 6469 736b 2d74       'aws-disk-t
-000171c0: 6965 7227 2c0a 2020 2020 2020 2020 2020  ier',.          
-000171d0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-000171e0: 2020 2020 6627 736b 7920 6c61 756e 6368      f'sky launch
-000171f0: 202d 7920 2d63 207b 6e61 6d65 7d20 2d2d   -y -c {name} --
-00017200: 636c 6f75 6420 6177 7320 2d2d 7265 6769  cloud aws --regi
-00017210: 6f6e 207b 7265 6769 6f6e 7d20 270a 2020  on {region} '.  
-00017220: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-00017230: 2d2d 6469 736b 2d74 6965 7220 7b64 6973  --disk-tier {dis
-00017240: 6b5f 7469 6572 7d20 6563 686f 2022 6865  k_tier} echo "he
-00017250: 6c6c 6f20 736b 7922 272c 0a20 2020 2020  llo sky"',.     
-00017260: 2020 2020 2020 2020 2020 2066 2769 643d             f'id=
-00017270: 6061 7773 2065 6332 2064 6573 6372 6962  `aws ec2 describ
-00017280: 652d 696e 7374 616e 6365 7320 2d2d 7265  e-instances --re
-00017290: 6769 6f6e 207b 7265 6769 6f6e 7d20 2d2d  gion {region} --
-000172a0: 6669 6c74 6572 7320 270a 2020 2020 2020  filters '.      
-000172b0: 2020 2020 2020 2020 2020 6627 4e61 6d65            f'Name
-000172c0: 3d74 6167 3a72 6179 2d63 6c75 7374 6572  =tag:ray-cluster
-000172d0: 2d6e 616d 652c 5661 6c75 6573 3d7b 6e61  -name,Values={na
-000172e0: 6d65 7d20 2d2d 7175 6572 7920 270a 2020  me} --query '.  
-000172f0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-00017300: 5265 7365 7276 6174 696f 6e73 5b5d 2e49  Reservations[].I
-00017310: 6e73 7461 6e63 6573 5b5d 2e49 6e73 7461  nstances[].Insta
-00017320: 6e63 6549 6420 2d2d 6f75 7470 7574 2074  nceId --output t
-00017330: 6578 7460 3b20 2720 2b0a 2020 2020 2020  ext`; ' +.      
-00017340: 2020 2020 2020 2020 2020 5f67 6574 5f61            _get_a
-00017350: 7773 5f71 7565 7279 5f63 6f6d 6d61 6e64  ws_query_command
-00017360: 2872 6567 696f 6e2c 2027 2469 6427 2c20  (region, '$id', 
-00017370: 2756 6f6c 756d 6554 7970 6527 2c0a 2020  'VolumeType',.  
-00017380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173a0: 2020 2020 2073 7065 6373 5b27 6469 736b       specs['disk
-000173b0: 5f74 6965 7227 5d29 202b 0a20 2020 2020  _tier']) +.     
-000173c0: 2020 2020 2020 2020 2020 2028 2727 2069             ('' i
-000173d0: 6620 6469 736b 5f74 6965 7220 3d3d 2027  f disk_tier == '
-000173e0: 6c6f 7727 2065 6c73 650a 2020 2020 2020  low' else.      
-000173f0: 2020 2020 2020 2020 2020 2028 5f67 6574             (_get
-00017400: 5f61 7773 5f71 7565 7279 5f63 6f6d 6d61  _aws_query_comma
-00017410: 6e64 2872 6567 696f 6e2c 2027 2469 6427  nd(region, '$id'
-00017420: 2c20 2749 6f70 7327 2c0a 2020 2020 2020  , 'Iops',.      
-00017430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017450: 2020 2073 7065 6373 5b27 6469 736b 5f69     specs['disk_i
-00017460: 6f70 7327 5d29 202b 0a20 2020 2020 2020  ops']) +.       
-00017470: 2020 2020 2020 2020 2020 205f 6765 745f             _get_
-00017480: 6177 735f 7175 6572 795f 636f 6d6d 616e  aws_query_comman
-00017490: 6428 7265 6769 6f6e 2c20 2724 6964 272c  d(region, '$id',
-000174a0: 2027 5468 726f 7567 6870 7574 272c 0a20   'Throughput',. 
-000174b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174d0: 2020 2020 2020 2020 7370 6563 735b 2764          specs['d
-000174e0: 6973 6b5f 7468 726f 7567 6870 7574 275d  isk_throughput']
-000174f0: 2929 292c 0a20 2020 2020 2020 2020 2020  ))),.           
-00017500: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
-00017510: 6627 736b 7920 646f 776e 202d 7920 7b6e  f'sky down -y {n
-00017520: 616d 657d 272c 0a20 2020 2020 2020 2020  ame}',.         
-00017530: 2020 2074 696d 656f 7574 3d31 3020 2a20     timeout=10 * 
-00017540: 3630 2c20 2023 2031 3020 6d69 6e73 2020  60,  # 10 mins  
-00017550: 2869 7420 7461 6b65 7320 6172 6f75 6e64  (it takes around
-00017560: 207e 3620 6d69 6e73 290a 2020 2020 2020   ~6 mins).      
-00017570: 2020 290a 2020 2020 2020 2020 7275 6e5f    ).        run_
-00017580: 6f6e 655f 7465 7374 2874 6573 7429 0a0a  one_test(test)..
-00017590: 0a40 7079 7465 7374 2e6d 6172 6b2e 6763  .@pytest.mark.gc
-000175a0: 700a 6465 6620 7465 7374 5f67 6370 5f64  p.def test_gcp_d
-000175b0: 6973 6b5f 7469 6572 2829 3a0a 2020 2020  isk_tier():.    
-000175c0: 666f 7220 6469 736b 5f74 6965 7220 696e  for disk_tier in
-000175d0: 205b 276c 6f77 272c 2027 6d65 6469 756d   ['low', 'medium
-000175e0: 272c 2027 6869 6768 275d 3a0a 2020 2020  ', 'high']:.    
-000175f0: 2020 2020 7479 7065 203d 2047 4350 2e5f      type = GCP._
-00017600: 6765 745f 6469 736b 5f74 7970 6528 6469  get_disk_type(di
-00017610: 736b 5f74 6965 7229 0a20 2020 2020 2020  sk_tier).       
-00017620: 206e 616d 6520 3d20 5f67 6574 5f63 6c75   name = _get_clu
-00017630: 7374 6572 5f6e 616d 6528 2920 2b20 272d  ster_name() + '-
-00017640: 2720 2b20 6469 736b 5f74 6965 720a 2020  ' + disk_tier.  
-00017650: 2020 2020 2020 7265 6769 6f6e 203d 2027        region = '
-00017660: 7573 2d77 6573 7432 270a 2020 2020 2020  us-west2'.      
-00017670: 2020 7465 7374 203d 2054 6573 7428 0a20    test = Test(. 
-00017680: 2020 2020 2020 2020 2020 2027 6763 702d             'gcp-
-00017690: 6469 736b 2d74 6965 7227 2c0a 2020 2020  disk-tier',.    
-000176a0: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
-000176b0: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-000176c0: 6c61 756e 6368 202d 7920 2d63 207b 6e61  launch -y -c {na
-000176d0: 6d65 7d20 2d2d 636c 6f75 6420 6763 7020  me} --cloud gcp 
-000176e0: 2d2d 7265 6769 6f6e 207b 7265 6769 6f6e  --region {region
-000176f0: 7d20 270a 2020 2020 2020 2020 2020 2020  } '.            
-00017700: 2020 2020 6627 2d2d 6469 736b 2d74 6965      f'--disk-tie
-00017710: 7220 7b64 6973 6b5f 7469 6572 7d20 6563  r {disk_tier} ec
-00017720: 686f 2022 6865 6c6c 6f20 736b 7922 272c  ho "hello sky"',
-00017730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017740: 2066 276e 616d 653d 6067 636c 6f75 6420   f'name=`gcloud 
-00017750: 636f 6d70 7574 6520 696e 7374 616e 6365  compute instance
-00017760: 7320 6c69 7374 202d 2d66 696c 7465 723d  s list --filter=
-00017770: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00017780: 2020 6627 226c 6162 656c 732e 7261 792d    f'"labels.ray-
-00017790: 636c 7573 7465 722d 6e61 6d65 3a7b 6e61  cluster-name:{na
-000177a0: 6d65 7d22 202d 2d66 6f72 6d61 743d 2276  me}" --format="v
-000177b0: 616c 7565 286e 616d 6529 2260 3b20 270a  alue(name)"`; '.
-000177c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177d0: 6627 6763 6c6f 7564 2063 6f6d 7075 7465  f'gcloud compute
-000177e0: 2064 6973 6b73 206c 6973 7420 2d2d 6669   disks list --fi
-000177f0: 6c74 6572 3d22 6e61 6d65 3d24 6e61 6d65  lter="name=$name
-00017800: 2220 270a 2020 2020 2020 2020 2020 2020  " '.            
-00017810: 2020 2020 6627 2d2d 666f 726d 6174 3d22      f'--format="
-00017820: 7661 6c75 6528 7479 7065 2922 207c 2067  value(type)" | g
-00017830: 7265 7020 7b74 7970 657d 2027 0a20 2020  rep {type} '.   
-00017840: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-00017850: 2020 2020 2020 2020 6627 736b 7920 646f          f'sky do
-00017860: 776e 202d 7920 7b6e 616d 657d 272c 0a20  wn -y {name}',. 
-00017870: 2020 2020 2020 2020 2020 2074 696d 656f             timeo
-00017880: 7574 3d36 202a 2036 302c 2020 2320 3620  ut=6 * 60,  # 6 
-00017890: 6d69 6e73 2020 2869 7420 7461 6b65 7320  mins  (it takes 
-000178a0: 6172 6f75 6e64 207e 3320 6d69 6e73 290a  around ~3 mins).
-000178b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000178c0: 2020 7275 6e5f 6f6e 655f 7465 7374 2874    run_one_test(t
-000178d0: 6573 7429 0a0a 0a40 7079 7465 7374 2e6d  est)...@pytest.m
-000178e0: 6172 6b2e 617a 7572 650a 6465 6620 7465  ark.azure.def te
-000178f0: 7374 5f61 7a75 7265 5f64 6973 6b5f 7469  st_azure_disk_ti
-00017900: 6572 2829 3a0a 2020 2020 666f 7220 6469  er():.    for di
-00017910: 736b 5f74 6965 7220 696e 205b 276c 6f77  sk_tier in ['low
-00017920: 272c 2027 6d65 6469 756d 275d 3a0a 2020  ', 'medium']:.  
-00017930: 2020 2020 2020 7479 7065 203d 2041 7a75        type = Azu
-00017940: 7265 2e5f 6765 745f 6469 736b 5f74 7970  re._get_disk_typ
-00017950: 6528 6469 736b 5f74 6965 7229 0a20 2020  e(disk_tier).   
-00017960: 2020 2020 206e 616d 6520 3d20 5f67 6574       name = _get
-00017970: 5f63 6c75 7374 6572 5f6e 616d 6528 2920  _cluster_name() 
-00017980: 2b20 272d 2720 2b20 6469 736b 5f74 6965  + '-' + disk_tie
-00017990: 720a 2020 2020 2020 2020 7265 6769 6f6e  r.        region
-000179a0: 203d 2027 7765 7374 7573 3227 0a20 2020   = 'westus2'.   
-000179b0: 2020 2020 2074 6573 7420 3d20 5465 7374       test = Test
-000179c0: 280a 2020 2020 2020 2020 2020 2020 2761  (.            'a
-000179d0: 7a75 7265 2d64 6973 6b2d 7469 6572 272c  zure-disk-tier',
-000179e0: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
-000179f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00017a00: 2773 6b79 206c 6175 6e63 6820 2d79 202d  'sky launch -y -
-00017a10: 6320 7b6e 616d 657d 202d 2d63 6c6f 7564  c {name} --cloud
-00017a20: 2061 7a75 7265 202d 2d72 6567 696f 6e20   azure --region 
-00017a30: 7b72 6567 696f 6e7d 2027 0a20 2020 2020  {region} '.     
-00017a40: 2020 2020 2020 2020 2020 2066 272d 2d64             f'--d
-00017a50: 6973 6b2d 7469 6572 207b 6469 736b 5f74  isk-tier {disk_t
-00017a60: 6965 727d 2065 6368 6f20 2268 656c 6c6f  ier} echo "hello
-00017a70: 2073 6b79 2227 2c0a 2020 2020 2020 2020   sky"',.        
-00017a80: 2020 2020 2020 2020 6627 617a 2072 6573          f'az res
-00017a90: 6f75 7263 6520 6c69 7374 202d 2d74 6167  ource list --tag
-00017aa0: 2072 6179 2d63 6c75 7374 6572 2d6e 616d   ray-cluster-nam
-00017ab0: 653d 7b6e 616d 657d 202d 2d71 7565 7279  e={name} --query
-00017ac0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-00017ad0: 2020 2066 2722 5b3f 7479 7065 3d3d 5c27     f'"[?type==\'
-00017ae0: 4d69 6372 6f73 6f66 742e 436f 6d70 7574  Microsoft.Comput
-00017af0: 652f 6469 736b 735c 275d 2e73 6b75 2e6e  e/disks\'].sku.n
-00017b00: 616d 6522 2027 0a20 2020 2020 2020 2020  ame" '.         
-00017b10: 2020 2020 2020 2066 272d 2d6f 7574 7075         f'--outpu
-00017b20: 7420 7473 7620 7c20 6772 6570 207b 7479  t tsv | grep {ty
-00017b30: 7065 7d27 0a20 2020 2020 2020 2020 2020  pe}'.           
-00017b40: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
-00017b50: 6627 736b 7920 646f 776e 202d 7920 7b6e  f'sky down -y {n
-00017b60: 616d 657d 272c 0a20 2020 2020 2020 2020  ame}',.         
-00017b70: 2020 2074 696d 656f 7574 3d32 3020 2a20     timeout=20 * 
-00017b80: 3630 2c20 2023 2032 3020 6d69 6e73 2020  60,  # 20 mins  
-00017b90: 2869 7420 7461 6b65 7320 6172 6f75 6e64  (it takes around
-00017ba0: 207e 3132 206d 696e 7329 0a20 2020 2020   ~12 mins).     
-00017bb0: 2020 2029 0a20 2020 2020 2020 2072 756e     ).        run
-00017bc0: 5f6f 6e65 5f74 6573 7428 7465 7374 290a  _one_test(test).
-00017bd0: 0a0a 2320 2d2d 2d2d 2d2d 2054 6573 7469  ..# ------ Testi
-00017be0: 6e67 205a 6572 6f20 5175 6f74 6120 4661  ng Zero Quota Fa
-00017bf0: 696c 6f76 6572 202d 2d2d 2d2d 2d0a 4070  ilover ------.@p
-00017c00: 7974 6573 742e 6d61 726b 2e61 7773 0a64  ytest.mark.aws.d
-00017c10: 6566 2074 6573 745f 6177 735f 7a65 726f  ef test_aws_zero
-00017c20: 5f71 756f 7461 5f66 6169 6c6f 7665 7228  _quota_failover(
-00017c30: 293a 0a0a 2020 2020 6e61 6d65 203d 205f  ):..    name = _
-00017c40: 6765 745f 636c 7573 7465 725f 6e61 6d65  get_cluster_name
-00017c50: 2829 0a20 2020 2072 6567 696f 6e20 3d20  ().    region = 
-00017c60: 6765 745f 6177 735f 7265 6769 6f6e 5f66  get_aws_region_f
-00017c70: 6f72 5f71 756f 7461 5f66 6169 6c6f 7665  or_quota_failove
-00017c80: 7228 290a 0a20 2020 2069 6620 6e6f 7420  r()..    if not 
-00017c90: 7265 6769 6f6e 3a0a 2020 2020 2020 2020  region:.        
-00017ca0: 7079 7465 7374 2e78 6661 696c 280a 2020  pytest.xfail(.  
-00017cb0: 2020 2020 2020 2020 2020 2755 6e61 626c            'Unabl
-00017cc0: 6520 746f 2074 6573 7420 7a65 726f 2071  e to test zero q
-00017cd0: 756f 7461 2066 6169 6c6f 7665 7220 6f70  uota failover op
-00017ce0: 7469 6d69 7a61 7469 6f6e 20e2 8094 2071  timization ... q
-00017cf0: 756f 7461 7320 270a 2020 2020 2020 2020  uotas '.        
-00017d00: 2020 2020 2766 6f72 2045 4332 2050 3320      'for EC2 P3 
-00017d10: 696e 7374 616e 6365 7320 7765 7265 2066  instances were f
-00017d20: 6f75 6e64 206f 6e20 616c 6c20 4157 5320  ound on all AWS 
-00017d30: 7265 6769 6f6e 732e 2049 7320 7468 6973  regions. Is this
-00017d40: 2027 0a20 2020 2020 2020 2020 2020 2027   '.            '
-00017d50: 6578 7065 6374 6564 2066 6f72 2079 6f75  expected for you
-00017d60: 7220 6163 636f 756e 743f 2729 0a20 2020  r account?').   
-00017d70: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-00017d80: 2074 6573 7420 3d20 5465 7374 280a 2020   test = Test(.  
-00017d90: 2020 2020 2020 2761 7773 2d7a 6572 6f2d        'aws-zero-
-00017da0: 7175 6f74 612d 6661 696c 6f76 6572 272c  quota-failover',
-00017db0: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
-00017dc0: 2020 2020 2020 2066 2773 6b79 206c 6175         f'sky lau
-00017dd0: 6e63 6820 2d79 202d 6320 7b6e 616d 657d  nch -y -c {name}
-00017de0: 202d 2d63 6c6f 7564 2061 7773 202d 2d72   --cloud aws --r
-00017df0: 6567 696f 6e20 7b72 6567 696f 6e7d 202d  egion {region} -
-00017e00: 2d67 7075 7320 5631 3030 3a38 202d 2d75  -gpus V100:8 --u
-00017e10: 7365 2d73 706f 7420 7c20 6772 6570 2022  se-spot | grep "
-00017e20: 466f 756e 6420 6e6f 2071 756f 7461 2227  Found no quota"'
-00017e30: 2c0a 2020 2020 2020 2020 5d2c 0a20 2020  ,.        ],.   
-00017e40: 2020 2020 2066 2773 6b79 2064 6f77 6e20       f'sky down 
-00017e50: 2d79 207b 6e61 6d65 7d27 2c0a 2020 2020  -y {name}',.    
-00017e60: 290a 2020 2020 7275 6e5f 6f6e 655f 7465  ).    run_one_te
-00017e70: 7374 2874 6573 7429 0a0a 0a40 7079 7465  st(test)...@pyte
-00017e80: 7374 2e6d 6172 6b2e 6763 700a 6465 6620  st.mark.gcp.def 
-00017e90: 7465 7374 5f67 6370 5f7a 6572 6f5f 7175  test_gcp_zero_qu
-00017ea0: 6f74 615f 6661 696c 6f76 6572 2829 3a0a  ota_failover():.
-00017eb0: 0a20 2020 206e 616d 6520 3d20 5f67 6574  .    name = _get
-00017ec0: 5f63 6c75 7374 6572 5f6e 616d 6528 290a  _cluster_name().
-00017ed0: 2020 2020 7265 6769 6f6e 203d 2067 6574      region = get
-00017ee0: 5f67 6370 5f72 6567 696f 6e5f 666f 725f  _gcp_region_for_
-00017ef0: 7175 6f74 615f 6661 696c 6f76 6572 2829  quota_failover()
-00017f00: 0a0a 2020 2020 6966 206e 6f74 2072 6567  ..    if not reg
-00017f10: 696f 6e3a 0a20 2020 2020 2020 2070 7974  ion:.        pyt
-00017f20: 6573 742e 7866 6169 6c28 0a20 2020 2020  est.xfail(.     
-00017f30: 2020 2020 2020 2027 556e 6162 6c65 2074         'Unable t
-00017f40: 6f20 7465 7374 207a 6572 6f20 7175 6f74  o test zero quot
-00017f50: 6120 6661 696c 6f76 6572 206f 7074 696d  a failover optim
-00017f60: 697a 6174 696f 6e20 e280 9420 7175 6f74  ization ... quot
-00017f70: 6173 2027 0a20 2020 2020 2020 2020 2020  as '.           
-00017f80: 2027 666f 7220 4131 3030 2d38 3047 4220   'for A100-80GB 
-00017f90: 4750 5573 2077 6572 6520 666f 756e 6420  GPUs were found 
-00017fa0: 6f6e 2061 6c6c 2047 4350 2072 6567 696f  on all GCP regio
-00017fb0: 6e73 2e20 4973 2074 6869 7320 270a 2020  ns. Is this '.  
-00017fc0: 2020 2020 2020 2020 2020 2765 7870 6563            'expec
-00017fd0: 7465 6420 666f 7220 796f 7572 2061 6363  ted for your acc
-00017fe0: 6f75 6e74 3f27 290a 2020 2020 2020 2020  ount?').        
-00017ff0: 7265 7475 726e 0a0a 2020 2020 7465 7374  return..    test
-00018000: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
-00018010: 2027 6763 702d 7a65 726f 2d71 756f 7461   'gcp-zero-quota
-00018020: 2d66 6169 6c6f 7665 7227 2c0a 2020 2020  -failover',.    
-00018030: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-00018040: 2020 6627 736b 7920 6c61 756e 6368 202d    f'sky launch -
-00018050: 7920 2d63 207b 6e61 6d65 7d20 2d2d 636c  y -c {name} --cl
-00018060: 6f75 6420 6763 7020 2d2d 7265 6769 6f6e  oud gcp --region
-00018070: 207b 7265 6769 6f6e 7d20 2d2d 6770 7573   {region} --gpus
-00018080: 2041 3130 302d 3830 4742 3a31 202d 2d75   A100-80GB:1 --u
-00018090: 7365 2d73 706f 7420 7c20 6772 6570 2022  se-spot | grep "
-000180a0: 466f 756e 6420 6e6f 2071 756f 7461 2227  Found no quota"'
-000180b0: 2c0a 2020 2020 2020 2020 5d2c 0a20 2020  ,.        ],.   
-000180c0: 2020 2020 2066 2773 6b79 2064 6f77 6e20       f'sky down 
-000180d0: 2d79 207b 6e61 6d65 7d27 2c0a 2020 2020  -y {name}',.    
-000180e0: 290a 2020 2020 7275 6e5f 6f6e 655f 7465  ).    run_one_te
-000180f0: 7374 2874 6573 7429 0a0a 0a23 202d 2d2d  st(test)...# ---
-00018100: 2d2d 2d2d 2054 6573 7469 6e67 2075 7365  ---- Testing use
-00018110: 7220 7261 7920 636c 7573 7465 7220 2d2d  r ray cluster --
-00018120: 2d2d 2d2d 2d2d 0a64 6566 2074 6573 745f  ------.def test_
-00018130: 7573 6572 5f72 6179 5f63 6c75 7374 6572  user_ray_cluster
-00018140: 2829 3a0a 2020 2020 6e61 6d65 203d 205f  ():.    name = _
-00018150: 6765 745f 636c 7573 7465 725f 6e61 6d65  get_cluster_name
-00018160: 2829 0a20 2020 2074 6573 7420 3d20 5465  ().    test = Te
-00018170: 7374 280a 2020 2020 2020 2020 2775 7365  st(.        'use
-00018180: 722d 7261 792d 636c 7573 7465 7227 2c0a  r-ray-cluster',.
-00018190: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
-000181a0: 2020 2020 2020 6627 736b 7920 6c61 756e        f'sky laun
-000181b0: 6368 202d 7920 2d63 207b 6e61 6d65 7d20  ch -y -c {name} 
-000181c0: 2272 6179 2073 7461 7274 202d 2d68 6561  "ray start --hea
-000181d0: 6422 272c 0a20 2020 2020 2020 2020 2020  d"',.           
-000181e0: 2066 2773 6b79 2065 7865 6320 7b6e 616d   f'sky exec {nam
-000181f0: 657d 2022 6563 686f 2068 6922 272c 0a20  e} "echo hi"',. 
-00018200: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-00018210: 206c 6f67 7320 7b6e 616d 657d 2031 202d   logs {name} 1 -
-00018220: 2d73 7461 7475 7327 2c0a 2020 2020 2020  -status',.      
-00018230: 2020 2020 2020 6627 736b 7920 7374 6174        f'sky stat
-00018240: 7573 202d 7220 7c20 6772 6570 207b 6e61  us -r | grep {na
-00018250: 6d65 7d20 7c20 6772 6570 2055 5027 2c0a  me} | grep UP',.
-00018260: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-00018270: 7920 6578 6563 207b 6e61 6d65 7d20 2265  y exec {name} "e
-00018280: 6368 6f20 6279 6522 272c 0a20 2020 2020  cho bye"',.     
-00018290: 2020 2020 2020 2066 2773 6b79 206c 6f67         f'sky log
-000182a0: 7320 7b6e 616d 657d 2032 202d 2d73 7461  s {name} 2 --sta
-000182b0: 7475 7327 2c0a 2020 2020 2020 2020 5d2c  tus',.        ],
-000182c0: 0a20 2020 2020 2020 2066 2773 6b79 2064  .        f'sky d
-000182d0: 6f77 6e20 2d79 207b 6e61 6d65 7d27 2c0a  own -y {name}',.
-000182e0: 2020 2020 290a 2020 2020 7275 6e5f 6f6e      ).    run_on
-000182f0: 655f 7465 7374 2874 6573 7429 0a0a 0a23  e_test(test)...#
-00018300: 202d 2d2d 2d2d 2d2d 2054 6573 7469 6e67   ------- Testing
-00018310: 2074 6865 2063 6f72 6520 4150 4920 2d2d   the core API --
-00018320: 2d2d 2d2d 2d2d 0a23 204d 6f73 7420 6f66  ------.# Most of
-00018330: 2074 6865 2063 6f72 6520 4150 4973 2068   the core APIs h
-00018340: 6176 6520 6265 656e 2074 6573 7465 6420  ave been tested 
-00018350: 696e 2074 6865 2043 4c49 2074 6573 7473  in the CLI tests
-00018360: 2e0a 2320 5468 6573 6520 7465 7374 7320  ..# These tests 
-00018370: 6172 6520 666f 7220 7465 7374 696e 6720  are for testing 
-00018380: 7468 6520 7265 7475 726e 2076 616c 7565  the return value
-00018390: 206f 6620 7468 6520 4150 4973 206e 6f74   of the APIs not
-000183a0: 2066 756c 6c79 2075 7365 6420 696e 2043   fully used in C
-000183b0: 4c49 2e0a 6465 6620 7465 7374 5f63 6f72  LI..def test_cor
-000183c0: 655f 6170 6928 293a 0a20 2020 206e 616d  e_api():.    nam
-000183d0: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
-000183e0: 5f6e 616d 6528 290a 2020 2020 736b 792e  _name().    sky.
-000183f0: 6c61 756e 6368 0a20 2020 2023 2054 4f44  launch.    # TOD
-00018400: 4f28 7a68 7775 293a 2041 6464 2061 2074  O(zhwu): Add a t
-00018410: 6573 7420 666f 7220 636f 7265 2061 7069  est for core api
-00018420: 2e0a 0a0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  ....# ----------
-00018430: 2054 6573 7469 6e67 2053 746f 7261 6765   Testing Storage
-00018440: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 636c 6173   ----------.clas
-00018450: 7320 5465 7374 5374 6f72 6167 6557 6974  s TestStorageWit
-00018460: 6843 7265 6465 6e74 6961 6c73 3a0a 2020  hCredentials:.  
-00018470: 2020 2222 2253 746f 7261 6765 2074 6573    """Storage tes
-00018480: 7473 2077 6869 6368 2072 6571 7569 7265  ts which require
-00018490: 2063 7265 6465 6e74 6961 6c73 2061 6e64   credentials and
-000184a0: 206e 6574 776f 726b 2063 6f6e 6e65 6374   network connect
-000184b0: 696f 6e22 2222 0a0a 2020 2020 4157 535f  ion"""..    AWS_
-000184c0: 494e 5641 4c49 445f 4e41 4d45 5320 3d20  INVALID_NAMES = 
-000184d0: 5b0a 2020 2020 2020 2020 2761 6227 2c20  [.        'ab', 
-000184e0: 2023 206c 6573 7320 7468 616e 2033 2063   # less than 3 c
-000184f0: 6861 7261 6374 6572 730a 2020 2020 2020  haracters.      
-00018500: 2020 2761 6263 6465 6667 6869 6a6b 6c6d    'abcdefghijklm
-00018510: 6e6f 7071 7273 7475 7677 7879 7a61 6263  nopqrstuvwxyzabc
-00018520: 6465 6667 6869 6a6b 6c6d 6e6f 7071 7273  defghijklmnopqrs
-00018530: 7475 7677 7879 7a61 6263 6465 6667 6869  tuvwxyzabcdefghi
-00018540: 6a6b 6c6d 6e6f 7071 7273 7475 7677 7879  jklmnopqrstuvwxy
-00018550: 7a31 272c 0a20 2020 2020 2020 2023 206d  z1',.        # m
-00018560: 6f72 6520 7468 616e 2036 3320 6368 6172  ore than 63 char
-00018570: 6163 7465 7273 0a20 2020 2020 2020 2027  acters.        '
-00018580: 4162 6364 6566 272c 2020 2320 636f 6e74  Abcdef',  # cont
-00018590: 6169 6e73 2061 6e20 7570 7065 7263 6173  ains an uppercas
-000185a0: 6520 6c65 7474 6572 0a20 2020 2020 2020  e letter.       
-000185b0: 2027 6162 6320 6465 6627 2c20 2023 2063   'abc def',  # c
-000185c0: 6f6e 7461 696e 7320 6120 7370 6163 650a  ontains a space.
-000185d0: 2020 2020 2020 2020 2761 6263 2e2e 6465          'abc..de
-000185e0: 6627 2c20 2023 2074 776f 2061 646a 6163  f',  # two adjac
-000185f0: 656e 7420 7065 7269 6f64 730a 2020 2020  ent periods.    
-00018600: 2020 2020 2731 3932 2e31 3638 2e35 2e34      '192.168.5.4
-00018610: 272c 2020 2320 666f 726d 6174 7465 6420  ',  # formatted 
-00018620: 6173 2061 6e20 4950 2061 6464 7265 7373  as an IP address
-00018630: 0a20 2020 2020 2020 2027 786e 2d2d 6275  .        'xn--bu
-00018640: 636b 6574 272c 2020 2320 7374 6172 7473  cket',  # starts
-00018650: 2077 6974 6820 2778 6e2d 2d27 2070 7265   with 'xn--' pre
-00018660: 6669 780a 2020 2020 2020 2020 2762 7563  fix.        'buc
-00018670: 6b65 742d 7333 616c 6961 7327 2c20 2023  ket-s3alias',  #
-00018680: 2065 6e64 7320 7769 7468 2027 2d73 3361   ends with '-s3a
-00018690: 6c69 6173 2720 7375 6666 6978 0a20 2020  lias' suffix.   
-000186a0: 2020 2020 2027 6275 636b 6574 2d2d 6f6c       'bucket--ol
-000186b0: 2d73 3327 2c20 2023 2065 6e64 7320 7769  -s3',  # ends wi
-000186c0: 7468 2027 2d2d 6f6c 2d73 3327 2073 7566  th '--ol-s3' suf
-000186d0: 6669 780a 2020 2020 2020 2020 272e 6162  fix.        '.ab
-000186e0: 6327 2c20 2023 2073 7461 7274 7320 7769  c',  # starts wi
-000186f0: 7468 2061 2064 6f74 0a20 2020 2020 2020  th a dot.       
-00018700: 2027 6162 632e 272c 2020 2320 656e 6473   'abc.',  # ends
-00018710: 2077 6974 6820 6120 646f 740a 2020 2020   with a dot.    
-00018720: 2020 2020 272d 6162 6327 2c20 2023 2073      '-abc',  # s
-00018730: 7461 7274 7320 7769 7468 2061 2068 7970  tarts with a hyp
-00018740: 6865 6e0a 2020 2020 2020 2020 2761 6263  hen.        'abc
-00018750: 2d27 2c20 2023 2065 6e64 7320 7769 7468  -',  # ends with
-00018760: 2061 2068 7970 6865 6e0a 2020 2020 5d0a   a hyphen.    ].
-00018770: 0a20 2020 2047 4353 5f49 4e56 414c 4944  .    GCS_INVALID
-00018780: 5f4e 414d 4553 203d 205b 0a20 2020 2020  _NAMES = [.     
-00018790: 2020 2027 6162 272c 2020 2320 6c65 7373     'ab',  # less
-000187a0: 2074 6861 6e20 3320 6368 6172 6163 7465   than 3 characte
-000187b0: 7273 0a20 2020 2020 2020 2027 6162 6364  rs.        'abcd
-000187c0: 6566 6768 696a 6b6c 6d6e 6f70 7172 7374  efghijklmnopqrst
-000187d0: 7576 7778 797a 6162 6364 6566 6768 696a  uvwxyzabcdefghij
-000187e0: 6b6c 6d6e 6f70 7172 7374 7576 7778 797a  klmnopqrstuvwxyz
-000187f0: 6162 6364 6566 6768 696a 6b6c 6d6e 6f70  abcdefghijklmnop
-00018800: 7172 7374 7576 7778 797a 3127 2c0a 2020  qrstuvwxyz1',.  
-00018810: 2020 2020 2020 2320 6d6f 7265 2074 6861        # more tha
-00018820: 6e20 3633 2063 6861 7261 6374 6572 7320  n 63 characters 
-00018830: 2877 6974 686f 7574 2064 6f74 7329 0a20  (without dots). 
-00018840: 2020 2020 2020 2027 4162 6364 6566 272c         'Abcdef',
-00018850: 2020 2320 636f 6e74 6169 6e73 2061 6e20    # contains an 
-00018860: 7570 7065 7263 6173 6520 6c65 7474 6572  uppercase letter
-00018870: 0a20 2020 2020 2020 2027 6162 6320 6465  .        'abc de
-00018880: 6627 2c20 2023 2063 6f6e 7461 696e 7320  f',  # contains 
-00018890: 6120 7370 6163 650a 2020 2020 2020 2020  a space.        
-000188a0: 2761 6263 2e2e 6465 6627 2c20 2023 2074  'abc..def',  # t
-000188b0: 776f 2061 646a 6163 656e 7420 7065 7269  wo adjacent peri
-000188c0: 6f64 730a 2020 2020 2020 2020 2761 6263  ods.        'abc
-000188d0: 5f2e 6465 662e 6768 692e 6a6b 6c6d 6e6f  _.def.ghi.jklmno
-000188e0: 7071 7273 7475 7677 7879 7a61 6263 6465  pqrstuvwxyzabcde
-000188f0: 6667 6869 6a6b 6c6d 6e6f 7071 7273 7475  fghijklmnopqrstu
-00018900: 7677 7879 7a61 6263 6465 6667 6869 6a6b  vwxyzabcdefghijk
-00018910: 6c6d 6e6f 7071 7273 7475 7677 7879 7a31  lmnopqrstuvwxyz1
-00018920: 270a 2020 2020 2020 2020 2320 4d6f 7265  '.        # More
-00018930: 2074 6861 6e20 3633 2063 6861 7261 6374   than 63 charact
-00018940: 6572 7320 6265 7477 6565 6e20 646f 7473  ers between dots
-00018950: 0a20 2020 2020 2020 2027 6162 635f 2e64  .        'abc_.d
-00018960: 6566 2e67 6869 2e6a 6b6c 6d6e 6f70 7172  ef.ghi.jklmnopqr
-00018970: 7374 7576 7778 797a 6162 6364 6566 6768  stuvwxyzabcdefgh
-00018980: 696a 6b6c 6d6e 6f70 7166 6768 696a 6b6c  ijklmnopqfghijkl
-00018990: 6d6e 6f70 7172 7374 7576 7727 202a 2035  mnopqrstuvw' * 5
-000189a0: 2c0a 2020 2020 2020 2020 2320 6d6f 7265  ,.        # more
-000189b0: 2074 6861 6e20 3232 3220 6368 6172 6163   than 222 charac
-000189c0: 7465 7273 2028 7769 7468 2064 6f74 7329  ters (with dots)
-000189d0: 0a20 2020 2020 2020 2027 3139 322e 3136  .        '192.16
-000189e0: 382e 352e 3427 2c20 2023 2066 6f72 6d61  8.5.4',  # forma
-000189f0: 7474 6564 2061 7320 616e 2049 5020 6164  tted as an IP ad
-00018a00: 6472 6573 730a 2020 2020 2020 2020 2767  dress.        'g
-00018a10: 6f6f 6762 7563 6b65 7427 2c20 2023 2073  oogbucket',  # s
-00018a20: 7461 7274 7320 7769 7468 2027 676f 6f67  tarts with 'goog
-00018a30: 2720 7072 6566 6978 0a20 2020 2020 2020  ' prefix.       
-00018a40: 2027 676f 6f67 6c65 6275 636b 6574 272c   'googlebucket',
-00018a50: 2020 2320 636f 6e74 6169 6e73 2027 676f    # contains 'go
-00018a60: 6f67 6c65 270a 2020 2020 2020 2020 2767  ogle'.        'g
-00018a70: 3030 676c 6562 7563 6b65 7427 2c20 2023  00glebucket',  #
-00018a80: 2076 6172 6961 6e74 206f 6620 2767 6f6f   variant of 'goo
-00018a90: 676c 6527 0a20 2020 2020 2020 2027 676f  gle'.        'go
-00018aa0: 3067 6c65 6275 636b 6574 272c 2020 2320  0glebucket',  # 
-00018ab0: 7661 7269 616e 7420 6f66 2027 676f 6f67  variant of 'goog
-00018ac0: 6c65 270a 2020 2020 2020 2020 2767 306f  le'.        'g0o
-00018ad0: 676c 6562 7563 6b65 7427 2c20 2023 2076  glebucket',  # v
-00018ae0: 6172 6961 6e74 206f 6620 2767 6f6f 676c  ariant of 'googl
-00018af0: 6527 0a20 2020 2020 2020 2027 2e61 6263  e'.        '.abc
-00018b00: 272c 2020 2320 7374 6172 7473 2077 6974  ',  # starts wit
-00018b10: 6820 6120 646f 740a 2020 2020 2020 2020  h a dot.        
-00018b20: 2761 6263 2e27 2c20 2023 2065 6e64 7320  'abc.',  # ends 
-00018b30: 7769 7468 2061 2064 6f74 0a20 2020 2020  with a dot.     
-00018b40: 2020 2027 5f61 6263 272c 2020 2320 7374     '_abc',  # st
-00018b50: 6172 7473 2077 6974 6820 616e 2075 6e64  arts with an und
-00018b60: 6572 7363 6f72 650a 2020 2020 2020 2020  erscore.        
-00018b70: 2761 6263 5f27 2c20 2023 2065 6e64 7320  'abc_',  # ends 
-00018b80: 7769 7468 2061 6e20 756e 6465 7273 636f  with an undersco
-00018b90: 7265 0a20 2020 205d 0a0a 2020 2020 4073  re.    ]..    @s
-00018ba0: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
-00018bb0: 6465 6620 636c 695f 6465 6c65 7465 5f63  def cli_delete_c
-00018bc0: 6d64 2873 746f 7265 5f74 7970 652c 2062  md(store_type, b
-00018bd0: 7563 6b65 745f 6e61 6d65 293a 0a20 2020  ucket_name):.   
-00018be0: 2020 2020 2069 6620 7374 6f72 655f 7479       if store_ty
-00018bf0: 7065 203d 3d20 7374 6f72 6167 655f 6c69  pe == storage_li
-00018c00: 622e 5374 6f72 6554 7970 652e 5333 3a0a  b.StoreType.S3:.
-00018c10: 2020 2020 2020 2020 2020 2020 7572 6c20              url 
-00018c20: 3d20 6627 7333 3a2f 2f7b 6275 636b 6574  = f's3://{bucket
-00018c30: 5f6e 616d 657d 270a 2020 2020 2020 2020  _name}'.        
-00018c40: 2020 2020 7265 7475 726e 2066 2761 7773      return f'aws
-00018c50: 2073 3320 7262 207b 7572 6c7d 202d 2d66   s3 rb {url} --f
-00018c60: 6f72 6365 270a 2020 2020 2020 2020 6966  orce'.        if
-00018c70: 2073 746f 7265 5f74 7970 6520 3d3d 2073   store_type == s
-00018c80: 746f 7261 6765 5f6c 6962 2e53 746f 7265  torage_lib.Store
-00018c90: 5479 7065 2e47 4353 3a0a 2020 2020 2020  Type.GCS:.      
-00018ca0: 2020 2020 2020 7572 6c20 3d20 6627 6773        url = f'gs
-00018cb0: 3a2f 2f7b 6275 636b 6574 5f6e 616d 657d  ://{bucket_name}
-00018cc0: 270a 2020 2020 2020 2020 2020 2020 7265  '.            re
-00018cd0: 7475 726e 2066 2767 7375 7469 6c20 2d6d  turn f'gsutil -m
-00018ce0: 2072 6d20 2d72 207b 7572 6c7d 270a 2020   rm -r {url}'.  
-00018cf0: 2020 2020 2020 6966 2073 746f 7265 5f74        if store_t
-00018d00: 7970 6520 3d3d 2073 746f 7261 6765 5f6c  ype == storage_l
-00018d10: 6962 2e53 746f 7265 5479 7065 2e52 323a  ib.StoreType.R2:
-00018d20: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
-00018d30: 706f 696e 745f 7572 6c20 3d20 636c 6f75  point_url = clou
-00018d40: 6466 6c61 7265 2e63 7265 6174 655f 656e  dflare.create_en
-00018d50: 6470 6f69 6e74 2829 0a20 2020 2020 2020  dpoint().       
-00018d60: 2020 2020 2075 726c 203d 2066 2773 333a       url = f's3:
-00018d70: 2f2f 7b62 7563 6b65 745f 6e61 6d65 7d27  //{bucket_name}'
-00018d80: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00018d90: 7572 6e20 6627 4157 535f 5348 4152 4544  urn f'AWS_SHARED
-00018da0: 5f43 5245 4445 4e54 4941 4c53 5f46 494c  _CREDENTIALS_FIL
-00018db0: 453d 7b63 6c6f 7564 666c 6172 652e 5232  E={cloudflare.R2
-00018dc0: 5f43 5245 4445 4e54 4941 4c53 5f50 4154  _CREDENTIALS_PAT
-00018dd0: 487d 2061 7773 2073 3320 7262 207b 7572  H} aws s3 rb {ur
-00018de0: 6c7d 202d 2d66 6f72 6365 202d 2d65 6e64  l} --force --end
-00018df0: 706f 696e 7420 7b65 6e64 706f 696e 745f  point {endpoint_
-00018e00: 7572 6c7d 202d 2d70 726f 6669 6c65 3d72  url} --profile=r
-00018e10: 3227 0a0a 2020 2020 4073 7461 7469 636d  2'..    @staticm
-00018e20: 6574 686f 640a 2020 2020 6465 6620 636c  ethod.    def cl
-00018e30: 695f 6c73 5f63 6d64 2873 746f 7265 5f74  i_ls_cmd(store_t
-00018e40: 7970 652c 2062 7563 6b65 745f 6e61 6d65  ype, bucket_name
-00018e50: 2c20 7375 6666 6978 3d27 2729 3a0a 2020  , suffix=''):.  
-00018e60: 2020 2020 2020 6966 2073 746f 7265 5f74        if store_t
-00018e70: 7970 6520 3d3d 2073 746f 7261 6765 5f6c  ype == storage_l
-00018e80: 6962 2e53 746f 7265 5479 7065 2e53 333a  ib.StoreType.S3:
-00018e90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00018ea0: 7375 6666 6978 3a0a 2020 2020 2020 2020  suffix:.        
-00018eb0: 2020 2020 2020 2020 7572 6c20 3d20 6627          url = f'
-00018ec0: 7333 3a2f 2f7b 6275 636b 6574 5f6e 616d  s3://{bucket_nam
-00018ed0: 657d 2f7b 7375 6666 6978 7d27 0a20 2020  e}/{suffix}'.   
-00018ee0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00018ef0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00018f00: 726c 203d 2066 2773 333a 2f2f 7b62 7563  rl = f's3://{buc
-00018f10: 6b65 745f 6e61 6d65 7d27 0a20 2020 2020  ket_name}'.     
-00018f20: 2020 2020 2020 2072 6574 7572 6e20 6627         return f'
-00018f30: 6177 7320 7333 206c 7320 7b75 726c 7d27  aws s3 ls {url}'
-00018f40: 0a20 2020 2020 2020 2069 6620 7374 6f72  .        if stor
-00018f50: 655f 7479 7065 203d 3d20 7374 6f72 6167  e_type == storag
-00018f60: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
-00018f70: 4743 533a 0a20 2020 2020 2020 2020 2020  GCS:.           
-00018f80: 2069 6620 7375 6666 6978 3a0a 2020 2020   if suffix:.    
-00018f90: 2020 2020 2020 2020 2020 2020 7572 6c20              url 
-00018fa0: 3d20 6627 6773 3a2f 2f7b 6275 636b 6574  = f'gs://{bucket
-00018fb0: 5f6e 616d 657d 2f7b 7375 6666 6978 7d27  _name}/{suffix}'
-00018fc0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00018fd0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00018fe0: 2020 2075 726c 203d 2066 2767 733a 2f2f     url = f'gs://
-00018ff0: 7b62 7563 6b65 745f 6e61 6d65 7d27 0a20  {bucket_name}'. 
-00019000: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00019010: 6e20 6627 6773 7574 696c 206c 7320 7b75  n f'gsutil ls {u
-00019020: 726c 7d27 0a20 2020 2020 2020 2069 6620  rl}'.        if 
-00019030: 7374 6f72 655f 7479 7065 203d 3d20 7374  store_type == st
-00019040: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
-00019050: 7970 652e 5232 3a0a 2020 2020 2020 2020  ype.R2:.        
-00019060: 2020 2020 656e 6470 6f69 6e74 5f75 726c      endpoint_url
-00019070: 203d 2063 6c6f 7564 666c 6172 652e 6372   = cloudflare.cr
-00019080: 6561 7465 5f65 6e64 706f 696e 7428 290a  eate_endpoint().
-00019090: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000190a0: 7566 6669 783a 0a20 2020 2020 2020 2020  uffix:.         
-000190b0: 2020 2020 2020 2075 726c 203d 2066 2773         url = f's
-000190c0: 333a 2f2f 7b62 7563 6b65 745f 6e61 6d65  3://{bucket_name
-000190d0: 7d2f 7b73 7566 6669 787d 270a 2020 2020  }/{suffix}'.    
-000190e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000190f0: 2020 2020 2020 2020 2020 2020 2020 7572                ur
-00019100: 6c20 3d20 6627 7333 3a2f 2f7b 6275 636b  l = f's3://{buck
-00019110: 6574 5f6e 616d 657d 270a 2020 2020 2020  et_name}'.      
-00019120: 2020 2020 2020 7265 7475 726e 2066 2741        return f'A
-00019130: 5753 5f53 4841 5245 445f 4352 4544 454e  WS_SHARED_CREDEN
-00019140: 5449 414c 535f 4649 4c45 3d7b 636c 6f75  TIALS_FILE={clou
-00019150: 6466 6c61 7265 2e52 325f 4352 4544 454e  dflare.R2_CREDEN
-00019160: 5449 414c 535f 5041 5448 7d20 6177 7320  TIALS_PATH} aws 
-00019170: 7333 206c 7320 7b75 726c 7d20 2d2d 656e  s3 ls {url} --en
-00019180: 6470 6f69 6e74 207b 656e 6470 6f69 6e74  dpoint {endpoint
-00019190: 5f75 726c 7d20 2d2d 7072 6f66 696c 653d  _url} --profile=
-000191a0: 7232 270a 0a20 2020 2040 7079 7465 7374  r2'..    @pytest
-000191b0: 2e66 6978 7475 7265 0a20 2020 2064 6566  .fixture.    def
-000191c0: 2074 6d70 5f73 6f75 7263 6528 7365 6c66   tmp_source(self
-000191d0: 2c20 746d 705f 7061 7468 293a 0a20 2020  , tmp_path):.   
-000191e0: 2020 2020 2023 2043 7265 6174 6573 2061       # Creates a
-000191f0: 2074 656d 706f 7261 7279 2064 6972 6563   temporary direc
-00019200: 746f 7279 2077 6974 6820 6120 6669 6c65  tory with a file
-00019210: 2069 6e20 6974 0a20 2020 2020 2020 2074   in it.        t
-00019220: 6d70 5f64 6972 203d 2074 6d70 5f70 6174  mp_dir = tmp_pat
-00019230: 6820 2f20 2774 6d70 2d73 6f75 7263 6527  h / 'tmp-source'
-00019240: 0a20 2020 2020 2020 2074 6d70 5f64 6972  .        tmp_dir
-00019250: 2e6d 6b64 6972 2829 0a20 2020 2020 2020  .mkdir().       
-00019260: 2074 6d70 5f66 696c 6520 3d20 746d 705f   tmp_file = tmp_
-00019270: 6469 7220 2f20 2774 6d70 2d66 696c 6527  dir / 'tmp-file'
-00019280: 0a20 2020 2020 2020 2074 6d70 5f66 696c  .        tmp_fil
-00019290: 652e 7772 6974 655f 7465 7874 2827 7465  e.write_text('te
-000192a0: 7374 2729 0a20 2020 2020 2020 2063 6972  st').        cir
-000192b0: 636c 655f 6c69 6e6b 203d 2074 6d70 5f64  cle_link = tmp_d
-000192c0: 6972 202f 2027 6369 7263 6c65 2d6c 696e  ir / 'circle-lin
-000192d0: 6b27 0a20 2020 2020 2020 2063 6972 636c  k'.        circl
-000192e0: 655f 6c69 6e6b 2e73 796d 6c69 6e6b 5f74  e_link.symlink_t
-000192f0: 6f28 746d 705f 6469 722c 2074 6172 6765  o(tmp_dir, targe
-00019300: 745f 6973 5f64 6972 6563 746f 7279 3d54  t_is_directory=T
-00019310: 7275 6529 0a20 2020 2020 2020 2079 6965  rue).        yie
-00019320: 6c64 2073 7472 2874 6d70 5f64 6972 290a  ld str(tmp_dir).
-00019330: 0a20 2020 2040 7079 7465 7374 2e66 6978  .    @pytest.fix
-00019340: 7475 7265 0a20 2020 2064 6566 2074 6d70  ture.    def tmp
-00019350: 5f62 7563 6b65 745f 6e61 6d65 2873 656c  _bucket_name(sel
-00019360: 6629 3a0a 2020 2020 2020 2020 2320 4372  f):.        # Cr
-00019370: 6561 7465 7320 6120 7465 6d70 6f72 6172  eates a temporar
-00019380: 7920 6275 636b 6574 206e 616d 650a 2020  y bucket name.  
-00019390: 2020 2020 2020 2320 7469 6d65 2e74 696d        # time.tim
-000193a0: 6528 2920 7265 7475 726e 7320 7661 7279  e() returns vary
-000193b0: 696e 6720 7072 6563 6973 696f 6e20 6f6e  ing precision on
-000193c0: 2064 6966 6665 7265 6e74 2073 7973 7465   different syste
-000193d0: 6d73 2c20 736f 2077 650a 2020 2020 2020  ms, so we.      
-000193e0: 2020 2320 7265 706c 6163 6520 7468 6520    # replace the 
-000193f0: 6465 6369 6d61 6c20 706f 696e 7420 616e  decimal point an
-00019400: 6420 7573 6520 7768 6174 6576 6572 2070  d use whatever p
-00019410: 7265 6369 7369 6f6e 2077 6520 6361 6e20  recision we can 
-00019420: 6765 742e 0a20 2020 2020 2020 2074 696d  get..        tim
-00019430: 6573 7461 6d70 203d 2073 7472 2874 696d  estamp = str(tim
-00019440: 652e 7469 6d65 2829 292e 7265 706c 6163  e.time()).replac
-00019450: 6528 272e 272c 2027 2729 0a20 2020 2020  e('.', '').     
-00019460: 2020 2079 6965 6c64 2066 2773 6b79 2d74     yield f'sky-t
-00019470: 6573 742d 7b74 696d 6573 7461 6d70 7d27  est-{timestamp}'
-00019480: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-00019490: 686f 640a 2020 2020 6465 6620 7969 656c  hod.    def yiel
-000194a0: 645f 7374 6f72 6167 655f 6f62 6a65 6374  d_storage_object
-000194b0: 280a 2020 2020 2020 2020 2020 2020 6e61  (.            na
-000194c0: 6d65 3a20 4f70 7469 6f6e 616c 5b73 7472  me: Optional[str
-000194d0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-000194e0: 2020 2020 2020 736f 7572 6365 3a20 4f70        source: Op
-000194f0: 7469 6f6e 616c 5b73 746f 7261 6765 5f6c  tional[storage_l
-00019500: 6962 2e50 6174 685d 203d 204e 6f6e 652c  ib.Path] = None,
-00019510: 0a20 2020 2020 2020 2020 2020 2073 746f  .            sto
-00019520: 7265 733a 204f 7074 696f 6e61 6c5b 4469  res: Optional[Di
-00019530: 6374 5b73 746f 7261 6765 5f6c 6962 2e53  ct[storage_lib.S
-00019540: 746f 7265 5479 7065 2c0a 2020 2020 2020  toreType,.      
-00019550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019560: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
-00019570: 6167 655f 6c69 622e 4162 7374 7261 6374  age_lib.Abstract
-00019580: 5374 6f72 655d 5d20 3d20 4e6f 6e65 2c0a  Store]] = None,.
-00019590: 2020 2020 2020 2020 2020 2020 7065 7273              pers
-000195a0: 6973 7465 6e74 3a20 4f70 7469 6f6e 616c  istent: Optional
-000195b0: 5b62 6f6f 6c5d 203d 2054 7275 652c 0a20  [bool] = True,. 
-000195c0: 2020 2020 2020 2020 2020 206d 6f64 653a             mode:
-000195d0: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
-000195e0: 7261 6765 4d6f 6465 203d 2073 746f 7261  rageMode = stora
-000195f0: 6765 5f6c 6962 2e53 746f 7261 6765 4d6f  ge_lib.StorageMo
-00019600: 6465 2e4d 4f55 4e54 293a 0a20 2020 2020  de.MOUNT):.     
-00019610: 2020 2023 2043 7265 6174 6573 2061 2074     # Creates a t
-00019620: 656d 706f 7261 7279 2073 746f 7261 6765  emporary storage
-00019630: 206f 626a 6563 742e 2053 746f 7265 7320   object. Stores 
-00019640: 6d75 7374 2062 6520 6164 6465 6420 696e  must be added in
-00019650: 2074 6865 2074 6573 742e 0a20 2020 2020   the test..     
-00019660: 2020 2073 746f 7261 6765 5f6f 626a 203d     storage_obj =
-00019670: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
-00019680: 7261 6765 286e 616d 653d 6e61 6d65 2c0a  rage(name=name,.
-00019690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196b0: 2020 2020 2020 2020 2020 736f 7572 6365            source
-000196c0: 3d73 6f75 7263 652c 0a20 2020 2020 2020  =source,.       
-000196d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196f0: 2020 2073 746f 7265 733d 7374 6f72 6573     stores=stores
-00019700: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00019710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019720: 2020 2020 2020 2020 2020 2020 7065 7273              pers
-00019730: 6973 7465 6e74 3d70 6572 7369 7374 656e  istent=persisten
-00019740: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-00019750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019760: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00019770: 653d 6d6f 6465 290a 2020 2020 2020 2020  e=mode).        
-00019780: 7969 656c 6420 7374 6f72 6167 655f 6f62  yield storage_ob
-00019790: 6a0a 2020 2020 2020 2020 6861 6e64 6c65  j.        handle
-000197a0: 203d 2067 6c6f 6261 6c5f 7573 6572 5f73   = global_user_s
-000197b0: 7461 7465 2e67 6574 5f68 616e 646c 655f  tate.get_handle_
-000197c0: 6672 6f6d 5f73 746f 7261 6765 5f6e 616d  from_storage_nam
-000197d0: 6528 0a20 2020 2020 2020 2020 2020 2073  e(.            s
-000197e0: 746f 7261 6765 5f6f 626a 2e6e 616d 6529  torage_obj.name)
-000197f0: 0a20 2020 2020 2020 2069 6620 6861 6e64  .        if hand
-00019800: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-00019810: 2320 4966 2068 616e 646c 6520 6578 6973  # If handle exis
-00019820: 7473 2c20 6465 6c65 7465 206d 616e 7561  ts, delete manua
-00019830: 6c6c 790a 2020 2020 2020 2020 2020 2020  lly.            
-00019840: 2320 544f 444f 2872 6f6d 696c 6229 3a20  # TODO(romilb): 
-00019850: 5468 6973 2069 7320 706f 7465 6e74 6961  This is potentia
-00019860: 6c6c 7920 7269 736b 7920 2d20 6966 2074  lly risky - if t
-00019870: 6865 2064 656c 6574 6520 6d65 7468 6f64  he delete method
-00019880: 2068 6173 0a20 2020 2020 2020 2020 2020   has.           
-00019890: 2023 2020 2062 7567 732c 2074 6869 7320   #   bugs, this 
-000198a0: 6361 6e20 6361 7573 6520 7265 736f 7572  can cause resour
-000198b0: 6365 206c 6561 6b73 2e20 4964 6561 6c6c  ce leaks. Ideall
-000198c0: 7920 7765 2073 686f 756c 6420 6d61 6e75  y we should manu
-000198d0: 616c 6c79 0a20 2020 2020 2020 2020 2020  ally.           
-000198e0: 2023 2020 2065 6a65 6374 2073 746f 7261   #   eject stora
-000198f0: 6765 2066 726f 6d20 676c 6f62 616c 5f75  ge from global_u
-00019900: 7365 725f 7374 6174 6520 616e 6420 6465  ser_state and de
-00019910: 6c65 7465 2074 6865 2062 7563 6b65 7420  lete the bucket 
-00019920: 7573 696e 670a 2020 2020 2020 2020 2020  using.          
-00019930: 2020 2320 2020 626f 746f 3320 6469 7265    #   boto3 dire
-00019940: 6374 6c79 2e0a 2020 2020 2020 2020 2020  ctly..          
-00019950: 2020 7374 6f72 6167 655f 6f62 6a2e 6465    storage_obj.de
-00019960: 6c65 7465 2829 0a0a 2020 2020 4070 7974  lete()..    @pyt
-00019970: 6573 742e 6669 7874 7572 650a 2020 2020  est.fixture.    
-00019980: 6465 6620 746d 705f 7363 7261 7463 685f  def tmp_scratch_
-00019990: 7374 6f72 6167 655f 6f62 6a28 7365 6c66  storage_obj(self
-000199a0: 2c20 746d 705f 6275 636b 6574 5f6e 616d  , tmp_bucket_nam
-000199b0: 6529 3a0a 2020 2020 2020 2020 2320 4372  e):.        # Cr
-000199c0: 6561 7465 7320 6120 7374 6f72 6167 6520  eates a storage 
-000199d0: 6f62 6a65 6374 2077 6974 6820 6e6f 2073  object with no s
-000199e0: 6f75 7263 6520 746f 2063 7265 6174 6520  ource to create 
-000199f0: 6120 7363 7261 7463 6820 7374 6f72 6167  a scratch storag
-00019a00: 652e 0a20 2020 2020 2020 2023 2053 746f  e..        # Sto
-00019a10: 7265 7320 6d75 7374 2062 6520 6164 6465  res must be adde
-00019a20: 6420 696e 2074 6865 2074 6573 742e 0a20  d in the test.. 
-00019a30: 2020 2020 2020 2079 6965 6c64 2066 726f         yield fro
-00019a40: 6d20 7365 6c66 2e79 6965 6c64 5f73 746f  m self.yield_sto
-00019a50: 7261 6765 5f6f 626a 6563 7428 6e61 6d65  rage_object(name
-00019a60: 3d74 6d70 5f62 7563 6b65 745f 6e61 6d65  =tmp_bucket_name
-00019a70: 290a 0a20 2020 2040 7079 7465 7374 2e66  )..    @pytest.f
-00019a80: 6978 7475 7265 0a20 2020 2064 6566 2074  ixture.    def t
-00019a90: 6d70 5f6d 756c 7469 706c 655f 7363 7261  mp_multiple_scra
-00019aa0: 7463 685f 7374 6f72 6167 655f 6f62 6a28  tch_storage_obj(
-00019ab0: 7365 6c66 293a 0a20 2020 2020 2020 2023  self):.        #
-00019ac0: 2043 7265 6174 6573 2061 206c 6973 7420   Creates a list 
-00019ad0: 6f66 2035 2073 746f 7261 6765 206f 626a  of 5 storage obj
-00019ae0: 6563 7473 2077 6974 6820 6e6f 2073 6f75  ects with no sou
-00019af0: 7263 6520 746f 2063 7265 6174 650a 2020  rce to create.  
-00019b00: 2020 2020 2020 2320 6d75 6c74 6970 6c65        # multiple
-00019b10: 2073 6372 6174 6368 2073 746f 7261 6765   scratch storage
-00019b20: 732e 0a20 2020 2020 2020 2023 2053 746f  s..        # Sto
-00019b30: 7265 7320 666f 7220 6561 6368 206f 626a  res for each obj
-00019b40: 6563 7420 696e 2074 6865 206c 6973 7420  ect in the list 
-00019b50: 6d75 7374 2062 6520 6164 6465 6420 696e  must be added in
-00019b60: 2074 6865 2074 6573 742e 0a20 2020 2020   the test..     
-00019b70: 2020 2073 746f 7261 6765 5f6d 756c 745f     storage_mult_
-00019b80: 6f62 6a20 3d20 5b5d 0a20 2020 2020 2020  obj = [].       
-00019b90: 2066 6f72 205f 2069 6e20 7261 6e67 6528   for _ in range(
-00019ba0: 3529 3a0a 2020 2020 2020 2020 2020 2020  5):.            
-00019bb0: 7469 6d65 7374 616d 7020 3d20 7374 7228  timestamp = str(
-00019bc0: 7469 6d65 2e74 696d 6528 2929 2e72 6570  time.time()).rep
-00019bd0: 6c61 6365 2827 2e27 2c20 2727 290a 2020  lace('.', '').  
-00019be0: 2020 2020 2020 2020 2020 7374 6f72 655f            store_
-00019bf0: 6f62 6a20 3d20 7374 6f72 6167 655f 6c69  obj = storage_li
-00019c00: 622e 5374 6f72 6167 6528 6e61 6d65 3d66  b.Storage(name=f
-00019c10: 2773 6b79 2d74 6573 742d 7b74 696d 6573  'sky-test-{times
-00019c20: 7461 6d70 7d27 290a 2020 2020 2020 2020  tamp}').        
-00019c30: 2020 2020 7374 6f72 6167 655f 6d75 6c74      storage_mult
-00019c40: 5f6f 626a 2e61 7070 656e 6428 7374 6f72  _obj.append(stor
-00019c50: 655f 6f62 6a29 0a20 2020 2020 2020 2079  e_obj).        y
-00019c60: 6965 6c64 2073 746f 7261 6765 5f6d 756c  ield storage_mul
-00019c70: 745f 6f62 6a0a 2020 2020 2020 2020 666f  t_obj.        fo
-00019c80: 7220 7374 6f72 6167 655f 6f62 6a20 696e  r storage_obj in
-00019c90: 2073 746f 7261 6765 5f6d 756c 745f 6f62   storage_mult_ob
-00019ca0: 6a3a 0a20 2020 2020 2020 2020 2020 2068  j:.            h
-00019cb0: 616e 646c 6520 3d20 676c 6f62 616c 5f75  andle = global_u
-00019cc0: 7365 725f 7374 6174 652e 6765 745f 6861  ser_state.get_ha
-00019cd0: 6e64 6c65 5f66 726f 6d5f 7374 6f72 6167  ndle_from_storag
-00019ce0: 655f 6e61 6d65 280a 2020 2020 2020 2020  e_name(.        
-00019cf0: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
-00019d00: 6f62 6a2e 6e61 6d65 290a 2020 2020 2020  obj.name).      
-00019d10: 2020 2020 2020 6966 2068 616e 646c 653a        if handle:
-00019d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019d30: 2023 2049 6620 6861 6e64 6c65 2065 7869   # If handle exi
-00019d40: 7374 732c 2064 656c 6574 6520 6d61 6e75  sts, delete manu
-00019d50: 616c 6c79 0a20 2020 2020 2020 2020 2020  ally.           
-00019d60: 2020 2020 2023 2054 4f44 4f28 726f 6d69       # TODO(romi
-00019d70: 6c62 293a 2054 6869 7320 6973 2070 6f74  lb): This is pot
-00019d80: 656e 7469 616c 6c79 2072 6973 6b79 202d  entially risky -
-00019d90: 2069 6620 7468 6520 6465 6c65 7465 206d   if the delete m
-00019da0: 6574 686f 6420 6861 730a 2020 2020 2020  ethod has.      
-00019db0: 2020 2020 2020 2020 2020 2320 6275 6773            # bugs
-00019dc0: 2c20 7468 6973 2063 616e 2063 6175 7365  , this can cause
-00019dd0: 2072 6573 6f75 7263 6520 6c65 616b 732e   resource leaks.
-00019de0: 2049 6465 616c 6c79 2077 6520 7368 6f75   Ideally we shou
-00019df0: 6c64 206d 616e 7561 6c6c 790a 2020 2020  ld manually.    
-00019e00: 2020 2020 2020 2020 2020 2020 2320 656a              # ej
-00019e10: 6563 7420 7374 6f72 6167 6520 6672 6f6d  ect storage from
-00019e20: 2067 6c6f 6261 6c5f 7573 6572 5f73 7461   global_user_sta
-00019e30: 7465 2061 6e64 2064 656c 6574 6520 7468  te and delete th
-00019e40: 6520 6275 636b 6574 2075 7369 6e67 0a20  e bucket using. 
-00019e50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00019e60: 2062 6f74 6f33 2064 6972 6563 746c 792e   boto3 directly.
-00019e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019e80: 2073 746f 7261 6765 5f6f 626a 2e64 656c   storage_obj.del
-00019e90: 6574 6528 290a 0a20 2020 2040 7079 7465  ete()..    @pyte
-00019ea0: 7374 2e66 6978 7475 7265 0a20 2020 2064  st.fixture.    d
-00019eb0: 6566 2074 6d70 5f6c 6f63 616c 5f73 746f  ef tmp_local_sto
-00019ec0: 7261 6765 5f6f 626a 2873 656c 662c 2074  rage_obj(self, t
-00019ed0: 6d70 5f62 7563 6b65 745f 6e61 6d65 2c20  mp_bucket_name, 
-00019ee0: 746d 705f 736f 7572 6365 293a 0a20 2020  tmp_source):.   
-00019ef0: 2020 2020 2023 2043 7265 6174 6573 2061       # Creates a
-00019f00: 2074 656d 706f 7261 7279 2073 746f 7261   temporary stora
-00019f10: 6765 206f 626a 6563 742e 2053 746f 7265  ge object. Store
-00019f20: 7320 6d75 7374 2062 6520 6164 6465 6420  s must be added 
-00019f30: 696e 2074 6865 2074 6573 742e 0a20 2020  in the test..   
-00019f40: 2020 2020 2079 6965 6c64 2066 726f 6d20       yield from 
-00019f50: 7365 6c66 2e79 6965 6c64 5f73 746f 7261  self.yield_stora
-00019f60: 6765 5f6f 626a 6563 7428 6e61 6d65 3d74  ge_object(name=t
-00019f70: 6d70 5f62 7563 6b65 745f 6e61 6d65 2c0a  mp_bucket_name,.
-00019f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019fa0: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
-00019fb0: 7263 653d 746d 705f 736f 7572 6365 290a  rce=tmp_source).
-00019fc0: 0a20 2020 2040 7079 7465 7374 2e66 6978  .    @pytest.fix
-00019fd0: 7475 7265 0a20 2020 2064 6566 2074 6d70  ture.    def tmp
-00019fe0: 5f6c 6f63 616c 5f6c 6973 745f 7374 6f72  _local_list_stor
-00019ff0: 6167 655f 6f62 6a28 7365 6c66 2c20 746d  age_obj(self, tm
-0001a000: 705f 6275 636b 6574 5f6e 616d 652c 2074  p_bucket_name, t
-0001a010: 6d70 5f73 6f75 7263 6529 3a0a 2020 2020  mp_source):.    
-0001a020: 2020 2020 2320 4372 6561 7465 7320 6120      # Creates a 
-0001a030: 7465 6d70 2073 746f 7261 6765 206f 626a  temp storage obj
-0001a040: 6563 7420 7768 6963 6820 7573 6573 2061  ect which uses a
-0001a050: 206c 6973 7420 6f66 2070 6174 6873 2061   list of paths a
-0001a060: 7320 736f 7572 6365 2e0a 2020 2020 2020  s source..      
-0001a070: 2020 2320 5374 6f72 6573 206d 7573 7420    # Stores must 
-0001a080: 6265 2061 6464 6564 2069 6e20 7468 6520  be added in the 
-0001a090: 7465 7374 2e20 4166 7465 7220 7570 6c6f  test. After uplo
-0001a0a0: 6164 2c20 7468 6520 6275 636b 6574 2073  ad, the bucket s
-0001a0b0: 686f 756c 640a 2020 2020 2020 2020 2320  hould.        # 
-0001a0c0: 6861 7665 2074 776f 2066 696c 6573 202d  have two files -
-0001a0d0: 202f 746d 702d 6669 6c65 2061 6e64 202f   /tmp-file and /
-0001a0e0: 746d 702d 736f 7572 6365 2f74 6d70 2d66  tmp-source/tmp-f
-0001a0f0: 696c 650a 2020 2020 2020 2020 6c69 7374  ile.        list
-0001a100: 5f73 6f75 7263 6520 3d20 5b74 6d70 5f73  _source = [tmp_s
-0001a110: 6f75 7263 652c 2074 6d70 5f73 6f75 7263  ource, tmp_sourc
-0001a120: 6520 2b20 272f 746d 702d 6669 6c65 275d  e + '/tmp-file']
-0001a130: 0a20 2020 2020 2020 2079 6965 6c64 2066  .        yield f
-0001a140: 726f 6d20 7365 6c66 2e79 6965 6c64 5f73  rom self.yield_s
-0001a150: 746f 7261 6765 5f6f 626a 6563 7428 6e61  torage_object(na
-0001a160: 6d65 3d74 6d70 5f62 7563 6b65 745f 6e61  me=tmp_bucket_na
-0001a170: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-0001a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a1a0: 2073 6f75 7263 653d 6c69 7374 5f73 6f75   source=list_sou
-0001a1b0: 7263 6529 0a0a 2020 2020 4070 7974 6573  rce)..    @pytes
-0001a1c0: 742e 6669 7874 7572 650a 2020 2020 6465  t.fixture.    de
-0001a1d0: 6620 746d 705f 6275 6c6b 5f64 656c 5f73  f tmp_bulk_del_s
-0001a1e0: 746f 7261 6765 5f6f 626a 2873 656c 662c  torage_obj(self,
-0001a1f0: 2074 6d70 5f62 7563 6b65 745f 6e61 6d65   tmp_bucket_name
-0001a200: 293a 0a20 2020 2020 2020 2023 2043 7265  ):.        # Cre
-0001a210: 6174 6573 2061 2074 656d 706f 7261 7279  ates a temporary
-0001a220: 2073 746f 7261 6765 206f 626a 6563 7420   storage object 
-0001a230: 666f 7220 7465 7374 696e 6720 6275 6c6b  for testing bulk
-0001a240: 2064 656c 6574 696f 6e2e 0a20 2020 2020   deletion..     
-0001a250: 2020 2023 2053 746f 7265 7320 6d75 7374     # Stores must
-0001a260: 2062 6520 6164 6465 6420 696e 2074 6865   be added in the
-0001a270: 2074 6573 742e 0a20 2020 2020 2020 2077   test..        w
-0001a280: 6974 6820 7465 6d70 6669 6c65 2e54 656d  ith tempfile.Tem
-0001a290: 706f 7261 7279 4469 7265 6374 6f72 7928  poraryDirectory(
-0001a2a0: 2920 6173 2074 6d70 6469 723a 0a20 2020  ) as tmpdir:.   
-0001a2b0: 2020 2020 2020 2020 2073 7562 7072 6f63           subproc
-0001a2c0: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
-0001a2d0: 2866 276d 6b64 6972 202d 7020 7b74 6d70  (f'mkdir -p {tmp
-0001a2e0: 6469 727d 2f66 6f6c 6465 727b 7b30 3030  dir}/folder{{000
-0001a2f0: 2e2e 3235 357d 7d27 2c0a 2020 2020 2020  ..255}}',.      
-0001a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a310: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-0001a320: 656c 6c3d 5472 7565 290a 2020 2020 2020  ell=True).      
-0001a330: 2020 2020 2020 7375 6270 726f 6365 7373        subprocess
-0001a340: 2e63 6865 636b 5f6f 7574 7075 7428 6627  .check_output(f'
-0001a350: 746f 7563 6820 7b74 6d70 6469 727d 2f74  touch {tmpdir}/t
-0001a360: 6573 747b 7b30 3030 2e2e 3235 357d 7d2e  est{{000..255}}.
-0001a370: 7478 7427 2c0a 2020 2020 2020 2020 2020  txt',.          
-0001a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a390: 2020 2020 2020 2020 2020 7368 656c 6c3d            shell=
-0001a3a0: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-0001a3b0: 2020 7375 6270 726f 6365 7373 2e63 6865    subprocess.che
-0001a3c0: 636b 5f6f 7574 7075 7428 0a20 2020 2020  ck_output(.     
-0001a3d0: 2020 2020 2020 2020 2020 2066 2774 6f75             f'tou
-0001a3e0: 6368 207b 746d 7064 6972 7d2f 666f 6c64  ch {tmpdir}/fold
-0001a3f0: 6572 7b7b 3030 302e 2e32 3535 7d7d 2f74  er{{000..255}}/t
-0001a400: 6573 742e 7478 7427 2c20 7368 656c 6c3d  est.txt', shell=
-0001a410: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-0001a420: 2020 7969 656c 6420 6672 6f6d 2073 656c    yield from sel
-0001a430: 662e 7969 656c 645f 7374 6f72 6167 655f  f.yield_storage_
-0001a440: 6f62 6a65 6374 286e 616d 653d 746d 705f  object(name=tmp_
-0001a450: 6275 636b 6574 5f6e 616d 652c 0a20 2020  bucket_name,.   
-0001a460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a480: 2020 2020 2020 2020 2020 2020 2020 736f                so
-0001a490: 7572 6365 3d74 6d70 6469 7229 0a0a 2020  urce=tmpdir)..  
-0001a4a0: 2020 4070 7974 6573 742e 6669 7874 7572    @pytest.fixtur
-0001a4b0: 650a 2020 2020 6465 6620 746d 705f 636f  e.    def tmp_co
-0001a4c0: 7079 5f6d 6e74 5f65 7869 7374 696e 675f  py_mnt_existing_
-0001a4d0: 7374 6f72 6167 655f 6f62 6a28 7365 6c66  storage_obj(self
-0001a4e0: 2c20 746d 705f 7363 7261 7463 685f 7374  , tmp_scratch_st
-0001a4f0: 6f72 6167 655f 6f62 6a29 3a0a 2020 2020  orage_obj):.    
-0001a500: 2020 2020 2320 4372 6561 7465 7320 6120      # Creates a 
-0001a510: 636f 7079 206d 6f75 6e74 2073 746f 7261  copy mount stora
-0001a520: 6765 2077 6869 6368 2072 6575 7365 7320  ge which reuses 
-0001a530: 616e 2065 7869 7374 696e 6720 7374 6f72  an existing stor
-0001a540: 6167 6520 6f62 6a65 6374 2e0a 2020 2020  age object..    
-0001a550: 2020 2020 746d 705f 7363 7261 7463 685f      tmp_scratch_
-0001a560: 7374 6f72 6167 655f 6f62 6a2e 6164 645f  storage_obj.add_
-0001a570: 7374 6f72 6528 7374 6f72 6167 655f 6c69  store(storage_li
-0001a580: 622e 5374 6f72 6554 7970 652e 5333 290a  b.StoreType.S3).
-0001a590: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
-0001a5a0: 6e61 6d65 203d 2074 6d70 5f73 6372 6174  name = tmp_scrat
-0001a5b0: 6368 5f73 746f 7261 6765 5f6f 626a 2e6e  ch_storage_obj.n
-0001a5c0: 616d 650a 0a20 2020 2020 2020 2023 2054  ame..        # T
-0001a5d0: 7279 2074 6f20 696e 6974 6961 6c69 7a65  ry to initialize
-0001a5e0: 2061 6e6f 7468 6572 2073 746f 7261 6765   another storage
-0001a5f0: 2077 6974 6820 7468 6520 7374 6f72 6167   with the storag
-0001a600: 6520 6f62 6a65 6374 2063 7265 6174 6564  e object created
-0001a610: 0a20 2020 2020 2020 2023 2061 626f 7665  .        # above
-0001a620: 2c20 6275 7420 6e6f 7720 696e 2043 4f50  , but now in COP
-0001a630: 5920 6d6f 6465 2e20 5468 6973 2073 686f  Y mode. This sho
-0001a640: 756c 6420 7375 6363 6565 642e 0a20 2020  uld succeed..   
-0001a650: 2020 2020 2079 6965 6c64 2066 726f 6d20       yield from 
-0001a660: 7365 6c66 2e79 6965 6c64 5f73 746f 7261  self.yield_stora
-0001a670: 6765 5f6f 626a 6563 7428 6e61 6d65 3d73  ge_object(name=s
-0001a680: 746f 7261 6765 5f6e 616d 652c 0a20 2020  torage_name,.   
-0001a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6b0: 2020 2020 2020 2020 2020 6d6f 6465 3d73            mode=s
-0001a6c0: 746f 7261 6765 5f6c 6962 2e53 746f 7261  torage_lib.Stora
-0001a6d0: 6765 4d6f 6465 2e43 4f50 5929 0a0a 2020  geMode.COPY)..  
-0001a6e0: 2020 4070 7974 6573 742e 6669 7874 7572    @pytest.fixtur
-0001a6f0: 650a 2020 2020 6465 6620 746d 705f 6177  e.    def tmp_aw
-0001a700: 7363 6c69 5f62 7563 6b65 7428 7365 6c66  scli_bucket(self
-0001a710: 2c20 746d 705f 6275 636b 6574 5f6e 616d  , tmp_bucket_nam
-0001a720: 6529 3a0a 2020 2020 2020 2020 2320 4372  e):.        # Cr
-0001a730: 6561 7465 7320 6120 7465 6d70 6f72 6172  eates a temporar
-0001a740: 7920 6275 636b 6574 2075 7369 6e67 2061  y bucket using a
-0001a750: 7773 636c 690a 2020 2020 2020 2020 7375  wscli.        su
-0001a760: 6270 726f 6365 7373 2e63 6865 636b 5f63  bprocess.check_c
-0001a770: 616c 6c28 5b27 6177 7327 2c20 2773 3327  all(['aws', 's3'
-0001a780: 2c20 276d 6227 2c20 6627 7333 3a2f 2f7b  , 'mb', f's3://{
-0001a790: 746d 705f 6275 636b 6574 5f6e 616d 657d  tmp_bucket_name}
-0001a7a0: 275d 290a 2020 2020 2020 2020 7969 656c  ']).        yiel
-0001a7b0: 6420 746d 705f 6275 636b 6574 5f6e 616d  d tmp_bucket_nam
-0001a7c0: 650a 2020 2020 2020 2020 7375 6270 726f  e.        subpro
-0001a7d0: 6365 7373 2e63 6865 636b 5f63 616c 6c28  cess.check_call(
-0001a7e0: 0a20 2020 2020 2020 2020 2020 205b 2761  .            ['a
-0001a7f0: 7773 272c 2027 7333 272c 2027 7262 272c  ws', 's3', 'rb',
-0001a800: 2066 2773 333a 2f2f 7b74 6d70 5f62 7563   f's3://{tmp_buc
-0001a810: 6b65 745f 6e61 6d65 7d27 2c20 272d 2d66  ket_name}', '--f
-0001a820: 6f72 6365 275d 290a 0a20 2020 2040 7079  orce'])..    @py
-0001a830: 7465 7374 2e66 6978 7475 7265 0a20 2020  test.fixture.   
-0001a840: 2064 6566 2074 6d70 5f67 7375 7469 6c5f   def tmp_gsutil_
-0001a850: 6275 636b 6574 2873 656c 662c 2074 6d70  bucket(self, tmp
-0001a860: 5f62 7563 6b65 745f 6e61 6d65 293a 0a20  _bucket_name):. 
-0001a870: 2020 2020 2020 2023 2043 7265 6174 6573         # Creates
-0001a880: 2061 2074 656d 706f 7261 7279 2062 7563   a temporary buc
-0001a890: 6b65 7420 7573 696e 6720 6773 7574 696c  ket using gsutil
-0001a8a0: 0a20 2020 2020 2020 2073 7562 7072 6f63  .        subproc
-0001a8b0: 6573 732e 6368 6563 6b5f 6361 6c6c 285b  ess.check_call([
-0001a8c0: 2767 7375 7469 6c27 2c20 276d 6227 2c20  'gsutil', 'mb', 
-0001a8d0: 6627 6773 3a2f 2f7b 746d 705f 6275 636b  f'gs://{tmp_buck
-0001a8e0: 6574 5f6e 616d 657d 275d 290a 2020 2020  et_name}']).    
-0001a8f0: 2020 2020 7969 656c 6420 746d 705f 6275      yield tmp_bu
-0001a900: 636b 6574 5f6e 616d 650a 2020 2020 2020  cket_name.      
-0001a910: 2020 7375 6270 726f 6365 7373 2e63 6865    subprocess.che
-0001a920: 636b 5f63 616c 6c28 5b27 6773 7574 696c  ck_call(['gsutil
-0001a930: 272c 2027 726d 272c 2027 2d72 272c 2066  ', 'rm', '-r', f
-0001a940: 2767 733a 2f2f 7b74 6d70 5f62 7563 6b65  'gs://{tmp_bucke
-0001a950: 745f 6e61 6d65 7d27 5d29 0a0a 2020 2020  t_name}'])..    
-0001a960: 4070 7974 6573 742e 6669 7874 7572 650a  @pytest.fixture.
-0001a970: 2020 2020 6465 6620 746d 705f 6177 7363      def tmp_awsc
-0001a980: 6c69 5f62 7563 6b65 745f 7232 2873 656c  li_bucket_r2(sel
-0001a990: 662c 2074 6d70 5f62 7563 6b65 745f 6e61  f, tmp_bucket_na
-0001a9a0: 6d65 293a 0a20 2020 2020 2020 2023 2043  me):.        # C
-0001a9b0: 7265 6174 6573 2061 2074 656d 706f 7261  reates a tempora
-0001a9c0: 7279 2062 7563 6b65 7420 7573 696e 6720  ry bucket using 
-0001a9d0: 6177 7363 6c69 0a20 2020 2020 2020 2065  awscli.        e
-0001a9e0: 6e64 706f 696e 745f 7572 6c20 3d20 636c  ndpoint_url = cl
-0001a9f0: 6f75 6466 6c61 7265 2e63 7265 6174 655f  oudflare.create_
-0001aa00: 656e 6470 6f69 6e74 2829 0a20 2020 2020  endpoint().     
-0001aa10: 2020 2073 7562 7072 6f63 6573 732e 6368     subprocess.ch
-0001aa20: 6563 6b5f 6361 6c6c 280a 2020 2020 2020  eck_call(.      
-0001aa30: 2020 2020 2020 6627 4157 535f 5348 4152        f'AWS_SHAR
-0001aa40: 4544 5f43 5245 4445 4e54 4941 4c53 5f46  ED_CREDENTIALS_F
-0001aa50: 494c 453d 7b63 6c6f 7564 666c 6172 652e  ILE={cloudflare.
-0001aa60: 5232 5f43 5245 4445 4e54 4941 4c53 5f50  R2_CREDENTIALS_P
-0001aa70: 4154 487d 2061 7773 2073 3320 6d62 2073  ATH} aws s3 mb s
-0001aa80: 333a 2f2f 7b74 6d70 5f62 7563 6b65 745f  3://{tmp_bucket_
-0001aa90: 6e61 6d65 7d20 2d2d 656e 6470 6f69 6e74  name} --endpoint
-0001aaa0: 207b 656e 6470 6f69 6e74 5f75 726c 7d20   {endpoint_url} 
-0001aab0: 2d2d 7072 6f66 696c 653d 7232 272c 0a20  --profile=r2',. 
-0001aac0: 2020 2020 2020 2020 2020 2073 6865 6c6c             shell
-0001aad0: 3d54 7275 6529 0a20 2020 2020 2020 2079  =True).        y
-0001aae0: 6965 6c64 2074 6d70 5f62 7563 6b65 745f  ield tmp_bucket_
-0001aaf0: 6e61 6d65 0a20 2020 2020 2020 2073 7562  name.        sub
-0001ab00: 7072 6f63 6573 732e 6368 6563 6b5f 6361  process.check_ca
-0001ab10: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
-0001ab20: 6627 4157 535f 5348 4152 4544 5f43 5245  f'AWS_SHARED_CRE
-0001ab30: 4445 4e54 4941 4c53 5f46 494c 453d 7b63  DENTIALS_FILE={c
-0001ab40: 6c6f 7564 666c 6172 652e 5232 5f43 5245  loudflare.R2_CRE
-0001ab50: 4445 4e54 4941 4c53 5f50 4154 487d 2061  DENTIALS_PATH} a
-0001ab60: 7773 2073 3320 7262 2073 333a 2f2f 7b74  ws s3 rb s3://{t
-0001ab70: 6d70 5f62 7563 6b65 745f 6e61 6d65 7d20  mp_bucket_name} 
-0001ab80: 2d2d 666f 7263 6520 2d2d 656e 6470 6f69  --force --endpoi
-0001ab90: 6e74 207b 656e 6470 6f69 6e74 5f75 726c  nt {endpoint_url
-0001aba0: 7d20 2d2d 7072 6f66 696c 653d 7232 272c  } --profile=r2',
-0001abb0: 0a20 2020 2020 2020 2020 2020 2073 6865  .            she
-0001abc0: 6c6c 3d54 7275 6529 0a0a 2020 2020 4070  ll=True)..    @p
-0001abd0: 7974 6573 742e 6669 7874 7572 650a 2020  ytest.fixture.  
-0001abe0: 2020 6465 6620 746d 705f 7075 626c 6963    def tmp_public
-0001abf0: 5f73 746f 7261 6765 5f6f 626a 2873 656c  _storage_obj(sel
-0001ac00: 662c 2072 6571 7565 7374 293a 0a20 2020  f, request):.   
-0001ac10: 2020 2020 2023 2049 6e69 7469 616c 697a       # Initializ
-0001ac20: 6573 2061 2073 746f 7261 6765 206f 626a  es a storage obj
-0001ac30: 6563 7420 7769 7468 2061 2070 7562 6c69  ect with a publi
-0001ac40: 6320 6275 636b 6574 0a20 2020 2020 2020  c bucket.       
-0001ac50: 2073 746f 7261 6765 5f6f 626a 203d 2073   storage_obj = s
-0001ac60: 746f 7261 6765 5f6c 6962 2e53 746f 7261  torage_lib.Stora
-0001ac70: 6765 2873 6f75 7263 653d 7265 7175 6573  ge(source=reques
-0001ac80: 742e 7061 7261 6d29 0a20 2020 2020 2020  t.param).       
-0001ac90: 2079 6965 6c64 2073 746f 7261 6765 5f6f   yield storage_o
-0001aca0: 626a 0a20 2020 2020 2020 2023 2054 6869  bj.        # Thi
-0001acb0: 7320 646f 6573 206e 6f74 2072 6571 7569  s does not requi
-0001acc0: 7265 2061 6e79 2064 656c 6574 696f 6e20  re any deletion 
-0001acd0: 6c6f 6769 6320 6265 6361 7573 6520 6974  logic because it
-0001ace0: 2069 7320 6120 7075 626c 6963 2062 7563   is a public buc
-0001acf0: 6b65 740a 2020 2020 2020 2020 2320 616e  ket.        # an
-0001ad00: 6420 7368 6f75 6c64 206e 6f74 2067 6574  d should not get
-0001ad10: 2061 6464 6564 2074 6f20 676c 6f62 616c   added to global
-0001ad20: 5f75 7365 725f 7374 6174 652e 0a0a 2020  _user_state...  
-0001ad30: 2020 4070 7974 6573 742e 6d61 726b 2e70    @pytest.mark.p
-0001ad40: 6172 616d 6574 7269 7a65 2827 7374 6f72  arametrize('stor
-0001ad50: 655f 7479 7065 272c 205b 0a20 2020 2020  e_type', [.     
-0001ad60: 2020 2073 746f 7261 6765 5f6c 6962 2e53     storage_lib.S
-0001ad70: 746f 7265 5479 7065 2e53 332c 2073 746f  toreType.S3, sto
-0001ad80: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
-0001ad90: 7065 2e47 4353 2c0a 2020 2020 2020 2020  pe.GCS,.        
-0001ada0: 7079 7465 7374 2e70 6172 616d 2873 746f  pytest.param(sto
-0001adb0: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
-0001adc0: 7065 2e52 322c 206d 6172 6b73 3d70 7974  pe.R2, marks=pyt
-0001add0: 6573 742e 6d61 726b 2e63 6c6f 7564 666c  est.mark.cloudfl
-0001ade0: 6172 6529 0a20 2020 205d 290a 2020 2020  are).    ]).    
-0001adf0: 6465 6620 7465 7374 5f6e 6577 5f62 7563  def test_new_buc
-0001ae00: 6b65 745f 6372 6561 7469 6f6e 5f61 6e64  ket_creation_and
-0001ae10: 5f64 656c 6574 696f 6e28 7365 6c66 2c20  _deletion(self, 
-0001ae20: 746d 705f 6c6f 6361 6c5f 7374 6f72 6167  tmp_local_storag
-0001ae30: 655f 6f62 6a2c 0a20 2020 2020 2020 2020  e_obj,.         
-0001ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae60: 2020 2020 2073 746f 7265 5f74 7970 6529       store_type)
-0001ae70: 3a0a 2020 2020 2020 2020 2320 4372 6561  :.        # Crea
-0001ae80: 7465 7320 6120 6e65 7720 6275 636b 6574  tes a new bucket
-0001ae90: 2077 6974 6820 6120 6c6f 6361 6c20 736f   with a local so
-0001aea0: 7572 6365 2c20 7570 6c6f 6164 7320 6669  urce, uploads fi
-0001aeb0: 6c65 7320 746f 2069 740a 2020 2020 2020  les to it.      
-0001aec0: 2020 2320 616e 6420 6465 6c65 7465 7320    # and deletes 
-0001aed0: 6974 2e0a 2020 2020 2020 2020 746d 705f  it..        tmp_
-0001aee0: 6c6f 6361 6c5f 7374 6f72 6167 655f 6f62  local_storage_ob
-0001aef0: 6a2e 6164 645f 7374 6f72 6528 7374 6f72  j.add_store(stor
-0001af00: 655f 7479 7065 290a 0a20 2020 2020 2020  e_type)..       
-0001af10: 2023 2052 756e 2073 6b79 2073 746f 7261   # Run sky stora
-0001af20: 6765 206c 7320 746f 2063 6865 636b 2069  ge ls to check i
-0001af30: 6620 7374 6f72 6167 6520 6f62 6a65 6374  f storage object
-0001af40: 2065 7869 7374 7320 696e 2074 6865 206f   exists in the o
-0001af50: 7574 7075 740a 2020 2020 2020 2020 6f75  utput.        ou
-0001af60: 7420 3d20 7375 6270 726f 6365 7373 2e63  t = subprocess.c
-0001af70: 6865 636b 5f6f 7574 7075 7428 5b27 736b  heck_output(['sk
-0001af80: 7927 2c20 2773 746f 7261 6765 272c 2027  y', 'storage', '
-0001af90: 6c73 275d 290a 2020 2020 2020 2020 6173  ls']).        as
-0001afa0: 7365 7274 2074 6d70 5f6c 6f63 616c 5f73  sert tmp_local_s
-0001afb0: 746f 7261 6765 5f6f 626a 2e6e 616d 6520  torage_obj.name 
-0001afc0: 696e 206f 7574 2e64 6563 6f64 6528 2775  in out.decode('u
-0001afd0: 7466 2d38 2729 0a0a 2020 2020 2020 2020  tf-8')..        
-0001afe0: 2320 5275 6e20 736b 7920 7374 6f72 6167  # Run sky storag
-0001aff0: 6520 6465 6c65 7465 2074 6f20 6465 6c65  e delete to dele
-0001b000: 7465 2074 6865 2073 746f 7261 6765 206f  te the storage o
-0001b010: 626a 6563 740a 2020 2020 2020 2020 7375  bject.        su
-0001b020: 6270 726f 6365 7373 2e63 6865 636b 5f6f  bprocess.check_o
-0001b030: 7574 7075 7428 0a20 2020 2020 2020 2020  utput(.         
-0001b040: 2020 205b 2773 6b79 272c 2027 7374 6f72     ['sky', 'stor
-0001b050: 6167 6527 2c20 2764 656c 6574 6527 2c20  age', 'delete', 
-0001b060: 746d 705f 6c6f 6361 6c5f 7374 6f72 6167  tmp_local_storag
-0001b070: 655f 6f62 6a2e 6e61 6d65 5d29 0a0a 2020  e_obj.name])..  
-0001b080: 2020 2020 2020 2320 5275 6e20 736b 7920        # Run sky 
-0001b090: 7374 6f72 6167 6520 6c73 2074 6f20 6368  storage ls to ch
-0001b0a0: 6563 6b20 6966 2073 746f 7261 6765 206f  eck if storage o
-0001b0b0: 626a 6563 7420 6973 2064 656c 6574 6564  bject is deleted
-0001b0c0: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
-0001b0d0: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
-0001b0e0: 6f75 7470 7574 285b 2773 6b79 272c 2027  output(['sky', '
-0001b0f0: 7374 6f72 6167 6527 2c20 276c 7327 5d29  storage', 'ls'])
-0001b100: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0001b110: 746d 705f 6c6f 6361 6c5f 7374 6f72 6167  tmp_local_storag
-0001b120: 655f 6f62 6a2e 6e61 6d65 206e 6f74 2069  e_obj.name not i
-0001b130: 6e20 6f75 742e 6465 636f 6465 2827 7574  n out.decode('ut
-0001b140: 662d 3827 290a 0a20 2020 2040 7079 7465  f-8')..    @pyte
-0001b150: 7374 2e6d 6172 6b2e 7864 6973 745f 6772  st.mark.xdist_gr
-0001b160: 6f75 7028 276d 756c 7469 706c 655f 6275  oup('multiple_bu
-0001b170: 636b 6574 5f64 656c 6574 696f 6e27 290a  cket_deletion').
-0001b180: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-0001b190: 2e70 6172 616d 6574 7269 7a65 2827 7374  .parametrize('st
-0001b1a0: 6f72 655f 7479 7065 272c 205b 0a20 2020  ore_type', [.   
-0001b1b0: 2020 2020 2073 746f 7261 6765 5f6c 6962       storage_lib
-0001b1c0: 2e53 746f 7265 5479 7065 2e53 332c 2073  .StoreType.S3, s
-0001b1d0: 746f 7261 6765 5f6c 6962 2e53 746f 7265  torage_lib.Store
-0001b1e0: 5479 7065 2e47 4353 2c0a 2020 2020 2020  Type.GCS,.      
-0001b1f0: 2020 7079 7465 7374 2e70 6172 616d 2873    pytest.param(s
-0001b200: 746f 7261 6765 5f6c 6962 2e53 746f 7265  torage_lib.Store
-0001b210: 5479 7065 2e52 322c 206d 6172 6b73 3d70  Type.R2, marks=p
-0001b220: 7974 6573 742e 6d61 726b 2e63 6c6f 7564  ytest.mark.cloud
-0001b230: 666c 6172 6529 0a20 2020 205d 290a 2020  flare).    ]).  
-0001b240: 2020 6465 6620 7465 7374 5f6d 756c 7469    def test_multi
-0001b250: 706c 655f 6275 636b 6574 735f 6372 6561  ple_buckets_crea
-0001b260: 7469 6f6e 5f61 6e64 5f64 656c 6574 696f  tion_and_deletio
-0001b270: 6e28 0a20 2020 2020 2020 2020 2020 2073  n(.            s
-0001b280: 656c 662c 2074 6d70 5f6d 756c 7469 706c  elf, tmp_multipl
-0001b290: 655f 7363 7261 7463 685f 7374 6f72 6167  e_scratch_storag
-0001b2a0: 655f 6f62 6a2c 2073 746f 7265 5f74 7970  e_obj, store_typ
-0001b2b0: 6529 3a0a 2020 2020 2020 2020 2320 4372  e):.        # Cr
-0001b2c0: 6561 7465 7320 6d75 6c74 6970 6c65 206e  eates multiple n
-0001b2d0: 6577 2062 7563 6b65 7473 2835 2062 7563  ew buckets(5 buc
-0001b2e0: 6b65 7473 2920 7769 7468 2061 206c 6f63  kets) with a loc
-0001b2f0: 616c 2073 6f75 7263 650a 2020 2020 2020  al source.      
-0001b300: 2020 2320 616e 6420 6465 6c65 7465 7320    # and deletes 
-0001b310: 7468 656d 2e0a 2020 2020 2020 2020 7374  them..        st
-0001b320: 6f72 6167 655f 6f62 6a5f 6e61 6d65 203d  orage_obj_name =
-0001b330: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
-0001b340: 7374 6f72 655f 6f62 6a20 696e 2074 6d70  store_obj in tmp
-0001b350: 5f6d 756c 7469 706c 655f 7363 7261 7463  _multiple_scratc
-0001b360: 685f 7374 6f72 6167 655f 6f62 6a3a 0a20  h_storage_obj:. 
-0001b370: 2020 2020 2020 2020 2020 2073 746f 7265             store
-0001b380: 5f6f 626a 2e61 6464 5f73 746f 7265 2873  _obj.add_store(s
-0001b390: 746f 7265 5f74 7970 6529 0a20 2020 2020  tore_type).     
-0001b3a0: 2020 2020 2020 2073 746f 7261 6765 5f6f         storage_o
-0001b3b0: 626a 5f6e 616d 652e 6170 7065 6e64 2873  bj_name.append(s
-0001b3c0: 746f 7265 5f6f 626a 2e6e 616d 6529 0a0a  tore_obj.name)..
-0001b3d0: 2020 2020 2020 2020 2320 5275 6e20 736b          # Run sk
-0001b3e0: 7920 7374 6f72 6167 6520 6c73 2074 6f20  y storage ls to 
-0001b3f0: 6368 6563 6b20 6966 2061 6c6c 2073 746f  check if all sto
-0001b400: 7261 6765 206f 626a 6563 7473 2065 7869  rage objects exi
-0001b410: 7374 7320 696e 2074 6865 0a20 2020 2020  sts in the.     
-0001b420: 2020 2023 206f 7574 7075 7420 6669 6c74     # output filt
-0001b430: 6572 6564 2062 7920 7374 6f72 6520 7479  ered by store ty
-0001b440: 7065 0a20 2020 2020 2020 206f 7574 5f61  pe.        out_a
-0001b450: 6c6c 203d 2073 7562 7072 6f63 6573 732e  ll = subprocess.
-0001b460: 6368 6563 6b5f 6f75 7470 7574 285b 2773  check_output(['s
-0001b470: 6b79 272c 2027 7374 6f72 6167 6527 2c20  ky', 'storage', 
-0001b480: 276c 7327 5d29 0a20 2020 2020 2020 206f  'ls']).        o
-0001b490: 7574 203d 205b 0a20 2020 2020 2020 2020  ut = [.         
-0001b4a0: 2020 2069 7465 6d2e 7370 6c69 7428 295b     item.split()[
-0001b4b0: 305d 0a20 2020 2020 2020 2020 2020 2066  0].            f
-0001b4c0: 6f72 2069 7465 6d20 696e 206f 7574 5f61  or item in out_a
-0001b4d0: 6c6c 2e64 6563 6f64 6528 2775 7466 2d38  ll.decode('utf-8
-0001b4e0: 2729 2e73 706c 6974 6c69 6e65 7328 290a  ').splitlines().
-0001b4f0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0001b500: 746f 7265 5f74 7970 652e 7661 6c75 6520  tore_type.value 
-0001b510: 696e 2069 7465 6d0a 2020 2020 2020 2020  in item.        
-0001b520: 5d0a 2020 2020 2020 2020 6173 7365 7274  ].        assert
-0001b530: 2061 6c6c 285b 6974 656d 2069 6e20 6f75   all([item in ou
-0001b540: 7420 666f 7220 6974 656d 2069 6e20 7374  t for item in st
-0001b550: 6f72 6167 655f 6f62 6a5f 6e61 6d65 5d29  orage_obj_name])
-0001b560: 0a0a 2020 2020 2020 2020 2320 5275 6e20  ..        # Run 
-0001b570: 736b 7920 7374 6f72 6167 6520 6465 6c65  sky storage dele
-0001b580: 7465 2061 6c6c 2074 6f20 6465 6c65 7465  te all to delete
-0001b590: 2061 6c6c 2073 746f 7261 6765 206f 626a   all storage obj
-0001b5a0: 6563 7473 0a20 2020 2020 2020 2064 656c  ects.        del
-0001b5b0: 6574 655f 636d 6420 3d20 5b27 736b 7927  ete_cmd = ['sky'
-0001b5c0: 2c20 2773 746f 7261 6765 272c 2027 6465  , 'storage', 'de
-0001b5d0: 6c65 7465 275d 0a20 2020 2020 2020 2064  lete'].        d
-0001b5e0: 656c 6574 655f 636d 6420 2b3d 2073 746f  elete_cmd += sto
-0001b5f0: 7261 6765 5f6f 626a 5f6e 616d 650a 2020  rage_obj_name.  
-0001b600: 2020 2020 2020 7375 6270 726f 6365 7373        subprocess
-0001b610: 2e63 6865 636b 5f6f 7574 7075 7428 6465  .check_output(de
-0001b620: 6c65 7465 5f63 6d64 290a 0a20 2020 2020  lete_cmd)..     
-0001b630: 2020 2023 2052 756e 2073 6b79 2073 746f     # Run sky sto
-0001b640: 7261 6765 206c 7320 746f 2063 6865 636b  rage ls to check
-0001b650: 2069 6620 616c 6c20 7374 6f72 6167 6520   if all storage 
-0001b660: 6f62 6a65 6374 7320 6669 6c74 6572 6564  objects filtered
-0001b670: 2062 7920 7374 6f72 650a 2020 2020 2020   by store.      
-0001b680: 2020 2320 7479 7065 2061 7265 2064 656c    # type are del
-0001b690: 6574 6564 0a20 2020 2020 2020 206f 7574  eted.        out
-0001b6a0: 5f61 6c6c 203d 2073 7562 7072 6f63 6573  _all = subproces
-0001b6b0: 732e 6368 6563 6b5f 6f75 7470 7574 285b  s.check_output([
-0001b6c0: 2773 6b79 272c 2027 7374 6f72 6167 6527  'sky', 'storage'
-0001b6d0: 2c20 276c 7327 5d29 0a20 2020 2020 2020  , 'ls']).       
-0001b6e0: 206f 7574 203d 205b 0a20 2020 2020 2020   out = [.       
-0001b6f0: 2020 2020 2069 7465 6d2e 7370 6c69 7428       item.split(
-0001b700: 295b 305d 0a20 2020 2020 2020 2020 2020  )[0].           
-0001b710: 2066 6f72 2069 7465 6d20 696e 206f 7574   for item in out
-0001b720: 5f61 6c6c 2e64 6563 6f64 6528 2775 7466  _all.decode('utf
-0001b730: 2d38 2729 2e73 706c 6974 6c69 6e65 7328  -8').splitlines(
-0001b740: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0001b750: 2073 746f 7265 5f74 7970 652e 7661 6c75   store_type.valu
-0001b760: 6520 696e 2069 7465 6d0a 2020 2020 2020  e in item.      
-0001b770: 2020 5d0a 2020 2020 2020 2020 6173 7365    ].        asse
-0001b780: 7274 2061 6c6c 285b 6974 656d 206e 6f74  rt all([item not
-0001b790: 2069 6e20 6f75 7420 666f 7220 6974 656d   in out for item
-0001b7a0: 2069 6e20 7374 6f72 6167 655f 6f62 6a5f   in storage_obj_
-0001b7b0: 6e61 6d65 5d29 0a0a 2020 2020 4070 7974  name])..    @pyt
-0001b7c0: 6573 742e 6d61 726b 2e70 6172 616d 6574  est.mark.paramet
-0001b7d0: 7269 7a65 2827 7374 6f72 655f 7479 7065  rize('store_type
-0001b7e0: 272c 205b 0a20 2020 2020 2020 2073 746f  ', [.        sto
-0001b7f0: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
-0001b800: 7065 2e53 332c 2073 746f 7261 6765 5f6c  pe.S3, storage_l
-0001b810: 6962 2e53 746f 7265 5479 7065 2e47 4353  ib.StoreType.GCS
-0001b820: 2c0a 2020 2020 2020 2020 7079 7465 7374  ,.        pytest
-0001b830: 2e70 6172 616d 2873 746f 7261 6765 5f6c  .param(storage_l
-0001b840: 6962 2e53 746f 7265 5479 7065 2e52 322c  ib.StoreType.R2,
-0001b850: 206d 6172 6b73 3d70 7974 6573 742e 6d61   marks=pytest.ma
-0001b860: 726b 2e63 6c6f 7564 666c 6172 6529 0a20  rk.cloudflare). 
-0001b870: 2020 205d 290a 2020 2020 6465 6620 7465     ]).    def te
-0001b880: 7374 5f62 7563 6b65 745f 6578 7465 726e  st_bucket_extern
-0001b890: 616c 5f64 656c 6574 696f 6e28 7365 6c66  al_deletion(self
-0001b8a0: 2c20 746d 705f 7363 7261 7463 685f 7374  , tmp_scratch_st
-0001b8b0: 6f72 6167 655f 6f62 6a2c 0a20 2020 2020  orage_obj,.     
-0001b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8e0: 2073 746f 7265 5f74 7970 6529 3a0a 2020   store_type):.  
-0001b8f0: 2020 2020 2020 2320 4372 6561 7465 7320        # Creates 
-0001b900: 6120 6275 636b 6574 2c20 6465 6c65 7465  a bucket, delete
-0001b910: 7320 6974 2065 7874 6572 6e61 6c6c 7920  s it externally 
-0001b920: 7573 696e 6720 636c 6f75 6420 636c 6920  using cloud cli 
-0001b930: 636f 6d6d 616e 6473 0a20 2020 2020 2020  commands.       
-0001b940: 2023 2061 6e64 2074 6865 6e20 7472 6965   # and then trie
-0001b950: 7320 746f 2064 656c 6574 6520 6974 2075  s to delete it u
-0001b960: 7369 6e67 2073 6b79 2073 746f 7261 6765  sing sky storage
-0001b970: 2064 656c 6574 652e 0a20 2020 2020 2020   delete..       
-0001b980: 2074 6d70 5f73 6372 6174 6368 5f73 746f   tmp_scratch_sto
-0001b990: 7261 6765 5f6f 626a 2e61 6464 5f73 746f  rage_obj.add_sto
-0001b9a0: 7265 2873 746f 7265 5f74 7970 6529 0a0a  re(store_type)..
-0001b9b0: 2020 2020 2020 2020 2320 5275 6e20 736b          # Run sk
-0001b9c0: 7920 7374 6f72 6167 6520 6c73 2074 6f20  y storage ls to 
-0001b9d0: 6368 6563 6b20 6966 2073 746f 7261 6765  check if storage
-0001b9e0: 206f 626a 6563 7420 6578 6973 7473 2069   object exists i
-0001b9f0: 6e20 7468 6520 6f75 7470 7574 0a20 2020  n the output.   
-0001ba00: 2020 2020 206f 7574 203d 2073 7562 7072       out = subpr
-0001ba10: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
-0001ba20: 7574 285b 2773 6b79 272c 2027 7374 6f72  ut(['sky', 'stor
-0001ba30: 6167 6527 2c20 276c 7327 5d29 0a20 2020  age', 'ls']).   
-0001ba40: 2020 2020 2061 7373 6572 7420 746d 705f       assert tmp_
-0001ba50: 7363 7261 7463 685f 7374 6f72 6167 655f  scratch_storage_
-0001ba60: 6f62 6a2e 6e61 6d65 2069 6e20 6f75 742e  obj.name in out.
-0001ba70: 6465 636f 6465 2827 7574 662d 3827 290a  decode('utf-8').
-0001ba80: 0a20 2020 2020 2020 2023 2044 656c 6574  .        # Delet
-0001ba90: 6520 6275 636b 6574 2065 7874 6572 6e61  e bucket externa
-0001baa0: 6c6c 790a 2020 2020 2020 2020 636d 6420  lly.        cmd 
-0001bab0: 3d20 7365 6c66 2e63 6c69 5f64 656c 6574  = self.cli_delet
-0001bac0: 655f 636d 6428 7374 6f72 655f 7479 7065  e_cmd(store_type
-0001bad0: 2c20 746d 705f 7363 7261 7463 685f 7374  , tmp_scratch_st
-0001bae0: 6f72 6167 655f 6f62 6a2e 6e61 6d65 290a  orage_obj.name).
-0001baf0: 2020 2020 2020 2020 7375 6270 726f 6365          subproce
-0001bb00: 7373 2e63 6865 636b 5f6f 7574 7075 7428  ss.check_output(
-0001bb10: 636d 642c 2073 6865 6c6c 3d54 7275 6529  cmd, shell=True)
-0001bb20: 0a0a 2020 2020 2020 2020 2320 5275 6e20  ..        # Run 
-0001bb30: 736b 7920 7374 6f72 6167 6520 6465 6c65  sky storage dele
-0001bb40: 7465 2074 6f20 6465 6c65 7465 2074 6865  te to delete the
-0001bb50: 2073 746f 7261 6765 206f 626a 6563 740a   storage object.
-0001bb60: 2020 2020 2020 2020 6f75 7420 3d20 7375          out = su
-0001bb70: 6270 726f 6365 7373 2e63 6865 636b 5f6f  bprocess.check_o
-0001bb80: 7574 7075 7428 0a20 2020 2020 2020 2020  utput(.         
-0001bb90: 2020 205b 2773 6b79 272c 2027 7374 6f72     ['sky', 'stor
-0001bba0: 6167 6527 2c20 2764 656c 6574 6527 2c20  age', 'delete', 
-0001bbb0: 746d 705f 7363 7261 7463 685f 7374 6f72  tmp_scratch_stor
-0001bbc0: 6167 655f 6f62 6a2e 6e61 6d65 5d29 0a20  age_obj.name]). 
-0001bbd0: 2020 2020 2020 2023 204d 616b 6520 7375         # Make su
-0001bbe0: 7265 2062 7563 6b65 7420 7761 7320 6e6f  re bucket was no
-0001bbf0: 7420 6372 6561 7465 6420 6475 7269 6e67  t created during
-0001bc00: 2064 656c 6574 696f 6e20 2873 6565 2069   deletion (see i
-0001bc10: 7373 7565 2023 3133 3232 290a 2020 2020  ssue #1322).    
-0001bc20: 2020 2020 6173 7365 7274 2027 6372 6561      assert 'crea
-0001bc30: 7465 6427 206e 6f74 2069 6e20 6f75 742e  ted' not in out.
-0001bc40: 6465 636f 6465 2827 7574 662d 3827 292e  decode('utf-8').
-0001bc50: 6c6f 7765 7228 290a 0a20 2020 2020 2020  lower()..       
-0001bc60: 2023 2052 756e 2073 6b79 2073 746f 7261   # Run sky stora
-0001bc70: 6765 206c 7320 746f 2063 6865 636b 2069  ge ls to check i
-0001bc80: 6620 7374 6f72 6167 6520 6f62 6a65 6374  f storage object
-0001bc90: 2069 7320 6465 6c65 7465 640a 2020 2020   is deleted.    
-0001bca0: 2020 2020 6f75 7420 3d20 7375 6270 726f      out = subpro
-0001bcb0: 6365 7373 2e63 6865 636b 5f6f 7574 7075  cess.check_outpu
-0001bcc0: 7428 5b27 736b 7927 2c20 2773 746f 7261  t(['sky', 'stora
-0001bcd0: 6765 272c 2027 6c73 275d 290a 2020 2020  ge', 'ls']).    
-0001bce0: 2020 2020 6173 7365 7274 2074 6d70 5f73      assert tmp_s
-0001bcf0: 6372 6174 6368 5f73 746f 7261 6765 5f6f  cratch_storage_o
-0001bd00: 626a 2e6e 616d 6520 6e6f 7420 696e 206f  bj.name not in o
-0001bd10: 7574 2e64 6563 6f64 6528 2775 7466 2d38  ut.decode('utf-8
-0001bd20: 2729 0a0a 2020 2020 4070 7974 6573 742e  ')..    @pytest.
-0001bd30: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
-0001bd40: 2827 7374 6f72 655f 7479 7065 272c 205b  ('store_type', [
-0001bd50: 0a20 2020 2020 2020 2073 746f 7261 6765  .        storage
-0001bd60: 5f6c 6962 2e53 746f 7265 5479 7065 2e53  _lib.StoreType.S
-0001bd70: 332c 2073 746f 7261 6765 5f6c 6962 2e53  3, storage_lib.S
-0001bd80: 746f 7265 5479 7065 2e47 4353 2c0a 2020  toreType.GCS,.  
-0001bd90: 2020 2020 2020 7079 7465 7374 2e70 6172        pytest.par
-0001bda0: 616d 2873 746f 7261 6765 5f6c 6962 2e53  am(storage_lib.S
-0001bdb0: 746f 7265 5479 7065 2e52 322c 206d 6172  toreType.R2, mar
-0001bdc0: 6b73 3d70 7974 6573 742e 6d61 726b 2e63  ks=pytest.mark.c
-0001bdd0: 6c6f 7564 666c 6172 6529 0a20 2020 205d  loudflare).    ]
-0001bde0: 290a 2020 2020 6465 6620 7465 7374 5f62  ).    def test_b
-0001bdf0: 7563 6b65 745f 6275 6c6b 5f64 656c 6574  ucket_bulk_delet
-0001be00: 696f 6e28 7365 6c66 2c20 7374 6f72 655f  ion(self, store_
-0001be10: 7479 7065 2c20 746d 705f 6275 6c6b 5f64  type, tmp_bulk_d
-0001be20: 656c 5f73 746f 7261 6765 5f6f 626a 293a  el_storage_obj):
-0001be30: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
-0001be40: 6573 2061 2074 656d 7020 666f 6c64 6572  es a temp folder
-0001be50: 2077 6974 6820 6f76 6572 2032 3536 2066   with over 256 f
-0001be60: 696c 6573 2061 6e64 2066 6f6c 6465 7273  iles and folders
-0001be70: 2c20 7570 6c6f 6164 0a20 2020 2020 2020  , upload.       
-0001be80: 2023 2066 696c 6573 2061 6e64 2066 6f6c   # files and fol
-0001be90: 6465 7273 2074 6f20 6120 6e65 7720 6275  ders to a new bu
-0001bea0: 636b 6574 2c20 7468 656e 2064 656c 6574  cket, then delet
-0001beb0: 6520 6275 636b 6574 2e0a 2020 2020 2020  e bucket..      
-0001bec0: 2020 746d 705f 6275 6c6b 5f64 656c 5f73    tmp_bulk_del_s
-0001bed0: 746f 7261 6765 5f6f 626a 2e61 6464 5f73  torage_obj.add_s
-0001bee0: 746f 7265 2873 746f 7265 5f74 7970 6529  tore(store_type)
-0001bef0: 0a0a 2020 2020 2020 2020 7375 6270 726f  ..        subpro
-0001bf00: 6365 7373 2e63 6865 636b 5f6f 7574 7075  cess.check_outpu
-0001bf10: 7428 0a20 2020 2020 2020 2020 2020 205b  t(.            [
-0001bf20: 2773 6b79 272c 2027 7374 6f72 6167 6527  'sky', 'storage'
-0001bf30: 2c20 2764 656c 6574 6527 2c20 746d 705f  , 'delete', tmp_
-0001bf40: 6275 6c6b 5f64 656c 5f73 746f 7261 6765  bulk_del_storage
-0001bf50: 5f6f 626a 2e6e 616d 655d 290a 0a20 2020  _obj.name])..   
-0001bf60: 2020 2020 206f 7574 7075 7420 3d20 7375       output = su
-0001bf70: 6270 726f 6365 7373 2e63 6865 636b 5f6f  bprocess.check_o
-0001bf80: 7574 7075 7428 5b27 736b 7927 2c20 2773  utput(['sky', 's
-0001bf90: 746f 7261 6765 272c 2027 6c73 275d 290a  torage', 'ls']).
-0001bfa0: 2020 2020 2020 2020 6173 7365 7274 2074          assert t
-0001bfb0: 6d70 5f62 756c 6b5f 6465 6c5f 7374 6f72  mp_bulk_del_stor
-0001bfc0: 6167 655f 6f62 6a2e 6e61 6d65 206e 6f74  age_obj.name not
-0001bfd0: 2069 6e20 6f75 7470 7574 2e64 6563 6f64   in output.decod
-0001bfe0: 6528 2775 7466 2d38 2729 0a0a 2020 2020  e('utf-8')..    
-0001bff0: 4070 7974 6573 742e 6d61 726b 2e70 6172  @pytest.mark.par
-0001c000: 616d 6574 7269 7a65 280a 2020 2020 2020  ametrize(.      
-0001c010: 2020 2774 6d70 5f70 7562 6c69 635f 7374    'tmp_public_st
-0001c020: 6f72 6167 655f 6f62 6a2c 2073 746f 7265  orage_obj, store
-0001c030: 5f74 7970 6527 2c0a 2020 2020 2020 2020  _type',.        
-0001c040: 5b28 2773 333a 2f2f 7463 6761 2d32 2d6f  [('s3://tcga-2-o
-0001c050: 7065 6e27 2c20 7374 6f72 6167 655f 6c69  pen', storage_li
-0001c060: 622e 5374 6f72 6554 7970 652e 5333 292c  b.StoreType.S3),
-0001c070: 0a20 2020 2020 2020 2020 2827 7333 3a2f  .         ('s3:/
-0001c080: 2f64 6967 6974 616c 636f 7270 6f72 6127  /digitalcorpora'
-0001c090: 2c20 7374 6f72 6167 655f 6c69 622e 5374  , storage_lib.St
-0001c0a0: 6f72 6554 7970 652e 5333 292c 0a20 2020  oreType.S3),.   
-0001c0b0: 2020 2020 2020 2827 6773 3a2f 2f67 6370        ('gs://gcp
-0001c0c0: 2d70 7562 6c69 632d 6461 7461 2d73 656e  -public-data-sen
-0001c0d0: 7469 6e65 6c2d 3227 2c20 7374 6f72 6167  tinel-2', storag
-0001c0e0: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
-0001c0f0: 4743 5329 5d2c 0a20 2020 2020 2020 2069  GCS)],.        i
-0001c100: 6e64 6972 6563 743d 5b27 746d 705f 7075  ndirect=['tmp_pu
-0001c110: 626c 6963 5f73 746f 7261 6765 5f6f 626a  blic_storage_obj
-0001c120: 275d 290a 2020 2020 6465 6620 7465 7374  ']).    def test
-0001c130: 5f70 7562 6c69 635f 6275 636b 6574 2873  _public_bucket(s
-0001c140: 656c 662c 2074 6d70 5f70 7562 6c69 635f  elf, tmp_public_
-0001c150: 7374 6f72 6167 655f 6f62 6a2c 2073 746f  storage_obj, sto
-0001c160: 7265 5f74 7970 6529 3a0a 2020 2020 2020  re_type):.      
-0001c170: 2020 2320 4372 6561 7465 7320 6120 6e65    # Creates a ne
-0001c180: 7720 6275 636b 6574 2077 6974 6820 6120  w bucket with a 
-0001c190: 7075 626c 6963 2073 6f75 7263 6520 616e  public source an
-0001c1a0: 6420 7665 7269 6669 6573 2074 6861 7420  d verifies that 
-0001c1b0: 6974 2069 7320 6e6f 740a 2020 2020 2020  it is not.      
-0001c1c0: 2020 2320 6164 6465 6420 746f 2067 6c6f    # added to glo
-0001c1d0: 6261 6c5f 7573 6572 5f73 7461 7465 2e0a  bal_user_state..
-0001c1e0: 2020 2020 2020 2020 746d 705f 7075 626c          tmp_publ
-0001c1f0: 6963 5f73 746f 7261 6765 5f6f 626a 2e61  ic_storage_obj.a
-0001c200: 6464 5f73 746f 7265 2873 746f 7265 5f74  dd_store(store_t
-0001c210: 7970 6529 0a0a 2020 2020 2020 2020 2320  ype)..        # 
-0001c220: 5275 6e20 736b 7920 7374 6f72 6167 6520  Run sky storage 
-0001c230: 6c73 2074 6f20 6368 6563 6b20 6966 2073  ls to check if s
-0001c240: 746f 7261 6765 206f 626a 6563 7420 6578  torage object ex
-0001c250: 6973 7473 2069 6e20 7468 6520 6f75 7470  ists in the outp
-0001c260: 7574 0a20 2020 2020 2020 206f 7574 203d  ut.        out =
-0001c270: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
-0001c280: 6b5f 6f75 7470 7574 285b 2773 6b79 272c  k_output(['sky',
-0001c290: 2027 7374 6f72 6167 6527 2c20 276c 7327   'storage', 'ls'
-0001c2a0: 5d29 0a20 2020 2020 2020 2061 7373 6572  ]).        asser
-0001c2b0: 7420 746d 705f 7075 626c 6963 5f73 746f  t tmp_public_sto
-0001c2c0: 7261 6765 5f6f 626a 2e6e 616d 6520 6e6f  rage_obj.name no
-0001c2d0: 7420 696e 206f 7574 2e64 6563 6f64 6528  t in out.decode(
-0001c2e0: 2775 7466 2d38 2729 0a0a 2020 2020 4070  'utf-8')..    @p
-0001c2f0: 7974 6573 742e 6d61 726b 2e70 6172 616d  ytest.mark.param
-0001c300: 6574 7269 7a65 2827 6e6f 6e65 7869 7374  etrize('nonexist
-0001c310: 5f62 7563 6b65 745f 7572 6c27 2c20 5b0a  _bucket_url', [.
-0001c320: 2020 2020 2020 2020 2773 333a 2f2f 7b72          's3://{r
-0001c330: 616e 646f 6d5f 6e61 6d65 7d27 2c20 2767  andom_name}', 'g
-0001c340: 733a 2f2f 7b72 616e 646f 6d5f 6e61 6d65  s://{random_name
-0001c350: 7d27 2c0a 2020 2020 2020 2020 7079 7465  }',.        pyte
-0001c360: 7374 2e70 6172 616d 2827 7232 3a2f 2f7b  st.param('r2://{
-0001c370: 7261 6e64 6f6d 5f6e 616d 657d 272c 206d  random_name}', m
-0001c380: 6172 6b73 3d70 7974 6573 742e 6d61 726b  arks=pytest.mark
-0001c390: 2e63 6c6f 7564 666c 6172 6529 0a20 2020  .cloudflare).   
-0001c3a0: 205d 290a 2020 2020 6465 6620 7465 7374   ]).    def test
-0001c3b0: 5f6e 6f6e 6578 6973 7465 6e74 5f62 7563  _nonexistent_buc
-0001c3c0: 6b65 7428 7365 6c66 2c20 6e6f 6e65 7869  ket(self, nonexi
-0001c3d0: 7374 5f62 7563 6b65 745f 7572 6c29 3a0a  st_bucket_url):.
-0001c3e0: 2020 2020 2020 2020 2320 4174 7465 6d70          # Attemp
-0001c3f0: 7473 2074 6f20 6372 6561 7465 2066 6574  ts to create fet
-0001c400: 6368 2061 2073 7472 6f61 6765 2077 6974  ch a stroage wit
-0001c410: 6820 6120 6e6f 6e2d 6578 6973 7465 6e74  h a non-existent
-0001c420: 2073 6f75 7263 652e 0a20 2020 2020 2020   source..       
-0001c430: 2023 2047 656e 6572 6174 6520 6120 7261   # Generate a ra
-0001c440: 6e64 6f6d 2062 7563 6b65 7420 6e61 6d65  ndom bucket name
-0001c450: 2061 6e64 2076 6572 6966 7920 6974 2064   and verify it d
-0001c460: 6f65 736e 2774 2065 7869 7374 3a0a 2020  oesn't exist:.  
-0001c470: 2020 2020 2020 7265 7472 795f 636f 756e        retry_coun
-0001c480: 7420 3d20 300a 2020 2020 2020 2020 7768  t = 0.        wh
-0001c490: 696c 6520 5472 7565 3a0a 2020 2020 2020  ile True:.      
-0001c4a0: 2020 2020 2020 6e6f 6e65 7869 7374 5f62        nonexist_b
-0001c4b0: 7563 6b65 745f 6e61 6d65 203d 2073 7472  ucket_name = str
-0001c4c0: 2875 7569 642e 7575 6964 3428 2929 0a20  (uuid.uuid4()). 
-0001c4d0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0001c4e0: 6e65 7869 7374 5f62 7563 6b65 745f 7572  nexist_bucket_ur
-0001c4f0: 6c2e 7374 6172 7473 7769 7468 2827 7333  l.startswith('s3
-0001c500: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-0001c510: 2020 2020 636f 6d6d 616e 6420 3d20 6627      command = f'
-0001c520: 6177 7320 7333 6170 6920 6865 6164 2d62  aws s3api head-b
-0001c530: 7563 6b65 7420 2d2d 6275 636b 6574 207b  ucket --bucket {
-0001c540: 6e6f 6e65 7869 7374 5f62 7563 6b65 745f  nonexist_bucket_
-0001c550: 6e61 6d65 7d27 0a20 2020 2020 2020 2020  name}'.         
-0001c560: 2020 2020 2020 2065 7870 6563 7465 645f         expected_
-0001c570: 6f75 7470 7574 203d 2027 3430 3427 0a20  output = '404'. 
-0001c580: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0001c590: 6e6f 6e65 7869 7374 5f62 7563 6b65 745f  nonexist_bucket_
-0001c5a0: 7572 6c2e 7374 6172 7473 7769 7468 2827  url.startswith('
-0001c5b0: 6773 2729 3a0a 2020 2020 2020 2020 2020  gs'):.          
-0001c5c0: 2020 2020 2020 636f 6d6d 616e 6420 3d20        command = 
-0001c5d0: 6627 6773 7574 696c 206c 7320 7b6e 6f6e  f'gsutil ls {non
-0001c5e0: 6578 6973 745f 6275 636b 6574 5f75 726c  exist_bucket_url
-0001c5f0: 2e66 6f72 6d61 7428 7261 6e64 6f6d 5f6e  .format(random_n
-0001c600: 616d 653d 6e6f 6e65 7869 7374 5f62 7563  ame=nonexist_buc
-0001c610: 6b65 745f 6e61 6d65 297d 270a 2020 2020  ket_name)}'.    
-0001c620: 2020 2020 2020 2020 2020 2020 6578 7065              expe
-0001c630: 6374 6564 5f6f 7574 7075 7420 3d20 2742  cted_output = 'B
-0001c640: 7563 6b65 744e 6f74 466f 756e 6445 7863  ucketNotFoundExc
-0001c650: 6570 7469 6f6e 270a 2020 2020 2020 2020  eption'.        
-0001c660: 2020 2020 656c 6966 206e 6f6e 6578 6973      elif nonexis
-0001c670: 745f 6275 636b 6574 5f75 726c 2e73 7461  t_bucket_url.sta
-0001c680: 7274 7377 6974 6828 2772 3227 293a 0a20  rtswith('r2'):. 
-0001c690: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0001c6a0: 6e64 706f 696e 745f 7572 6c20 3d20 636c  ndpoint_url = cl
-0001c6b0: 6f75 6466 6c61 7265 2e63 7265 6174 655f  oudflare.create_
-0001c6c0: 656e 6470 6f69 6e74 2829 0a20 2020 2020  endpoint().     
-0001c6d0: 2020 2020 2020 2020 2020 2063 6f6d 6d61             comma
-0001c6e0: 6e64 203d 2066 2741 5753 5f53 4841 5245  nd = f'AWS_SHARE
-0001c6f0: 445f 4352 4544 454e 5449 414c 535f 4649  D_CREDENTIALS_FI
-0001c700: 4c45 3d7b 636c 6f75 6466 6c61 7265 2e52  LE={cloudflare.R
-0001c710: 325f 4352 4544 454e 5449 414c 535f 5041  2_CREDENTIALS_PA
-0001c720: 5448 7d20 6177 7320 7333 6170 6920 6865  TH} aws s3api he
-0001c730: 6164 2d62 7563 6b65 7420 2d2d 6275 636b  ad-bucket --buck
-0001c740: 6574 207b 6e6f 6e65 7869 7374 5f62 7563  et {nonexist_buc
-0001c750: 6b65 745f 6e61 6d65 7d20 2d2d 656e 6470  ket_name} --endp
-0001c760: 6f69 6e74 207b 656e 6470 6f69 6e74 5f75  oint {endpoint_u
-0001c770: 726c 7d20 2d2d 7072 6f66 696c 653d 7232  rl} --profile=r2
-0001c780: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-0001c790: 2020 6578 7065 6374 6564 5f6f 7574 7075    expected_outpu
-0001c7a0: 7420 3d20 2734 3034 270a 2020 2020 2020  t = '404'.      
-0001c7b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001c7c0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0001c7d0: 6520 5661 6c75 6545 7272 6f72 2827 556e  e ValueError('Un
-0001c7e0: 7375 7070 6f72 7465 6420 6275 636b 6574  supported bucket
-0001c7f0: 2074 7970 6520 270a 2020 2020 2020 2020   type '.        
-0001c800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c810: 2020 2020 2020 2020 2066 277b 6e6f 6e65           f'{none
-0001c820: 7869 7374 5f62 7563 6b65 745f 7572 6c7d  xist_bucket_url}
-0001c830: 2729 0a0a 2020 2020 2020 2020 2020 2020  ')..            
-0001c840: 2320 4368 6563 6b20 6966 2062 7563 6b65  # Check if bucke
-0001c850: 7420 6578 6973 7473 2075 7369 6e67 2074  t exists using t
-0001c860: 6865 2063 6c69 3a0a 2020 2020 2020 2020  he cli:.        
-0001c870: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0001c880: 2020 2020 2020 2020 206f 7574 203d 2073           out = s
-0001c890: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
-0001c8a0: 6f75 7470 7574 2863 6f6d 6d61 6e64 2c0a  output(command,.
-0001c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c8d0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0001c8e0: 6465 7272 3d73 7562 7072 6f63 6573 732e  derr=subprocess.
-0001c8f0: 5354 444f 5554 2c0a 2020 2020 2020 2020  STDOUT,.        
-0001c900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c920: 2020 2020 2020 7368 656c 6c3d 5472 7565        shell=True
-0001c930: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
-0001c940: 6365 7074 2073 7562 7072 6f63 6573 732e  cept subprocess.
-0001c950: 4361 6c6c 6564 5072 6f63 6573 7345 7272  CalledProcessErr
-0001c960: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
-0001c970: 2020 2020 2020 2020 206f 7574 203d 2065           out = e
-0001c980: 2e6f 7574 7075 740a 2020 2020 2020 2020  .output.        
-0001c990: 2020 2020 6f75 7420 3d20 6f75 742e 6465      out = out.de
-0001c9a0: 636f 6465 2827 7574 662d 3827 290a 2020  code('utf-8').  
-0001c9b0: 2020 2020 2020 2020 2020 6966 2065 7870            if exp
-0001c9c0: 6563 7465 645f 6f75 7470 7574 2069 6e20  ected_output in 
-0001c9d0: 6f75 743a 0a20 2020 2020 2020 2020 2020  out:.           
-0001c9e0: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-0001c9f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001ca00: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0001ca10: 7279 5f63 6f75 6e74 202b 3d20 310a 2020  ry_count += 1.  
-0001ca20: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001ca30: 2072 6574 7279 5f63 6f75 6e74 203e 2033   retry_count > 3
-0001ca40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001ca50: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
-0001ca60: 696d 6545 7272 6f72 2827 556e 6162 6c65  imeError('Unable
-0001ca70: 2074 6f20 6669 6e64 2061 206e 6f6e 6578   to find a nonex
-0001ca80: 6973 7465 6e74 2062 7563 6b65 7420 270a  istent bucket '.
-0001ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001caa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cab0: 2020 2020 2020 2027 746f 2075 7365 2e20         'to use. 
-0001cac0: 5468 6973 2069 7320 6869 676c 7920 756e  This is higly un
-0001cad0: 6c69 6b65 6c79 202d 2027 0a20 2020 2020  likely - '.     
-0001cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001caf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cb00: 2020 2763 6865 636b 2069 6620 7468 6520    'check if the 
-0001cb10: 7465 7374 7320 6172 6520 636f 7272 6563  tests are correc
-0001cb20: 742e 2729 0a0a 2020 2020 2020 2020 7769  t.')..        wi
-0001cb30: 7468 2070 7974 6573 742e 7261 6973 6573  th pytest.raises
-0001cb40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001cb50: 2020 736b 792e 6578 6365 7074 696f 6e73    sky.exceptions
-0001cb60: 2e53 746f 7261 6765 4275 636b 6574 4765  .StorageBucketGe
-0001cb70: 7445 7272 6f72 2c0a 2020 2020 2020 2020  tError,.        
-0001cb80: 2020 2020 2020 2020 6d61 7463 683d 2741          match='A
-0001cb90: 7474 656d 7074 6564 2074 6f20 636f 6e6e  ttempted to conn
-0001cba0: 6563 7420 746f 2061 206e 6f6e 2d65 7869  ect to a non-exi
-0001cbb0: 7374 656e 7420 6275 636b 6574 2729 3a0a  stent bucket'):.
-0001cbc0: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
-0001cbd0: 6167 655f 6f62 6a20 3d20 7374 6f72 6167  age_obj = storag
-0001cbe0: 655f 6c69 622e 5374 6f72 6167 6528 736f  e_lib.Storage(so
-0001cbf0: 7572 6365 3d6e 6f6e 6578 6973 745f 6275  urce=nonexist_bu
-0001cc00: 636b 6574 5f75 726c 2e66 6f72 6d61 7428  cket_url.format(
-0001cc10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001cc20: 2072 616e 646f 6d5f 6e61 6d65 3d6e 6f6e   random_name=non
-0001cc30: 6578 6973 745f 6275 636b 6574 5f6e 616d  exist_bucket_nam
-0001cc40: 6529 290a 0a20 2020 2040 7079 7465 7374  e))..    @pytest
-0001cc50: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
-0001cc60: 6528 2770 7269 7661 7465 5f62 7563 6b65  e('private_bucke
-0001cc70: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
-0001cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc90: 205b 6627 7333 3a2f 2f69 6d61 6765 6e65   [f's3://imagene
-0001cca0: 7427 2c20 6627 6773 3a2f 2f69 6d61 6765  t', f'gs://image
-0001ccb0: 6e65 7427 5d29 0a20 2020 2064 6566 2074  net']).    def t
-0001ccc0: 6573 745f 7072 6976 6174 655f 6275 636b  est_private_buck
-0001ccd0: 6574 2873 656c 662c 2070 7269 7661 7465  et(self, private
-0001cce0: 5f62 7563 6b65 7429 3a0a 2020 2020 2020  _bucket):.      
-0001ccf0: 2020 2320 4174 7465 6d70 7473 2074 6f20    # Attempts to 
-0001cd00: 6163 6365 7373 2070 7269 7661 7465 2062  access private b
-0001cd10: 7563 6b65 7473 206e 6f74 2062 656c 6f6e  uckets not belon
-0001cd20: 6769 6e67 2074 6f20 7468 6520 7573 6572  ging to the user
-0001cd30: 2e0a 2020 2020 2020 2020 2320 5468 6573  ..        # Thes
-0001cd40: 6520 6275 636b 6574 7320 6172 6520 6b6e  e buckets are kn
-0001cd50: 6f77 6e20 746f 2062 6520 7072 6976 6174  own to be privat
-0001cd60: 652c 2062 7574 206d 6179 206e 6565 6420  e, but may need 
-0001cd70: 746f 2062 6520 7570 6461 7465 6420 6966  to be updated if
-0001cd80: 0a20 2020 2020 2020 2023 2074 6865 7920  .        # they 
-0001cd90: 6172 6520 7265 6d6f 7665 6420 6279 2074  are removed by t
-0001cda0: 6865 6972 206f 776e 6572 732e 0a20 2020  heir owners..   
-0001cdb0: 2020 2020 2070 7269 7661 7465 5f62 7563       private_buc
-0001cdc0: 6b65 745f 6e61 6d65 203d 2075 726c 6c69  ket_name = urlli
-0001cdd0: 622e 7061 7273 652e 7572 6c73 706c 6974  b.parse.urlsplit
-0001cde0: 2870 7269 7661 7465 5f62 7563 6b65 7429  (private_bucket)
-0001cdf0: 2e6e 6574 6c6f 630a 2020 2020 2020 2020  .netloc.        
-0001ce00: 7769 7468 2070 7974 6573 742e 7261 6973  with pytest.rais
-0001ce10: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
-0001ce20: 2020 2020 736b 792e 6578 6365 7074 696f      sky.exceptio
-0001ce30: 6e73 2e53 746f 7261 6765 4275 636b 6574  ns.StorageBucket
-0001ce40: 4765 7445 7272 6f72 2c0a 2020 2020 2020  GetError,.      
-0001ce50: 2020 2020 2020 2020 2020 6d61 7463 683d            match=
-0001ce60: 7374 6f72 6167 655f 6c69 622e 5f42 5543  storage_lib._BUC
-0001ce70: 4b45 545f 4641 494c 5f54 4f5f 434f 4e4e  KET_FAIL_TO_CONN
-0001ce80: 4543 545f 4d45 5353 4147 452e 666f 726d  ECT_MESSAGE.form
-0001ce90: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
-0001cea0: 2020 2020 2020 2020 6e61 6d65 3d70 7269          name=pri
-0001ceb0: 7661 7465 5f62 7563 6b65 745f 6e61 6d65  vate_bucket_name
-0001cec0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-0001ced0: 7374 6f72 6167 655f 6f62 6a20 3d20 7374  storage_obj = st
-0001cee0: 6f72 6167 655f 6c69 622e 5374 6f72 6167  orage_lib.Storag
-0001cef0: 6528 736f 7572 6365 3d70 7269 7661 7465  e(source=private
-0001cf00: 5f62 7563 6b65 7429 0a0a 2020 2020 4070  _bucket)..    @p
-0001cf10: 7974 6573 742e 6d61 726b 2e70 6172 616d  ytest.mark.param
-0001cf20: 6574 7269 7a65 2827 6578 745f 6275 636b  etrize('ext_buck
-0001cf30: 6574 5f66 6978 7475 7265 2c20 7374 6f72  et_fixture, stor
-0001cf40: 655f 7479 7065 272c 0a20 2020 2020 2020  e_type',.       
-0001cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cf60: 2020 2020 2020 5b28 2774 6d70 5f61 7773        [('tmp_aws
-0001cf70: 636c 695f 6275 636b 6574 272c 2073 746f  cli_bucket', sto
-0001cf80: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
-0001cf90: 7065 2e53 3329 2c0a 2020 2020 2020 2020  pe.S3),.        
-0001cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cfb0: 2020 2020 2020 2827 746d 705f 6773 7574        ('tmp_gsut
-0001cfc0: 696c 5f62 7563 6b65 7427 2c20 7374 6f72  il_bucket', stor
-0001cfd0: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
-0001cfe0: 652e 4743 5329 2c0a 2020 2020 2020 2020  e.GCS),.        
-0001cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d000: 2020 2020 2020 7079 7465 7374 2e70 6172        pytest.par
-0001d010: 616d 2827 746d 705f 6177 7363 6c69 5f62  am('tmp_awscli_b
-0001d020: 7563 6b65 745f 7232 272c 0a20 2020 2020  ucket_r2',.     
-0001d030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d050: 2020 2020 2020 7374 6f72 6167 655f 6c69        storage_li
-0001d060: 622e 5374 6f72 6554 7970 652e 5232 2c0a  b.StoreType.R2,.
-0001d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d090: 2020 2020 2020 2020 2020 206d 6172 6b73             marks
-0001d0a0: 3d70 7974 6573 742e 6d61 726b 2e63 6c6f  =pytest.mark.clo
-0001d0b0: 7564 666c 6172 6529 5d29 0a20 2020 2064  udflare)]).    d
-0001d0c0: 6566 2074 6573 745f 7570 6c6f 6164 5f74  ef test_upload_t
-0001d0d0: 6f5f 6578 6973 7469 6e67 5f62 7563 6b65  o_existing_bucke
-0001d0e0: 7428 7365 6c66 2c20 6578 745f 6275 636b  t(self, ext_buck
-0001d0f0: 6574 5f66 6978 7475 7265 2c20 7265 7175  et_fixture, requ
-0001d100: 6573 742c 0a20 2020 2020 2020 2020 2020  est,.           
-0001d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d120: 2020 2020 2020 2020 2020 2020 746d 705f              tmp_
-0001d130: 736f 7572 6365 2c20 7374 6f72 655f 7479  source, store_ty
-0001d140: 7065 293a 0a20 2020 2020 2020 2023 2054  pe):.        # T
-0001d150: 7269 6573 2075 706c 6f61 6469 6e67 2065  ries uploading e
-0001d160: 7869 7374 696e 6720 6669 6c65 7320 746f  xisting files to
-0001d170: 206e 6577 6c79 2063 7265 6174 6564 2062   newly created b
-0001d180: 7563 6b65 7420 286f 7574 7369 6465 206f  ucket (outside o
-0001d190: 660a 2020 2020 2020 2020 2320 736b 7929  f.        # sky)
-0001d1a0: 2061 6e64 2076 6572 6966 6965 7320 7468   and verifies th
-0001d1b0: 6174 2066 696c 6573 2061 7265 2077 7269  at files are wri
-0001d1c0: 7474 656e 2e0a 2020 2020 2020 2020 6275  tten..        bu
-0001d1d0: 636b 6574 5f6e 616d 6520 3d20 7265 7175  cket_name = requ
-0001d1e0: 6573 742e 6765 7466 6978 7475 7265 7661  est.getfixtureva
-0001d1f0: 6c75 6528 6578 745f 6275 636b 6574 5f66  lue(ext_bucket_f
-0001d200: 6978 7475 7265 290a 2020 2020 2020 2020  ixture).        
-0001d210: 7374 6f72 6167 655f 6f62 6a20 3d20 7374  storage_obj = st
-0001d220: 6f72 6167 655f 6c69 622e 5374 6f72 6167  orage_lib.Storag
-0001d230: 6528 6e61 6d65 3d62 7563 6b65 745f 6e61  e(name=bucket_na
-0001d240: 6d65 2c20 736f 7572 6365 3d74 6d70 5f73  me, source=tmp_s
-0001d250: 6f75 7263 6529 0a20 2020 2020 2020 2073  ource).        s
-0001d260: 746f 7261 6765 5f6f 626a 2e61 6464 5f73  torage_obj.add_s
-0001d270: 746f 7265 2873 746f 7265 5f74 7970 6529  tore(store_type)
-0001d280: 0a0a 2020 2020 2020 2020 2320 4368 6563  ..        # Chec
-0001d290: 6b20 6966 2074 6d70 5f73 6f75 7263 652f  k if tmp_source/
-0001d2a0: 746d 702d 6669 6c65 2065 7869 7374 7320  tmp-file exists 
-0001d2b0: 696e 2074 6865 2062 7563 6b65 7420 7573  in the bucket us
-0001d2c0: 696e 6720 6177 7320 636c 690a 2020 2020  ing aws cli.    
-0001d2d0: 2020 2020 6f75 7420 3d20 7375 6270 726f      out = subpro
-0001d2e0: 6365 7373 2e63 6865 636b 5f6f 7574 7075  cess.check_outpu
-0001d2f0: 7428 7365 6c66 2e63 6c69 5f6c 735f 636d  t(self.cli_ls_cm
-0001d300: 6428 7374 6f72 655f 7479 7065 2c20 6275  d(store_type, bu
-0001d310: 636b 6574 5f6e 616d 6529 2c0a 2020 2020  cket_name),.    
-0001d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d340: 2020 7368 656c 6c3d 5472 7565 290a 2020    shell=True).  
-0001d350: 2020 2020 2020 6173 7365 7274 2027 746d        assert 'tm
-0001d360: 702d 6669 6c65 2720 696e 206f 7574 2e64  p-file' in out.d
-0001d370: 6563 6f64 6528 2775 7466 2d38 2729 2c20  ecode('utf-8'), 
-0001d380: 5c0a 2020 2020 2020 2020 2020 2020 2746  \.            'F
-0001d390: 696c 6520 6e6f 7420 666f 756e 6420 696e  ile not found in
-0001d3a0: 2062 7563 6b65 7420 2d20 6f75 7470 7574   bucket - output
-0001d3b0: 2077 6173 203a 207b 7d27 2e66 6f72 6d61   was : {}'.forma
-0001d3c0: 7428 6f75 742e 6465 636f 6465 0a20 2020  t(out.decode.   
-0001d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d400: 2020 2020 2020 2020 2020 2020 2028 2775               ('u
-0001d410: 7466 2d38 2729 290a 0a20 2020 2020 2020  tf-8'))..       
-0001d420: 2023 2043 6865 636b 2073 796d 6c69 6e6b   # Check symlink
-0001d430: 7320 2d20 7379 6d6c 696e 6b73 2064 6f6e  s - symlinks don
-0001d440: 2774 2067 6574 2063 6f70 6965 6420 6279  't get copied by
-0001d450: 2073 6b79 2073 746f 7261 6765 0a20 2020   sky storage.   
-0001d460: 2020 2020 2061 7373 6572 7420 2870 6174       assert (pat
-0001d470: 686c 6962 2e50 6174 6828 746d 705f 736f  hlib.Path(tmp_so
-0001d480: 7572 6365 2920 2f20 2763 6972 636c 652d  urce) / 'circle-
-0001d490: 6c69 6e6b 2729 2e69 735f 7379 6d6c 696e  link').is_symlin
-0001d4a0: 6b28 292c 2028 0a20 2020 2020 2020 2020  k(), (.         
-0001d4b0: 2020 2027 6369 7263 6c65 2d6c 696e 6b20     'circle-link 
-0001d4c0: 7761 7320 6e6f 7420 666f 756e 6420 696e  was not found in
-0001d4d0: 2074 6865 2075 706c 6f61 6420 736f 7572   the upload sour
-0001d4e0: 6365 202d 2027 0a20 2020 2020 2020 2020  ce - '.         
-0001d4f0: 2020 2027 6172 6520 7468 6520 7465 7374     'are the test
-0001d500: 2066 6978 7475 7265 7320 636f 7272 6563   fixtures correc
-0001d510: 743f 2729 0a20 2020 2020 2020 2061 7373  t?').        ass
-0001d520: 6572 7420 2763 6972 636c 652d 6c69 6e6b  ert 'circle-link
-0001d530: 2720 6e6f 7420 696e 206f 7574 2e64 6563  ' not in out.dec
-0001d540: 6f64 6528 2775 7466 2d38 2729 2c20 280a  ode('utf-8'), (.
-0001d550: 2020 2020 2020 2020 2020 2020 2753 796d              'Sym
-0001d560: 6c69 6e6b 2066 6f75 6e64 2069 6e20 6275  link found in bu
-0001d570: 636b 6574 202d 206c 7320 6f75 7470 7574  cket - ls output
-0001d580: 2077 6173 203a 207b 7d27 2e66 6f72 6d61   was : {}'.forma
-0001d590: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-0001d5a0: 2020 206f 7574 2e64 6563 6f64 6528 2775     out.decode('u
-0001d5b0: 7466 2d38 2729 2929 0a0a 2020 2020 2020  tf-8')))..      
-0001d5c0: 2020 2320 5275 6e20 736b 7920 7374 6f72    # Run sky stor
-0001d5d0: 6167 6520 6c73 2074 6f20 6368 6563 6b20  age ls to check 
-0001d5e0: 6966 2073 746f 7261 6765 206f 626a 6563  if storage objec
-0001d5f0: 7420 6578 6973 7473 2069 6e20 7468 6520  t exists in the 
-0001d600: 6f75 7470 7574 2e0a 2020 2020 2020 2020  output..        
-0001d610: 2320 4974 2073 686f 756c 6420 6e6f 7420  # It should not 
-0001d620: 6578 6973 7420 6265 6361 7573 6520 7468  exist because th
-0001d630: 6520 6275 636b 6574 2077 6173 2063 7265  e bucket was cre
-0001d640: 6174 6564 2065 7874 6572 6e61 6c6c 792e  ated externally.
-0001d650: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
-0001d660: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
-0001d670: 6f75 7470 7574 285b 2773 6b79 272c 2027  output(['sky', '
-0001d680: 7374 6f72 6167 6527 2c20 276c 7327 5d29  storage', 'ls'])
-0001d690: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0001d6a0: 7374 6f72 6167 655f 6f62 6a2e 6e61 6d65  storage_obj.name
-0001d6b0: 206e 6f74 2069 6e20 6f75 742e 6465 636f   not in out.deco
-0001d6c0: 6465 2827 7574 662d 3827 290a 0a20 2020  de('utf-8')..   
-0001d6d0: 2064 6566 2074 6573 745f 636f 7079 5f6d   def test_copy_m
-0001d6e0: 6f75 6e74 5f65 7869 7374 696e 675f 7374  ount_existing_st
-0001d6f0: 6f72 6167 6528 7365 6c66 2c0a 2020 2020  orage(self,.    
-0001d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d720: 2020 2020 2074 6d70 5f63 6f70 795f 6d6e       tmp_copy_mn
-0001d730: 745f 6578 6973 7469 6e67 5f73 746f 7261  t_existing_stora
-0001d740: 6765 5f6f 626a 293a 0a20 2020 2020 2020  ge_obj):.       
-0001d750: 2023 2043 7265 6174 6573 2061 2062 7563   # Creates a buc
-0001d760: 6b65 7420 7769 7468 206e 6f20 736f 7572  ket with no sour
-0001d770: 6365 2069 6e20 4d4f 554e 5420 6d6f 6465  ce in MOUNT mode
-0001d780: 2028 656d 7074 7920 6275 636b 6574 292c   (empty bucket),
-0001d790: 2061 6e64 0a20 2020 2020 2020 2023 2074   and.        # t
-0001d7a0: 6865 6e20 7472 6965 7320 746f 206c 6f61  hen tries to loa
-0001d7b0: 6420 7468 6520 7361 6d65 2073 746f 7261  d the same stora
-0001d7c0: 6765 2069 6e20 434f 5059 206d 6f64 652e  ge in COPY mode.
-0001d7d0: 0a20 2020 2020 2020 2074 6d70 5f63 6f70  .        tmp_cop
-0001d7e0: 795f 6d6e 745f 6578 6973 7469 6e67 5f73  y_mnt_existing_s
-0001d7f0: 746f 7261 6765 5f6f 626a 2e61 6464 5f73  torage_obj.add_s
-0001d800: 746f 7265 2873 746f 7261 6765 5f6c 6962  tore(storage_lib
-0001d810: 2e53 746f 7265 5479 7065 2e53 3329 0a20  .StoreType.S3). 
-0001d820: 2020 2020 2020 2073 746f 7261 6765 5f6e         storage_n
-0001d830: 616d 6520 3d20 746d 705f 636f 7079 5f6d  ame = tmp_copy_m
-0001d840: 6e74 5f65 7869 7374 696e 675f 7374 6f72  nt_existing_stor
-0001d850: 6167 655f 6f62 6a2e 6e61 6d65 0a0a 2020  age_obj.name..  
-0001d860: 2020 2020 2020 2320 4368 6563 6b20 6073        # Check `s
-0001d870: 6b79 2073 746f 7261 6765 206c 7360 2074  ky storage ls` t
-0001d880: 6f20 656e 7375 7265 2073 746f 7261 6765  o ensure storage
-0001d890: 206f 626a 6563 7420 6578 6973 7473 0a20   object exists. 
-0001d8a0: 2020 2020 2020 206f 7574 203d 2073 7562         out = sub
-0001d8b0: 7072 6f63 6573 732e 6368 6563 6b5f 6f75  process.check_ou
-0001d8c0: 7470 7574 285b 2773 6b79 272c 2027 7374  tput(['sky', 'st
-0001d8d0: 6f72 6167 6527 2c20 276c 7327 5d29 2e64  orage', 'ls']).d
-0001d8e0: 6563 6f64 6528 2775 7466 2d38 2729 0a20  ecode('utf-8'). 
-0001d8f0: 2020 2020 2020 2061 7373 6572 7420 7374         assert st
-0001d900: 6f72 6167 655f 6e61 6d65 2069 6e20 6f75  orage_name in ou
-0001d910: 742c 2066 2753 746f 7261 6765 207b 7374  t, f'Storage {st
-0001d920: 6f72 6167 655f 6e61 6d65 7d20 6e6f 7420  orage_name} not 
-0001d930: 666f 756e 6420 696e 2073 6b79 2073 746f  found in sky sto
-0001d940: 7261 6765 206c 732e 270a 0a20 2020 2040  rage ls.'..    @
-0001d950: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
-0001d960: 6d65 7472 697a 6528 2773 746f 7265 5f74  metrize('store_t
-0001d970: 7970 6527 2c20 5b0a 2020 2020 2020 2020  ype', [.        
-0001d980: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-0001d990: 6554 7970 652e 5333 2c20 7374 6f72 6167  eType.S3, storag
-0001d9a0: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
-0001d9b0: 4743 532c 0a20 2020 2020 2020 2070 7974  GCS,.        pyt
-0001d9c0: 6573 742e 7061 7261 6d28 7374 6f72 6167  est.param(storag
-0001d9d0: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
-0001d9e0: 5232 2c20 6d61 726b 733d 7079 7465 7374  R2, marks=pytest
-0001d9f0: 2e6d 6172 6b2e 636c 6f75 6466 6c61 7265  .mark.cloudflare
-0001da00: 290a 2020 2020 5d29 0a20 2020 2064 6566  ).    ]).    def
-0001da10: 2074 6573 745f 6c69 7374 5f73 6f75 7263   test_list_sourc
-0001da20: 6528 7365 6c66 2c20 746d 705f 6c6f 6361  e(self, tmp_loca
-0001da30: 6c5f 6c69 7374 5f73 746f 7261 6765 5f6f  l_list_storage_o
-0001da40: 626a 2c20 7374 6f72 655f 7479 7065 293a  bj, store_type):
-0001da50: 0a20 2020 2020 2020 2023 2055 7365 7320  .        # Uses 
-0001da60: 6120 6c69 7374 2069 6e20 7468 6520 736f  a list in the so
-0001da70: 7572 6365 2066 6965 6c64 2074 6f20 7370  urce field to sp
-0001da80: 6563 6966 7920 6120 6669 6c65 2061 6e64  ecify a file and
-0001da90: 2061 2064 6972 6563 746f 7279 2074 6f0a   a directory to.
-0001daa0: 2020 2020 2020 2020 2320 6265 2075 706c          # be upl
-0001dab0: 6f61 6465 6420 746f 2074 6865 2073 746f  oaded to the sto
-0001dac0: 7261 6765 206f 626a 6563 742e 0a20 2020  rage object..   
-0001dad0: 2020 2020 2074 6d70 5f6c 6f63 616c 5f6c       tmp_local_l
-0001dae0: 6973 745f 7374 6f72 6167 655f 6f62 6a2e  ist_storage_obj.
-0001daf0: 6164 645f 7374 6f72 6528 7374 6f72 655f  add_store(store_
-0001db00: 7479 7065 290a 0a20 2020 2020 2020 2023  type)..        #
-0001db10: 2043 6865 636b 2069 6620 746d 702d 6669   Check if tmp-fi
-0001db20: 6c65 2065 7869 7374 7320 696e 2074 6865  le exists in the
-0001db30: 2062 7563 6b65 7420 726f 6f74 2075 7369   bucket root usi
-0001db40: 6e67 2063 6c69 0a20 2020 2020 2020 206f  ng cli.        o
-0001db50: 7574 203d 2073 7562 7072 6f63 6573 732e  ut = subprocess.
-0001db60: 6368 6563 6b5f 6f75 7470 7574 2873 656c  check_output(sel
-0001db70: 662e 636c 695f 6c73 5f63 6d64 280a 2020  f.cli_ls_cmd(.  
-0001db80: 2020 2020 2020 2020 2020 7374 6f72 655f            store_
-0001db90: 7479 7065 2c20 746d 705f 6c6f 6361 6c5f  type, tmp_local_
-0001dba0: 6c69 7374 5f73 746f 7261 6765 5f6f 626a  list_storage_obj
-0001dbb0: 2e6e 616d 6529 2c0a 2020 2020 2020 2020  .name),.        
-0001dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dbd0: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-0001dbe0: 656c 6c3d 5472 7565 290a 2020 2020 2020  ell=True).      
-0001dbf0: 2020 6173 7365 7274 2027 746d 702d 6669    assert 'tmp-fi
-0001dc00: 6c65 2720 696e 206f 7574 2e64 6563 6f64  le' in out.decod
-0001dc10: 6528 2775 7466 2d38 2729 2c20 5c0a 2020  e('utf-8'), \.  
-0001dc20: 2020 2020 2020 2020 2020 2746 696c 6520            'File 
-0001dc30: 6e6f 7420 666f 756e 6420 696e 2062 7563  not found in buc
-0001dc40: 6b65 7420 2d20 6f75 7470 7574 2077 6173  ket - output was
-0001dc50: 203a 207b 7d27 2e66 6f72 6d61 7428 6f75   : {}'.format(ou
-0001dc60: 742e 6465 636f 6465 0a20 2020 2020 2020  t.decode.       
-0001dc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e60: 7374 6172 7420 2d79 207b 6e61 6d65 7d27  start -y {name}'
+00016e70: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+00016e80: 736b 7920 6578 6563 202d 2d6e 756d 2d6e  sky exec --num-n
+00016e90: 6f64 6573 3d32 207b 6e61 6d65 7d20 6578  odes=2 {name} ex
+00016ea0: 616d 706c 6573 2f61 7a75 7265 5f73 7461  amples/azure_sta
+00016eb0: 7274 5f73 746f 702e 7961 6d6c 272c 0a20  rt_stop.yaml',. 
+00016ec0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+00016ed0: 206c 6f67 7320 7b6e 616d 657d 2032 202d   logs {name} 2 -
+00016ee0: 2d73 7461 7475 7327 2c20 2023 2045 6e73  -status',  # Ens
+00016ef0: 7572 6520 7468 6520 6a6f 6220 7375 6363  ure the job succ
+00016f00: 6565 6465 642e 0a20 2020 2020 2020 205d  eeded..        ]
+00016f10: 2c0a 2020 2020 2020 2020 6627 736b 7920  ,.        f'sky 
+00016f20: 646f 776e 202d 7920 7b6e 616d 657d 272c  down -y {name}',
+00016f30: 0a20 2020 2020 2020 2074 696d 656f 7574  .        timeout
+00016f40: 3d33 3020 2a20 3630 2c20 2023 2033 3020  =30 * 60,  # 30 
+00016f50: 6d69 6e73 2020 2869 7420 7461 6b65 7320  mins  (it takes 
+00016f60: 6172 6f75 6e64 207e 3233 206d 696e 7329  around ~23 mins)
+00016f70: 0a20 2020 2029 0a20 2020 2072 756e 5f6f  .    ).    run_o
+00016f80: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
+00016f90: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2054 6573  # ---------- Tes
+00016fa0: 7469 6e67 2065 6e76 2066 6f72 2064 6973  ting env for dis
+00016fb0: 6b20 7469 6572 202d 2d2d 2d2d 2d2d 2d2d  k tier ---------
+00016fc0: 2d0a 4070 7974 6573 742e 6d61 726b 2e61  -.@pytest.mark.a
+00016fd0: 7773 0a64 6566 2074 6573 745f 6177 735f  ws.def test_aws_
+00016fe0: 6469 736b 5f74 6965 7228 293a 0a0a 2020  disk_tier():..  
+00016ff0: 2020 6465 6620 5f67 6574 5f61 7773 5f71    def _get_aws_q
+00017000: 7565 7279 5f63 6f6d 6d61 6e64 2872 6567  uery_command(reg
+00017010: 696f 6e2c 2069 6e73 7461 6e63 655f 6964  ion, instance_id
+00017020: 2c20 6669 656c 642c 2065 7870 6563 7465  , field, expecte
+00017030: 6429 3a0a 2020 2020 2020 2020 7265 7475  d):.        retu
+00017040: 726e 2028 6627 6177 7320 6563 3220 6465  rn (f'aws ec2 de
+00017050: 7363 7269 6265 2d76 6f6c 756d 6573 202d  scribe-volumes -
+00017060: 2d72 6567 696f 6e20 7b72 6567 696f 6e7d  -region {region}
+00017070: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+00017080: 2020 2066 272d 2d66 696c 7465 7273 204e     f'--filters N
+00017090: 616d 653d 6174 7461 6368 6d65 6e74 2e69  ame=attachment.i
+000170a0: 6e73 7461 6e63 652d 6964 2c56 616c 7565  nstance-id,Value
+000170b0: 733d 7b69 6e73 7461 6e63 655f 6964 7d20  s={instance_id} 
+000170c0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+000170d0: 2020 6627 2d2d 7175 6572 7920 566f 6c75    f'--query Volu
+000170e0: 6d65 735b 2a5d 2e7b 6669 656c 647d 207c  mes[*].{field} |
+000170f0: 2067 7265 7020 7b65 7870 6563 7465 647d   grep {expected}
+00017100: 203b 2027 290a 0a20 2020 2066 6f72 2064   ; ')..    for d
+00017110: 6973 6b5f 7469 6572 2069 6e20 5b27 6c6f  isk_tier in ['lo
+00017120: 7727 2c20 276d 6564 6975 6d27 2c20 2768  w', 'medium', 'h
+00017130: 6967 6827 5d3a 0a20 2020 2020 2020 2073  igh']:.        s
+00017140: 7065 6373 203d 2041 5753 2e5f 6765 745f  pecs = AWS._get_
+00017150: 6469 736b 5f73 7065 6373 2864 6973 6b5f  disk_specs(disk_
+00017160: 7469 6572 290a 2020 2020 2020 2020 6e61  tier).        na
+00017170: 6d65 203d 205f 6765 745f 636c 7573 7465  me = _get_cluste
+00017180: 725f 6e61 6d65 2829 202b 2027 2d27 202b  r_name() + '-' +
+00017190: 2064 6973 6b5f 7469 6572 0a20 2020 2020   disk_tier.     
+000171a0: 2020 2072 6567 696f 6e20 3d20 2775 732d     region = 'us-
+000171b0: 7765 7374 2d32 270a 2020 2020 2020 2020  west-2'.        
+000171c0: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
+000171d0: 2020 2020 2020 2020 2027 6177 732d 6469           'aws-di
+000171e0: 736b 2d74 6965 7227 2c0a 2020 2020 2020  sk-tier',.      
+000171f0: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00017200: 2020 2020 2020 2020 6627 736b 7920 6c61          f'sky la
+00017210: 756e 6368 202d 7920 2d63 207b 6e61 6d65  unch -y -c {name
+00017220: 7d20 2d2d 636c 6f75 6420 6177 7320 2d2d  } --cloud aws --
+00017230: 7265 6769 6f6e 207b 7265 6769 6f6e 7d20  region {region} 
+00017240: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00017250: 2020 6627 2d2d 6469 736b 2d74 6965 7220    f'--disk-tier 
+00017260: 7b64 6973 6b5f 7469 6572 7d20 6563 686f  {disk_tier} echo
+00017270: 2022 6865 6c6c 6f20 736b 7922 272c 0a20   "hello sky"',. 
+00017280: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00017290: 2769 643d 6061 7773 2065 6332 2064 6573  'id=`aws ec2 des
+000172a0: 6372 6962 652d 696e 7374 616e 6365 7320  cribe-instances 
+000172b0: 2d2d 7265 6769 6f6e 207b 7265 6769 6f6e  --region {region
+000172c0: 7d20 2d2d 6669 6c74 6572 7320 270a 2020  } --filters '.  
+000172d0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+000172e0: 4e61 6d65 3d74 6167 3a72 6179 2d63 6c75  Name=tag:ray-clu
+000172f0: 7374 6572 2d6e 616d 652c 5661 6c75 6573  ster-name,Values
+00017300: 3d7b 6e61 6d65 7d20 2d2d 7175 6572 7920  ={name} --query 
+00017310: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00017320: 2020 6627 5265 7365 7276 6174 696f 6e73    f'Reservations
+00017330: 5b5d 2e49 6e73 7461 6e63 6573 5b5d 2e49  [].Instances[].I
+00017340: 6e73 7461 6e63 6549 6420 2d2d 6f75 7470  nstanceId --outp
+00017350: 7574 2074 6578 7460 3b20 2720 2b0a 2020  ut text`; ' +.  
+00017360: 2020 2020 2020 2020 2020 2020 2020 5f67                _g
+00017370: 6574 5f61 7773 5f71 7565 7279 5f63 6f6d  et_aws_query_com
+00017380: 6d61 6e64 2872 6567 696f 6e2c 2027 2469  mand(region, '$i
+00017390: 6427 2c20 2756 6f6c 756d 6554 7970 6527  d', 'VolumeType'
+000173a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000173b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173c0: 2020 2020 2020 2020 2073 7065 6373 5b27           specs['
+000173d0: 6469 736b 5f74 6965 7227 5d29 202b 0a20  disk_tier']) +. 
+000173e0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+000173f0: 2727 2069 6620 6469 736b 5f74 6965 7220  '' if disk_tier 
+00017400: 3d3d 2027 6c6f 7727 2065 6c73 650a 2020  == 'low' else.  
+00017410: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00017420: 5f67 6574 5f61 7773 5f71 7565 7279 5f63  _get_aws_query_c
+00017430: 6f6d 6d61 6e64 2872 6567 696f 6e2c 2027  ommand(region, '
+00017440: 2469 6427 2c20 2749 6f70 7327 2c0a 2020  $id', 'Iops',.  
+00017450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017470: 2020 2020 2020 2073 7065 6373 5b27 6469         specs['di
+00017480: 736b 5f69 6f70 7327 5d29 202b 0a20 2020  sk_iops']) +.   
+00017490: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+000174a0: 6765 745f 6177 735f 7175 6572 795f 636f  get_aws_query_co
+000174b0: 6d6d 616e 6428 7265 6769 6f6e 2c20 2724  mmand(region, '$
+000174c0: 6964 272c 2027 5468 726f 7567 6870 7574  id', 'Throughput
+000174d0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+000174e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174f0: 2020 2020 2020 2020 2020 2020 7370 6563              spec
+00017500: 735b 2764 6973 6b5f 7468 726f 7567 6870  s['disk_throughp
+00017510: 7574 275d 2929 292c 0a20 2020 2020 2020  ut']))),.       
+00017520: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00017530: 2020 2020 6627 736b 7920 646f 776e 202d      f'sky down -
+00017540: 7920 7b6e 616d 657d 272c 0a20 2020 2020  y {name}',.     
+00017550: 2020 2020 2020 2074 696d 656f 7574 3d31         timeout=1
+00017560: 3020 2a20 3630 2c20 2023 2031 3020 6d69  0 * 60,  # 10 mi
+00017570: 6e73 2020 2869 7420 7461 6b65 7320 6172  ns  (it takes ar
+00017580: 6f75 6e64 207e 3620 6d69 6e73 290a 2020  ound ~6 mins).  
+00017590: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000175a0: 7275 6e5f 6f6e 655f 7465 7374 2874 6573  run_one_test(tes
+000175b0: 7429 0a0a 0a40 7079 7465 7374 2e6d 6172  t)...@pytest.mar
+000175c0: 6b2e 6763 700a 6465 6620 7465 7374 5f67  k.gcp.def test_g
+000175d0: 6370 5f64 6973 6b5f 7469 6572 2829 3a0a  cp_disk_tier():.
+000175e0: 2020 2020 666f 7220 6469 736b 5f74 6965      for disk_tie
+000175f0: 7220 696e 205b 276c 6f77 272c 2027 6d65  r in ['low', 'me
+00017600: 6469 756d 272c 2027 6869 6768 275d 3a0a  dium', 'high']:.
+00017610: 2020 2020 2020 2020 7479 7065 203d 2047          type = G
+00017620: 4350 2e5f 6765 745f 6469 736b 5f74 7970  CP._get_disk_typ
+00017630: 6528 6469 736b 5f74 6965 7229 0a20 2020  e(disk_tier).   
+00017640: 2020 2020 206e 616d 6520 3d20 5f67 6574       name = _get
+00017650: 5f63 6c75 7374 6572 5f6e 616d 6528 2920  _cluster_name() 
+00017660: 2b20 272d 2720 2b20 6469 736b 5f74 6965  + '-' + disk_tie
+00017670: 720a 2020 2020 2020 2020 7265 6769 6f6e  r.        region
+00017680: 203d 2027 7573 2d77 6573 7432 270a 2020   = 'us-west2'.  
+00017690: 2020 2020 2020 7465 7374 203d 2054 6573        test = Tes
+000176a0: 7428 0a20 2020 2020 2020 2020 2020 2027  t(.            '
+000176b0: 6763 702d 6469 736b 2d74 6965 7227 2c0a  gcp-disk-tier',.
+000176c0: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
+000176d0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+000176e0: 736b 7920 6c61 756e 6368 202d 7920 2d63  sky launch -y -c
+000176f0: 207b 6e61 6d65 7d20 2d2d 636c 6f75 6420   {name} --cloud 
+00017700: 6763 7020 2d2d 7265 6769 6f6e 207b 7265  gcp --region {re
+00017710: 6769 6f6e 7d20 270a 2020 2020 2020 2020  gion} '.        
+00017720: 2020 2020 2020 2020 6627 2d2d 6469 736b          f'--disk
+00017730: 2d74 6965 7220 7b64 6973 6b5f 7469 6572  -tier {disk_tier
+00017740: 7d20 6563 686f 2022 6865 6c6c 6f20 736b  } echo "hello sk
+00017750: 7922 272c 0a20 2020 2020 2020 2020 2020  y"',.           
+00017760: 2020 2020 2066 276e 616d 653d 6067 636c       f'name=`gcl
+00017770: 6f75 6420 636f 6d70 7574 6520 696e 7374  oud compute inst
+00017780: 616e 6365 7320 6c69 7374 202d 2d66 696c  ances list --fil
+00017790: 7465 723d 270a 2020 2020 2020 2020 2020  ter='.          
+000177a0: 2020 2020 2020 6627 226c 6162 656c 732e        f'"labels.
+000177b0: 7261 792d 636c 7573 7465 722d 6e61 6d65  ray-cluster-name
+000177c0: 3a7b 6e61 6d65 7d22 202d 2d66 6f72 6d61  :{name}" --forma
+000177d0: 743d 2276 616c 7565 286e 616d 6529 2260  t="value(name)"`
+000177e0: 3b20 270a 2020 2020 2020 2020 2020 2020  ; '.            
+000177f0: 2020 2020 6627 6763 6c6f 7564 2063 6f6d      f'gcloud com
+00017800: 7075 7465 2064 6973 6b73 206c 6973 7420  pute disks list 
+00017810: 2d2d 6669 6c74 6572 3d22 6e61 6d65 3d24  --filter="name=$
+00017820: 6e61 6d65 2220 270a 2020 2020 2020 2020  name" '.        
+00017830: 2020 2020 2020 2020 6627 2d2d 666f 726d          f'--form
+00017840: 6174 3d22 7661 6c75 6528 7479 7065 2922  at="value(type)"
+00017850: 207c 2067 7265 7020 7b74 7970 657d 2027   | grep {type} '
+00017860: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
+00017870: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+00017880: 7920 646f 776e 202d 7920 7b6e 616d 657d  y down -y {name}
+00017890: 272c 0a20 2020 2020 2020 2020 2020 2074  ',.            t
+000178a0: 696d 656f 7574 3d36 202a 2036 302c 2020  imeout=6 * 60,  
+000178b0: 2320 3620 6d69 6e73 2020 2869 7420 7461  # 6 mins  (it ta
+000178c0: 6b65 7320 6172 6f75 6e64 207e 3320 6d69  kes around ~3 mi
+000178d0: 6e73 290a 2020 2020 2020 2020 290a 2020  ns).        ).  
+000178e0: 2020 2020 2020 7275 6e5f 6f6e 655f 7465        run_one_te
+000178f0: 7374 2874 6573 7429 0a0a 0a40 7079 7465  st(test)...@pyte
+00017900: 7374 2e6d 6172 6b2e 617a 7572 650a 6465  st.mark.azure.de
+00017910: 6620 7465 7374 5f61 7a75 7265 5f64 6973  f test_azure_dis
+00017920: 6b5f 7469 6572 2829 3a0a 2020 2020 666f  k_tier():.    fo
+00017930: 7220 6469 736b 5f74 6965 7220 696e 205b  r disk_tier in [
+00017940: 276c 6f77 272c 2027 6d65 6469 756d 275d  'low', 'medium']
+00017950: 3a0a 2020 2020 2020 2020 7479 7065 203d  :.        type =
+00017960: 2041 7a75 7265 2e5f 6765 745f 6469 736b   Azure._get_disk
+00017970: 5f74 7970 6528 6469 736b 5f74 6965 7229  _type(disk_tier)
+00017980: 0a20 2020 2020 2020 206e 616d 6520 3d20  .        name = 
+00017990: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
+000179a0: 6528 2920 2b20 272d 2720 2b20 6469 736b  e() + '-' + disk
+000179b0: 5f74 6965 720a 2020 2020 2020 2020 7265  _tier.        re
+000179c0: 6769 6f6e 203d 2027 7765 7374 7573 3227  gion = 'westus2'
+000179d0: 0a20 2020 2020 2020 2074 6573 7420 3d20  .        test = 
+000179e0: 5465 7374 280a 2020 2020 2020 2020 2020  Test(.          
+000179f0: 2020 2761 7a75 7265 2d64 6973 6b2d 7469    'azure-disk-ti
+00017a00: 6572 272c 0a20 2020 2020 2020 2020 2020  er',.           
+00017a10: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00017a20: 2020 2066 2773 6b79 206c 6175 6e63 6820     f'sky launch 
+00017a30: 2d79 202d 6320 7b6e 616d 657d 202d 2d63  -y -c {name} --c
+00017a40: 6c6f 7564 2061 7a75 7265 202d 2d72 6567  loud azure --reg
+00017a50: 696f 6e20 7b72 6567 696f 6e7d 2027 0a20  ion {region} '. 
+00017a60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00017a70: 272d 2d64 6973 6b2d 7469 6572 207b 6469  '--disk-tier {di
+00017a80: 736b 5f74 6965 727d 2065 6368 6f20 2268  sk_tier} echo "h
+00017a90: 656c 6c6f 2073 6b79 2227 2c0a 2020 2020  ello sky"',.    
+00017aa0: 2020 2020 2020 2020 2020 2020 6627 617a              f'az
+00017ab0: 2072 6573 6f75 7263 6520 6c69 7374 202d   resource list -
+00017ac0: 2d74 6167 2072 6179 2d63 6c75 7374 6572  -tag ray-cluster
+00017ad0: 2d6e 616d 653d 7b6e 616d 657d 202d 2d71  -name={name} --q
+00017ae0: 7565 7279 2027 0a20 2020 2020 2020 2020  uery '.         
+00017af0: 2020 2020 2020 2066 2722 5b3f 7479 7065         f'"[?type
+00017b00: 3d3d 5c27 4d69 6372 6f73 6f66 742e 436f  ==\'Microsoft.Co
+00017b10: 6d70 7574 652f 6469 736b 735c 275d 2e73  mpute/disks\'].s
+00017b20: 6b75 2e6e 616d 6522 2027 0a20 2020 2020  ku.name" '.     
+00017b30: 2020 2020 2020 2020 2020 2066 272d 2d6f             f'--o
+00017b40: 7574 7075 7420 7473 7620 7c20 6772 6570  utput tsv | grep
+00017b50: 207b 7479 7065 7d27 0a20 2020 2020 2020   {type}'.       
+00017b60: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00017b70: 2020 2020 6627 736b 7920 646f 776e 202d      f'sky down -
+00017b80: 7920 7b6e 616d 657d 272c 0a20 2020 2020  y {name}',.     
+00017b90: 2020 2020 2020 2074 696d 656f 7574 3d32         timeout=2
+00017ba0: 3020 2a20 3630 2c20 2023 2032 3020 6d69  0 * 60,  # 20 mi
+00017bb0: 6e73 2020 2869 7420 7461 6b65 7320 6172  ns  (it takes ar
+00017bc0: 6f75 6e64 207e 3132 206d 696e 7329 0a20  ound ~12 mins). 
+00017bd0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00017be0: 2072 756e 5f6f 6e65 5f74 6573 7428 7465   run_one_test(te
+00017bf0: 7374 290a 0a0a 2320 2d2d 2d2d 2d2d 2054  st)...# ------ T
+00017c00: 6573 7469 6e67 205a 6572 6f20 5175 6f74  esting Zero Quot
+00017c10: 6120 4661 696c 6f76 6572 202d 2d2d 2d2d  a Failover -----
+00017c20: 2d0a 4070 7974 6573 742e 6d61 726b 2e61  -.@pytest.mark.a
+00017c30: 7773 0a64 6566 2074 6573 745f 6177 735f  ws.def test_aws_
+00017c40: 7a65 726f 5f71 756f 7461 5f66 6169 6c6f  zero_quota_failo
+00017c50: 7665 7228 293a 0a0a 2020 2020 6e61 6d65  ver():..    name
+00017c60: 203d 205f 6765 745f 636c 7573 7465 725f   = _get_cluster_
+00017c70: 6e61 6d65 2829 0a20 2020 2072 6567 696f  name().    regio
+00017c80: 6e20 3d20 6765 745f 6177 735f 7265 6769  n = get_aws_regi
+00017c90: 6f6e 5f66 6f72 5f71 756f 7461 5f66 6169  on_for_quota_fai
+00017ca0: 6c6f 7665 7228 290a 0a20 2020 2069 6620  lover()..    if 
+00017cb0: 6e6f 7420 7265 6769 6f6e 3a0a 2020 2020  not region:.    
+00017cc0: 2020 2020 7079 7465 7374 2e78 6661 696c      pytest.xfail
+00017cd0: 280a 2020 2020 2020 2020 2020 2020 2755  (.            'U
+00017ce0: 6e61 626c 6520 746f 2074 6573 7420 7a65  nable to test ze
+00017cf0: 726f 2071 756f 7461 2066 6169 6c6f 7665  ro quota failove
+00017d00: 7220 6f70 7469 6d69 7a61 7469 6f6e 20e2  r optimization .
+00017d10: 8094 2071 756f 7461 7320 270a 2020 2020  .. quotas '.    
+00017d20: 2020 2020 2020 2020 2766 6f72 2045 4332          'for EC2
+00017d30: 2050 3320 696e 7374 616e 6365 7320 7765   P3 instances we
+00017d40: 7265 2066 6f75 6e64 206f 6e20 616c 6c20  re found on all 
+00017d50: 4157 5320 7265 6769 6f6e 732e 2049 7320  AWS regions. Is 
+00017d60: 7468 6973 2027 0a20 2020 2020 2020 2020  this '.         
+00017d70: 2020 2027 6578 7065 6374 6564 2066 6f72     'expected for
+00017d80: 2079 6f75 7220 6163 636f 756e 743f 2729   your account?')
+00017d90: 0a20 2020 2020 2020 2072 6574 7572 6e0a  .        return.
+00017da0: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
+00017db0: 280a 2020 2020 2020 2020 2761 7773 2d7a  (.        'aws-z
+00017dc0: 6572 6f2d 7175 6f74 612d 6661 696c 6f76  ero-quota-failov
+00017dd0: 6572 272c 0a20 2020 2020 2020 205b 0a20  er',.        [. 
+00017de0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+00017df0: 206c 6175 6e63 6820 2d79 202d 6320 7b6e   launch -y -c {n
+00017e00: 616d 657d 202d 2d63 6c6f 7564 2061 7773  ame} --cloud aws
+00017e10: 202d 2d72 6567 696f 6e20 7b72 6567 696f   --region {regio
+00017e20: 6e7d 202d 2d67 7075 7320 5631 3030 3a38  n} --gpus V100:8
+00017e30: 202d 2d75 7365 2d73 706f 7420 7c20 6772   --use-spot | gr
+00017e40: 6570 2022 466f 756e 6420 6e6f 2071 756f  ep "Found no quo
+00017e50: 7461 2227 2c0a 2020 2020 2020 2020 5d2c  ta"',.        ],
+00017e60: 0a20 2020 2020 2020 2066 2773 6b79 2064  .        f'sky d
+00017e70: 6f77 6e20 2d79 207b 6e61 6d65 7d27 2c0a  own -y {name}',.
+00017e80: 2020 2020 290a 2020 2020 7275 6e5f 6f6e      ).    run_on
+00017e90: 655f 7465 7374 2874 6573 7429 0a0a 0a40  e_test(test)...@
+00017ea0: 7079 7465 7374 2e6d 6172 6b2e 6763 700a  pytest.mark.gcp.
+00017eb0: 6465 6620 7465 7374 5f67 6370 5f7a 6572  def test_gcp_zer
+00017ec0: 6f5f 7175 6f74 615f 6661 696c 6f76 6572  o_quota_failover
+00017ed0: 2829 3a0a 0a20 2020 206e 616d 6520 3d20  ():..    name = 
+00017ee0: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
+00017ef0: 6528 290a 2020 2020 7265 6769 6f6e 203d  e().    region =
+00017f00: 2067 6574 5f67 6370 5f72 6567 696f 6e5f   get_gcp_region_
+00017f10: 666f 725f 7175 6f74 615f 6661 696c 6f76  for_quota_failov
+00017f20: 6572 2829 0a0a 2020 2020 6966 206e 6f74  er()..    if not
+00017f30: 2072 6567 696f 6e3a 0a20 2020 2020 2020   region:.       
+00017f40: 2070 7974 6573 742e 7866 6169 6c28 0a20   pytest.xfail(. 
+00017f50: 2020 2020 2020 2020 2020 2027 556e 6162             'Unab
+00017f60: 6c65 2074 6f20 7465 7374 207a 6572 6f20  le to test zero 
+00017f70: 7175 6f74 6120 6661 696c 6f76 6572 206f  quota failover o
+00017f80: 7074 696d 697a 6174 696f 6e20 e280 9420  ptimization ... 
+00017f90: 7175 6f74 6173 2027 0a20 2020 2020 2020  quotas '.       
+00017fa0: 2020 2020 2027 666f 7220 4131 3030 2d38       'for A100-8
+00017fb0: 3047 4220 4750 5573 2077 6572 6520 666f  0GB GPUs were fo
+00017fc0: 756e 6420 6f6e 2061 6c6c 2047 4350 2072  und on all GCP r
+00017fd0: 6567 696f 6e73 2e20 4973 2074 6869 7320  egions. Is this 
+00017fe0: 270a 2020 2020 2020 2020 2020 2020 2765  '.            'e
+00017ff0: 7870 6563 7465 6420 666f 7220 796f 7572  xpected for your
+00018000: 2061 6363 6f75 6e74 3f27 290a 2020 2020   account?').    
+00018010: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+00018020: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
+00018030: 2020 2020 2027 6763 702d 7a65 726f 2d71       'gcp-zero-q
+00018040: 756f 7461 2d66 6169 6c6f 7665 7227 2c0a  uota-failover',.
+00018050: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
+00018060: 2020 2020 2020 6627 736b 7920 6c61 756e        f'sky laun
+00018070: 6368 202d 7920 2d63 207b 6e61 6d65 7d20  ch -y -c {name} 
+00018080: 2d2d 636c 6f75 6420 6763 7020 2d2d 7265  --cloud gcp --re
+00018090: 6769 6f6e 207b 7265 6769 6f6e 7d20 2d2d  gion {region} --
+000180a0: 6770 7573 2041 3130 302d 3830 4742 3a31  gpus A100-80GB:1
+000180b0: 202d 2d75 7365 2d73 706f 7420 7c20 6772   --use-spot | gr
+000180c0: 6570 2022 466f 756e 6420 6e6f 2071 756f  ep "Found no quo
+000180d0: 7461 2227 2c0a 2020 2020 2020 2020 5d2c  ta"',.        ],
+000180e0: 0a20 2020 2020 2020 2066 2773 6b79 2064  .        f'sky d
+000180f0: 6f77 6e20 2d79 207b 6e61 6d65 7d27 2c0a  own -y {name}',.
+00018100: 2020 2020 290a 2020 2020 7275 6e5f 6f6e      ).    run_on
+00018110: 655f 7465 7374 2874 6573 7429 0a0a 0a23  e_test(test)...#
+00018120: 202d 2d2d 2d2d 2d2d 2054 6573 7469 6e67   ------- Testing
+00018130: 2075 7365 7220 7261 7920 636c 7573 7465   user ray cluste
+00018140: 7220 2d2d 2d2d 2d2d 2d2d 0a64 6566 2074  r --------.def t
+00018150: 6573 745f 7573 6572 5f72 6179 5f63 6c75  est_user_ray_clu
+00018160: 7374 6572 2829 3a0a 2020 2020 6e61 6d65  ster():.    name
+00018170: 203d 205f 6765 745f 636c 7573 7465 725f   = _get_cluster_
+00018180: 6e61 6d65 2829 0a20 2020 2074 6573 7420  name().    test 
+00018190: 3d20 5465 7374 280a 2020 2020 2020 2020  = Test(.        
+000181a0: 2775 7365 722d 7261 792d 636c 7573 7465  'user-ray-cluste
+000181b0: 7227 2c0a 2020 2020 2020 2020 5b0a 2020  r',.        [.  
+000181c0: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+000181d0: 6c61 756e 6368 202d 7920 2d63 207b 6e61  launch -y -c {na
+000181e0: 6d65 7d20 2272 6179 2073 7461 7274 202d  me} "ray start -
+000181f0: 2d68 6561 6422 272c 0a20 2020 2020 2020  -head"',.       
+00018200: 2020 2020 2066 2773 6b79 2065 7865 6320       f'sky exec 
+00018210: 7b6e 616d 657d 2022 6563 686f 2068 6922  {name} "echo hi"
+00018220: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+00018230: 2773 6b79 206c 6f67 7320 7b6e 616d 657d  'sky logs {name}
+00018240: 2031 202d 2d73 7461 7475 7327 2c0a 2020   1 --status',.  
+00018250: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+00018260: 7374 6174 7573 202d 7220 7c20 6772 6570  status -r | grep
+00018270: 207b 6e61 6d65 7d20 7c20 6772 6570 2055   {name} | grep U
+00018280: 5027 2c0a 2020 2020 2020 2020 2020 2020  P',.            
+00018290: 6627 736b 7920 6578 6563 207b 6e61 6d65  f'sky exec {name
+000182a0: 7d20 2265 6368 6f20 6279 6522 272c 0a20  } "echo bye"',. 
+000182b0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+000182c0: 206c 6f67 7320 7b6e 616d 657d 2032 202d   logs {name} 2 -
+000182d0: 2d73 7461 7475 7327 2c0a 2020 2020 2020  -status',.      
+000182e0: 2020 5d2c 0a20 2020 2020 2020 2066 2773    ],.        f's
+000182f0: 6b79 2064 6f77 6e20 2d79 207b 6e61 6d65  ky down -y {name
+00018300: 7d27 2c0a 2020 2020 290a 2020 2020 7275  }',.    ).    ru
+00018310: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
+00018320: 0a0a 0a23 202d 2d2d 2d2d 2d2d 2054 6573  ...# ------- Tes
+00018330: 7469 6e67 2074 6865 2063 6f72 6520 4150  ting the core AP
+00018340: 4920 2d2d 2d2d 2d2d 2d2d 0a23 204d 6f73  I --------.# Mos
+00018350: 7420 6f66 2074 6865 2063 6f72 6520 4150  t of the core AP
+00018360: 4973 2068 6176 6520 6265 656e 2074 6573  Is have been tes
+00018370: 7465 6420 696e 2074 6865 2043 4c49 2074  ted in the CLI t
+00018380: 6573 7473 2e0a 2320 5468 6573 6520 7465  ests..# These te
+00018390: 7374 7320 6172 6520 666f 7220 7465 7374  sts are for test
+000183a0: 696e 6720 7468 6520 7265 7475 726e 2076  ing the return v
+000183b0: 616c 7565 206f 6620 7468 6520 4150 4973  alue of the APIs
+000183c0: 206e 6f74 2066 756c 6c79 2075 7365 6420   not fully used 
+000183d0: 696e 2043 4c49 2e0a 6465 6620 7465 7374  in CLI..def test
+000183e0: 5f63 6f72 655f 6170 6928 293a 0a20 2020  _core_api():.   
+000183f0: 206e 616d 6520 3d20 5f67 6574 5f63 6c75   name = _get_clu
+00018400: 7374 6572 5f6e 616d 6528 290a 2020 2020  ster_name().    
+00018410: 736b 792e 6c61 756e 6368 0a20 2020 2023  sky.launch.    #
+00018420: 2054 4f44 4f28 7a68 7775 293a 2041 6464   TODO(zhwu): Add
+00018430: 2061 2074 6573 7420 666f 7220 636f 7265   a test for core
+00018440: 2061 7069 2e0a 0a0a 2320 2d2d 2d2d 2d2d   api....# ------
+00018450: 2d2d 2d2d 2054 6573 7469 6e67 2053 746f  ---- Testing Sto
+00018460: 7261 6765 202d 2d2d 2d2d 2d2d 2d2d 2d0a  rage ----------.
+00018470: 636c 6173 7320 5465 7374 5374 6f72 6167  class TestStorag
+00018480: 6557 6974 6843 7265 6465 6e74 6961 6c73  eWithCredentials
+00018490: 3a0a 2020 2020 2222 2253 746f 7261 6765  :.    """Storage
+000184a0: 2074 6573 7473 2077 6869 6368 2072 6571   tests which req
+000184b0: 7569 7265 2063 7265 6465 6e74 6961 6c73  uire credentials
+000184c0: 2061 6e64 206e 6574 776f 726b 2063 6f6e   and network con
+000184d0: 6e65 6374 696f 6e22 2222 0a0a 2020 2020  nection"""..    
+000184e0: 4157 535f 494e 5641 4c49 445f 4e41 4d45  AWS_INVALID_NAME
+000184f0: 5320 3d20 5b0a 2020 2020 2020 2020 2761  S = [.        'a
+00018500: 6227 2c20 2023 206c 6573 7320 7468 616e  b',  # less than
+00018510: 2033 2063 6861 7261 6374 6572 730a 2020   3 characters.  
+00018520: 2020 2020 2020 2761 6263 6465 6667 6869        'abcdefghi
+00018530: 6a6b 6c6d 6e6f 7071 7273 7475 7677 7879  jklmnopqrstuvwxy
+00018540: 7a61 6263 6465 6667 6869 6a6b 6c6d 6e6f  zabcdefghijklmno
+00018550: 7071 7273 7475 7677 7879 7a61 6263 6465  pqrstuvwxyzabcde
+00018560: 6667 6869 6a6b 6c6d 6e6f 7071 7273 7475  fghijklmnopqrstu
+00018570: 7677 7879 7a31 272c 0a20 2020 2020 2020  vwxyz1',.       
+00018580: 2023 206d 6f72 6520 7468 616e 2036 3320   # more than 63 
+00018590: 6368 6172 6163 7465 7273 0a20 2020 2020  characters.     
+000185a0: 2020 2027 4162 6364 6566 272c 2020 2320     'Abcdef',  # 
+000185b0: 636f 6e74 6169 6e73 2061 6e20 7570 7065  contains an uppe
+000185c0: 7263 6173 6520 6c65 7474 6572 0a20 2020  rcase letter.   
+000185d0: 2020 2020 2027 6162 6320 6465 6627 2c20       'abc def', 
+000185e0: 2023 2063 6f6e 7461 696e 7320 6120 7370   # contains a sp
+000185f0: 6163 650a 2020 2020 2020 2020 2761 6263  ace.        'abc
+00018600: 2e2e 6465 6627 2c20 2023 2074 776f 2061  ..def',  # two a
+00018610: 646a 6163 656e 7420 7065 7269 6f64 730a  djacent periods.
+00018620: 2020 2020 2020 2020 2731 3932 2e31 3638          '192.168
+00018630: 2e35 2e34 272c 2020 2320 666f 726d 6174  .5.4',  # format
+00018640: 7465 6420 6173 2061 6e20 4950 2061 6464  ted as an IP add
+00018650: 7265 7373 0a20 2020 2020 2020 2027 786e  ress.        'xn
+00018660: 2d2d 6275 636b 6574 272c 2020 2320 7374  --bucket',  # st
+00018670: 6172 7473 2077 6974 6820 2778 6e2d 2d27  arts with 'xn--'
+00018680: 2070 7265 6669 780a 2020 2020 2020 2020   prefix.        
+00018690: 2762 7563 6b65 742d 7333 616c 6961 7327  'bucket-s3alias'
+000186a0: 2c20 2023 2065 6e64 7320 7769 7468 2027  ,  # ends with '
+000186b0: 2d73 3361 6c69 6173 2720 7375 6666 6978  -s3alias' suffix
+000186c0: 0a20 2020 2020 2020 2027 6275 636b 6574  .        'bucket
+000186d0: 2d2d 6f6c 2d73 3327 2c20 2023 2065 6e64  --ol-s3',  # end
+000186e0: 7320 7769 7468 2027 2d2d 6f6c 2d73 3327  s with '--ol-s3'
+000186f0: 2073 7566 6669 780a 2020 2020 2020 2020   suffix.        
+00018700: 272e 6162 6327 2c20 2023 2073 7461 7274  '.abc',  # start
+00018710: 7320 7769 7468 2061 2064 6f74 0a20 2020  s with a dot.   
+00018720: 2020 2020 2027 6162 632e 272c 2020 2320       'abc.',  # 
+00018730: 656e 6473 2077 6974 6820 6120 646f 740a  ends with a dot.
+00018740: 2020 2020 2020 2020 272d 6162 6327 2c20          '-abc', 
+00018750: 2023 2073 7461 7274 7320 7769 7468 2061   # starts with a
+00018760: 2068 7970 6865 6e0a 2020 2020 2020 2020   hyphen.        
+00018770: 2761 6263 2d27 2c20 2023 2065 6e64 7320  'abc-',  # ends 
+00018780: 7769 7468 2061 2068 7970 6865 6e0a 2020  with a hyphen.  
+00018790: 2020 5d0a 0a20 2020 2047 4353 5f49 4e56    ]..    GCS_INV
+000187a0: 414c 4944 5f4e 414d 4553 203d 205b 0a20  ALID_NAMES = [. 
+000187b0: 2020 2020 2020 2027 6162 272c 2020 2320         'ab',  # 
+000187c0: 6c65 7373 2074 6861 6e20 3320 6368 6172  less than 3 char
+000187d0: 6163 7465 7273 0a20 2020 2020 2020 2027  acters.        '
+000187e0: 6162 6364 6566 6768 696a 6b6c 6d6e 6f70  abcdefghijklmnop
+000187f0: 7172 7374 7576 7778 797a 6162 6364 6566  qrstuvwxyzabcdef
+00018800: 6768 696a 6b6c 6d6e 6f70 7172 7374 7576  ghijklmnopqrstuv
+00018810: 7778 797a 6162 6364 6566 6768 696a 6b6c  wxyzabcdefghijkl
+00018820: 6d6e 6f70 7172 7374 7576 7778 797a 3127  mnopqrstuvwxyz1'
+00018830: 2c0a 2020 2020 2020 2020 2320 6d6f 7265  ,.        # more
+00018840: 2074 6861 6e20 3633 2063 6861 7261 6374   than 63 charact
+00018850: 6572 7320 2877 6974 686f 7574 2064 6f74  ers (without dot
+00018860: 7329 0a20 2020 2020 2020 2027 4162 6364  s).        'Abcd
+00018870: 6566 272c 2020 2320 636f 6e74 6169 6e73  ef',  # contains
+00018880: 2061 6e20 7570 7065 7263 6173 6520 6c65   an uppercase le
+00018890: 7474 6572 0a20 2020 2020 2020 2027 6162  tter.        'ab
+000188a0: 6320 6465 6627 2c20 2023 2063 6f6e 7461  c def',  # conta
+000188b0: 696e 7320 6120 7370 6163 650a 2020 2020  ins a space.    
+000188c0: 2020 2020 2761 6263 2e2e 6465 6627 2c20      'abc..def', 
+000188d0: 2023 2074 776f 2061 646a 6163 656e 7420   # two adjacent 
+000188e0: 7065 7269 6f64 730a 2020 2020 2020 2020  periods.        
+000188f0: 2761 6263 5f2e 6465 662e 6768 692e 6a6b  'abc_.def.ghi.jk
+00018900: 6c6d 6e6f 7071 7273 7475 7677 7879 7a61  lmnopqrstuvwxyza
+00018910: 6263 6465 6667 6869 6a6b 6c6d 6e6f 7071  bcdefghijklmnopq
+00018920: 7273 7475 7677 7879 7a61 6263 6465 6667  rstuvwxyzabcdefg
+00018930: 6869 6a6b 6c6d 6e6f 7071 7273 7475 7677  hijklmnopqrstuvw
+00018940: 7879 7a31 270a 2020 2020 2020 2020 2320  xyz1'.        # 
+00018950: 4d6f 7265 2074 6861 6e20 3633 2063 6861  More than 63 cha
+00018960: 7261 6374 6572 7320 6265 7477 6565 6e20  racters between 
+00018970: 646f 7473 0a20 2020 2020 2020 2027 6162  dots.        'ab
+00018980: 635f 2e64 6566 2e67 6869 2e6a 6b6c 6d6e  c_.def.ghi.jklmn
+00018990: 6f70 7172 7374 7576 7778 797a 6162 6364  opqrstuvwxyzabcd
+000189a0: 6566 6768 696a 6b6c 6d6e 6f70 7166 6768  efghijklmnopqfgh
+000189b0: 696a 6b6c 6d6e 6f70 7172 7374 7576 7727  ijklmnopqrstuvw'
+000189c0: 202a 2035 2c0a 2020 2020 2020 2020 2320   * 5,.        # 
+000189d0: 6d6f 7265 2074 6861 6e20 3232 3220 6368  more than 222 ch
+000189e0: 6172 6163 7465 7273 2028 7769 7468 2064  aracters (with d
+000189f0: 6f74 7329 0a20 2020 2020 2020 2027 3139  ots).        '19
+00018a00: 322e 3136 382e 352e 3427 2c20 2023 2066  2.168.5.4',  # f
+00018a10: 6f72 6d61 7474 6564 2061 7320 616e 2049  ormatted as an I
+00018a20: 5020 6164 6472 6573 730a 2020 2020 2020  P address.      
+00018a30: 2020 2767 6f6f 6762 7563 6b65 7427 2c20    'googbucket', 
+00018a40: 2023 2073 7461 7274 7320 7769 7468 2027   # starts with '
+00018a50: 676f 6f67 2720 7072 6566 6978 0a20 2020  goog' prefix.   
+00018a60: 2020 2020 2027 676f 6f67 6c65 6275 636b       'googlebuck
+00018a70: 6574 272c 2020 2320 636f 6e74 6169 6e73  et',  # contains
+00018a80: 2027 676f 6f67 6c65 270a 2020 2020 2020   'google'.      
+00018a90: 2020 2767 3030 676c 6562 7563 6b65 7427    'g00glebucket'
+00018aa0: 2c20 2023 2076 6172 6961 6e74 206f 6620  ,  # variant of 
+00018ab0: 2767 6f6f 676c 6527 0a20 2020 2020 2020  'google'.       
+00018ac0: 2027 676f 3067 6c65 6275 636b 6574 272c   'go0glebucket',
+00018ad0: 2020 2320 7661 7269 616e 7420 6f66 2027    # variant of '
+00018ae0: 676f 6f67 6c65 270a 2020 2020 2020 2020  google'.        
+00018af0: 2767 306f 676c 6562 7563 6b65 7427 2c20  'g0oglebucket', 
+00018b00: 2023 2076 6172 6961 6e74 206f 6620 2767   # variant of 'g
+00018b10: 6f6f 676c 6527 0a20 2020 2020 2020 2027  oogle'.        '
+00018b20: 2e61 6263 272c 2020 2320 7374 6172 7473  .abc',  # starts
+00018b30: 2077 6974 6820 6120 646f 740a 2020 2020   with a dot.    
+00018b40: 2020 2020 2761 6263 2e27 2c20 2023 2065      'abc.',  # e
+00018b50: 6e64 7320 7769 7468 2061 2064 6f74 0a20  nds with a dot. 
+00018b60: 2020 2020 2020 2027 5f61 6263 272c 2020         '_abc',  
+00018b70: 2320 7374 6172 7473 2077 6974 6820 616e  # starts with an
+00018b80: 2075 6e64 6572 7363 6f72 650a 2020 2020   underscore.    
+00018b90: 2020 2020 2761 6263 5f27 2c20 2023 2065      'abc_',  # e
+00018ba0: 6e64 7320 7769 7468 2061 6e20 756e 6465  nds with an unde
+00018bb0: 7273 636f 7265 0a20 2020 205d 0a0a 2020  rscore.    ]..  
+00018bc0: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
+00018bd0: 2020 2020 6465 6620 636c 695f 6465 6c65      def cli_dele
+00018be0: 7465 5f63 6d64 2873 746f 7265 5f74 7970  te_cmd(store_typ
+00018bf0: 652c 2062 7563 6b65 745f 6e61 6d65 293a  e, bucket_name):
+00018c00: 0a20 2020 2020 2020 2069 6620 7374 6f72  .        if stor
+00018c10: 655f 7479 7065 203d 3d20 7374 6f72 6167  e_type == storag
+00018c20: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
+00018c30: 5333 3a0a 2020 2020 2020 2020 2020 2020  S3:.            
+00018c40: 7572 6c20 3d20 6627 7333 3a2f 2f7b 6275  url = f's3://{bu
+00018c50: 636b 6574 5f6e 616d 657d 270a 2020 2020  cket_name}'.    
+00018c60: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00018c70: 2761 7773 2073 3320 7262 207b 7572 6c7d  'aws s3 rb {url}
+00018c80: 202d 2d66 6f72 6365 270a 2020 2020 2020   --force'.      
+00018c90: 2020 6966 2073 746f 7265 5f74 7970 6520    if store_type 
+00018ca0: 3d3d 2073 746f 7261 6765 5f6c 6962 2e53  == storage_lib.S
+00018cb0: 746f 7265 5479 7065 2e47 4353 3a0a 2020  toreType.GCS:.  
+00018cc0: 2020 2020 2020 2020 2020 7572 6c20 3d20            url = 
+00018cd0: 6627 6773 3a2f 2f7b 6275 636b 6574 5f6e  f'gs://{bucket_n
+00018ce0: 616d 657d 270a 2020 2020 2020 2020 2020  ame}'.          
+00018cf0: 2020 7265 7475 726e 2066 2767 7375 7469    return f'gsuti
+00018d00: 6c20 2d6d 2072 6d20 2d72 207b 7572 6c7d  l -m rm -r {url}
+00018d10: 270a 2020 2020 2020 2020 6966 2073 746f  '.        if sto
+00018d20: 7265 5f74 7970 6520 3d3d 2073 746f 7261  re_type == stora
+00018d30: 6765 5f6c 6962 2e53 746f 7265 5479 7065  ge_lib.StoreType
+00018d40: 2e52 323a 0a20 2020 2020 2020 2020 2020  .R2:.           
+00018d50: 2065 6e64 706f 696e 745f 7572 6c20 3d20   endpoint_url = 
+00018d60: 636c 6f75 6466 6c61 7265 2e63 7265 6174  cloudflare.creat
+00018d70: 655f 656e 6470 6f69 6e74 2829 0a20 2020  e_endpoint().   
+00018d80: 2020 2020 2020 2020 2075 726c 203d 2066           url = f
+00018d90: 2773 333a 2f2f 7b62 7563 6b65 745f 6e61  's3://{bucket_na
+00018da0: 6d65 7d27 0a20 2020 2020 2020 2020 2020  me}'.           
+00018db0: 2072 6574 7572 6e20 6627 4157 535f 5348   return f'AWS_SH
+00018dc0: 4152 4544 5f43 5245 4445 4e54 4941 4c53  ARED_CREDENTIALS
+00018dd0: 5f46 494c 453d 7b63 6c6f 7564 666c 6172  _FILE={cloudflar
+00018de0: 652e 5232 5f43 5245 4445 4e54 4941 4c53  e.R2_CREDENTIALS
+00018df0: 5f50 4154 487d 2061 7773 2073 3320 7262  _PATH} aws s3 rb
+00018e00: 207b 7572 6c7d 202d 2d66 6f72 6365 202d   {url} --force -
+00018e10: 2d65 6e64 706f 696e 7420 7b65 6e64 706f  -endpoint {endpo
+00018e20: 696e 745f 7572 6c7d 202d 2d70 726f 6669  int_url} --profi
+00018e30: 6c65 3d72 3227 0a0a 2020 2020 4073 7461  le=r2'..    @sta
+00018e40: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
+00018e50: 6620 636c 695f 6c73 5f63 6d64 2873 746f  f cli_ls_cmd(sto
+00018e60: 7265 5f74 7970 652c 2062 7563 6b65 745f  re_type, bucket_
+00018e70: 6e61 6d65 2c20 7375 6666 6978 3d27 2729  name, suffix='')
+00018e80: 3a0a 2020 2020 2020 2020 6966 2073 746f  :.        if sto
+00018e90: 7265 5f74 7970 6520 3d3d 2073 746f 7261  re_type == stora
+00018ea0: 6765 5f6c 6962 2e53 746f 7265 5479 7065  ge_lib.StoreType
+00018eb0: 2e53 333a 0a20 2020 2020 2020 2020 2020  .S3:.           
+00018ec0: 2069 6620 7375 6666 6978 3a0a 2020 2020   if suffix:.    
+00018ed0: 2020 2020 2020 2020 2020 2020 7572 6c20              url 
+00018ee0: 3d20 6627 7333 3a2f 2f7b 6275 636b 6574  = f's3://{bucket
+00018ef0: 5f6e 616d 657d 2f7b 7375 6666 6978 7d27  _name}/{suffix}'
+00018f00: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00018f10: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00018f20: 2020 2075 726c 203d 2066 2773 333a 2f2f     url = f's3://
+00018f30: 7b62 7563 6b65 745f 6e61 6d65 7d27 0a20  {bucket_name}'. 
+00018f40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00018f50: 6e20 6627 6177 7320 7333 206c 7320 7b75  n f'aws s3 ls {u
+00018f60: 726c 7d27 0a20 2020 2020 2020 2069 6620  rl}'.        if 
+00018f70: 7374 6f72 655f 7479 7065 203d 3d20 7374  store_type == st
+00018f80: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
+00018f90: 7970 652e 4743 533a 0a20 2020 2020 2020  ype.GCS:.       
+00018fa0: 2020 2020 2069 6620 7375 6666 6978 3a0a       if suffix:.
+00018fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fc0: 7572 6c20 3d20 6627 6773 3a2f 2f7b 6275  url = f'gs://{bu
+00018fd0: 636b 6574 5f6e 616d 657d 2f7b 7375 6666  cket_name}/{suff
+00018fe0: 6978 7d27 0a20 2020 2020 2020 2020 2020  ix}'.           
+00018ff0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00019000: 2020 2020 2020 2075 726c 203d 2066 2767         url = f'g
+00019010: 733a 2f2f 7b62 7563 6b65 745f 6e61 6d65  s://{bucket_name
+00019020: 7d27 0a20 2020 2020 2020 2020 2020 2072  }'.            r
+00019030: 6574 7572 6e20 6627 6773 7574 696c 206c  eturn f'gsutil l
+00019040: 7320 7b75 726c 7d27 0a20 2020 2020 2020  s {url}'.       
+00019050: 2069 6620 7374 6f72 655f 7479 7065 203d   if store_type =
+00019060: 3d20 7374 6f72 6167 655f 6c69 622e 5374  = storage_lib.St
+00019070: 6f72 6554 7970 652e 5232 3a0a 2020 2020  oreType.R2:.    
+00019080: 2020 2020 2020 2020 656e 6470 6f69 6e74          endpoint
+00019090: 5f75 726c 203d 2063 6c6f 7564 666c 6172  _url = cloudflar
+000190a0: 652e 6372 6561 7465 5f65 6e64 706f 696e  e.create_endpoin
+000190b0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+000190c0: 6966 2073 7566 6669 783a 0a20 2020 2020  if suffix:.     
+000190d0: 2020 2020 2020 2020 2020 2075 726c 203d             url =
+000190e0: 2066 2773 333a 2f2f 7b62 7563 6b65 745f   f's3://{bucket_
+000190f0: 6e61 6d65 7d2f 7b73 7566 6669 787d 270a  name}/{suffix}'.
+00019100: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00019110: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00019120: 2020 7572 6c20 3d20 6627 7333 3a2f 2f7b    url = f's3://{
+00019130: 6275 636b 6574 5f6e 616d 657d 270a 2020  bucket_name}'.  
+00019140: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00019150: 2066 2741 5753 5f53 4841 5245 445f 4352   f'AWS_SHARED_CR
+00019160: 4544 454e 5449 414c 535f 4649 4c45 3d7b  EDENTIALS_FILE={
+00019170: 636c 6f75 6466 6c61 7265 2e52 325f 4352  cloudflare.R2_CR
+00019180: 4544 454e 5449 414c 535f 5041 5448 7d20  EDENTIALS_PATH} 
+00019190: 6177 7320 7333 206c 7320 7b75 726c 7d20  aws s3 ls {url} 
+000191a0: 2d2d 656e 6470 6f69 6e74 207b 656e 6470  --endpoint {endp
+000191b0: 6f69 6e74 5f75 726c 7d20 2d2d 7072 6f66  oint_url} --prof
+000191c0: 696c 653d 7232 270a 0a20 2020 2040 7079  ile=r2'..    @py
+000191d0: 7465 7374 2e66 6978 7475 7265 0a20 2020  test.fixture.   
+000191e0: 2064 6566 2074 6d70 5f73 6f75 7263 6528   def tmp_source(
+000191f0: 7365 6c66 2c20 746d 705f 7061 7468 293a  self, tmp_path):
+00019200: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+00019210: 6573 2061 2074 656d 706f 7261 7279 2064  es a temporary d
+00019220: 6972 6563 746f 7279 2077 6974 6820 6120  irectory with a 
+00019230: 6669 6c65 2069 6e20 6974 0a20 2020 2020  file in it.     
+00019240: 2020 2074 6d70 5f64 6972 203d 2074 6d70     tmp_dir = tmp
+00019250: 5f70 6174 6820 2f20 2774 6d70 2d73 6f75  _path / 'tmp-sou
+00019260: 7263 6527 0a20 2020 2020 2020 2074 6d70  rce'.        tmp
+00019270: 5f64 6972 2e6d 6b64 6972 2829 0a20 2020  _dir.mkdir().   
+00019280: 2020 2020 2074 6d70 5f66 696c 6520 3d20       tmp_file = 
+00019290: 746d 705f 6469 7220 2f20 2774 6d70 2d66  tmp_dir / 'tmp-f
+000192a0: 696c 6527 0a20 2020 2020 2020 2074 6d70  ile'.        tmp
+000192b0: 5f66 696c 652e 7772 6974 655f 7465 7874  _file.write_text
+000192c0: 2827 7465 7374 2729 0a20 2020 2020 2020  ('test').       
+000192d0: 2063 6972 636c 655f 6c69 6e6b 203d 2074   circle_link = t
+000192e0: 6d70 5f64 6972 202f 2027 6369 7263 6c65  mp_dir / 'circle
+000192f0: 2d6c 696e 6b27 0a20 2020 2020 2020 2063  -link'.        c
+00019300: 6972 636c 655f 6c69 6e6b 2e73 796d 6c69  ircle_link.symli
+00019310: 6e6b 5f74 6f28 746d 705f 6469 722c 2074  nk_to(tmp_dir, t
+00019320: 6172 6765 745f 6973 5f64 6972 6563 746f  arget_is_directo
+00019330: 7279 3d54 7275 6529 0a20 2020 2020 2020  ry=True).       
+00019340: 2079 6965 6c64 2073 7472 2874 6d70 5f64   yield str(tmp_d
+00019350: 6972 290a 0a20 2020 2040 7079 7465 7374  ir)..    @pytest
+00019360: 2e66 6978 7475 7265 0a20 2020 2064 6566  .fixture.    def
+00019370: 2074 6d70 5f62 7563 6b65 745f 6e61 6d65   tmp_bucket_name
+00019380: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00019390: 2320 4372 6561 7465 7320 6120 7465 6d70  # Creates a temp
+000193a0: 6f72 6172 7920 6275 636b 6574 206e 616d  orary bucket nam
+000193b0: 650a 2020 2020 2020 2020 2320 7469 6d65  e.        # time
+000193c0: 2e74 696d 6528 2920 7265 7475 726e 7320  .time() returns 
+000193d0: 7661 7279 696e 6720 7072 6563 6973 696f  varying precisio
+000193e0: 6e20 6f6e 2064 6966 6665 7265 6e74 2073  n on different s
+000193f0: 7973 7465 6d73 2c20 736f 2077 650a 2020  ystems, so we.  
+00019400: 2020 2020 2020 2320 7265 706c 6163 6520        # replace 
+00019410: 7468 6520 6465 6369 6d61 6c20 706f 696e  the decimal poin
+00019420: 7420 616e 6420 7573 6520 7768 6174 6576  t and use whatev
+00019430: 6572 2070 7265 6369 7369 6f6e 2077 6520  er precision we 
+00019440: 6361 6e20 6765 742e 0a20 2020 2020 2020  can get..       
+00019450: 2074 696d 6573 7461 6d70 203d 2073 7472   timestamp = str
+00019460: 2874 696d 652e 7469 6d65 2829 292e 7265  (time.time()).re
+00019470: 706c 6163 6528 272e 272c 2027 2729 0a20  place('.', ''). 
+00019480: 2020 2020 2020 2079 6965 6c64 2066 2773         yield f's
+00019490: 6b79 2d74 6573 742d 7b74 696d 6573 7461  ky-test-{timesta
+000194a0: 6d70 7d27 0a0a 2020 2020 4073 7461 7469  mp}'..    @stati
+000194b0: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
+000194c0: 7969 656c 645f 7374 6f72 6167 655f 6f62  yield_storage_ob
+000194d0: 6a65 6374 280a 2020 2020 2020 2020 2020  ject(.          
+000194e0: 2020 6e61 6d65 3a20 4f70 7469 6f6e 616c    name: Optional
+000194f0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+00019500: 2020 2020 2020 2020 2020 736f 7572 6365            source
+00019510: 3a20 4f70 7469 6f6e 616c 5b73 746f 7261  : Optional[stora
+00019520: 6765 5f6c 6962 2e50 6174 685d 203d 204e  ge_lib.Path] = N
+00019530: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00019540: 2073 746f 7265 733a 204f 7074 696f 6e61   stores: Optiona
+00019550: 6c5b 4469 6374 5b73 746f 7261 6765 5f6c  l[Dict[storage_l
+00019560: 6962 2e53 746f 7265 5479 7065 2c0a 2020  ib.StoreType,.  
+00019570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019590: 7374 6f72 6167 655f 6c69 622e 4162 7374  storage_lib.Abst
+000195a0: 7261 6374 5374 6f72 655d 5d20 3d20 4e6f  ractStore]] = No
+000195b0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+000195c0: 7065 7273 6973 7465 6e74 3a20 4f70 7469  persistent: Opti
+000195d0: 6f6e 616c 5b62 6f6f 6c5d 203d 2054 7275  onal[bool] = Tru
+000195e0: 652c 0a20 2020 2020 2020 2020 2020 206d  e,.            m
+000195f0: 6f64 653a 2073 746f 7261 6765 5f6c 6962  ode: storage_lib
+00019600: 2e53 746f 7261 6765 4d6f 6465 203d 2073  .StorageMode = s
+00019610: 746f 7261 6765 5f6c 6962 2e53 746f 7261  torage_lib.Stora
+00019620: 6765 4d6f 6465 2e4d 4f55 4e54 293a 0a20  geMode.MOUNT):. 
+00019630: 2020 2020 2020 2023 2043 7265 6174 6573         # Creates
+00019640: 2061 2074 656d 706f 7261 7279 2073 746f   a temporary sto
+00019650: 7261 6765 206f 626a 6563 742e 2053 746f  rage object. Sto
+00019660: 7265 7320 6d75 7374 2062 6520 6164 6465  res must be adde
+00019670: 6420 696e 2074 6865 2074 6573 742e 0a20  d in the test.. 
+00019680: 2020 2020 2020 2073 746f 7261 6765 5f6f         storage_o
+00019690: 626a 203d 2073 746f 7261 6765 5f6c 6962  bj = storage_lib
+000196a0: 2e53 746f 7261 6765 286e 616d 653d 6e61  .Storage(name=na
+000196b0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+000196c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196d0: 2020 2020 2020 2020 2020 2020 2020 736f                so
+000196e0: 7572 6365 3d73 6f75 7263 652c 0a20 2020  urce=source,.   
+000196f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019710: 2020 2020 2020 2073 746f 7265 733d 7374         stores=st
+00019720: 6f72 6573 2c0a 2020 2020 2020 2020 2020  ores,.          
+00019730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019750: 7065 7273 6973 7465 6e74 3d70 6572 7369  persistent=persi
+00019760: 7374 656e 742c 0a20 2020 2020 2020 2020  stent,.         
+00019770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019790: 206d 6f64 653d 6d6f 6465 290a 2020 2020   mode=mode).    
+000197a0: 2020 2020 7969 656c 6420 7374 6f72 6167      yield storag
+000197b0: 655f 6f62 6a0a 2020 2020 2020 2020 6861  e_obj.        ha
+000197c0: 6e64 6c65 203d 2067 6c6f 6261 6c5f 7573  ndle = global_us
+000197d0: 6572 5f73 7461 7465 2e67 6574 5f68 616e  er_state.get_han
+000197e0: 646c 655f 6672 6f6d 5f73 746f 7261 6765  dle_from_storage
+000197f0: 5f6e 616d 6528 0a20 2020 2020 2020 2020  _name(.         
+00019800: 2020 2073 746f 7261 6765 5f6f 626a 2e6e     storage_obj.n
+00019810: 616d 6529 0a20 2020 2020 2020 2069 6620  ame).        if 
+00019820: 6861 6e64 6c65 3a0a 2020 2020 2020 2020  handle:.        
+00019830: 2020 2020 2320 4966 2068 616e 646c 6520      # If handle 
+00019840: 6578 6973 7473 2c20 6465 6c65 7465 206d  exists, delete m
+00019850: 616e 7561 6c6c 790a 2020 2020 2020 2020  anually.        
+00019860: 2020 2020 2320 544f 444f 2872 6f6d 696c      # TODO(romil
+00019870: 6229 3a20 5468 6973 2069 7320 706f 7465  b): This is pote
+00019880: 6e74 6961 6c6c 7920 7269 736b 7920 2d20  ntially risky - 
+00019890: 6966 2074 6865 2064 656c 6574 6520 6d65  if the delete me
+000198a0: 7468 6f64 2068 6173 0a20 2020 2020 2020  thod has.       
+000198b0: 2020 2020 2023 2020 2062 7567 732c 2074       #   bugs, t
+000198c0: 6869 7320 6361 6e20 6361 7573 6520 7265  his can cause re
+000198d0: 736f 7572 6365 206c 6561 6b73 2e20 4964  source leaks. Id
+000198e0: 6561 6c6c 7920 7765 2073 686f 756c 6420  eally we should 
+000198f0: 6d61 6e75 616c 6c79 0a20 2020 2020 2020  manually.       
+00019900: 2020 2020 2023 2020 2065 6a65 6374 2073       #   eject s
+00019910: 746f 7261 6765 2066 726f 6d20 676c 6f62  torage from glob
+00019920: 616c 5f75 7365 725f 7374 6174 6520 616e  al_user_state an
+00019930: 6420 6465 6c65 7465 2074 6865 2062 7563  d delete the buc
+00019940: 6b65 7420 7573 696e 670a 2020 2020 2020  ket using.      
+00019950: 2020 2020 2020 2320 2020 626f 746f 3320        #   boto3 
+00019960: 6469 7265 6374 6c79 2e0a 2020 2020 2020  directly..      
+00019970: 2020 2020 2020 7374 6f72 6167 655f 6f62        storage_ob
+00019980: 6a2e 6465 6c65 7465 2829 0a0a 2020 2020  j.delete()..    
+00019990: 4070 7974 6573 742e 6669 7874 7572 650a  @pytest.fixture.
+000199a0: 2020 2020 6465 6620 746d 705f 7363 7261      def tmp_scra
+000199b0: 7463 685f 7374 6f72 6167 655f 6f62 6a28  tch_storage_obj(
+000199c0: 7365 6c66 2c20 746d 705f 6275 636b 6574  self, tmp_bucket
+000199d0: 5f6e 616d 6529 3a0a 2020 2020 2020 2020  _name):.        
+000199e0: 2320 4372 6561 7465 7320 6120 7374 6f72  # Creates a stor
+000199f0: 6167 6520 6f62 6a65 6374 2077 6974 6820  age object with 
+00019a00: 6e6f 2073 6f75 7263 6520 746f 2063 7265  no source to cre
+00019a10: 6174 6520 6120 7363 7261 7463 6820 7374  ate a scratch st
+00019a20: 6f72 6167 652e 0a20 2020 2020 2020 2023  orage..        #
+00019a30: 2053 746f 7265 7320 6d75 7374 2062 6520   Stores must be 
+00019a40: 6164 6465 6420 696e 2074 6865 2074 6573  added in the tes
+00019a50: 742e 0a20 2020 2020 2020 2079 6965 6c64  t..        yield
+00019a60: 2066 726f 6d20 7365 6c66 2e79 6965 6c64   from self.yield
+00019a70: 5f73 746f 7261 6765 5f6f 626a 6563 7428  _storage_object(
+00019a80: 6e61 6d65 3d74 6d70 5f62 7563 6b65 745f  name=tmp_bucket_
+00019a90: 6e61 6d65 290a 0a20 2020 2040 7079 7465  name)..    @pyte
+00019aa0: 7374 2e66 6978 7475 7265 0a20 2020 2064  st.fixture.    d
+00019ab0: 6566 2074 6d70 5f6d 756c 7469 706c 655f  ef tmp_multiple_
+00019ac0: 7363 7261 7463 685f 7374 6f72 6167 655f  scratch_storage_
+00019ad0: 6f62 6a28 7365 6c66 293a 0a20 2020 2020  obj(self):.     
+00019ae0: 2020 2023 2043 7265 6174 6573 2061 206c     # Creates a l
+00019af0: 6973 7420 6f66 2035 2073 746f 7261 6765  ist of 5 storage
+00019b00: 206f 626a 6563 7473 2077 6974 6820 6e6f   objects with no
+00019b10: 2073 6f75 7263 6520 746f 2063 7265 6174   source to creat
+00019b20: 650a 2020 2020 2020 2020 2320 6d75 6c74  e.        # mult
+00019b30: 6970 6c65 2073 6372 6174 6368 2073 746f  iple scratch sto
+00019b40: 7261 6765 732e 0a20 2020 2020 2020 2023  rages..        #
+00019b50: 2053 746f 7265 7320 666f 7220 6561 6368   Stores for each
+00019b60: 206f 626a 6563 7420 696e 2074 6865 206c   object in the l
+00019b70: 6973 7420 6d75 7374 2062 6520 6164 6465  ist must be adde
+00019b80: 6420 696e 2074 6865 2074 6573 742e 0a20  d in the test.. 
+00019b90: 2020 2020 2020 2073 746f 7261 6765 5f6d         storage_m
+00019ba0: 756c 745f 6f62 6a20 3d20 5b5d 0a20 2020  ult_obj = [].   
+00019bb0: 2020 2020 2066 6f72 205f 2069 6e20 7261       for _ in ra
+00019bc0: 6e67 6528 3529 3a0a 2020 2020 2020 2020  nge(5):.        
+00019bd0: 2020 2020 7469 6d65 7374 616d 7020 3d20      timestamp = 
+00019be0: 7374 7228 7469 6d65 2e74 696d 6528 2929  str(time.time())
+00019bf0: 2e72 6570 6c61 6365 2827 2e27 2c20 2727  .replace('.', ''
+00019c00: 290a 2020 2020 2020 2020 2020 2020 7374  ).            st
+00019c10: 6f72 655f 6f62 6a20 3d20 7374 6f72 6167  ore_obj = storag
+00019c20: 655f 6c69 622e 5374 6f72 6167 6528 6e61  e_lib.Storage(na
+00019c30: 6d65 3d66 2773 6b79 2d74 6573 742d 7b74  me=f'sky-test-{t
+00019c40: 696d 6573 7461 6d70 7d27 290a 2020 2020  imestamp}').    
+00019c50: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
+00019c60: 6d75 6c74 5f6f 626a 2e61 7070 656e 6428  mult_obj.append(
+00019c70: 7374 6f72 655f 6f62 6a29 0a20 2020 2020  store_obj).     
+00019c80: 2020 2079 6965 6c64 2073 746f 7261 6765     yield storage
+00019c90: 5f6d 756c 745f 6f62 6a0a 2020 2020 2020  _mult_obj.      
+00019ca0: 2020 666f 7220 7374 6f72 6167 655f 6f62    for storage_ob
+00019cb0: 6a20 696e 2073 746f 7261 6765 5f6d 756c  j in storage_mul
+00019cc0: 745f 6f62 6a3a 0a20 2020 2020 2020 2020  t_obj:.         
+00019cd0: 2020 2068 616e 646c 6520 3d20 676c 6f62     handle = glob
+00019ce0: 616c 5f75 7365 725f 7374 6174 652e 6765  al_user_state.ge
+00019cf0: 745f 6861 6e64 6c65 5f66 726f 6d5f 7374  t_handle_from_st
+00019d00: 6f72 6167 655f 6e61 6d65 280a 2020 2020  orage_name(.    
+00019d10: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
+00019d20: 6167 655f 6f62 6a2e 6e61 6d65 290a 2020  age_obj.name).  
+00019d30: 2020 2020 2020 2020 2020 6966 2068 616e            if han
+00019d40: 646c 653a 0a20 2020 2020 2020 2020 2020  dle:.           
+00019d50: 2020 2020 2023 2049 6620 6861 6e64 6c65       # If handle
+00019d60: 2065 7869 7374 732c 2064 656c 6574 6520   exists, delete 
+00019d70: 6d61 6e75 616c 6c79 0a20 2020 2020 2020  manually.       
+00019d80: 2020 2020 2020 2020 2023 2054 4f44 4f28           # TODO(
+00019d90: 726f 6d69 6c62 293a 2054 6869 7320 6973  romilb): This is
+00019da0: 2070 6f74 656e 7469 616c 6c79 2072 6973   potentially ris
+00019db0: 6b79 202d 2069 6620 7468 6520 6465 6c65  ky - if the dele
+00019dc0: 7465 206d 6574 686f 6420 6861 730a 2020  te method has.  
+00019dd0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00019de0: 6275 6773 2c20 7468 6973 2063 616e 2063  bugs, this can c
+00019df0: 6175 7365 2072 6573 6f75 7263 6520 6c65  ause resource le
+00019e00: 616b 732e 2049 6465 616c 6c79 2077 6520  aks. Ideally we 
+00019e10: 7368 6f75 6c64 206d 616e 7561 6c6c 790a  should manually.
+00019e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e30: 2320 656a 6563 7420 7374 6f72 6167 6520  # eject storage 
+00019e40: 6672 6f6d 2067 6c6f 6261 6c5f 7573 6572  from global_user
+00019e50: 5f73 7461 7465 2061 6e64 2064 656c 6574  _state and delet
+00019e60: 6520 7468 6520 6275 636b 6574 2075 7369  e the bucket usi
+00019e70: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
+00019e80: 2020 2023 2062 6f74 6f33 2064 6972 6563     # boto3 direc
+00019e90: 746c 792e 0a20 2020 2020 2020 2020 2020  tly..           
+00019ea0: 2020 2020 2073 746f 7261 6765 5f6f 626a       storage_obj
+00019eb0: 2e64 656c 6574 6528 290a 0a20 2020 2040  .delete()..    @
+00019ec0: 7079 7465 7374 2e66 6978 7475 7265 0a20  pytest.fixture. 
+00019ed0: 2020 2064 6566 2074 6d70 5f6c 6f63 616c     def tmp_local
+00019ee0: 5f73 746f 7261 6765 5f6f 626a 2873 656c  _storage_obj(sel
+00019ef0: 662c 2074 6d70 5f62 7563 6b65 745f 6e61  f, tmp_bucket_na
+00019f00: 6d65 2c20 746d 705f 736f 7572 6365 293a  me, tmp_source):
+00019f10: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+00019f20: 6573 2061 2074 656d 706f 7261 7279 2073  es a temporary s
+00019f30: 746f 7261 6765 206f 626a 6563 742e 2053  torage object. S
+00019f40: 746f 7265 7320 6d75 7374 2062 6520 6164  tores must be ad
+00019f50: 6465 6420 696e 2074 6865 2074 6573 742e  ded in the test.
+00019f60: 0a20 2020 2020 2020 2079 6965 6c64 2066  .        yield f
+00019f70: 726f 6d20 7365 6c66 2e79 6965 6c64 5f73  rom self.yield_s
+00019f80: 746f 7261 6765 5f6f 626a 6563 7428 6e61  torage_object(na
+00019f90: 6d65 3d74 6d70 5f62 7563 6b65 745f 6e61  me=tmp_bucket_na
+00019fa0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00019fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019fd0: 2073 6f75 7263 653d 746d 705f 736f 7572   source=tmp_sour
+00019fe0: 6365 290a 0a20 2020 2040 7079 7465 7374  ce)..    @pytest
+00019ff0: 2e66 6978 7475 7265 0a20 2020 2064 6566  .fixture.    def
+0001a000: 2074 6d70 5f6c 6f63 616c 5f6c 6973 745f   tmp_local_list_
+0001a010: 7374 6f72 6167 655f 6f62 6a28 7365 6c66  storage_obj(self
+0001a020: 2c20 746d 705f 6275 636b 6574 5f6e 616d  , tmp_bucket_nam
+0001a030: 652c 2074 6d70 5f73 6f75 7263 6529 3a0a  e, tmp_source):.
+0001a040: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+0001a050: 7320 6120 7465 6d70 2073 746f 7261 6765  s a temp storage
+0001a060: 206f 626a 6563 7420 7768 6963 6820 7573   object which us
+0001a070: 6573 2061 206c 6973 7420 6f66 2070 6174  es a list of pat
+0001a080: 6873 2061 7320 736f 7572 6365 2e0a 2020  hs as source..  
+0001a090: 2020 2020 2020 2320 5374 6f72 6573 206d        # Stores m
+0001a0a0: 7573 7420 6265 2061 6464 6564 2069 6e20  ust be added in 
+0001a0b0: 7468 6520 7465 7374 2e20 4166 7465 7220  the test. After 
+0001a0c0: 7570 6c6f 6164 2c20 7468 6520 6275 636b  upload, the buck
+0001a0d0: 6574 2073 686f 756c 640a 2020 2020 2020  et should.      
+0001a0e0: 2020 2320 6861 7665 2074 776f 2066 696c    # have two fil
+0001a0f0: 6573 202d 202f 746d 702d 6669 6c65 2061  es - /tmp-file a
+0001a100: 6e64 202f 746d 702d 736f 7572 6365 2f74  nd /tmp-source/t
+0001a110: 6d70 2d66 696c 650a 2020 2020 2020 2020  mp-file.        
+0001a120: 6c69 7374 5f73 6f75 7263 6520 3d20 5b74  list_source = [t
+0001a130: 6d70 5f73 6f75 7263 652c 2074 6d70 5f73  mp_source, tmp_s
+0001a140: 6f75 7263 6520 2b20 272f 746d 702d 6669  ource + '/tmp-fi
+0001a150: 6c65 275d 0a20 2020 2020 2020 2079 6965  le'].        yie
+0001a160: 6c64 2066 726f 6d20 7365 6c66 2e79 6965  ld from self.yie
+0001a170: 6c64 5f73 746f 7261 6765 5f6f 626a 6563  ld_storage_objec
+0001a180: 7428 6e61 6d65 3d74 6d70 5f62 7563 6b65  t(name=tmp_bucke
+0001a190: 745f 6e61 6d65 2c0a 2020 2020 2020 2020  t_name,.        
+0001a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1c0: 2020 2020 2073 6f75 7263 653d 6c69 7374       source=list
+0001a1d0: 5f73 6f75 7263 6529 0a0a 2020 2020 4070  _source)..    @p
+0001a1e0: 7974 6573 742e 6669 7874 7572 650a 2020  ytest.fixture.  
+0001a1f0: 2020 6465 6620 746d 705f 6275 6c6b 5f64    def tmp_bulk_d
+0001a200: 656c 5f73 746f 7261 6765 5f6f 626a 2873  el_storage_obj(s
+0001a210: 656c 662c 2074 6d70 5f62 7563 6b65 745f  elf, tmp_bucket_
+0001a220: 6e61 6d65 293a 0a20 2020 2020 2020 2023  name):.        #
+0001a230: 2043 7265 6174 6573 2061 2074 656d 706f   Creates a tempo
+0001a240: 7261 7279 2073 746f 7261 6765 206f 626a  rary storage obj
+0001a250: 6563 7420 666f 7220 7465 7374 696e 6720  ect for testing 
+0001a260: 6275 6c6b 2064 656c 6574 696f 6e2e 0a20  bulk deletion.. 
+0001a270: 2020 2020 2020 2023 2053 746f 7265 7320         # Stores 
+0001a280: 6d75 7374 2062 6520 6164 6465 6420 696e  must be added in
+0001a290: 2074 6865 2074 6573 742e 0a20 2020 2020   the test..     
+0001a2a0: 2020 2077 6974 6820 7465 6d70 6669 6c65     with tempfile
+0001a2b0: 2e54 656d 706f 7261 7279 4469 7265 6374  .TemporaryDirect
+0001a2c0: 6f72 7928 2920 6173 2074 6d70 6469 723a  ory() as tmpdir:
+0001a2d0: 0a20 2020 2020 2020 2020 2020 2073 7562  .            sub
+0001a2e0: 7072 6f63 6573 732e 6368 6563 6b5f 6f75  process.check_ou
+0001a2f0: 7470 7574 2866 276d 6b64 6972 202d 7020  tput(f'mkdir -p 
+0001a300: 7b74 6d70 6469 727d 2f66 6f6c 6465 727b  {tmpdir}/folder{
+0001a310: 7b30 3030 2e2e 3235 357d 7d27 2c0a 2020  {000..255}}',.  
+0001a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a340: 2020 7368 656c 6c3d 5472 7565 290a 2020    shell=True).  
+0001a350: 2020 2020 2020 2020 2020 7375 6270 726f            subpro
+0001a360: 6365 7373 2e63 6865 636b 5f6f 7574 7075  cess.check_outpu
+0001a370: 7428 6627 746f 7563 6820 7b74 6d70 6469  t(f'touch {tmpdi
+0001a380: 727d 2f74 6573 747b 7b30 3030 2e2e 3235  r}/test{{000..25
+0001a390: 357d 7d2e 7478 7427 2c0a 2020 2020 2020  5}}.txt',.      
+0001a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a3b0: 2020 2020 2020 2020 2020 2020 2020 7368                sh
+0001a3c0: 656c 6c3d 5472 7565 290a 2020 2020 2020  ell=True).      
+0001a3d0: 2020 2020 2020 7375 6270 726f 6365 7373        subprocess
+0001a3e0: 2e63 6865 636b 5f6f 7574 7075 7428 0a20  .check_output(. 
+0001a3f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001a400: 2774 6f75 6368 207b 746d 7064 6972 7d2f  'touch {tmpdir}/
+0001a410: 666f 6c64 6572 7b7b 3030 302e 2e32 3535  folder{{000..255
+0001a420: 7d7d 2f74 6573 742e 7478 7427 2c20 7368  }}/test.txt', sh
+0001a430: 656c 6c3d 5472 7565 290a 2020 2020 2020  ell=True).      
+0001a440: 2020 2020 2020 7969 656c 6420 6672 6f6d        yield from
+0001a450: 2073 656c 662e 7969 656c 645f 7374 6f72   self.yield_stor
+0001a460: 6167 655f 6f62 6a65 6374 286e 616d 653d  age_object(name=
+0001a470: 746d 705f 6275 636b 6574 5f6e 616d 652c  tmp_bucket_name,
+0001a480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4b0: 2020 736f 7572 6365 3d74 6d70 6469 7229    source=tmpdir)
+0001a4c0: 0a0a 2020 2020 4070 7974 6573 742e 6669  ..    @pytest.fi
+0001a4d0: 7874 7572 650a 2020 2020 6465 6620 746d  xture.    def tm
+0001a4e0: 705f 636f 7079 5f6d 6e74 5f65 7869 7374  p_copy_mnt_exist
+0001a4f0: 696e 675f 7374 6f72 6167 655f 6f62 6a28  ing_storage_obj(
+0001a500: 7365 6c66 2c20 746d 705f 7363 7261 7463  self, tmp_scratc
+0001a510: 685f 7374 6f72 6167 655f 6f62 6a29 3a0a  h_storage_obj):.
+0001a520: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+0001a530: 7320 6120 636f 7079 206d 6f75 6e74 2073  s a copy mount s
+0001a540: 746f 7261 6765 2077 6869 6368 2072 6575  torage which reu
+0001a550: 7365 7320 616e 2065 7869 7374 696e 6720  ses an existing 
+0001a560: 7374 6f72 6167 6520 6f62 6a65 6374 2e0a  storage object..
+0001a570: 2020 2020 2020 2020 746d 705f 7363 7261          tmp_scra
+0001a580: 7463 685f 7374 6f72 6167 655f 6f62 6a2e  tch_storage_obj.
+0001a590: 6164 645f 7374 6f72 6528 7374 6f72 6167  add_store(storag
+0001a5a0: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
+0001a5b0: 5333 290a 2020 2020 2020 2020 7374 6f72  S3).        stor
+0001a5c0: 6167 655f 6e61 6d65 203d 2074 6d70 5f73  age_name = tmp_s
+0001a5d0: 6372 6174 6368 5f73 746f 7261 6765 5f6f  cratch_storage_o
+0001a5e0: 626a 2e6e 616d 650a 0a20 2020 2020 2020  bj.name..       
+0001a5f0: 2023 2054 7279 2074 6f20 696e 6974 6961   # Try to initia
+0001a600: 6c69 7a65 2061 6e6f 7468 6572 2073 746f  lize another sto
+0001a610: 7261 6765 2077 6974 6820 7468 6520 7374  rage with the st
+0001a620: 6f72 6167 6520 6f62 6a65 6374 2063 7265  orage object cre
+0001a630: 6174 6564 0a20 2020 2020 2020 2023 2061  ated.        # a
+0001a640: 626f 7665 2c20 6275 7420 6e6f 7720 696e  bove, but now in
+0001a650: 2043 4f50 5920 6d6f 6465 2e20 5468 6973   COPY mode. This
+0001a660: 2073 686f 756c 6420 7375 6363 6565 642e   should succeed.
+0001a670: 0a20 2020 2020 2020 2079 6965 6c64 2066  .        yield f
+0001a680: 726f 6d20 7365 6c66 2e79 6965 6c64 5f73  rom self.yield_s
+0001a690: 746f 7261 6765 5f6f 626a 6563 7428 6e61  torage_object(na
+0001a6a0: 6d65 3d73 746f 7261 6765 5f6e 616d 652c  me=storage_name,
+0001a6b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6d0: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+0001a6e0: 6465 3d73 746f 7261 6765 5f6c 6962 2e53  de=storage_lib.S
+0001a6f0: 746f 7261 6765 4d6f 6465 2e43 4f50 5929  torageMode.COPY)
+0001a700: 0a0a 2020 2020 4070 7974 6573 742e 6669  ..    @pytest.fi
+0001a710: 7874 7572 650a 2020 2020 6465 6620 746d  xture.    def tm
+0001a720: 705f 6177 7363 6c69 5f62 7563 6b65 7428  p_awscli_bucket(
+0001a730: 7365 6c66 2c20 746d 705f 6275 636b 6574  self, tmp_bucket
+0001a740: 5f6e 616d 6529 3a0a 2020 2020 2020 2020  _name):.        
+0001a750: 2320 4372 6561 7465 7320 6120 7465 6d70  # Creates a temp
+0001a760: 6f72 6172 7920 6275 636b 6574 2075 7369  orary bucket usi
+0001a770: 6e67 2061 7773 636c 690a 2020 2020 2020  ng awscli.      
+0001a780: 2020 7375 6270 726f 6365 7373 2e63 6865    subprocess.che
+0001a790: 636b 5f63 616c 6c28 5b27 6177 7327 2c20  ck_call(['aws', 
+0001a7a0: 2773 3327 2c20 276d 6227 2c20 6627 7333  's3', 'mb', f's3
+0001a7b0: 3a2f 2f7b 746d 705f 6275 636b 6574 5f6e  ://{tmp_bucket_n
+0001a7c0: 616d 657d 275d 290a 2020 2020 2020 2020  ame}']).        
+0001a7d0: 7969 656c 6420 746d 705f 6275 636b 6574  yield tmp_bucket
+0001a7e0: 5f6e 616d 650a 2020 2020 2020 2020 7375  _name.        su
+0001a7f0: 6270 726f 6365 7373 2e63 6865 636b 5f63  bprocess.check_c
+0001a800: 616c 6c28 0a20 2020 2020 2020 2020 2020  all(.           
+0001a810: 205b 2761 7773 272c 2027 7333 272c 2027   ['aws', 's3', '
+0001a820: 7262 272c 2066 2773 333a 2f2f 7b74 6d70  rb', f's3://{tmp
+0001a830: 5f62 7563 6b65 745f 6e61 6d65 7d27 2c20  _bucket_name}', 
+0001a840: 272d 2d66 6f72 6365 275d 290a 0a20 2020  '--force'])..   
+0001a850: 2040 7079 7465 7374 2e66 6978 7475 7265   @pytest.fixture
+0001a860: 0a20 2020 2064 6566 2074 6d70 5f67 7375  .    def tmp_gsu
+0001a870: 7469 6c5f 6275 636b 6574 2873 656c 662c  til_bucket(self,
+0001a880: 2074 6d70 5f62 7563 6b65 745f 6e61 6d65   tmp_bucket_name
+0001a890: 293a 0a20 2020 2020 2020 2023 2043 7265  ):.        # Cre
+0001a8a0: 6174 6573 2061 2074 656d 706f 7261 7279  ates a temporary
+0001a8b0: 2062 7563 6b65 7420 7573 696e 6720 6773   bucket using gs
+0001a8c0: 7574 696c 0a20 2020 2020 2020 2073 7562  util.        sub
+0001a8d0: 7072 6f63 6573 732e 6368 6563 6b5f 6361  process.check_ca
+0001a8e0: 6c6c 285b 2767 7375 7469 6c27 2c20 276d  ll(['gsutil', 'm
+0001a8f0: 6227 2c20 6627 6773 3a2f 2f7b 746d 705f  b', f'gs://{tmp_
+0001a900: 6275 636b 6574 5f6e 616d 657d 275d 290a  bucket_name}']).
+0001a910: 2020 2020 2020 2020 7969 656c 6420 746d          yield tm
+0001a920: 705f 6275 636b 6574 5f6e 616d 650a 2020  p_bucket_name.  
+0001a930: 2020 2020 2020 7375 6270 726f 6365 7373        subprocess
+0001a940: 2e63 6865 636b 5f63 616c 6c28 5b27 6773  .check_call(['gs
+0001a950: 7574 696c 272c 2027 726d 272c 2027 2d72  util', 'rm', '-r
+0001a960: 272c 2066 2767 733a 2f2f 7b74 6d70 5f62  ', f'gs://{tmp_b
+0001a970: 7563 6b65 745f 6e61 6d65 7d27 5d29 0a0a  ucket_name}'])..
+0001a980: 2020 2020 4070 7974 6573 742e 6669 7874      @pytest.fixt
+0001a990: 7572 650a 2020 2020 6465 6620 746d 705f  ure.    def tmp_
+0001a9a0: 6177 7363 6c69 5f62 7563 6b65 745f 7232  awscli_bucket_r2
+0001a9b0: 2873 656c 662c 2074 6d70 5f62 7563 6b65  (self, tmp_bucke
+0001a9c0: 745f 6e61 6d65 293a 0a20 2020 2020 2020  t_name):.       
+0001a9d0: 2023 2043 7265 6174 6573 2061 2074 656d   # Creates a tem
+0001a9e0: 706f 7261 7279 2062 7563 6b65 7420 7573  porary bucket us
+0001a9f0: 696e 6720 6177 7363 6c69 0a20 2020 2020  ing awscli.     
+0001aa00: 2020 2065 6e64 706f 696e 745f 7572 6c20     endpoint_url 
+0001aa10: 3d20 636c 6f75 6466 6c61 7265 2e63 7265  = cloudflare.cre
+0001aa20: 6174 655f 656e 6470 6f69 6e74 2829 0a20  ate_endpoint(). 
+0001aa30: 2020 2020 2020 2073 7562 7072 6f63 6573         subproces
+0001aa40: 732e 6368 6563 6b5f 6361 6c6c 280a 2020  s.check_call(.  
+0001aa50: 2020 2020 2020 2020 2020 6627 4157 535f            f'AWS_
+0001aa60: 5348 4152 4544 5f43 5245 4445 4e54 4941  SHARED_CREDENTIA
+0001aa70: 4c53 5f46 494c 453d 7b63 6c6f 7564 666c  LS_FILE={cloudfl
+0001aa80: 6172 652e 5232 5f43 5245 4445 4e54 4941  are.R2_CREDENTIA
+0001aa90: 4c53 5f50 4154 487d 2061 7773 2073 3320  LS_PATH} aws s3 
+0001aaa0: 6d62 2073 333a 2f2f 7b74 6d70 5f62 7563  mb s3://{tmp_buc
+0001aab0: 6b65 745f 6e61 6d65 7d20 2d2d 656e 6470  ket_name} --endp
+0001aac0: 6f69 6e74 207b 656e 6470 6f69 6e74 5f75  oint {endpoint_u
+0001aad0: 726c 7d20 2d2d 7072 6f66 696c 653d 7232  rl} --profile=r2
+0001aae0: 272c 0a20 2020 2020 2020 2020 2020 2073  ',.            s
+0001aaf0: 6865 6c6c 3d54 7275 6529 0a20 2020 2020  hell=True).     
+0001ab00: 2020 2079 6965 6c64 2074 6d70 5f62 7563     yield tmp_buc
+0001ab10: 6b65 745f 6e61 6d65 0a20 2020 2020 2020  ket_name.       
+0001ab20: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
+0001ab30: 6b5f 6361 6c6c 280a 2020 2020 2020 2020  k_call(.        
+0001ab40: 2020 2020 6627 4157 535f 5348 4152 4544      f'AWS_SHARED
+0001ab50: 5f43 5245 4445 4e54 4941 4c53 5f46 494c  _CREDENTIALS_FIL
+0001ab60: 453d 7b63 6c6f 7564 666c 6172 652e 5232  E={cloudflare.R2
+0001ab70: 5f43 5245 4445 4e54 4941 4c53 5f50 4154  _CREDENTIALS_PAT
+0001ab80: 487d 2061 7773 2073 3320 7262 2073 333a  H} aws s3 rb s3:
+0001ab90: 2f2f 7b74 6d70 5f62 7563 6b65 745f 6e61  //{tmp_bucket_na
+0001aba0: 6d65 7d20 2d2d 666f 7263 6520 2d2d 656e  me} --force --en
+0001abb0: 6470 6f69 6e74 207b 656e 6470 6f69 6e74  dpoint {endpoint
+0001abc0: 5f75 726c 7d20 2d2d 7072 6f66 696c 653d  _url} --profile=
+0001abd0: 7232 272c 0a20 2020 2020 2020 2020 2020  r2',.           
+0001abe0: 2073 6865 6c6c 3d54 7275 6529 0a0a 2020   shell=True)..  
+0001abf0: 2020 4070 7974 6573 742e 6669 7874 7572    @pytest.fixtur
+0001ac00: 650a 2020 2020 6465 6620 746d 705f 7075  e.    def tmp_pu
+0001ac10: 626c 6963 5f73 746f 7261 6765 5f6f 626a  blic_storage_obj
+0001ac20: 2873 656c 662c 2072 6571 7565 7374 293a  (self, request):
+0001ac30: 0a20 2020 2020 2020 2023 2049 6e69 7469  .        # Initi
+0001ac40: 616c 697a 6573 2061 2073 746f 7261 6765  alizes a storage
+0001ac50: 206f 626a 6563 7420 7769 7468 2061 2070   object with a p
+0001ac60: 7562 6c69 6320 6275 636b 6574 0a20 2020  ublic bucket.   
+0001ac70: 2020 2020 2073 746f 7261 6765 5f6f 626a       storage_obj
+0001ac80: 203d 2073 746f 7261 6765 5f6c 6962 2e53   = storage_lib.S
+0001ac90: 746f 7261 6765 2873 6f75 7263 653d 7265  torage(source=re
+0001aca0: 7175 6573 742e 7061 7261 6d29 0a20 2020  quest.param).   
+0001acb0: 2020 2020 2079 6965 6c64 2073 746f 7261       yield stora
+0001acc0: 6765 5f6f 626a 0a20 2020 2020 2020 2023  ge_obj.        #
+0001acd0: 2054 6869 7320 646f 6573 206e 6f74 2072   This does not r
+0001ace0: 6571 7569 7265 2061 6e79 2064 656c 6574  equire any delet
+0001acf0: 696f 6e20 6c6f 6769 6320 6265 6361 7573  ion logic becaus
+0001ad00: 6520 6974 2069 7320 6120 7075 626c 6963  e it is a public
+0001ad10: 2062 7563 6b65 740a 2020 2020 2020 2020   bucket.        
+0001ad20: 2320 616e 6420 7368 6f75 6c64 206e 6f74  # and should not
+0001ad30: 2067 6574 2061 6464 6564 2074 6f20 676c   get added to gl
+0001ad40: 6f62 616c 5f75 7365 725f 7374 6174 652e  obal_user_state.
+0001ad50: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
+0001ad60: 726b 2e70 6172 616d 6574 7269 7a65 2827  rk.parametrize('
+0001ad70: 7374 6f72 655f 7479 7065 272c 205b 0a20  store_type', [. 
+0001ad80: 2020 2020 2020 2073 746f 7261 6765 5f6c         storage_l
+0001ad90: 6962 2e53 746f 7265 5479 7065 2e53 332c  ib.StoreType.S3,
+0001ada0: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
+0001adb0: 7265 5479 7065 2e47 4353 2c0a 2020 2020  reType.GCS,.    
+0001adc0: 2020 2020 7079 7465 7374 2e70 6172 616d      pytest.param
+0001add0: 2873 746f 7261 6765 5f6c 6962 2e53 746f  (storage_lib.Sto
+0001ade0: 7265 5479 7065 2e52 322c 206d 6172 6b73  reType.R2, marks
+0001adf0: 3d70 7974 6573 742e 6d61 726b 2e63 6c6f  =pytest.mark.clo
+0001ae00: 7564 666c 6172 6529 0a20 2020 205d 290a  udflare).    ]).
+0001ae10: 2020 2020 6465 6620 7465 7374 5f6e 6577      def test_new
+0001ae20: 5f62 7563 6b65 745f 6372 6561 7469 6f6e  _bucket_creation
+0001ae30: 5f61 6e64 5f64 656c 6574 696f 6e28 7365  _and_deletion(se
+0001ae40: 6c66 2c20 746d 705f 6c6f 6361 6c5f 7374  lf, tmp_local_st
+0001ae50: 6f72 6167 655f 6f62 6a2c 0a20 2020 2020  orage_obj,.     
+0001ae60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae80: 2020 2020 2020 2020 2073 746f 7265 5f74           store_t
+0001ae90: 7970 6529 3a0a 2020 2020 2020 2020 2320  ype):.        # 
+0001aea0: 4372 6561 7465 7320 6120 6e65 7720 6275  Creates a new bu
+0001aeb0: 636b 6574 2077 6974 6820 6120 6c6f 6361  cket with a loca
+0001aec0: 6c20 736f 7572 6365 2c20 7570 6c6f 6164  l source, upload
+0001aed0: 7320 6669 6c65 7320 746f 2069 740a 2020  s files to it.  
+0001aee0: 2020 2020 2020 2320 616e 6420 6465 6c65        # and dele
+0001aef0: 7465 7320 6974 2e0a 2020 2020 2020 2020  tes it..        
+0001af00: 746d 705f 6c6f 6361 6c5f 7374 6f72 6167  tmp_local_storag
+0001af10: 655f 6f62 6a2e 6164 645f 7374 6f72 6528  e_obj.add_store(
+0001af20: 7374 6f72 655f 7479 7065 290a 0a20 2020  store_type)..   
+0001af30: 2020 2020 2023 2052 756e 2073 6b79 2073       # Run sky s
+0001af40: 746f 7261 6765 206c 7320 746f 2063 6865  torage ls to che
+0001af50: 636b 2069 6620 7374 6f72 6167 6520 6f62  ck if storage ob
+0001af60: 6a65 6374 2065 7869 7374 7320 696e 2074  ject exists in t
+0001af70: 6865 206f 7574 7075 740a 2020 2020 2020  he output.      
+0001af80: 2020 6f75 7420 3d20 7375 6270 726f 6365    out = subproce
+0001af90: 7373 2e63 6865 636b 5f6f 7574 7075 7428  ss.check_output(
+0001afa0: 5b27 736b 7927 2c20 2773 746f 7261 6765  ['sky', 'storage
+0001afb0: 272c 2027 6c73 275d 290a 2020 2020 2020  ', 'ls']).      
+0001afc0: 2020 6173 7365 7274 2074 6d70 5f6c 6f63    assert tmp_loc
+0001afd0: 616c 5f73 746f 7261 6765 5f6f 626a 2e6e  al_storage_obj.n
+0001afe0: 616d 6520 696e 206f 7574 2e64 6563 6f64  ame in out.decod
+0001aff0: 6528 2775 7466 2d38 2729 0a0a 2020 2020  e('utf-8')..    
+0001b000: 2020 2020 2320 5275 6e20 736b 7920 7374      # Run sky st
+0001b010: 6f72 6167 6520 6465 6c65 7465 2074 6f20  orage delete to 
+0001b020: 6465 6c65 7465 2074 6865 2073 746f 7261  delete the stora
+0001b030: 6765 206f 626a 6563 740a 2020 2020 2020  ge object.      
+0001b040: 2020 7375 6270 726f 6365 7373 2e63 6865    subprocess.che
+0001b050: 636b 5f6f 7574 7075 7428 0a20 2020 2020  ck_output(.     
+0001b060: 2020 2020 2020 205b 2773 6b79 272c 2027         ['sky', '
+0001b070: 7374 6f72 6167 6527 2c20 2764 656c 6574  storage', 'delet
+0001b080: 6527 2c20 746d 705f 6c6f 6361 6c5f 7374  e', tmp_local_st
+0001b090: 6f72 6167 655f 6f62 6a2e 6e61 6d65 5d29  orage_obj.name])
+0001b0a0: 0a0a 2020 2020 2020 2020 2320 5275 6e20  ..        # Run 
+0001b0b0: 736b 7920 7374 6f72 6167 6520 6c73 2074  sky storage ls t
+0001b0c0: 6f20 6368 6563 6b20 6966 2073 746f 7261  o check if stora
+0001b0d0: 6765 206f 626a 6563 7420 6973 2064 656c  ge object is del
+0001b0e0: 6574 6564 0a20 2020 2020 2020 206f 7574  eted.        out
+0001b0f0: 203d 2073 7562 7072 6f63 6573 732e 6368   = subprocess.ch
+0001b100: 6563 6b5f 6f75 7470 7574 285b 2773 6b79  eck_output(['sky
+0001b110: 272c 2027 7374 6f72 6167 6527 2c20 276c  ', 'storage', 'l
+0001b120: 7327 5d29 0a20 2020 2020 2020 2061 7373  s']).        ass
+0001b130: 6572 7420 746d 705f 6c6f 6361 6c5f 7374  ert tmp_local_st
+0001b140: 6f72 6167 655f 6f62 6a2e 6e61 6d65 206e  orage_obj.name n
+0001b150: 6f74 2069 6e20 6f75 742e 6465 636f 6465  ot in out.decode
+0001b160: 2827 7574 662d 3827 290a 0a20 2020 2040  ('utf-8')..    @
+0001b170: 7079 7465 7374 2e6d 6172 6b2e 7864 6973  pytest.mark.xdis
+0001b180: 745f 6772 6f75 7028 276d 756c 7469 706c  t_group('multipl
+0001b190: 655f 6275 636b 6574 5f64 656c 6574 696f  e_bucket_deletio
+0001b1a0: 6e27 290a 2020 2020 4070 7974 6573 742e  n').    @pytest.
+0001b1b0: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
+0001b1c0: 2827 7374 6f72 655f 7479 7065 272c 205b  ('store_type', [
+0001b1d0: 0a20 2020 2020 2020 2073 746f 7261 6765  .        storage
+0001b1e0: 5f6c 6962 2e53 746f 7265 5479 7065 2e53  _lib.StoreType.S
+0001b1f0: 332c 2073 746f 7261 6765 5f6c 6962 2e53  3, storage_lib.S
+0001b200: 746f 7265 5479 7065 2e47 4353 2c0a 2020  toreType.GCS,.  
+0001b210: 2020 2020 2020 7079 7465 7374 2e70 6172        pytest.par
+0001b220: 616d 2873 746f 7261 6765 5f6c 6962 2e53  am(storage_lib.S
+0001b230: 746f 7265 5479 7065 2e52 322c 206d 6172  toreType.R2, mar
+0001b240: 6b73 3d70 7974 6573 742e 6d61 726b 2e63  ks=pytest.mark.c
+0001b250: 6c6f 7564 666c 6172 6529 0a20 2020 205d  loudflare).    ]
+0001b260: 290a 2020 2020 6465 6620 7465 7374 5f6d  ).    def test_m
+0001b270: 756c 7469 706c 655f 6275 636b 6574 735f  ultiple_buckets_
+0001b280: 6372 6561 7469 6f6e 5f61 6e64 5f64 656c  creation_and_del
+0001b290: 6574 696f 6e28 0a20 2020 2020 2020 2020  etion(.         
+0001b2a0: 2020 2073 656c 662c 2074 6d70 5f6d 756c     self, tmp_mul
+0001b2b0: 7469 706c 655f 7363 7261 7463 685f 7374  tiple_scratch_st
+0001b2c0: 6f72 6167 655f 6f62 6a2c 2073 746f 7265  orage_obj, store
+0001b2d0: 5f74 7970 6529 3a0a 2020 2020 2020 2020  _type):.        
+0001b2e0: 2320 4372 6561 7465 7320 6d75 6c74 6970  # Creates multip
+0001b2f0: 6c65 206e 6577 2062 7563 6b65 7473 2835  le new buckets(5
+0001b300: 2062 7563 6b65 7473 2920 7769 7468 2061   buckets) with a
+0001b310: 206c 6f63 616c 2073 6f75 7263 650a 2020   local source.  
+0001b320: 2020 2020 2020 2320 616e 6420 6465 6c65        # and dele
+0001b330: 7465 7320 7468 656d 2e0a 2020 2020 2020  tes them..      
+0001b340: 2020 7374 6f72 6167 655f 6f62 6a5f 6e61    storage_obj_na
+0001b350: 6d65 203d 205b 5d0a 2020 2020 2020 2020  me = [].        
+0001b360: 666f 7220 7374 6f72 655f 6f62 6a20 696e  for store_obj in
+0001b370: 2074 6d70 5f6d 756c 7469 706c 655f 7363   tmp_multiple_sc
+0001b380: 7261 7463 685f 7374 6f72 6167 655f 6f62  ratch_storage_ob
+0001b390: 6a3a 0a20 2020 2020 2020 2020 2020 2073  j:.            s
+0001b3a0: 746f 7265 5f6f 626a 2e61 6464 5f73 746f  tore_obj.add_sto
+0001b3b0: 7265 2873 746f 7265 5f74 7970 6529 0a20  re(store_type). 
+0001b3c0: 2020 2020 2020 2020 2020 2073 746f 7261             stora
+0001b3d0: 6765 5f6f 626a 5f6e 616d 652e 6170 7065  ge_obj_name.appe
+0001b3e0: 6e64 2873 746f 7265 5f6f 626a 2e6e 616d  nd(store_obj.nam
+0001b3f0: 6529 0a0a 2020 2020 2020 2020 2320 5275  e)..        # Ru
+0001b400: 6e20 736b 7920 7374 6f72 6167 6520 6c73  n sky storage ls
+0001b410: 2074 6f20 6368 6563 6b20 6966 2061 6c6c   to check if all
+0001b420: 2073 746f 7261 6765 206f 626a 6563 7473   storage objects
+0001b430: 2065 7869 7374 7320 696e 2074 6865 0a20   exists in the. 
+0001b440: 2020 2020 2020 2023 206f 7574 7075 7420         # output 
+0001b450: 6669 6c74 6572 6564 2062 7920 7374 6f72  filtered by stor
+0001b460: 6520 7479 7065 0a20 2020 2020 2020 206f  e type.        o
+0001b470: 7574 5f61 6c6c 203d 2073 7562 7072 6f63  ut_all = subproc
+0001b480: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
+0001b490: 285b 2773 6b79 272c 2027 7374 6f72 6167  (['sky', 'storag
+0001b4a0: 6527 2c20 276c 7327 5d29 0a20 2020 2020  e', 'ls']).     
+0001b4b0: 2020 206f 7574 203d 205b 0a20 2020 2020     out = [.     
+0001b4c0: 2020 2020 2020 2069 7465 6d2e 7370 6c69         item.spli
+0001b4d0: 7428 295b 305d 0a20 2020 2020 2020 2020  t()[0].         
+0001b4e0: 2020 2066 6f72 2069 7465 6d20 696e 206f     for item in o
+0001b4f0: 7574 5f61 6c6c 2e64 6563 6f64 6528 2775  ut_all.decode('u
+0001b500: 7466 2d38 2729 2e73 706c 6974 6c69 6e65  tf-8').splitline
+0001b510: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+0001b520: 6966 2073 746f 7265 5f74 7970 652e 7661  if store_type.va
+0001b530: 6c75 6520 696e 2069 7465 6d0a 2020 2020  lue in item.    
+0001b540: 2020 2020 5d0a 2020 2020 2020 2020 6173      ].        as
+0001b550: 7365 7274 2061 6c6c 285b 6974 656d 2069  sert all([item i
+0001b560: 6e20 6f75 7420 666f 7220 6974 656d 2069  n out for item i
+0001b570: 6e20 7374 6f72 6167 655f 6f62 6a5f 6e61  n storage_obj_na
+0001b580: 6d65 5d29 0a0a 2020 2020 2020 2020 2320  me])..        # 
+0001b590: 5275 6e20 736b 7920 7374 6f72 6167 6520  Run sky storage 
+0001b5a0: 6465 6c65 7465 2061 6c6c 2074 6f20 6465  delete all to de
+0001b5b0: 6c65 7465 2061 6c6c 2073 746f 7261 6765  lete all storage
+0001b5c0: 206f 626a 6563 7473 0a20 2020 2020 2020   objects.       
+0001b5d0: 2064 656c 6574 655f 636d 6420 3d20 5b27   delete_cmd = ['
+0001b5e0: 736b 7927 2c20 2773 746f 7261 6765 272c  sky', 'storage',
+0001b5f0: 2027 6465 6c65 7465 275d 0a20 2020 2020   'delete'].     
+0001b600: 2020 2064 656c 6574 655f 636d 6420 2b3d     delete_cmd +=
+0001b610: 2073 746f 7261 6765 5f6f 626a 5f6e 616d   storage_obj_nam
+0001b620: 650a 2020 2020 2020 2020 7375 6270 726f  e.        subpro
+0001b630: 6365 7373 2e63 6865 636b 5f6f 7574 7075  cess.check_outpu
+0001b640: 7428 6465 6c65 7465 5f63 6d64 290a 0a20  t(delete_cmd).. 
+0001b650: 2020 2020 2020 2023 2052 756e 2073 6b79         # Run sky
+0001b660: 2073 746f 7261 6765 206c 7320 746f 2063   storage ls to c
+0001b670: 6865 636b 2069 6620 616c 6c20 7374 6f72  heck if all stor
+0001b680: 6167 6520 6f62 6a65 6374 7320 6669 6c74  age objects filt
+0001b690: 6572 6564 2062 7920 7374 6f72 650a 2020  ered by store.  
+0001b6a0: 2020 2020 2020 2320 7479 7065 2061 7265        # type are
+0001b6b0: 2064 656c 6574 6564 0a20 2020 2020 2020   deleted.       
+0001b6c0: 206f 7574 5f61 6c6c 203d 2073 7562 7072   out_all = subpr
+0001b6d0: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
+0001b6e0: 7574 285b 2773 6b79 272c 2027 7374 6f72  ut(['sky', 'stor
+0001b6f0: 6167 6527 2c20 276c 7327 5d29 0a20 2020  age', 'ls']).   
+0001b700: 2020 2020 206f 7574 203d 205b 0a20 2020       out = [.   
+0001b710: 2020 2020 2020 2020 2069 7465 6d2e 7370           item.sp
+0001b720: 6c69 7428 295b 305d 0a20 2020 2020 2020  lit()[0].       
+0001b730: 2020 2020 2066 6f72 2069 7465 6d20 696e       for item in
+0001b740: 206f 7574 5f61 6c6c 2e64 6563 6f64 6528   out_all.decode(
+0001b750: 2775 7466 2d38 2729 2e73 706c 6974 6c69  'utf-8').splitli
+0001b760: 6e65 7328 290a 2020 2020 2020 2020 2020  nes().          
+0001b770: 2020 6966 2073 746f 7265 5f74 7970 652e    if store_type.
+0001b780: 7661 6c75 6520 696e 2069 7465 6d0a 2020  value in item.  
+0001b790: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+0001b7a0: 6173 7365 7274 2061 6c6c 285b 6974 656d  assert all([item
+0001b7b0: 206e 6f74 2069 6e20 6f75 7420 666f 7220   not in out for 
+0001b7c0: 6974 656d 2069 6e20 7374 6f72 6167 655f  item in storage_
+0001b7d0: 6f62 6a5f 6e61 6d65 5d29 0a0a 2020 2020  obj_name])..    
+0001b7e0: 4070 7974 6573 742e 6d61 726b 2e70 6172  @pytest.mark.par
+0001b7f0: 616d 6574 7269 7a65 2827 7374 6f72 655f  ametrize('store_
+0001b800: 7479 7065 272c 205b 0a20 2020 2020 2020  type', [.       
+0001b810: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
+0001b820: 7265 5479 7065 2e53 332c 2073 746f 7261  reType.S3, stora
+0001b830: 6765 5f6c 6962 2e53 746f 7265 5479 7065  ge_lib.StoreType
+0001b840: 2e47 4353 2c0a 2020 2020 2020 2020 7079  .GCS,.        py
+0001b850: 7465 7374 2e70 6172 616d 2873 746f 7261  test.param(stora
+0001b860: 6765 5f6c 6962 2e53 746f 7265 5479 7065  ge_lib.StoreType
+0001b870: 2e52 322c 206d 6172 6b73 3d70 7974 6573  .R2, marks=pytes
+0001b880: 742e 6d61 726b 2e63 6c6f 7564 666c 6172  t.mark.cloudflar
+0001b890: 6529 0a20 2020 205d 290a 2020 2020 6465  e).    ]).    de
+0001b8a0: 6620 7465 7374 5f62 7563 6b65 745f 6578  f test_bucket_ex
+0001b8b0: 7465 726e 616c 5f64 656c 6574 696f 6e28  ternal_deletion(
+0001b8c0: 7365 6c66 2c20 746d 705f 7363 7261 7463  self, tmp_scratc
+0001b8d0: 685f 7374 6f72 6167 655f 6f62 6a2c 0a20  h_storage_obj,. 
+0001b8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b900: 2020 2020 2073 746f 7265 5f74 7970 6529       store_type)
+0001b910: 3a0a 2020 2020 2020 2020 2320 4372 6561  :.        # Crea
+0001b920: 7465 7320 6120 6275 636b 6574 2c20 6465  tes a bucket, de
+0001b930: 6c65 7465 7320 6974 2065 7874 6572 6e61  letes it externa
+0001b940: 6c6c 7920 7573 696e 6720 636c 6f75 6420  lly using cloud 
+0001b950: 636c 6920 636f 6d6d 616e 6473 0a20 2020  cli commands.   
+0001b960: 2020 2020 2023 2061 6e64 2074 6865 6e20       # and then 
+0001b970: 7472 6965 7320 746f 2064 656c 6574 6520  tries to delete 
+0001b980: 6974 2075 7369 6e67 2073 6b79 2073 746f  it using sky sto
+0001b990: 7261 6765 2064 656c 6574 652e 0a20 2020  rage delete..   
+0001b9a0: 2020 2020 2074 6d70 5f73 6372 6174 6368       tmp_scratch
+0001b9b0: 5f73 746f 7261 6765 5f6f 626a 2e61 6464  _storage_obj.add
+0001b9c0: 5f73 746f 7265 2873 746f 7265 5f74 7970  _store(store_typ
+0001b9d0: 6529 0a0a 2020 2020 2020 2020 2320 5275  e)..        # Ru
+0001b9e0: 6e20 736b 7920 7374 6f72 6167 6520 6c73  n sky storage ls
+0001b9f0: 2074 6f20 6368 6563 6b20 6966 2073 746f   to check if sto
+0001ba00: 7261 6765 206f 626a 6563 7420 6578 6973  rage object exis
+0001ba10: 7473 2069 6e20 7468 6520 6f75 7470 7574  ts in the output
+0001ba20: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
+0001ba30: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
+0001ba40: 6f75 7470 7574 285b 2773 6b79 272c 2027  output(['sky', '
+0001ba50: 7374 6f72 6167 6527 2c20 276c 7327 5d29  storage', 'ls'])
+0001ba60: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0001ba70: 746d 705f 7363 7261 7463 685f 7374 6f72  tmp_scratch_stor
+0001ba80: 6167 655f 6f62 6a2e 6e61 6d65 2069 6e20  age_obj.name in 
+0001ba90: 6f75 742e 6465 636f 6465 2827 7574 662d  out.decode('utf-
+0001baa0: 3827 290a 0a20 2020 2020 2020 2023 2044  8')..        # D
+0001bab0: 656c 6574 6520 6275 636b 6574 2065 7874  elete bucket ext
+0001bac0: 6572 6e61 6c6c 790a 2020 2020 2020 2020  ernally.        
+0001bad0: 636d 6420 3d20 7365 6c66 2e63 6c69 5f64  cmd = self.cli_d
+0001bae0: 656c 6574 655f 636d 6428 7374 6f72 655f  elete_cmd(store_
+0001baf0: 7479 7065 2c20 746d 705f 7363 7261 7463  type, tmp_scratc
+0001bb00: 685f 7374 6f72 6167 655f 6f62 6a2e 6e61  h_storage_obj.na
+0001bb10: 6d65 290a 2020 2020 2020 2020 7375 6270  me).        subp
+0001bb20: 726f 6365 7373 2e63 6865 636b 5f6f 7574  rocess.check_out
+0001bb30: 7075 7428 636d 642c 2073 6865 6c6c 3d54  put(cmd, shell=T
+0001bb40: 7275 6529 0a0a 2020 2020 2020 2020 2320  rue)..        # 
+0001bb50: 5275 6e20 736b 7920 7374 6f72 6167 6520  Run sky storage 
+0001bb60: 6465 6c65 7465 2074 6f20 6465 6c65 7465  delete to delete
+0001bb70: 2074 6865 2073 746f 7261 6765 206f 626a   the storage obj
+0001bb80: 6563 740a 2020 2020 2020 2020 6f75 7420  ect.        out 
+0001bb90: 3d20 7375 6270 726f 6365 7373 2e63 6865  = subprocess.che
+0001bba0: 636b 5f6f 7574 7075 7428 0a20 2020 2020  ck_output(.     
+0001bbb0: 2020 2020 2020 205b 2773 6b79 272c 2027         ['sky', '
+0001bbc0: 7374 6f72 6167 6527 2c20 2764 656c 6574  storage', 'delet
+0001bbd0: 6527 2c20 746d 705f 7363 7261 7463 685f  e', tmp_scratch_
+0001bbe0: 7374 6f72 6167 655f 6f62 6a2e 6e61 6d65  storage_obj.name
+0001bbf0: 5d29 0a20 2020 2020 2020 2023 204d 616b  ]).        # Mak
+0001bc00: 6520 7375 7265 2062 7563 6b65 7420 7761  e sure bucket wa
+0001bc10: 7320 6e6f 7420 6372 6561 7465 6420 6475  s not created du
+0001bc20: 7269 6e67 2064 656c 6574 696f 6e20 2873  ring deletion (s
+0001bc30: 6565 2069 7373 7565 2023 3133 3232 290a  ee issue #1322).
+0001bc40: 2020 2020 2020 2020 6173 7365 7274 2027          assert '
+0001bc50: 6372 6561 7465 6427 206e 6f74 2069 6e20  created' not in 
+0001bc60: 6f75 742e 6465 636f 6465 2827 7574 662d  out.decode('utf-
+0001bc70: 3827 292e 6c6f 7765 7228 290a 0a20 2020  8').lower()..   
+0001bc80: 2020 2020 2023 2052 756e 2073 6b79 2073       # Run sky s
+0001bc90: 746f 7261 6765 206c 7320 746f 2063 6865  torage ls to che
+0001bca0: 636b 2069 6620 7374 6f72 6167 6520 6f62  ck if storage ob
+0001bcb0: 6a65 6374 2069 7320 6465 6c65 7465 640a  ject is deleted.
+0001bcc0: 2020 2020 2020 2020 6f75 7420 3d20 7375          out = su
+0001bcd0: 6270 726f 6365 7373 2e63 6865 636b 5f6f  bprocess.check_o
+0001bce0: 7574 7075 7428 5b27 736b 7927 2c20 2773  utput(['sky', 's
+0001bcf0: 746f 7261 6765 272c 2027 6c73 275d 290a  torage', 'ls']).
+0001bd00: 2020 2020 2020 2020 6173 7365 7274 2074          assert t
+0001bd10: 6d70 5f73 6372 6174 6368 5f73 746f 7261  mp_scratch_stora
+0001bd20: 6765 5f6f 626a 2e6e 616d 6520 6e6f 7420  ge_obj.name not 
+0001bd30: 696e 206f 7574 2e64 6563 6f64 6528 2775  in out.decode('u
+0001bd40: 7466 2d38 2729 0a0a 2020 2020 4070 7974  tf-8')..    @pyt
+0001bd50: 6573 742e 6d61 726b 2e70 6172 616d 6574  est.mark.paramet
+0001bd60: 7269 7a65 2827 7374 6f72 655f 7479 7065  rize('store_type
+0001bd70: 272c 205b 0a20 2020 2020 2020 2073 746f  ', [.        sto
+0001bd80: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
+0001bd90: 7065 2e53 332c 2073 746f 7261 6765 5f6c  pe.S3, storage_l
+0001bda0: 6962 2e53 746f 7265 5479 7065 2e47 4353  ib.StoreType.GCS
+0001bdb0: 2c0a 2020 2020 2020 2020 7079 7465 7374  ,.        pytest
+0001bdc0: 2e70 6172 616d 2873 746f 7261 6765 5f6c  .param(storage_l
+0001bdd0: 6962 2e53 746f 7265 5479 7065 2e52 322c  ib.StoreType.R2,
+0001bde0: 206d 6172 6b73 3d70 7974 6573 742e 6d61   marks=pytest.ma
+0001bdf0: 726b 2e63 6c6f 7564 666c 6172 6529 0a20  rk.cloudflare). 
+0001be00: 2020 205d 290a 2020 2020 6465 6620 7465     ]).    def te
+0001be10: 7374 5f62 7563 6b65 745f 6275 6c6b 5f64  st_bucket_bulk_d
+0001be20: 656c 6574 696f 6e28 7365 6c66 2c20 7374  eletion(self, st
+0001be30: 6f72 655f 7479 7065 2c20 746d 705f 6275  ore_type, tmp_bu
+0001be40: 6c6b 5f64 656c 5f73 746f 7261 6765 5f6f  lk_del_storage_o
+0001be50: 626a 293a 0a20 2020 2020 2020 2023 2043  bj):.        # C
+0001be60: 7265 6174 6573 2061 2074 656d 7020 666f  reates a temp fo
+0001be70: 6c64 6572 2077 6974 6820 6f76 6572 2032  lder with over 2
+0001be80: 3536 2066 696c 6573 2061 6e64 2066 6f6c  56 files and fol
+0001be90: 6465 7273 2c20 7570 6c6f 6164 0a20 2020  ders, upload.   
+0001bea0: 2020 2020 2023 2066 696c 6573 2061 6e64       # files and
+0001beb0: 2066 6f6c 6465 7273 2074 6f20 6120 6e65   folders to a ne
+0001bec0: 7720 6275 636b 6574 2c20 7468 656e 2064  w bucket, then d
+0001bed0: 656c 6574 6520 6275 636b 6574 2e0a 2020  elete bucket..  
+0001bee0: 2020 2020 2020 746d 705f 6275 6c6b 5f64        tmp_bulk_d
+0001bef0: 656c 5f73 746f 7261 6765 5f6f 626a 2e61  el_storage_obj.a
+0001bf00: 6464 5f73 746f 7265 2873 746f 7265 5f74  dd_store(store_t
+0001bf10: 7970 6529 0a0a 2020 2020 2020 2020 7375  ype)..        su
+0001bf20: 6270 726f 6365 7373 2e63 6865 636b 5f6f  bprocess.check_o
+0001bf30: 7574 7075 7428 0a20 2020 2020 2020 2020  utput(.         
+0001bf40: 2020 205b 2773 6b79 272c 2027 7374 6f72     ['sky', 'stor
+0001bf50: 6167 6527 2c20 2764 656c 6574 6527 2c20  age', 'delete', 
+0001bf60: 746d 705f 6275 6c6b 5f64 656c 5f73 746f  tmp_bulk_del_sto
+0001bf70: 7261 6765 5f6f 626a 2e6e 616d 655d 290a  rage_obj.name]).
+0001bf80: 0a20 2020 2020 2020 206f 7574 7075 7420  .        output 
+0001bf90: 3d20 7375 6270 726f 6365 7373 2e63 6865  = subprocess.che
+0001bfa0: 636b 5f6f 7574 7075 7428 5b27 736b 7927  ck_output(['sky'
+0001bfb0: 2c20 2773 746f 7261 6765 272c 2027 6c73  , 'storage', 'ls
+0001bfc0: 275d 290a 2020 2020 2020 2020 6173 7365  ']).        asse
+0001bfd0: 7274 2074 6d70 5f62 756c 6b5f 6465 6c5f  rt tmp_bulk_del_
+0001bfe0: 7374 6f72 6167 655f 6f62 6a2e 6e61 6d65  storage_obj.name
+0001bff0: 206e 6f74 2069 6e20 6f75 7470 7574 2e64   not in output.d
+0001c000: 6563 6f64 6528 2775 7466 2d38 2729 0a0a  ecode('utf-8')..
+0001c010: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+0001c020: 2e70 6172 616d 6574 7269 7a65 280a 2020  .parametrize(.  
+0001c030: 2020 2020 2020 2774 6d70 5f70 7562 6c69        'tmp_publi
+0001c040: 635f 7374 6f72 6167 655f 6f62 6a2c 2073  c_storage_obj, s
+0001c050: 746f 7265 5f74 7970 6527 2c0a 2020 2020  tore_type',.    
+0001c060: 2020 2020 5b28 2773 333a 2f2f 7463 6761      [('s3://tcga
+0001c070: 2d32 2d6f 7065 6e27 2c20 7374 6f72 6167  -2-open', storag
+0001c080: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
+0001c090: 5333 292c 0a20 2020 2020 2020 2020 2827  S3),.         ('
+0001c0a0: 7333 3a2f 2f64 6967 6974 616c 636f 7270  s3://digitalcorp
+0001c0b0: 6f72 6127 2c20 7374 6f72 6167 655f 6c69  ora', storage_li
+0001c0c0: 622e 5374 6f72 6554 7970 652e 5333 292c  b.StoreType.S3),
+0001c0d0: 0a20 2020 2020 2020 2020 2827 6773 3a2f  .         ('gs:/
+0001c0e0: 2f67 6370 2d70 7562 6c69 632d 6461 7461  /gcp-public-data
+0001c0f0: 2d73 656e 7469 6e65 6c2d 3227 2c20 7374  -sentinel-2', st
+0001c100: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
+0001c110: 7970 652e 4743 5329 5d2c 0a20 2020 2020  ype.GCS)],.     
+0001c120: 2020 2069 6e64 6972 6563 743d 5b27 746d     indirect=['tm
+0001c130: 705f 7075 626c 6963 5f73 746f 7261 6765  p_public_storage
+0001c140: 5f6f 626a 275d 290a 2020 2020 6465 6620  _obj']).    def 
+0001c150: 7465 7374 5f70 7562 6c69 635f 6275 636b  test_public_buck
+0001c160: 6574 2873 656c 662c 2074 6d70 5f70 7562  et(self, tmp_pub
+0001c170: 6c69 635f 7374 6f72 6167 655f 6f62 6a2c  lic_storage_obj,
+0001c180: 2073 746f 7265 5f74 7970 6529 3a0a 2020   store_type):.  
+0001c190: 2020 2020 2020 2320 4372 6561 7465 7320        # Creates 
+0001c1a0: 6120 6e65 7720 6275 636b 6574 2077 6974  a new bucket wit
+0001c1b0: 6820 6120 7075 626c 6963 2073 6f75 7263  h a public sourc
+0001c1c0: 6520 616e 6420 7665 7269 6669 6573 2074  e and verifies t
+0001c1d0: 6861 7420 6974 2069 7320 6e6f 740a 2020  hat it is not.  
+0001c1e0: 2020 2020 2020 2320 6164 6465 6420 746f        # added to
+0001c1f0: 2067 6c6f 6261 6c5f 7573 6572 5f73 7461   global_user_sta
+0001c200: 7465 2e0a 2020 2020 2020 2020 746d 705f  te..        tmp_
+0001c210: 7075 626c 6963 5f73 746f 7261 6765 5f6f  public_storage_o
+0001c220: 626a 2e61 6464 5f73 746f 7265 2873 746f  bj.add_store(sto
+0001c230: 7265 5f74 7970 6529 0a0a 2020 2020 2020  re_type)..      
+0001c240: 2020 2320 5275 6e20 736b 7920 7374 6f72    # Run sky stor
+0001c250: 6167 6520 6c73 2074 6f20 6368 6563 6b20  age ls to check 
+0001c260: 6966 2073 746f 7261 6765 206f 626a 6563  if storage objec
+0001c270: 7420 6578 6973 7473 2069 6e20 7468 6520  t exists in the 
+0001c280: 6f75 7470 7574 0a20 2020 2020 2020 206f  output.        o
+0001c290: 7574 203d 2073 7562 7072 6f63 6573 732e  ut = subprocess.
+0001c2a0: 6368 6563 6b5f 6f75 7470 7574 285b 2773  check_output(['s
+0001c2b0: 6b79 272c 2027 7374 6f72 6167 6527 2c20  ky', 'storage', 
+0001c2c0: 276c 7327 5d29 0a20 2020 2020 2020 2061  'ls']).        a
+0001c2d0: 7373 6572 7420 746d 705f 7075 626c 6963  ssert tmp_public
+0001c2e0: 5f73 746f 7261 6765 5f6f 626a 2e6e 616d  _storage_obj.nam
+0001c2f0: 6520 6e6f 7420 696e 206f 7574 2e64 6563  e not in out.dec
+0001c300: 6f64 6528 2775 7466 2d38 2729 0a0a 2020  ode('utf-8')..  
+0001c310: 2020 4070 7974 6573 742e 6d61 726b 2e70    @pytest.mark.p
+0001c320: 6172 616d 6574 7269 7a65 2827 6e6f 6e65  arametrize('none
+0001c330: 7869 7374 5f62 7563 6b65 745f 7572 6c27  xist_bucket_url'
+0001c340: 2c20 5b0a 2020 2020 2020 2020 2773 333a  , [.        's3:
+0001c350: 2f2f 7b72 616e 646f 6d5f 6e61 6d65 7d27  //{random_name}'
+0001c360: 2c20 2767 733a 2f2f 7b72 616e 646f 6d5f  , 'gs://{random_
+0001c370: 6e61 6d65 7d27 2c0a 2020 2020 2020 2020  name}',.        
+0001c380: 7079 7465 7374 2e70 6172 616d 2827 7232  pytest.param('r2
+0001c390: 3a2f 2f7b 7261 6e64 6f6d 5f6e 616d 657d  ://{random_name}
+0001c3a0: 272c 206d 6172 6b73 3d70 7974 6573 742e  ', marks=pytest.
+0001c3b0: 6d61 726b 2e63 6c6f 7564 666c 6172 6529  mark.cloudflare)
+0001c3c0: 0a20 2020 205d 290a 2020 2020 6465 6620  .    ]).    def 
+0001c3d0: 7465 7374 5f6e 6f6e 6578 6973 7465 6e74  test_nonexistent
+0001c3e0: 5f62 7563 6b65 7428 7365 6c66 2c20 6e6f  _bucket(self, no
+0001c3f0: 6e65 7869 7374 5f62 7563 6b65 745f 7572  nexist_bucket_ur
+0001c400: 6c29 3a0a 2020 2020 2020 2020 2320 4174  l):.        # At
+0001c410: 7465 6d70 7473 2074 6f20 6372 6561 7465  tempts to create
+0001c420: 2066 6574 6368 2061 2073 7472 6f61 6765   fetch a stroage
+0001c430: 2077 6974 6820 6120 6e6f 6e2d 6578 6973   with a non-exis
+0001c440: 7465 6e74 2073 6f75 7263 652e 0a20 2020  tent source..   
+0001c450: 2020 2020 2023 2047 656e 6572 6174 6520       # Generate 
+0001c460: 6120 7261 6e64 6f6d 2062 7563 6b65 7420  a random bucket 
+0001c470: 6e61 6d65 2061 6e64 2076 6572 6966 7920  name and verify 
+0001c480: 6974 2064 6f65 736e 2774 2065 7869 7374  it doesn't exist
+0001c490: 3a0a 2020 2020 2020 2020 7265 7472 795f  :.        retry_
+0001c4a0: 636f 756e 7420 3d20 300a 2020 2020 2020  count = 0.      
+0001c4b0: 2020 7768 696c 6520 5472 7565 3a0a 2020    while True:.  
+0001c4c0: 2020 2020 2020 2020 2020 6e6f 6e65 7869            nonexi
+0001c4d0: 7374 5f62 7563 6b65 745f 6e61 6d65 203d  st_bucket_name =
+0001c4e0: 2073 7472 2875 7569 642e 7575 6964 3428   str(uuid.uuid4(
+0001c4f0: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
+0001c500: 6620 6e6f 6e65 7869 7374 5f62 7563 6b65  f nonexist_bucke
+0001c510: 745f 7572 6c2e 7374 6172 7473 7769 7468  t_url.startswith
+0001c520: 2827 7333 2729 3a0a 2020 2020 2020 2020  ('s3'):.        
+0001c530: 2020 2020 2020 2020 636f 6d6d 616e 6420          command 
+0001c540: 3d20 6627 6177 7320 7333 6170 6920 6865  = f'aws s3api he
+0001c550: 6164 2d62 7563 6b65 7420 2d2d 6275 636b  ad-bucket --buck
+0001c560: 6574 207b 6e6f 6e65 7869 7374 5f62 7563  et {nonexist_buc
+0001c570: 6b65 745f 6e61 6d65 7d27 0a20 2020 2020  ket_name}'.     
+0001c580: 2020 2020 2020 2020 2020 2065 7870 6563             expec
+0001c590: 7465 645f 6f75 7470 7574 203d 2027 3430  ted_output = '40
+0001c5a0: 3427 0a20 2020 2020 2020 2020 2020 2065  4'.            e
+0001c5b0: 6c69 6620 6e6f 6e65 7869 7374 5f62 7563  lif nonexist_buc
+0001c5c0: 6b65 745f 7572 6c2e 7374 6172 7473 7769  ket_url.startswi
+0001c5d0: 7468 2827 6773 2729 3a0a 2020 2020 2020  th('gs'):.      
+0001c5e0: 2020 2020 2020 2020 2020 636f 6d6d 616e            comman
+0001c5f0: 6420 3d20 6627 6773 7574 696c 206c 7320  d = f'gsutil ls 
+0001c600: 7b6e 6f6e 6578 6973 745f 6275 636b 6574  {nonexist_bucket
+0001c610: 5f75 726c 2e66 6f72 6d61 7428 7261 6e64  _url.format(rand
+0001c620: 6f6d 5f6e 616d 653d 6e6f 6e65 7869 7374  om_name=nonexist
+0001c630: 5f62 7563 6b65 745f 6e61 6d65 297d 270a  _bucket_name)}'.
+0001c640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c650: 6578 7065 6374 6564 5f6f 7574 7075 7420  expected_output 
+0001c660: 3d20 2742 7563 6b65 744e 6f74 466f 756e  = 'BucketNotFoun
+0001c670: 6445 7863 6570 7469 6f6e 270a 2020 2020  dException'.    
+0001c680: 2020 2020 2020 2020 656c 6966 206e 6f6e          elif non
+0001c690: 6578 6973 745f 6275 636b 6574 5f75 726c  exist_bucket_url
+0001c6a0: 2e73 7461 7274 7377 6974 6828 2772 3227  .startswith('r2'
+0001c6b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0001c6c0: 2020 2065 6e64 706f 696e 745f 7572 6c20     endpoint_url 
+0001c6d0: 3d20 636c 6f75 6466 6c61 7265 2e63 7265  = cloudflare.cre
+0001c6e0: 6174 655f 656e 6470 6f69 6e74 2829 0a20  ate_endpoint(). 
+0001c6f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001c700: 6f6d 6d61 6e64 203d 2066 2741 5753 5f53  ommand = f'AWS_S
+0001c710: 4841 5245 445f 4352 4544 454e 5449 414c  HARED_CREDENTIAL
+0001c720: 535f 4649 4c45 3d7b 636c 6f75 6466 6c61  S_FILE={cloudfla
+0001c730: 7265 2e52 325f 4352 4544 454e 5449 414c  re.R2_CREDENTIAL
+0001c740: 535f 5041 5448 7d20 6177 7320 7333 6170  S_PATH} aws s3ap
+0001c750: 6920 6865 6164 2d62 7563 6b65 7420 2d2d  i head-bucket --
+0001c760: 6275 636b 6574 207b 6e6f 6e65 7869 7374  bucket {nonexist
+0001c770: 5f62 7563 6b65 745f 6e61 6d65 7d20 2d2d  _bucket_name} --
+0001c780: 656e 6470 6f69 6e74 207b 656e 6470 6f69  endpoint {endpoi
+0001c790: 6e74 5f75 726c 7d20 2d2d 7072 6f66 696c  nt_url} --profil
+0001c7a0: 653d 7232 270a 2020 2020 2020 2020 2020  e=r2'.          
+0001c7b0: 2020 2020 2020 6578 7065 6374 6564 5f6f        expected_o
+0001c7c0: 7574 7075 7420 3d20 2734 3034 270a 2020  utput = '404'.  
+0001c7d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0001c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c7f0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0001c800: 2827 556e 7375 7070 6f72 7465 6420 6275  ('Unsupported bu
+0001c810: 636b 6574 2074 7970 6520 270a 2020 2020  cket type '.    
+0001c820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c830: 2020 2020 2020 2020 2020 2020 2066 277b               f'{
+0001c840: 6e6f 6e65 7869 7374 5f62 7563 6b65 745f  nonexist_bucket_
+0001c850: 7572 6c7d 2729 0a0a 2020 2020 2020 2020  url}')..        
+0001c860: 2020 2020 2320 4368 6563 6b20 6966 2062      # Check if b
+0001c870: 7563 6b65 7420 6578 6973 7473 2075 7369  ucket exists usi
+0001c880: 6e67 2074 6865 2063 6c69 3a0a 2020 2020  ng the cli:.    
+0001c890: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+0001c8a0: 2020 2020 2020 2020 2020 2020 206f 7574               out
+0001c8b0: 203d 2073 7562 7072 6f63 6573 732e 6368   = subprocess.ch
+0001c8c0: 6563 6b5f 6f75 7470 7574 2863 6f6d 6d61  eck_output(comma
+0001c8d0: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
+0001c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c900: 2020 7374 6465 7272 3d73 7562 7072 6f63    stderr=subproc
+0001c910: 6573 732e 5354 444f 5554 2c0a 2020 2020  ess.STDOUT,.    
+0001c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c940: 2020 2020 2020 2020 2020 7368 656c 6c3d            shell=
+0001c950: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+0001c960: 2020 6578 6365 7074 2073 7562 7072 6f63    except subproc
+0001c970: 6573 732e 4361 6c6c 6564 5072 6f63 6573  ess.CalledProces
+0001c980: 7345 7272 6f72 2061 7320 653a 0a20 2020  sError as e:.   
+0001c990: 2020 2020 2020 2020 2020 2020 206f 7574               out
+0001c9a0: 203d 2065 2e6f 7574 7075 740a 2020 2020   = e.output.    
+0001c9b0: 2020 2020 2020 2020 6f75 7420 3d20 6f75          out = ou
+0001c9c0: 742e 6465 636f 6465 2827 7574 662d 3827  t.decode('utf-8'
+0001c9d0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0001c9e0: 2065 7870 6563 7465 645f 6f75 7470 7574   expected_output
+0001c9f0: 2069 6e20 6f75 743a 0a20 2020 2020 2020   in out:.       
+0001ca00: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+0001ca10: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001ca20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ca30: 2072 6574 7279 5f63 6f75 6e74 202b 3d20   retry_count += 
+0001ca40: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+0001ca50: 2020 6966 2072 6574 7279 5f63 6f75 6e74    if retry_count
+0001ca60: 203e 2033 3a0a 2020 2020 2020 2020 2020   > 3:.          
+0001ca70: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0001ca80: 5275 6e74 696d 6545 7272 6f72 2827 556e  RuntimeError('Un
+0001ca90: 6162 6c65 2074 6f20 6669 6e64 2061 206e  able to find a n
+0001caa0: 6f6e 6578 6973 7465 6e74 2062 7563 6b65  onexistent bucke
+0001cab0: 7420 270a 2020 2020 2020 2020 2020 2020  t '.            
+0001cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cad0: 2020 2020 2020 2020 2020 2027 746f 2075             'to u
+0001cae0: 7365 2e20 5468 6973 2069 7320 6869 676c  se. This is higl
+0001caf0: 7920 756e 6c69 6b65 6c79 202d 2027 0a20  y unlikely - '. 
+0001cb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cb20: 2020 2020 2020 2763 6865 636b 2069 6620        'check if 
+0001cb30: 7468 6520 7465 7374 7320 6172 6520 636f  the tests are co
+0001cb40: 7272 6563 742e 2729 0a0a 2020 2020 2020  rrect.')..      
+0001cb50: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
+0001cb60: 6973 6573 280a 2020 2020 2020 2020 2020  ises(.          
+0001cb70: 2020 2020 2020 736b 792e 6578 6365 7074        sky.except
+0001cb80: 696f 6e73 2e53 746f 7261 6765 4275 636b  ions.StorageBuck
+0001cb90: 6574 4765 7445 7272 6f72 2c0a 2020 2020  etGetError,.    
+0001cba0: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
+0001cbb0: 683d 2741 7474 656d 7074 6564 2074 6f20  h='Attempted to 
+0001cbc0: 636f 6e6e 6563 7420 746f 2061 206e 6f6e  connect to a non
+0001cbd0: 2d65 7869 7374 656e 7420 6275 636b 6574  -existent bucket
+0001cbe0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+0001cbf0: 7374 6f72 6167 655f 6f62 6a20 3d20 7374  storage_obj = st
+0001cc00: 6f72 6167 655f 6c69 622e 5374 6f72 6167  orage_lib.Storag
+0001cc10: 6528 736f 7572 6365 3d6e 6f6e 6578 6973  e(source=nonexis
+0001cc20: 745f 6275 636b 6574 5f75 726c 2e66 6f72  t_bucket_url.for
+0001cc30: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+0001cc40: 2020 2020 2072 616e 646f 6d5f 6e61 6d65       random_name
+0001cc50: 3d6e 6f6e 6578 6973 745f 6275 636b 6574  =nonexist_bucket
+0001cc60: 5f6e 616d 6529 290a 0a20 2020 2040 7079  _name))..    @py
+0001cc70: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
+0001cc80: 7472 697a 6528 2770 7269 7661 7465 5f62  trize('private_b
+0001cc90: 7563 6b65 7427 2c0a 2020 2020 2020 2020  ucket',.        
+0001cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ccb0: 2020 2020 205b 6627 7333 3a2f 2f69 6d61       [f's3://ima
+0001ccc0: 6765 6e65 7427 2c20 6627 6773 3a2f 2f69  genet', f'gs://i
+0001ccd0: 6d61 6765 6e65 7427 5d29 0a20 2020 2064  magenet']).    d
+0001cce0: 6566 2074 6573 745f 7072 6976 6174 655f  ef test_private_
+0001ccf0: 6275 636b 6574 2873 656c 662c 2070 7269  bucket(self, pri
+0001cd00: 7661 7465 5f62 7563 6b65 7429 3a0a 2020  vate_bucket):.  
+0001cd10: 2020 2020 2020 2320 4174 7465 6d70 7473        # Attempts
+0001cd20: 2074 6f20 6163 6365 7373 2070 7269 7661   to access priva
+0001cd30: 7465 2062 7563 6b65 7473 206e 6f74 2062  te buckets not b
+0001cd40: 656c 6f6e 6769 6e67 2074 6f20 7468 6520  elonging to the 
+0001cd50: 7573 6572 2e0a 2020 2020 2020 2020 2320  user..        # 
+0001cd60: 5468 6573 6520 6275 636b 6574 7320 6172  These buckets ar
+0001cd70: 6520 6b6e 6f77 6e20 746f 2062 6520 7072  e known to be pr
+0001cd80: 6976 6174 652c 2062 7574 206d 6179 206e  ivate, but may n
+0001cd90: 6565 6420 746f 2062 6520 7570 6461 7465  eed to be update
+0001cda0: 6420 6966 0a20 2020 2020 2020 2023 2074  d if.        # t
+0001cdb0: 6865 7920 6172 6520 7265 6d6f 7665 6420  hey are removed 
+0001cdc0: 6279 2074 6865 6972 206f 776e 6572 732e  by their owners.
+0001cdd0: 0a20 2020 2020 2020 2070 7269 7661 7465  .        private
+0001cde0: 5f62 7563 6b65 745f 6e61 6d65 203d 2075  _bucket_name = u
+0001cdf0: 726c 6c69 622e 7061 7273 652e 7572 6c73  rllib.parse.urls
+0001ce00: 706c 6974 2870 7269 7661 7465 5f62 7563  plit(private_buc
+0001ce10: 6b65 7429 2e6e 6574 6c6f 630a 2020 2020  ket).netloc.    
+0001ce20: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
+0001ce30: 7261 6973 6573 280a 2020 2020 2020 2020  raises(.        
+0001ce40: 2020 2020 2020 2020 736b 792e 6578 6365          sky.exce
+0001ce50: 7074 696f 6e73 2e53 746f 7261 6765 4275  ptions.StorageBu
+0001ce60: 636b 6574 4765 7445 7272 6f72 2c0a 2020  cketGetError,.  
+0001ce70: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+0001ce80: 7463 683d 7374 6f72 6167 655f 6c69 622e  tch=storage_lib.
+0001ce90: 5f42 5543 4b45 545f 4641 494c 5f54 4f5f  _BUCKET_FAIL_TO_
+0001cea0: 434f 4e4e 4543 545f 4d45 5353 4147 452e  CONNECT_MESSAGE.
+0001ceb0: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+0001cec0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+0001ced0: 3d70 7269 7661 7465 5f62 7563 6b65 745f  =private_bucket_
+0001cee0: 6e61 6d65 2929 3a0a 2020 2020 2020 2020  name)):.        
+0001cef0: 2020 2020 7374 6f72 6167 655f 6f62 6a20      storage_obj 
+0001cf00: 3d20 7374 6f72 6167 655f 6c69 622e 5374  = storage_lib.St
+0001cf10: 6f72 6167 6528 736f 7572 6365 3d70 7269  orage(source=pri
+0001cf20: 7661 7465 5f62 7563 6b65 7429 0a0a 2020  vate_bucket)..  
+0001cf30: 2020 4070 7974 6573 742e 6d61 726b 2e70    @pytest.mark.p
+0001cf40: 6172 616d 6574 7269 7a65 2827 6578 745f  arametrize('ext_
+0001cf50: 6275 636b 6574 5f66 6978 7475 7265 2c20  bucket_fixture, 
+0001cf60: 7374 6f72 655f 7479 7065 272c 0a20 2020  store_type',.   
+0001cf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cf80: 2020 2020 2020 2020 2020 5b28 2774 6d70            [('tmp
+0001cf90: 5f61 7773 636c 695f 6275 636b 6574 272c  _awscli_bucket',
+0001cfa0: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
+0001cfb0: 7265 5479 7065 2e53 3329 2c0a 2020 2020  reType.S3),.    
+0001cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cfd0: 2020 2020 2020 2020 2020 2827 746d 705f            ('tmp_
+0001cfe0: 6773 7574 696c 5f62 7563 6b65 7427 2c20  gsutil_bucket', 
+0001cff0: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+0001d000: 6554 7970 652e 4743 5329 2c0a 2020 2020  eType.GCS),.    
+0001d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d020: 2020 2020 2020 2020 2020 7079 7465 7374            pytest
+0001d030: 2e70 6172 616d 2827 746d 705f 6177 7363  .param('tmp_awsc
+0001d040: 6c69 5f62 7563 6b65 745f 7232 272c 0a20  li_bucket_r2',. 
+0001d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d070: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
+0001d080: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
+0001d090: 5232 2c0a 2020 2020 2020 2020 2020 2020  R2,.            
+0001d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d0b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0001d0c0: 6172 6b73 3d70 7974 6573 742e 6d61 726b  arks=pytest.mark
+0001d0d0: 2e63 6c6f 7564 666c 6172 6529 5d29 0a20  .cloudflare)]). 
+0001d0e0: 2020 2064 6566 2074 6573 745f 7570 6c6f     def test_uplo
+0001d0f0: 6164 5f74 6f5f 6578 6973 7469 6e67 5f62  ad_to_existing_b
+0001d100: 7563 6b65 7428 7365 6c66 2c20 6578 745f  ucket(self, ext_
+0001d110: 6275 636b 6574 5f66 6978 7475 7265 2c20  bucket_fixture, 
+0001d120: 7265 7175 6573 742c 0a20 2020 2020 2020  request,.       
+0001d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d150: 746d 705f 736f 7572 6365 2c20 7374 6f72  tmp_source, stor
+0001d160: 655f 7479 7065 293a 0a20 2020 2020 2020  e_type):.       
+0001d170: 2023 2054 7269 6573 2075 706c 6f61 6469   # Tries uploadi
+0001d180: 6e67 2065 7869 7374 696e 6720 6669 6c65  ng existing file
+0001d190: 7320 746f 206e 6577 6c79 2063 7265 6174  s to newly creat
+0001d1a0: 6564 2062 7563 6b65 7420 286f 7574 7369  ed bucket (outsi
+0001d1b0: 6465 206f 660a 2020 2020 2020 2020 2320  de of.        # 
+0001d1c0: 736b 7929 2061 6e64 2076 6572 6966 6965  sky) and verifie
+0001d1d0: 7320 7468 6174 2066 696c 6573 2061 7265  s that files are
+0001d1e0: 2077 7269 7474 656e 2e0a 2020 2020 2020   written..      
+0001d1f0: 2020 6275 636b 6574 5f6e 616d 6520 3d20    bucket_name = 
+0001d200: 7265 7175 6573 742e 6765 7466 6978 7475  request.getfixtu
+0001d210: 7265 7661 6c75 6528 6578 745f 6275 636b  revalue(ext_buck
+0001d220: 6574 5f66 6978 7475 7265 290a 2020 2020  et_fixture).    
+0001d230: 2020 2020 7374 6f72 6167 655f 6f62 6a20      storage_obj 
+0001d240: 3d20 7374 6f72 6167 655f 6c69 622e 5374  = storage_lib.St
+0001d250: 6f72 6167 6528 6e61 6d65 3d62 7563 6b65  orage(name=bucke
+0001d260: 745f 6e61 6d65 2c20 736f 7572 6365 3d74  t_name, source=t
+0001d270: 6d70 5f73 6f75 7263 6529 0a20 2020 2020  mp_source).     
+0001d280: 2020 2073 746f 7261 6765 5f6f 626a 2e61     storage_obj.a
+0001d290: 6464 5f73 746f 7265 2873 746f 7265 5f74  dd_store(store_t
+0001d2a0: 7970 6529 0a0a 2020 2020 2020 2020 2320  ype)..        # 
+0001d2b0: 4368 6563 6b20 6966 2074 6d70 5f73 6f75  Check if tmp_sou
+0001d2c0: 7263 652f 746d 702d 6669 6c65 2065 7869  rce/tmp-file exi
+0001d2d0: 7374 7320 696e 2074 6865 2062 7563 6b65  sts in the bucke
+0001d2e0: 7420 7573 696e 6720 6177 7320 636c 690a  t using aws cli.
+0001d2f0: 2020 2020 2020 2020 6f75 7420 3d20 7375          out = su
+0001d300: 6270 726f 6365 7373 2e63 6865 636b 5f6f  bprocess.check_o
+0001d310: 7574 7075 7428 7365 6c66 2e63 6c69 5f6c  utput(self.cli_l
+0001d320: 735f 636d 6428 7374 6f72 655f 7479 7065  s_cmd(store_type
+0001d330: 2c20 6275 636b 6574 5f6e 616d 6529 2c0a  , bucket_name),.
+0001d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d360: 2020 2020 2020 7368 656c 6c3d 5472 7565        shell=True
+0001d370: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+0001d380: 2027 746d 702d 6669 6c65 2720 696e 206f   'tmp-file' in o
+0001d390: 7574 2e64 6563 6f64 6528 2775 7466 2d38  ut.decode('utf-8
+0001d3a0: 2729 2c20 5c0a 2020 2020 2020 2020 2020  '), \.          
+0001d3b0: 2020 2746 696c 6520 6e6f 7420 666f 756e    'File not foun
+0001d3c0: 6420 696e 2062 7563 6b65 7420 2d20 6f75  d in bucket - ou
+0001d3d0: 7470 7574 2077 6173 203a 207b 7d27 2e66  tput was : {}'.f
+0001d3e0: 6f72 6d61 7428 6f75 742e 6465 636f 6465  ormat(out.decode
+0001d3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d430: 2028 2775 7466 2d38 2729 290a 0a20 2020   ('utf-8'))..   
+0001d440: 2020 2020 2023 2043 6865 636b 2073 796d       # Check sym
+0001d450: 6c69 6e6b 7320 2d20 7379 6d6c 696e 6b73  links - symlinks
+0001d460: 2064 6f6e 2774 2067 6574 2063 6f70 6965   don't get copie
+0001d470: 6420 6279 2073 6b79 2073 746f 7261 6765  d by sky storage
+0001d480: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0001d490: 2870 6174 686c 6962 2e50 6174 6828 746d  (pathlib.Path(tm
+0001d4a0: 705f 736f 7572 6365 2920 2f20 2763 6972  p_source) / 'cir
+0001d4b0: 636c 652d 6c69 6e6b 2729 2e69 735f 7379  cle-link').is_sy
+0001d4c0: 6d6c 696e 6b28 292c 2028 0a20 2020 2020  mlink(), (.     
+0001d4d0: 2020 2020 2020 2027 6369 7263 6c65 2d6c         'circle-l
+0001d4e0: 696e 6b20 7761 7320 6e6f 7420 666f 756e  ink was not foun
+0001d4f0: 6420 696e 2074 6865 2075 706c 6f61 6420  d in the upload 
+0001d500: 736f 7572 6365 202d 2027 0a20 2020 2020  source - '.     
+0001d510: 2020 2020 2020 2027 6172 6520 7468 6520         'are the 
+0001d520: 7465 7374 2066 6978 7475 7265 7320 636f  test fixtures co
+0001d530: 7272 6563 743f 2729 0a20 2020 2020 2020  rrect?').       
+0001d540: 2061 7373 6572 7420 2763 6972 636c 652d   assert 'circle-
+0001d550: 6c69 6e6b 2720 6e6f 7420 696e 206f 7574  link' not in out
+0001d560: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
+0001d570: 2c20 280a 2020 2020 2020 2020 2020 2020  , (.            
+0001d580: 2753 796d 6c69 6e6b 2066 6f75 6e64 2069  'Symlink found i
+0001d590: 6e20 6275 636b 6574 202d 206c 7320 6f75  n bucket - ls ou
+0001d5a0: 7470 7574 2077 6173 203a 207b 7d27 2e66  tput was : {}'.f
+0001d5b0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+0001d5c0: 2020 2020 2020 206f 7574 2e64 6563 6f64         out.decod
+0001d5d0: 6528 2775 7466 2d38 2729 2929 0a0a 2020  e('utf-8')))..  
+0001d5e0: 2020 2020 2020 2320 5275 6e20 736b 7920        # Run sky 
+0001d5f0: 7374 6f72 6167 6520 6c73 2074 6f20 6368  storage ls to ch
+0001d600: 6563 6b20 6966 2073 746f 7261 6765 206f  eck if storage o
+0001d610: 626a 6563 7420 6578 6973 7473 2069 6e20  bject exists in 
+0001d620: 7468 6520 6f75 7470 7574 2e0a 2020 2020  the output..    
+0001d630: 2020 2020 2320 4974 2073 686f 756c 6420      # It should 
+0001d640: 6e6f 7420 6578 6973 7420 6265 6361 7573  not exist becaus
+0001d650: 6520 7468 6520 6275 636b 6574 2077 6173  e the bucket was
+0001d660: 2063 7265 6174 6564 2065 7874 6572 6e61   created externa
+0001d670: 6c6c 792e 0a20 2020 2020 2020 206f 7574  lly..        out
+0001d680: 203d 2073 7562 7072 6f63 6573 732e 6368   = subprocess.ch
+0001d690: 6563 6b5f 6f75 7470 7574 285b 2773 6b79  eck_output(['sky
+0001d6a0: 272c 2027 7374 6f72 6167 6527 2c20 276c  ', 'storage', 'l
+0001d6b0: 7327 5d29 0a20 2020 2020 2020 2061 7373  s']).        ass
+0001d6c0: 6572 7420 7374 6f72 6167 655f 6f62 6a2e  ert storage_obj.
+0001d6d0: 6e61 6d65 206e 6f74 2069 6e20 6f75 742e  name not in out.
+0001d6e0: 6465 636f 6465 2827 7574 662d 3827 290a  decode('utf-8').
+0001d6f0: 0a20 2020 2064 6566 2074 6573 745f 636f  .    def test_co
+0001d700: 7079 5f6d 6f75 6e74 5f65 7869 7374 696e  py_mount_existin
+0001d710: 675f 7374 6f72 6167 6528 7365 6c66 2c0a  g_storage(self,.
+0001d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d740: 2020 2020 2020 2020 2074 6d70 5f63 6f70           tmp_cop
+0001d750: 795f 6d6e 745f 6578 6973 7469 6e67 5f73  y_mnt_existing_s
+0001d760: 746f 7261 6765 5f6f 626a 293a 0a20 2020  torage_obj):.   
+0001d770: 2020 2020 2023 2043 7265 6174 6573 2061       # Creates a
+0001d780: 2062 7563 6b65 7420 7769 7468 206e 6f20   bucket with no 
+0001d790: 736f 7572 6365 2069 6e20 4d4f 554e 5420  source in MOUNT 
+0001d7a0: 6d6f 6465 2028 656d 7074 7920 6275 636b  mode (empty buck
+0001d7b0: 6574 292c 2061 6e64 0a20 2020 2020 2020  et), and.       
+0001d7c0: 2023 2074 6865 6e20 7472 6965 7320 746f   # then tries to
+0001d7d0: 206c 6f61 6420 7468 6520 7361 6d65 2073   load the same s
+0001d7e0: 746f 7261 6765 2069 6e20 434f 5059 206d  torage in COPY m
+0001d7f0: 6f64 652e 0a20 2020 2020 2020 2074 6d70  ode..        tmp
+0001d800: 5f63 6f70 795f 6d6e 745f 6578 6973 7469  _copy_mnt_existi
+0001d810: 6e67 5f73 746f 7261 6765 5f6f 626a 2e61  ng_storage_obj.a
+0001d820: 6464 5f73 746f 7265 2873 746f 7261 6765  dd_store(storage
+0001d830: 5f6c 6962 2e53 746f 7265 5479 7065 2e53  _lib.StoreType.S
+0001d840: 3329 0a20 2020 2020 2020 2073 746f 7261  3).        stora
+0001d850: 6765 5f6e 616d 6520 3d20 746d 705f 636f  ge_name = tmp_co
+0001d860: 7079 5f6d 6e74 5f65 7869 7374 696e 675f  py_mnt_existing_
+0001d870: 7374 6f72 6167 655f 6f62 6a2e 6e61 6d65  storage_obj.name
+0001d880: 0a0a 2020 2020 2020 2020 2320 4368 6563  ..        # Chec
+0001d890: 6b20 6073 6b79 2073 746f 7261 6765 206c  k `sky storage l
+0001d8a0: 7360 2074 6f20 656e 7375 7265 2073 746f  s` to ensure sto
+0001d8b0: 7261 6765 206f 626a 6563 7420 6578 6973  rage object exis
+0001d8c0: 7473 0a20 2020 2020 2020 206f 7574 203d  ts.        out =
+0001d8d0: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
+0001d8e0: 6b5f 6f75 7470 7574 285b 2773 6b79 272c  k_output(['sky',
+0001d8f0: 2027 7374 6f72 6167 6527 2c20 276c 7327   'storage', 'ls'
+0001d900: 5d29 2e64 6563 6f64 6528 2775 7466 2d38  ]).decode('utf-8
+0001d910: 2729 0a20 2020 2020 2020 2061 7373 6572  ').        asser
+0001d920: 7420 7374 6f72 6167 655f 6e61 6d65 2069  t storage_name i
+0001d930: 6e20 6f75 742c 2066 2753 746f 7261 6765  n out, f'Storage
+0001d940: 207b 7374 6f72 6167 655f 6e61 6d65 7d20   {storage_name} 
+0001d950: 6e6f 7420 666f 756e 6420 696e 2073 6b79  not found in sky
+0001d960: 2073 746f 7261 6765 206c 732e 270a 0a20   storage ls.'.. 
+0001d970: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+0001d980: 7061 7261 6d65 7472 697a 6528 2773 746f  parametrize('sto
+0001d990: 7265 5f74 7970 6527 2c20 5b0a 2020 2020  re_type', [.    
+0001d9a0: 2020 2020 7374 6f72 6167 655f 6c69 622e      storage_lib.
+0001d9b0: 5374 6f72 6554 7970 652e 5333 2c20 7374  StoreType.S3, st
+0001d9c0: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
+0001d9d0: 7970 652e 4743 532c 0a20 2020 2020 2020  ype.GCS,.       
+0001d9e0: 2070 7974 6573 742e 7061 7261 6d28 7374   pytest.param(st
+0001d9f0: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
+0001da00: 7970 652e 5232 2c20 6d61 726b 733d 7079  ype.R2, marks=py
+0001da10: 7465 7374 2e6d 6172 6b2e 636c 6f75 6466  test.mark.cloudf
+0001da20: 6c61 7265 290a 2020 2020 5d29 0a20 2020  lare).    ]).   
+0001da30: 2064 6566 2074 6573 745f 6c69 7374 5f73   def test_list_s
+0001da40: 6f75 7263 6528 7365 6c66 2c20 746d 705f  ource(self, tmp_
+0001da50: 6c6f 6361 6c5f 6c69 7374 5f73 746f 7261  local_list_stora
+0001da60: 6765 5f6f 626a 2c20 7374 6f72 655f 7479  ge_obj, store_ty
+0001da70: 7065 293a 0a20 2020 2020 2020 2023 2055  pe):.        # U
+0001da80: 7365 7320 6120 6c69 7374 2069 6e20 7468  ses a list in th
+0001da90: 6520 736f 7572 6365 2066 6965 6c64 2074  e source field t
+0001daa0: 6f20 7370 6563 6966 7920 6120 6669 6c65  o specify a file
+0001dab0: 2061 6e64 2061 2064 6972 6563 746f 7279   and a directory
+0001dac0: 2074 6f0a 2020 2020 2020 2020 2320 6265   to.        # be
+0001dad0: 2075 706c 6f61 6465 6420 746f 2074 6865   uploaded to the
+0001dae0: 2073 746f 7261 6765 206f 626a 6563 742e   storage object.
+0001daf0: 0a20 2020 2020 2020 2074 6d70 5f6c 6f63  .        tmp_loc
+0001db00: 616c 5f6c 6973 745f 7374 6f72 6167 655f  al_list_storage_
+0001db10: 6f62 6a2e 6164 645f 7374 6f72 6528 7374  obj.add_store(st
+0001db20: 6f72 655f 7479 7065 290a 0a20 2020 2020  ore_type)..     
+0001db30: 2020 2023 2043 6865 636b 2069 6620 746d     # Check if tm
+0001db40: 702d 6669 6c65 2065 7869 7374 7320 696e  p-file exists in
+0001db50: 2074 6865 2062 7563 6b65 7420 726f 6f74   the bucket root
+0001db60: 2075 7369 6e67 2063 6c69 0a20 2020 2020   using cli.     
+0001db70: 2020 206f 7574 203d 2073 7562 7072 6f63     out = subproc
+0001db80: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
+0001db90: 2873 656c 662e 636c 695f 6c73 5f63 6d64  (self.cli_ls_cmd
+0001dba0: 280a 2020 2020 2020 2020 2020 2020 7374  (.            st
+0001dbb0: 6f72 655f 7479 7065 2c20 746d 705f 6c6f  ore_type, tmp_lo
+0001dbc0: 6361 6c5f 6c69 7374 5f73 746f 7261 6765  cal_list_storage
+0001dbd0: 5f6f 626a 2e6e 616d 6529 2c0a 2020 2020  _obj.name),.    
+0001dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc00: 2020 7368 656c 6c3d 5472 7565 290a 2020    shell=True).  
+0001dc10: 2020 2020 2020 6173 7365 7274 2027 746d        assert 'tm
+0001dc20: 702d 6669 6c65 2720 696e 206f 7574 2e64  p-file' in out.d
+0001dc30: 6563 6f64 6528 2775 7466 2d38 2729 2c20  ecode('utf-8'), 
+0001dc40: 5c0a 2020 2020 2020 2020 2020 2020 2746  \.            'F
+0001dc50: 696c 6520 6e6f 7420 666f 756e 6420 696e  ile not found in
+0001dc60: 2062 7563 6b65 7420 2d20 6f75 7470 7574   bucket - output
+0001dc70: 2077 6173 203a 207b 7d27 2e66 6f72 6d61   was : {}'.forma
+0001dc80: 7428 6f75 742e 6465 636f 6465 0a20 2020  t(out.decode.   
 0001dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dca0: 2020 2020 2020 2020 2028 2775 7466 2d38           ('utf-8
-0001dcb0: 2729 290a 0a20 2020 2020 2020 2023 2043  '))..        # C
-0001dcc0: 6865 636b 2069 6620 746d 702d 6669 6c65  heck if tmp-file
-0001dcd0: 2065 7869 7374 7320 696e 2074 6865 2062   exists in the b
-0001dce0: 7563 6b65 742f 746d 702d 736f 7572 6365  ucket/tmp-source
-0001dcf0: 2075 7369 6e67 2063 6c69 0a20 2020 2020   using cli.     
-0001dd00: 2020 206f 7574 203d 2073 7562 7072 6f63     out = subproc
-0001dd10: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
-0001dd20: 2873 656c 662e 636c 695f 6c73 5f63 6d64  (self.cli_ls_cmd
-0001dd30: 280a 2020 2020 2020 2020 2020 2020 7374  (.            st
-0001dd40: 6f72 655f 7479 7065 2c20 746d 705f 6c6f  ore_type, tmp_lo
-0001dd50: 6361 6c5f 6c69 7374 5f73 746f 7261 6765  cal_list_storage
-0001dd60: 5f6f 626a 2e6e 616d 652c 2027 746d 702d  _obj.name, 'tmp-
-0001dd70: 736f 7572 6365 2f27 292c 0a20 2020 2020  source/'),.     
-0001dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dda0: 2073 6865 6c6c 3d54 7275 6529 0a20 2020   shell=True).   
-0001ddb0: 2020 2020 2061 7373 6572 7420 2774 6d70       assert 'tmp
-0001ddc0: 2d66 696c 6527 2069 6e20 6f75 742e 6465  -file' in out.de
-0001ddd0: 636f 6465 2827 7574 662d 3827 292c 205c  code('utf-8'), \
-0001dde0: 0a20 2020 2020 2020 2020 2020 2027 4669  .            'Fi
-0001ddf0: 6c65 206e 6f74 2066 6f75 6e64 2069 6e20  le not found in 
-0001de00: 6275 636b 6574 202d 206f 7574 7075 7420  bucket - output 
-0001de10: 7761 7320 3a20 7b7d 272e 666f 726d 6174  was : {}'.format
-0001de20: 286f 7574 2e64 6563 6f64 650a 2020 2020  (out.decode.    
-0001de30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dcc0: 2020 2020 2020 2020 2020 2020 2028 2775               ('u
+0001dcd0: 7466 2d38 2729 290a 0a20 2020 2020 2020  tf-8'))..       
+0001dce0: 2023 2043 6865 636b 2069 6620 746d 702d   # Check if tmp-
+0001dcf0: 6669 6c65 2065 7869 7374 7320 696e 2074  file exists in t
+0001dd00: 6865 2062 7563 6b65 742f 746d 702d 736f  he bucket/tmp-so
+0001dd10: 7572 6365 2075 7369 6e67 2063 6c69 0a20  urce using cli. 
+0001dd20: 2020 2020 2020 206f 7574 203d 2073 7562         out = sub
+0001dd30: 7072 6f63 6573 732e 6368 6563 6b5f 6f75  process.check_ou
+0001dd40: 7470 7574 2873 656c 662e 636c 695f 6c73  tput(self.cli_ls
+0001dd50: 5f63 6d64 280a 2020 2020 2020 2020 2020  _cmd(.          
+0001dd60: 2020 7374 6f72 655f 7479 7065 2c20 746d    store_type, tm
+0001dd70: 705f 6c6f 6361 6c5f 6c69 7374 5f73 746f  p_local_list_sto
+0001dd80: 7261 6765 5f6f 626a 2e6e 616d 652c 2027  rage_obj.name, '
+0001dd90: 746d 702d 736f 7572 6365 2f27 292c 0a20  tmp-source/'),. 
+0001dda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ddc0: 2020 2020 2073 6865 6c6c 3d54 7275 6529       shell=True)
+0001ddd0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0001dde0: 2774 6d70 2d66 696c 6527 2069 6e20 6f75  'tmp-file' in ou
+0001ddf0: 742e 6465 636f 6465 2827 7574 662d 3827  t.decode('utf-8'
+0001de00: 292c 205c 0a20 2020 2020 2020 2020 2020  ), \.           
+0001de10: 2027 4669 6c65 206e 6f74 2066 6f75 6e64   'File not found
+0001de20: 2069 6e20 6275 636b 6574 202d 206f 7574   in bucket - out
+0001de30: 7075 7420 7761 7320 3a20 7b7d 272e 666f  put was : {}'.fo
+0001de40: 726d 6174 286f 7574 2e64 6563 6f64 650a  rmat(out.decode.
 0001de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de60: 2020 2020 2020 2020 2020 2020 2827 7574              ('ut
-0001de70: 662d 3827 2929 0a0a 2020 2020 4070 7974  f-8'))..    @pyt
-0001de80: 6573 742e 6d61 726b 2e70 6172 616d 6574  est.mark.paramet
-0001de90: 7269 7a65 2827 696e 7661 6c69 645f 6e61  rize('invalid_na
-0001dea0: 6d65 5f6c 6973 742c 2073 746f 7265 5f74  me_list, store_t
-0001deb0: 7970 6527 2c0a 2020 2020 2020 2020 2020  ype',.          
-0001dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ded0: 2020 205b 2841 5753 5f49 4e56 414c 4944     [(AWS_INVALID
-0001dee0: 5f4e 414d 4553 2c20 7374 6f72 6167 655f  _NAMES, storage_
-0001def0: 6c69 622e 5374 6f72 6554 7970 652e 5333  lib.StoreType.S3
-0001df00: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0001df10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001df20: 2028 4743 535f 494e 5641 4c49 445f 4e41   (GCS_INVALID_NA
-0001df30: 4d45 532c 2073 746f 7261 6765 5f6c 6962  MES, storage_lib
-0001df40: 2e53 746f 7265 5479 7065 2e47 4353 292c  .StoreType.GCS),
-0001df50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001df60: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001df70: 7974 6573 742e 7061 7261 6d28 4157 535f  ytest.param(AWS_
-0001df80: 494e 5641 4c49 445f 4e41 4d45 532c 0a20  INVALID_NAMES,. 
-0001df90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dfb0: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
-0001dfc0: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
-0001dfd0: 5232 2c0a 2020 2020 2020 2020 2020 2020  R2,.            
-0001dfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dff0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0001e000: 6172 6b73 3d70 7974 6573 742e 6d61 726b  arks=pytest.mark
-0001e010: 2e63 6c6f 7564 666c 6172 6529 5d29 0a20  .cloudflare)]). 
-0001e020: 2020 2064 6566 2074 6573 745f 696e 7661     def test_inva
-0001e030: 6c69 645f 6e61 6d65 7328 7365 6c66 2c20  lid_names(self, 
-0001e040: 696e 7661 6c69 645f 6e61 6d65 5f6c 6973  invalid_name_lis
-0001e050: 742c 2073 746f 7265 5f74 7970 6529 3a0a  t, store_type):.
-0001e060: 2020 2020 2020 2020 2320 5573 6573 2061          # Uses a
-0001e070: 206c 6973 7420 696e 2074 6865 2073 6f75   list in the sou
-0001e080: 7263 6520 6669 656c 6420 746f 2073 7065  rce field to spe
-0001e090: 6369 6679 2061 2066 696c 6520 616e 6420  cify a file and 
-0001e0a0: 6120 6469 7265 6374 6f72 7920 746f 0a20  a directory to. 
-0001e0b0: 2020 2020 2020 2023 2062 6520 7570 6c6f         # be uplo
-0001e0c0: 6164 6564 2074 6f20 7468 6520 7374 6f72  aded to the stor
-0001e0d0: 6167 6520 6f62 6a65 6374 2e0a 2020 2020  age object..    
-0001e0e0: 2020 2020 666f 7220 6e61 6d65 2069 6e20      for name in 
-0001e0f0: 696e 7661 6c69 645f 6e61 6d65 5f6c 6973  invalid_name_lis
-0001e100: 743a 0a20 2020 2020 2020 2020 2020 2077  t:.            w
-0001e110: 6974 6820 7079 7465 7374 2e72 6169 7365  ith pytest.raise
-0001e120: 7328 736b 792e 6578 6365 7074 696f 6e73  s(sky.exceptions
-0001e130: 2e53 746f 7261 6765 4e61 6d65 4572 726f  .StorageNameErro
-0001e140: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-0001e150: 2020 2020 7374 6f72 6167 655f 6f62 6a20      storage_obj 
-0001e160: 3d20 7374 6f72 6167 655f 6c69 622e 5374  = storage_lib.St
-0001e170: 6f72 6167 6528 6e61 6d65 3d6e 616d 6529  orage(name=name)
-0001e180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e190: 2073 746f 7261 6765 5f6f 626a 2e61 6464   storage_obj.add
-0001e1a0: 5f73 746f 7265 2873 746f 7265 5f74 7970  _store(store_typ
-0001e1b0: 6529 0a0a 0a23 202d 2d2d 2d2d 2d2d 2d2d  e)...# ---------
-0001e1c0: 2d20 5465 7374 696e 6720 5941 4d4c 2053  - Testing YAML S
-0001e1d0: 7065 6373 202d 2d2d 2d2d 2d2d 2d2d 2d0a  pecs ----------.
-0001e1e0: 2320 4f75 7220 736b 7920 7374 6f72 6167  # Our sky storag
-0001e1f0: 6520 7265 7175 6972 6573 2063 7265 6465  e requires crede
-0001e200: 6e74 6961 6c73 2074 6f20 6368 6563 6b20  ntials to check 
-0001e210: 7468 6520 6275 636b 6574 2065 7869 7374  the bucket exist
-0001e220: 616e 6365 2077 6865 6e0a 2320 6c6f 6164  ance when.# load
-0001e230: 696e 6720 6120 7461 736b 2066 726f 6d20  ing a task from 
-0001e240: 7468 6520 7961 6d6c 2066 696c 652c 2073  the yaml file, s
-0001e250: 6f20 7765 2063 616e 6e6f 7420 6d61 6b65  o we cannot make
-0001e260: 2069 7420 6120 756e 6974 2074 6573 742e   it a unit test.
-0001e270: 0a63 6c61 7373 2054 6573 7459 616d 6c53  .class TestYamlS
-0001e280: 7065 6373 3a0a 2020 2020 2320 544f 444f  pecs:.    # TODO
-0001e290: 287a 6877 7529 3a20 4164 6420 7465 7374  (zhwu): Add test
-0001e2a0: 2066 6f72 2060 746f 5f79 616d 6c5f 636f   for `to_yaml_co
-0001e2b0: 6e66 6967 6020 666f 7220 7468 6520 5374  nfig` for the St
-0001e2c0: 6f72 6167 6520 6f62 6a65 6374 2e0a 2020  orage object..  
-0001e2d0: 2020 2320 2057 6520 7368 6f75 6c64 206e    #  We should n
-0001e2e0: 6f74 2075 7365 2060 6578 616d 706c 6573  ot use `examples
-0001e2f0: 2f73 746f 7261 6765 5f64 656d 6f2e 7961  /storage_demo.ya
-0001e300: 6d6c 6020 6865 7265 2c20 7369 6e63 6520  ml` here, since 
-0001e310: 6974 2072 6571 7569 7265 730a 2020 2020  it requires.    
-0001e320: 2320 2075 7365 7273 2074 6f20 656e 7375  #  users to ensu
-0001e330: 7265 2062 7563 6b65 7420 6e61 6d65 7320  re bucket names 
-0001e340: 746f 206e 6f74 2065 7869 7374 2061 6e64  to not exist and
-0001e350: 2f6f 7220 6265 2075 6e69 7175 652e 0a20  /or be unique.. 
-0001e360: 2020 205f 5445 5354 5f59 414d 4c5f 5041     _TEST_YAML_PA
-0001e370: 5448 5320 3d20 5b0a 2020 2020 2020 2020  THS = [.        
-0001e380: 2765 7861 6d70 6c65 732f 6d69 6e69 6d61  'examples/minima
-0001e390: 6c2e 7961 6d6c 272c 2027 6578 616d 706c  l.yaml', 'exampl
-0001e3a0: 6573 2f6d 616e 6167 6564 5f73 706f 742e  es/managed_spot.
-0001e3b0: 7961 6d6c 272c 0a20 2020 2020 2020 2027  yaml',.        '
-0001e3c0: 6578 616d 706c 6573 2f75 7369 6e67 5f66  examples/using_f
-0001e3d0: 696c 655f 6d6f 756e 7473 2e79 616d 6c27  ile_mounts.yaml'
-0001e3e0: 2c20 2765 7861 6d70 6c65 732f 7265 736e  , 'examples/resn
-0001e3f0: 6574 5f61 7070 2e79 616d 6c27 2c0a 2020  et_app.yaml',.  
-0001e400: 2020 2020 2020 2765 7861 6d70 6c65 732f        'examples/
-0001e410: 6d75 6c74 695f 686f 7374 6e61 6d65 2e79  multi_hostname.y
-0001e420: 616d 6c27 0a20 2020 205d 0a0a 2020 2020  aml'.    ]..    
-0001e430: 6465 6620 5f69 735f 6469 6374 5f73 7562  def _is_dict_sub
-0001e440: 7365 7428 7365 6c66 2c20 6431 2c20 6432  set(self, d1, d2
-0001e450: 293a 0a20 2020 2020 2020 2022 2222 4368  ):.        """Ch
-0001e460: 6563 6b20 6966 2064 3120 6973 2074 6865  eck if d1 is the
-0001e470: 2073 7562 7365 7420 6f66 2064 322e 2222   subset of d2.""
-0001e480: 220a 2020 2020 2020 2020 666f 7220 6b2c  ".        for k,
-0001e490: 2076 2069 6e20 6431 2e69 7465 6d73 2829   v in d1.items()
-0001e4a0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0001e4b0: 206b 206e 6f74 2069 6e20 6432 3a0a 2020   k not in d2:.  
-0001e4c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001e4d0: 2069 7369 6e73 7461 6e63 6528 762c 206c   isinstance(v, l
-0001e4e0: 6973 7429 206f 7220 6973 696e 7374 616e  ist) or isinstan
-0001e4f0: 6365 2876 2c20 6469 6374 293a 0a20 2020  ce(v, dict):.   
-0001e500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e510: 2061 7373 6572 7420 6c65 6e28 7629 203d   assert len(v) =
-0001e520: 3d20 302c 2028 6b2c 2076 290a 2020 2020  = 0, (k, v).    
-0001e530: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001e540: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001e550: 2020 2020 2020 6173 7365 7274 2046 616c        assert Fal
-0001e560: 7365 2c20 286b 2c20 7629 0a20 2020 2020  se, (k, v).     
-0001e570: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-0001e580: 7374 616e 6365 2876 2c20 6469 6374 293a  stance(v, dict):
-0001e590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e5a0: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
-0001e5b0: 6365 2864 325b 6b5d 2c20 6469 6374 292c  ce(d2[k], dict),
-0001e5c0: 2028 6b2c 2076 2c20 6432 290a 2020 2020   (k, v, d2).    
-0001e5d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001e5e0: 2e5f 6973 5f64 6963 745f 7375 6273 6574  ._is_dict_subset
-0001e5f0: 2876 2c20 6432 5b6b 5d29 0a20 2020 2020  (v, d2[k]).     
-0001e600: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-0001e610: 7374 616e 6365 2876 2c20 7374 7229 3a0a  stance(v, str):.
-0001e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e630: 6966 206b 203d 3d20 2761 6363 656c 6572  if k == 'acceler
-0001e640: 6174 6f72 7327 3a0a 2020 2020 2020 2020  ators':.        
-0001e650: 2020 2020 2020 2020 2020 2020 7265 736f              reso
-0001e660: 7572 6365 7320 3d20 736b 792e 5265 736f  urces = sky.Reso
-0001e670: 7572 6365 7328 290a 2020 2020 2020 2020  urces().        
-0001e680: 2020 2020 2020 2020 2020 2020 7265 736f              reso
-0001e690: 7572 6365 732e 5f73 6574 5f61 6363 656c  urces._set_accel
-0001e6a0: 6572 6174 6f72 7328 762c 204e 6f6e 6529  erators(v, None)
-0001e6b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e6c0: 2020 2020 2061 7373 6572 7420 7265 736f       assert reso
-0001e6d0: 7572 6365 732e 6163 6365 6c65 7261 746f  urces.accelerato
-0001e6e0: 7273 203d 3d20 6432 5b6b 5d2c 2028 6b2c  rs == d2[k], (k,
-0001e6f0: 2076 2c20 6432 290a 2020 2020 2020 2020   v, d2).        
-0001e700: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001e710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e720: 2020 6173 7365 7274 2076 2e6c 6f77 6572    assert v.lower
-0001e730: 2829 203d 3d20 6432 5b6b 5d2e 6c6f 7765  () == d2[k].lowe
-0001e740: 7228 292c 2028 6b2c 2076 2c20 6432 5b6b  r(), (k, v, d2[k
-0001e750: 5d29 0a20 2020 2020 2020 2020 2020 2065  ]).            e
-0001e760: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0001e770: 2020 2020 2061 7373 6572 7420 7620 3d3d       assert v ==
-0001e780: 2064 325b 6b5d 2c20 286b 2c20 762c 2064   d2[k], (k, v, d
-0001e790: 325b 6b5d 290a 0a20 2020 2064 6566 205f  2[k])..    def _
-0001e7a0: 6368 6563 6b5f 6571 7569 7661 6c65 6e74  check_equivalent
-0001e7b0: 2873 656c 662c 2079 616d 6c5f 7061 7468  (self, yaml_path
-0001e7c0: 293a 0a20 2020 2020 2020 2022 2222 4368  ):.        """Ch
-0001e7d0: 6563 6b20 6966 2074 6865 2079 616d 6c20  eck if the yaml 
-0001e7e0: 6973 2065 7175 6976 616c 656e 7420 6166  is equivalent af
-0001e7f0: 7465 7220 6c6f 6164 2061 6e64 2064 756d  ter load and dum
-0001e800: 7020 6167 6169 6e2e 2222 220a 2020 2020  p again.""".    
-0001e810: 2020 2020 6f72 6967 696e 5f74 6173 6b5f      origin_task_
-0001e820: 636f 6e66 6967 203d 2063 6f6d 6d6f 6e5f  config = common_
-0001e830: 7574 696c 732e 7265 6164 5f79 616d 6c28  utils.read_yaml(
-0001e840: 7961 6d6c 5f70 6174 6829 0a0a 2020 2020  yaml_path)..    
-0001e850: 2020 2020 7461 736b 203d 2073 6b79 2e54      task = sky.T
-0001e860: 6173 6b2e 6672 6f6d 5f79 616d 6c28 7961  ask.from_yaml(ya
-0001e870: 6d6c 5f70 6174 6829 0a20 2020 2020 2020  ml_path).       
-0001e880: 206e 6577 5f74 6173 6b5f 636f 6e66 6967   new_task_config
-0001e890: 203d 2074 6173 6b2e 746f 5f79 616d 6c5f   = task.to_yaml_
-0001e8a0: 636f 6e66 6967 2829 0a20 2020 2020 2020  config().       
-0001e8b0: 2023 2064 3120 3c3d 2064 320a 2020 2020   # d1 <= d2.    
-0001e8c0: 2020 2020 7365 6c66 2e5f 6973 5f64 6963      self._is_dic
-0001e8d0: 745f 7375 6273 6574 286f 7269 6769 6e5f  t_subset(origin_
-0001e8e0: 7461 736b 5f63 6f6e 6669 672c 206e 6577  task_config, new
-0001e8f0: 5f74 6173 6b5f 636f 6e66 6967 290a 0a20  _task_config).. 
-0001e900: 2020 2064 6566 2074 6573 745f 6c6f 6164     def test_load
-0001e910: 5f64 756d 705f 7961 6d6c 5f63 6f6e 6669  _dump_yaml_confi
-0001e920: 675f 6571 7569 7661 6c65 6e74 2873 656c  g_equivalent(sel
-0001e930: 6629 3a0a 2020 2020 2020 2020 2222 2254  f):.        """T
-0001e940: 6573 7420 6966 2074 6865 2079 616d 6c20  est if the yaml 
-0001e950: 636f 6e66 6967 2069 7320 6571 7569 7661  config is equiva
-0001e960: 6c65 6e74 2061 6674 6572 206c 6f61 6420  lent after load 
-0001e970: 616e 6420 6475 6d70 2061 6761 696e 2e22  and dump again."
-0001e980: 2222 0a20 2020 2020 2020 2070 6174 686c  "".        pathl
-0001e990: 6962 2e50 6174 6828 277e 2f64 6174 6173  ib.Path('~/datas
-0001e9a0: 6574 7327 292e 6578 7061 6e64 7573 6572  ets').expanduser
-0001e9b0: 2829 2e6d 6b64 6972 2865 7869 7374 5f6f  ().mkdir(exist_o
-0001e9c0: 6b3d 5472 7565 290a 2020 2020 2020 2020  k=True).        
-0001e9d0: 7061 7468 6c69 622e 5061 7468 2827 7e2f  pathlib.Path('~/
-0001e9e0: 746d 7066 696c 6527 292e 6578 7061 6e64  tmpfile').expand
-0001e9f0: 7573 6572 2829 2e74 6f75 6368 2829 0a20  user().touch(). 
-0001ea00: 2020 2020 2020 2070 6174 686c 6962 2e50         pathlib.P
-0001ea10: 6174 6828 277e 2f2e 7373 6827 292e 6578  ath('~/.ssh').ex
-0001ea20: 7061 6e64 7573 6572 2829 2e6d 6b64 6972  panduser().mkdir
-0001ea30: 2865 7869 7374 5f6f 6b3d 5472 7565 290a  (exist_ok=True).
-0001ea40: 2020 2020 2020 2020 7061 7468 6c69 622e          pathlib.
-0001ea50: 5061 7468 2827 7e2f 2e73 7368 2f69 645f  Path('~/.ssh/id_
-0001ea60: 7273 612e 7075 6227 292e 6578 7061 6e64  rsa.pub').expand
-0001ea70: 7573 6572 2829 2e74 6f75 6368 2829 0a20  user().touch(). 
-0001ea80: 2020 2020 2020 2070 6174 686c 6962 2e50         pathlib.P
-0001ea90: 6174 6828 277e 2f74 6d70 2d77 6f72 6b64  ath('~/tmp-workd
-0001eaa0: 6972 2729 2e65 7870 616e 6475 7365 7228  ir').expanduser(
-0001eab0: 292e 6d6b 6469 7228 6578 6973 745f 6f6b  ).mkdir(exist_ok
-0001eac0: 3d54 7275 6529 0a20 2020 2020 2020 2070  =True).        p
-0001ead0: 6174 686c 6962 2e50 6174 6828 277e 2f44  athlib.Path('~/D
-0001eae0: 6f77 6e6c 6f61 6473 2f74 7075 2729 2e65  ownloads/tpu').e
-0001eaf0: 7870 616e 6475 7365 7228 292e 6d6b 6469  xpanduser().mkdi
-0001eb00: 7228 7061 7265 6e74 733d 5472 7565 2c0a  r(parents=True,.
-0001eb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb40: 2020 2020 2020 2020 2020 2065 7869 7374             exist
-0001eb50: 5f6f 6b3d 5472 7565 290a 2020 2020 2020  _ok=True).      
-0001eb60: 2020 666f 7220 7961 6d6c 5f70 6174 6820    for yaml_path 
-0001eb70: 696e 2073 656c 662e 5f54 4553 545f 5941  in self._TEST_YA
-0001eb80: 4d4c 5f50 4154 4853 3a0a 2020 2020 2020  ML_PATHS:.      
-0001eb90: 2020 2020 2020 7365 6c66 2e5f 6368 6563        self._chec
-0001eba0: 6b5f 6571 7569 7661 6c65 6e74 2879 616d  k_equivalent(yam
-0001ebb0: 6c5f 7061 7468 290a                      l_path).
+0001de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de90: 2827 7574 662d 3827 2929 0a0a 2020 2020  ('utf-8'))..    
+0001dea0: 4070 7974 6573 742e 6d61 726b 2e70 6172  @pytest.mark.par
+0001deb0: 616d 6574 7269 7a65 2827 696e 7661 6c69  ametrize('invali
+0001dec0: 645f 6e61 6d65 5f6c 6973 742c 2073 746f  d_name_list, sto
+0001ded0: 7265 5f74 7970 6527 2c0a 2020 2020 2020  re_type',.      
+0001dee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001def0: 2020 2020 2020 205b 2841 5753 5f49 4e56         [(AWS_INV
+0001df00: 414c 4944 5f4e 414d 4553 2c20 7374 6f72  ALID_NAMES, stor
+0001df10: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
+0001df20: 652e 5333 292c 0a20 2020 2020 2020 2020  e.S3),.         
+0001df30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001df40: 2020 2020 2028 4743 535f 494e 5641 4c49       (GCS_INVALI
+0001df50: 445f 4e41 4d45 532c 2073 746f 7261 6765  D_NAMES, storage
+0001df60: 5f6c 6962 2e53 746f 7265 5479 7065 2e47  _lib.StoreType.G
+0001df70: 4353 292c 0a20 2020 2020 2020 2020 2020  CS),.           
+0001df80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001df90: 2020 2070 7974 6573 742e 7061 7261 6d28     pytest.param(
+0001dfa0: 4157 535f 494e 5641 4c49 445f 4e41 4d45  AWS_INVALID_NAME
+0001dfb0: 532c 0a20 2020 2020 2020 2020 2020 2020  S,.             
+0001dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dfd0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0001dfe0: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
+0001dff0: 7970 652e 5232 2c0a 2020 2020 2020 2020  ype.R2,.        
+0001e000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e020: 2020 206d 6172 6b73 3d70 7974 6573 742e     marks=pytest.
+0001e030: 6d61 726b 2e63 6c6f 7564 666c 6172 6529  mark.cloudflare)
+0001e040: 5d29 0a20 2020 2064 6566 2074 6573 745f  ]).    def test_
+0001e050: 696e 7661 6c69 645f 6e61 6d65 7328 7365  invalid_names(se
+0001e060: 6c66 2c20 696e 7661 6c69 645f 6e61 6d65  lf, invalid_name
+0001e070: 5f6c 6973 742c 2073 746f 7265 5f74 7970  _list, store_typ
+0001e080: 6529 3a0a 2020 2020 2020 2020 2320 5573  e):.        # Us
+0001e090: 6573 2061 206c 6973 7420 696e 2074 6865  es a list in the
+0001e0a0: 2073 6f75 7263 6520 6669 656c 6420 746f   source field to
+0001e0b0: 2073 7065 6369 6679 2061 2066 696c 6520   specify a file 
+0001e0c0: 616e 6420 6120 6469 7265 6374 6f72 7920  and a directory 
+0001e0d0: 746f 0a20 2020 2020 2020 2023 2062 6520  to.        # be 
+0001e0e0: 7570 6c6f 6164 6564 2074 6f20 7468 6520  uploaded to the 
+0001e0f0: 7374 6f72 6167 6520 6f62 6a65 6374 2e0a  storage object..
+0001e100: 2020 2020 2020 2020 666f 7220 6e61 6d65          for name
+0001e110: 2069 6e20 696e 7661 6c69 645f 6e61 6d65   in invalid_name
+0001e120: 5f6c 6973 743a 0a20 2020 2020 2020 2020  _list:.         
+0001e130: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
+0001e140: 6169 7365 7328 736b 792e 6578 6365 7074  aises(sky.except
+0001e150: 696f 6e73 2e53 746f 7261 6765 4e61 6d65  ions.StorageName
+0001e160: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+0001e170: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
+0001e180: 6f62 6a20 3d20 7374 6f72 6167 655f 6c69  obj = storage_li
+0001e190: 622e 5374 6f72 6167 6528 6e61 6d65 3d6e  b.Storage(name=n
+0001e1a0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
+0001e1b0: 2020 2020 2073 746f 7261 6765 5f6f 626a       storage_obj
+0001e1c0: 2e61 6464 5f73 746f 7265 2873 746f 7265  .add_store(store
+0001e1d0: 5f74 7970 6529 0a0a 0a23 202d 2d2d 2d2d  _type)...# -----
+0001e1e0: 2d2d 2d2d 2d20 5465 7374 696e 6720 5941  ----- Testing YA
+0001e1f0: 4d4c 2053 7065 6373 202d 2d2d 2d2d 2d2d  ML Specs -------
+0001e200: 2d2d 2d0a 2320 4f75 7220 736b 7920 7374  ---.# Our sky st
+0001e210: 6f72 6167 6520 7265 7175 6972 6573 2063  orage requires c
+0001e220: 7265 6465 6e74 6961 6c73 2074 6f20 6368  redentials to ch
+0001e230: 6563 6b20 7468 6520 6275 636b 6574 2065  eck the bucket e
+0001e240: 7869 7374 616e 6365 2077 6865 6e0a 2320  xistance when.# 
+0001e250: 6c6f 6164 696e 6720 6120 7461 736b 2066  loading a task f
+0001e260: 726f 6d20 7468 6520 7961 6d6c 2066 696c  rom the yaml fil
+0001e270: 652c 2073 6f20 7765 2063 616e 6e6f 7420  e, so we cannot 
+0001e280: 6d61 6b65 2069 7420 6120 756e 6974 2074  make it a unit t
+0001e290: 6573 742e 0a63 6c61 7373 2054 6573 7459  est..class TestY
+0001e2a0: 616d 6c53 7065 6373 3a0a 2020 2020 2320  amlSpecs:.    # 
+0001e2b0: 544f 444f 287a 6877 7529 3a20 4164 6420  TODO(zhwu): Add 
+0001e2c0: 7465 7374 2066 6f72 2060 746f 5f79 616d  test for `to_yam
+0001e2d0: 6c5f 636f 6e66 6967 6020 666f 7220 7468  l_config` for th
+0001e2e0: 6520 5374 6f72 6167 6520 6f62 6a65 6374  e Storage object
+0001e2f0: 2e0a 2020 2020 2320 2057 6520 7368 6f75  ..    #  We shou
+0001e300: 6c64 206e 6f74 2075 7365 2060 6578 616d  ld not use `exam
+0001e310: 706c 6573 2f73 746f 7261 6765 5f64 656d  ples/storage_dem
+0001e320: 6f2e 7961 6d6c 6020 6865 7265 2c20 7369  o.yaml` here, si
+0001e330: 6e63 6520 6974 2072 6571 7569 7265 730a  nce it requires.
+0001e340: 2020 2020 2320 2075 7365 7273 2074 6f20      #  users to 
+0001e350: 656e 7375 7265 2062 7563 6b65 7420 6e61  ensure bucket na
+0001e360: 6d65 7320 746f 206e 6f74 2065 7869 7374  mes to not exist
+0001e370: 2061 6e64 2f6f 7220 6265 2075 6e69 7175   and/or be uniqu
+0001e380: 652e 0a20 2020 205f 5445 5354 5f59 414d  e..    _TEST_YAM
+0001e390: 4c5f 5041 5448 5320 3d20 5b0a 2020 2020  L_PATHS = [.    
+0001e3a0: 2020 2020 2765 7861 6d70 6c65 732f 6d69      'examples/mi
+0001e3b0: 6e69 6d61 6c2e 7961 6d6c 272c 2027 6578  nimal.yaml', 'ex
+0001e3c0: 616d 706c 6573 2f6d 616e 6167 6564 5f73  amples/managed_s
+0001e3d0: 706f 742e 7961 6d6c 272c 0a20 2020 2020  pot.yaml',.     
+0001e3e0: 2020 2027 6578 616d 706c 6573 2f75 7369     'examples/usi
+0001e3f0: 6e67 5f66 696c 655f 6d6f 756e 7473 2e79  ng_file_mounts.y
+0001e400: 616d 6c27 2c20 2765 7861 6d70 6c65 732f  aml', 'examples/
+0001e410: 7265 736e 6574 5f61 7070 2e79 616d 6c27  resnet_app.yaml'
+0001e420: 2c0a 2020 2020 2020 2020 2765 7861 6d70  ,.        'examp
+0001e430: 6c65 732f 6d75 6c74 695f 686f 7374 6e61  les/multi_hostna
+0001e440: 6d65 2e79 616d 6c27 0a20 2020 205d 0a0a  me.yaml'.    ]..
+0001e450: 2020 2020 6465 6620 5f69 735f 6469 6374      def _is_dict
+0001e460: 5f73 7562 7365 7428 7365 6c66 2c20 6431  _subset(self, d1
+0001e470: 2c20 6432 293a 0a20 2020 2020 2020 2022  , d2):.        "
+0001e480: 2222 4368 6563 6b20 6966 2064 3120 6973  ""Check if d1 is
+0001e490: 2074 6865 2073 7562 7365 7420 6f66 2064   the subset of d
+0001e4a0: 322e 2222 220a 2020 2020 2020 2020 666f  2.""".        fo
+0001e4b0: 7220 6b2c 2076 2069 6e20 6431 2e69 7465  r k, v in d1.ite
+0001e4c0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+0001e4d0: 2020 6966 206b 206e 6f74 2069 6e20 6432    if k not in d2
+0001e4e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001e4f0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0001e500: 762c 206c 6973 7429 206f 7220 6973 696e  v, list) or isin
+0001e510: 7374 616e 6365 2876 2c20 6469 6374 293a  stance(v, dict):
+0001e520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e530: 2020 2020 2061 7373 6572 7420 6c65 6e28       assert len(
+0001e540: 7629 203d 3d20 302c 2028 6b2c 2076 290a  v) == 0, (k, v).
+0001e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e560: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001e570: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+0001e580: 2046 616c 7365 2c20 286b 2c20 7629 0a20   False, (k, v). 
+0001e590: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0001e5a0: 6973 696e 7374 616e 6365 2876 2c20 6469  isinstance(v, di
+0001e5b0: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
+0001e5c0: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
+0001e5d0: 7374 616e 6365 2864 325b 6b5d 2c20 6469  stance(d2[k], di
+0001e5e0: 6374 292c 2028 6b2c 2076 2c20 6432 290a  ct), (k, v, d2).
+0001e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e600: 7365 6c66 2e5f 6973 5f64 6963 745f 7375  self._is_dict_su
+0001e610: 6273 6574 2876 2c20 6432 5b6b 5d29 0a20  bset(v, d2[k]). 
+0001e620: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0001e630: 6973 696e 7374 616e 6365 2876 2c20 7374  isinstance(v, st
+0001e640: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0001e650: 2020 2020 6966 206b 203d 3d20 2761 6363      if k == 'acc
+0001e660: 656c 6572 6174 6f72 7327 3a0a 2020 2020  elerators':.    
+0001e670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e680: 7265 736f 7572 6365 7320 3d20 736b 792e  resources = sky.
+0001e690: 5265 736f 7572 6365 7328 290a 2020 2020  Resources().    
+0001e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e6b0: 7265 736f 7572 6365 732e 5f73 6574 5f61  resources._set_a
+0001e6c0: 6363 656c 6572 6174 6f72 7328 762c 204e  ccelerators(v, N
+0001e6d0: 6f6e 6529 0a20 2020 2020 2020 2020 2020  one).           
+0001e6e0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0001e6f0: 7265 736f 7572 6365 732e 6163 6365 6c65  resources.accele
+0001e700: 7261 746f 7273 203d 3d20 6432 5b6b 5d2c  rators == d2[k],
+0001e710: 2028 6b2c 2076 2c20 6432 290a 2020 2020   (k, v, d2).    
+0001e720: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0001e730: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001e740: 2020 2020 2020 6173 7365 7274 2076 2e6c        assert v.l
+0001e750: 6f77 6572 2829 203d 3d20 6432 5b6b 5d2e  ower() == d2[k].
+0001e760: 6c6f 7765 7228 292c 2028 6b2c 2076 2c20  lower(), (k, v, 
+0001e770: 6432 5b6b 5d29 0a20 2020 2020 2020 2020  d2[k]).         
+0001e780: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001e790: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0001e7a0: 7620 3d3d 2064 325b 6b5d 2c20 286b 2c20  v == d2[k], (k, 
+0001e7b0: 762c 2064 325b 6b5d 290a 0a20 2020 2064  v, d2[k])..    d
+0001e7c0: 6566 205f 6368 6563 6b5f 6571 7569 7661  ef _check_equiva
+0001e7d0: 6c65 6e74 2873 656c 662c 2079 616d 6c5f  lent(self, yaml_
+0001e7e0: 7061 7468 293a 0a20 2020 2020 2020 2022  path):.        "
+0001e7f0: 2222 4368 6563 6b20 6966 2074 6865 2079  ""Check if the y
+0001e800: 616d 6c20 6973 2065 7175 6976 616c 656e  aml is equivalen
+0001e810: 7420 6166 7465 7220 6c6f 6164 2061 6e64  t after load and
+0001e820: 2064 756d 7020 6167 6169 6e2e 2222 220a   dump again.""".
+0001e830: 2020 2020 2020 2020 6f72 6967 696e 5f74          origin_t
+0001e840: 6173 6b5f 636f 6e66 6967 203d 2063 6f6d  ask_config = com
+0001e850: 6d6f 6e5f 7574 696c 732e 7265 6164 5f79  mon_utils.read_y
+0001e860: 616d 6c28 7961 6d6c 5f70 6174 6829 0a0a  aml(yaml_path)..
+0001e870: 2020 2020 2020 2020 7461 736b 203d 2073          task = s
+0001e880: 6b79 2e54 6173 6b2e 6672 6f6d 5f79 616d  ky.Task.from_yam
+0001e890: 6c28 7961 6d6c 5f70 6174 6829 0a20 2020  l(yaml_path).   
+0001e8a0: 2020 2020 206e 6577 5f74 6173 6b5f 636f       new_task_co
+0001e8b0: 6e66 6967 203d 2074 6173 6b2e 746f 5f79  nfig = task.to_y
+0001e8c0: 616d 6c5f 636f 6e66 6967 2829 0a20 2020  aml_config().   
+0001e8d0: 2020 2020 2023 2064 3120 3c3d 2064 320a       # d1 <= d2.
+0001e8e0: 2020 2020 2020 2020 7365 6c66 2e5f 6973          self._is
+0001e8f0: 5f64 6963 745f 7375 6273 6574 286f 7269  _dict_subset(ori
+0001e900: 6769 6e5f 7461 736b 5f63 6f6e 6669 672c  gin_task_config,
+0001e910: 206e 6577 5f74 6173 6b5f 636f 6e66 6967   new_task_config
+0001e920: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0001e930: 6c6f 6164 5f64 756d 705f 7961 6d6c 5f63  load_dump_yaml_c
+0001e940: 6f6e 6669 675f 6571 7569 7661 6c65 6e74  onfig_equivalent
+0001e950: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001e960: 2222 2254 6573 7420 6966 2074 6865 2079  """Test if the y
+0001e970: 616d 6c20 636f 6e66 6967 2069 7320 6571  aml config is eq
+0001e980: 7569 7661 6c65 6e74 2061 6674 6572 206c  uivalent after l
+0001e990: 6f61 6420 616e 6420 6475 6d70 2061 6761  oad and dump aga
+0001e9a0: 696e 2e22 2222 0a20 2020 2020 2020 2070  in.""".        p
+0001e9b0: 6174 686c 6962 2e50 6174 6828 277e 2f64  athlib.Path('~/d
+0001e9c0: 6174 6173 6574 7327 292e 6578 7061 6e64  atasets').expand
+0001e9d0: 7573 6572 2829 2e6d 6b64 6972 2865 7869  user().mkdir(exi
+0001e9e0: 7374 5f6f 6b3d 5472 7565 290a 2020 2020  st_ok=True).    
+0001e9f0: 2020 2020 7061 7468 6c69 622e 5061 7468      pathlib.Path
+0001ea00: 2827 7e2f 746d 7066 696c 6527 292e 6578  ('~/tmpfile').ex
+0001ea10: 7061 6e64 7573 6572 2829 2e74 6f75 6368  panduser().touch
+0001ea20: 2829 0a20 2020 2020 2020 2070 6174 686c  ().        pathl
+0001ea30: 6962 2e50 6174 6828 277e 2f2e 7373 6827  ib.Path('~/.ssh'
+0001ea40: 292e 6578 7061 6e64 7573 6572 2829 2e6d  ).expanduser().m
+0001ea50: 6b64 6972 2865 7869 7374 5f6f 6b3d 5472  kdir(exist_ok=Tr
+0001ea60: 7565 290a 2020 2020 2020 2020 7061 7468  ue).        path
+0001ea70: 6c69 622e 5061 7468 2827 7e2f 2e73 7368  lib.Path('~/.ssh
+0001ea80: 2f69 645f 7273 612e 7075 6227 292e 6578  /id_rsa.pub').ex
+0001ea90: 7061 6e64 7573 6572 2829 2e74 6f75 6368  panduser().touch
+0001eaa0: 2829 0a20 2020 2020 2020 2070 6174 686c  ().        pathl
+0001eab0: 6962 2e50 6174 6828 277e 2f74 6d70 2d77  ib.Path('~/tmp-w
+0001eac0: 6f72 6b64 6972 2729 2e65 7870 616e 6475  orkdir').expandu
+0001ead0: 7365 7228 292e 6d6b 6469 7228 6578 6973  ser().mkdir(exis
+0001eae0: 745f 6f6b 3d54 7275 6529 0a20 2020 2020  t_ok=True).     
+0001eaf0: 2020 2070 6174 686c 6962 2e50 6174 6828     pathlib.Path(
+0001eb00: 277e 2f44 6f77 6e6c 6f61 6473 2f74 7075  '~/Downloads/tpu
+0001eb10: 2729 2e65 7870 616e 6475 7365 7228 292e  ').expanduser().
+0001eb20: 6d6b 6469 7228 7061 7265 6e74 733d 5472  mkdir(parents=Tr
+0001eb30: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+0001eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb60: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0001eb70: 7869 7374 5f6f 6b3d 5472 7565 290a 2020  xist_ok=True).  
+0001eb80: 2020 2020 2020 666f 7220 7961 6d6c 5f70        for yaml_p
+0001eb90: 6174 6820 696e 2073 656c 662e 5f54 4553  ath in self._TES
+0001eba0: 545f 5941 4d4c 5f50 4154 4853 3a0a 2020  T_YAML_PATHS:.  
+0001ebb0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0001ebc0: 6368 6563 6b5f 6571 7569 7661 6c65 6e74  check_equivalent
+0001ebd0: 2879 616d 6c5f 7061 7468 290a            (yaml_path).
```

### Comparing `skypilot-nightly-1.0.0.dev20230723/tests/test_spot.py` & `skypilot-nightly-1.0.0.dev20230724/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/tests/test_storage.py` & `skypilot-nightly-1.0.0.dev20230724/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230723/tests/test_wheels.py` & `skypilot-nightly-1.0.0.dev20230724/tests/test_wheels.py`

 * *Files identical despite different names*

