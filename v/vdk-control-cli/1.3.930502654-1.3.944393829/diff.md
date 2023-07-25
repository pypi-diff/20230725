# Comparing `tmp/vdk-control-cli-1.3.930502654.tar.gz` & `tmp/vdk-control-cli-1.3.944393829.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-control-cli-1.3.930502654.tar", last modified: Thu Jul 13 18:10:07 2023, max compression
+gzip compressed data, was "dist/vdk-control-cli-1.3.944393829.tar", last modified: Tue Jul 25 09:00:59 2023, max compression
```

## Comparing `vdk-control-cli-1.3.930502654.tar` & `vdk-control-cli-1.3.944393829.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5153 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1747 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/api/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/api/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/api/control/plugin/markers.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/api/control/plugin/specs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/common_group/
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/common_group/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/info_group/
--rw-rw-rw-   0 root         (0) root         (0)     1868 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/info_group/info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/
--rw-rw-rw-   0 root         (0) root         (0)    12776 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/create.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/delete.py
--rw-rw-rw-   0 root         (0) root         (0)     7121 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/deploy_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14343 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     5129 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/download_job.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/download_key.py
--rw-rw-rw-   0 root         (0) root         (0)    12207 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/execute.py
--rw-rw-rw-   0 root         (0) root         (0)     8735 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/list.py
--rw-rw-rw-   0 root         (0) root         (0)    11314 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/properties.py
--rw-rw-rw-   0 root         (0) root         (0)    11433 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/secrets.py
--rw-rw-rw-   0 root         (0) root         (0)     3403 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/show.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/login_group/
--rw-rw-rw-   0 root         (0) root         (0)     6510 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/login_group/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/logout_group/
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/logout_group/logout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/version_group/
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/version_group/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/default_options.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/defaults_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)     9551 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/exception/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/exception/vdk_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/job_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     4871 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/job_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/10_sql_step.sql
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/20_python_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/config.ini
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     3666 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     3715 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/plugin/control_plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/rest_lib/
--rw-rw-rw-   0 root         (0) root         (0)     3239 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/rest_lib/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/rest_lib/rest_client_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/
--rw-rw-rw-   0 root         (0) root         (0)     7297 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/control_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3690 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/output_printer.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-13 18:09:51.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/version_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-13 18:09:55.000000 vdk-control-cli-1.3.930502654/src/vdk/internal/control/vdk_control_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5153 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2426 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      185 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-13 18:10:07.000000 vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-13 18:09:55.000000 vdk-control-cli-1.3.930502654/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/api/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/api/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/api/control/plugin/markers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/api/control/plugin/specs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/common_group/
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/common_group/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/info_group/
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/info_group/info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/
+-rw-rw-rw-   0 root         (0) root         (0)    12776 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/create.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     7121 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/deploy_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14343 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     5129 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/download_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/download_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    12207 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     8735 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/list.py
+-rw-rw-rw-   0 root         (0) root         (0)    11314 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)    11433 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     3403 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/show.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/login_group/
+-rw-rw-rw-   0 root         (0) root         (0)     6510 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/login_group/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/logout_group/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/logout_group/logout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/version_group/
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/version_group/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/default_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/defaults_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9551 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/exception/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/exception/vdk_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/job_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/job_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/10_sql_step.sql
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/20_python_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2902 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/config.ini
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3666 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/plugin/control_plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/rest_lib/
+-rw-rw-rw-   0 root         (0) root         (0)     3239 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/rest_lib/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/rest_lib/rest_client_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     7297 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/control_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3690 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/output_printer.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/version_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-25 09:00:46.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/vdk_control_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      185 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-25 09:00:46.000000 vdk-control-cli-1.3.944393829/version.txt
```

### Comparing `vdk-control-cli-1.3.930502654/PKG-INFO` & `vdk-control-cli-1.3.944393829/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.930502654
+Version: 1.3.944393829
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.930502654/README.md` & `vdk-control-cli-1.3.944393829/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/setup.cfg` & `vdk-control-cli-1.3.944393829/setup.cfg`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/api/control/plugin/markers.py` & `vdk-control-cli-1.3.944393829/src/vdk/api/control/plugin/markers.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/api/control/plugin/specs.py` & `vdk-control-cli-1.3.944393829/src/vdk/api/control/plugin/specs.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/common_group/default.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/common_group/default.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/info_group/info.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/info_group/info.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/create.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/create.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/delete.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/deploy_cli.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/download_job.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/download_job.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/download_key.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/download_key.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/execute.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/execute.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/list.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/list.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/properties.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/properties.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/secrets.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/secrets.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/job/show.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/show.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/login_group/login.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/login_group/login.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/command_groups/version_group/version.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/version_group/version.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/defaults_config.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/defaults_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/log_config.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/configuration/vdk_config.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/vdk_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/exception/vdk_exception.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/exception/vdk_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/job_archive.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/job_archive.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/job_config.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/job_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/10_sql_step.sql` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/10_sql_step.sql`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/20_python_step.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/20_python_step.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/README.md` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/job/sample_job/config.ini` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/main.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/main.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/plugin/control_plugin_manager.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/plugin/control_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/rest_lib/factory.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/rest_lib/factory.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/rest_lib/rest_client_errors.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/rest_lib/rest_client_errors.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/cli_utils.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/control_utils.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/control_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/output_printer.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/output_printer.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk/internal/control/utils/version_utils.py` & `vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/PKG-INFO` & `vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.930502654
+Version: 1.3.944393829
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.930502654/src/vdk_control_cli.egg-info/SOURCES.txt` & `vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

