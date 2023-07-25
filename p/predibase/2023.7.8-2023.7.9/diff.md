# Comparing `tmp/predibase-2023.7.8.tar.gz` & `tmp/predibase-2023.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predibase-2023.7.8.tar", last modified: Tue Jul 18 20:04:24 2023, max compression
+gzip compressed data, was "predibase-2023.7.9.tar", last modified: Wed Jul 19 04:40:19 2023, max compression
```

## Comparing `predibase-2023.7.8.tar` & `predibase-2023.7.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:24.155298 predibase-2023.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 20:03:34.000000 predibase-2023.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 20:04:24.155298 predibase-2023.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-18 20:03:34.000000 predibase-2023.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:24.151298 predibase-2023.7.8/predibase/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:24.151298 predibase-2023.7.8/predibase/cli_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/cli_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/cli_commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/cli_commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/cli_commands/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/cli_commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/cli_commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/connection_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/dataset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/deployment_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/engine_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/llm_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/model_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/permission_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:24.151298 predibase-2023.7.8/predibase/pql/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/pql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/pql/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/pql/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/pql/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/query_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:24.155298 predibase-2023.7.8/predibase/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource/connection_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource/connection_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)    39312 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/resource_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/triton_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 20:04:23.000000 predibase-2023.7.8/predibase/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:24.151298 predibase-2023.7.8/predibase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 20:04:24.000000 predibase-2023.7.8/predibase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-18 20:04:24.000000 predibase-2023.7.8/predibase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:04:24.000000 predibase-2023.7.8/predibase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 20:04:24.000000 predibase-2023.7.8/predibase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:04:24.000000 predibase-2023.7.8/predibase.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-18 20:04:24.000000 predibase-2023.7.8/predibase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 20:04:24.000000 predibase-2023.7.8/predibase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:24.155298 predibase-2023.7.8/predibase_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase_notebook/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:04:24.155298 predibase-2023.7.8/predibase_notebook/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:34.000000 predibase-2023.7.8/predibase_notebook/nbextension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-18 20:04:23.000000 predibase-2023.7.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-18 20:03:34.000000 predibase-2023.7.8/requirements_predictor.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 20:04:24.155298 predibase-2023.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-18 20:03:34.000000 predibase-2023.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.931286 predibase-2023.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-19 04:39:16.000000 predibase-2023.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-19 04:40:19.931286 predibase-2023.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-19 04:39:16.000000 predibase-2023.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.927286 predibase-2023.7.9/predibase/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.927286 predibase-2023.7.9/predibase/cli_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/cli_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/cli_commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/cli_commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/cli_commands/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/cli_commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/cli_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/connection_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/dataset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/deployment_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/engine_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/llm_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/model_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/permission_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.927286 predibase-2023.7.9/predibase/pql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/pql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/pql/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/pql/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/pql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/query_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.931286 predibase-2023.7.9/predibase/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/connection_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/connection_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39312 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/triton_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.927286 predibase-2023.7.9/predibase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.931286 predibase-2023.7.9/predibase_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase_notebook/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.931286 predibase-2023.7.9/predibase_notebook/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase_notebook/nbextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-19 04:40:19.000000 predibase-2023.7.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-19 04:39:16.000000 predibase-2023.7.9/requirements_predictor.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 04:40:19.931286 predibase-2023.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-19 04:39:16.000000 predibase-2023.7.9/setup.py
```

### Comparing `predibase-2023.7.8/predibase/cli.py` & `predibase-2023.7.9/predibase/cli.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/cli_commands/delete.py` & `predibase-2023.7.9/predibase/cli_commands/delete.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/cli_commands/deploy.py` & `predibase-2023.7.9/predibase/cli_commands/deploy.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/cli_commands/prompt.py` & `predibase-2023.7.9/predibase/cli_commands/prompt.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/cli_commands/settings.py` & `predibase-2023.7.9/predibase/cli_commands/settings.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/cli_commands/utils.py` & `predibase-2023.7.9/predibase/cli_commands/utils.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/client.py` & `predibase-2023.7.9/predibase/client.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/connection.py` & `predibase-2023.7.9/predibase/connection.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/connection_mixin.py` & `predibase-2023.7.9/predibase/connection_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/dataset_mixin.py` & `predibase-2023.7.9/predibase/dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/deployment_mixin.py` & `predibase-2023.7.9/predibase/deployment_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/engine_mixin.py` & `predibase-2023.7.9/predibase/engine_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/llm_mixin.py` & `predibase-2023.7.9/predibase/llm_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,19 +46,15 @@
         if isinstance(dataset, Dataset):
             conn_id = dataset.connection_id
         elif isinstance(index, Dataset):
             conn_id = index.connection_id
         else:
             conn_id = self.list_connections()[0].id
 
-        df = self.session.execute(
-            query_str,
-            connection_id=conn_id,
-        )
-        return GeneratedResponse.to_responses(df) if not return_df else df
+        return self.session.execute(query_str, connection_id=conn_id)
 
     def deploy_llm(self, deployment_name: str, model_name: str, engine_template: Optional[str] = None):
         self.session.post_json(
             "/llms",
             json={
                 "name": deployment_name,
                 "modelName": model_name,
```

### Comparing `predibase-2023.7.8/predibase/model_mixin.py` & `predibase-2023.7.9/predibase/model_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/permission_mixin.py` & `predibase-2023.7.9/predibase/permission_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/pql/__init__.py` & `predibase-2023.7.9/predibase/pql/__init__.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/pql/adapter.py` & `predibase-2023.7.9/predibase/pql/adapter.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/pql/api.py` & `predibase-2023.7.9/predibase/pql/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #! /usr/bin/env python
 # Copyright (c) 2021 Predibase, Inc.
 
 import logging
+import platform
 import sys
 import time
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, Optional, Tuple, Union
 
 import pandas as pd
 import requests
 import requests.exceptions
 from urllib3.util import Retry
 
 from predibase.pql.adapter import TimeoutHTTPAdapter
 from predibase.pql.utils import get_results_df, retry
 from predibase.resource.user import User
+from predibase.version import __version__
 
 DEFAULT_API_ENDPOINT = "https://api.app.predibase.com/v1"
 DEFAULT_SERVING_ENDPOINT = "serving.app.predibase.com"
 
 
 class PQLException(RuntimeError):
     def __init__(self, message):
@@ -49,15 +51,15 @@
 
     def execute(
         self,
         statement: str,
         params: Dict[str, Any] = None,
         connection_id: Optional[int] = None,
         engine_id: Optional[int] = None,
-    ) -> int:
+    ) -> pd.DataFrame:
         if not self.is_plan_expired():
             if not statement.endswith(";"):
                 statement += ";"
 
             params = params or {}
             if self.verbose:
                 logging.info("-- EXECUTE:")
@@ -251,15 +253,18 @@
             timeout=self.timeout_in_seconds,
         )
         http.mount("https://", adapter)
         http.mount("http://", adapter)
         return http
 
     def _get_headers(self):
-        return {"Authorization": "Bearer " + self.token}
+        return {
+            "Authorization": "Bearer " + self.token,
+            "User-Agent": f"predibase-sdk/{__version__} ({platform.version()})",
+        }
 
     def _post(self, endpoint: str, data: Any = None, json: Any = None, **kwargs):
         return self._http().post(self.url + endpoint, data=data, json=json, headers=self._get_headers(), **kwargs)
 
     def _get(self, endpoint: str):
         return self._http().get(self.url + endpoint, headers=self._get_headers())
```

### Comparing `predibase-2023.7.8/predibase/pql/utils.py` & `predibase-2023.7.9/predibase/pql/utils.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/predictor.py` & `predibase-2023.7.9/predibase/predictor.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/query_mixin.py` & `predibase-2023.7.9/predibase/query_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/resource/config.py` & `predibase-2023.7.9/predibase/resource/config.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/resource/connection.py` & `predibase-2023.7.9/predibase/resource/connection.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/resource/connection_object.py` & `predibase-2023.7.9/predibase/resource/connection_object.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/resource/connection_properties.py` & `predibase-2023.7.9/predibase/resource/connection_properties.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/resource/dataset.py` & `predibase-2023.7.9/predibase/resource/dataset.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/resource/dataset_info.py` & `predibase-2023.7.9/predibase/resource/dataset_info.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/resource/deployment.py` & `predibase-2023.7.9/predibase/resource/deployment.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/resource/engine.py` & `predibase-2023.7.9/predibase/resource/engine.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/resource/llm.py` & `predibase-2023.7.9/predibase/resource/llm.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/resource/model.py` & `predibase-2023.7.9/predibase/resource/model.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/resource/query.py` & `predibase-2023.7.9/predibase/resource/query.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/resource/user.py` & `predibase-2023.7.9/predibase/resource/user.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/resource_util.py` & `predibase-2023.7.9/predibase/resource_util.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/triton_util.py` & `predibase-2023.7.9/predibase/triton_util.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase/util.py` & `predibase-2023.7.9/predibase/util.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase.egg-info/SOURCES.txt` & `predibase-2023.7.9/predibase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase_notebook/__init__.py` & `predibase-2023.7.9/predibase_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/predibase_notebook/env.py` & `predibase-2023.7.9/predibase_notebook/env.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.8/setup.py` & `predibase-2023.7.9/setup.py`

 * *Files identical despite different names*

