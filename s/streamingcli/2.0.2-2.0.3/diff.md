# Comparing `tmp/streamingcli-2.0.2.tar.gz` & `tmp/streamingcli-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamingcli-2.0.2.tar", last modified: Wed Jul 19 12:55:27 2023, max compression
+gzip compressed data, was "streamingcli-2.0.3.tar", last modified: Tue Jul 25 13:25:36 2023, max compression
```

## Comparing `streamingcli-2.0.2.tar` & `streamingcli-2.0.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.846861 streamingcli-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 12:55:22.000000 streamingcli-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-19 12:55:22.000000 streamingcli-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-19 12:55:27.846861 streamingcli-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-19 12:55:22.000000 streamingcli-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-19 12:55:27.000000 streamingcli-2.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-19 12:55:27.850861 streamingcli-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-19 12:55:22.000000 streamingcli-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.842861 streamingcli-2.0.2/streamingcli/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.842861 streamingcli-2.0.2/streamingcli/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/docker/login_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/docker_response_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.842861 streamingcli-2.0.2/streamingcli/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/jupyter/jar_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/jupyter/notebook_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.842861 streamingcli-2.0.2/streamingcli/platform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/platform/deployment_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/platform/jinja_prettifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.842861 streamingcli-2.0.2/streamingcli/platform/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/platform/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/platform/k8s/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/platform/k8s/deployment_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.846861 streamingcli-2.0.2/streamingcli/platform/ververica/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/platform/ververica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/platform/ververica/deployment_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/platform/ververica/deployment_target_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.846861 streamingcli-2.0.2/streamingcli/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/profile/profile_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.846861 streamingcli-2.0.2/streamingcli/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/project/build_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/project/deploy_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.846861 streamingcli-2.0.2/streamingcli/project/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/project/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/project/jupyter/jupyter_project_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/project/local_project_config.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/project/project_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/project/publish_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.846861 streamingcli-2.0.2/streamingcli/project/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/project/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/project/python/python_project_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/project/template_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.846861 streamingcli-2.0.2/streamingcli/project/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/project/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/project/templates/flink_app.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-19 12:55:22.000000 streamingcli-2.0.2/streamingcli/project/yaml_merger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.842861 streamingcli-2.0.2/streamingcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-19 12:55:27.000000 streamingcli-2.0.2/streamingcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-19 12:55:27.000000 streamingcli-2.0.2/streamingcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:55:27.000000 streamingcli-2.0.2/streamingcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-19 12:55:27.000000 streamingcli-2.0.2/streamingcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-19 12:55:27.000000 streamingcli-2.0.2/streamingcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-19 12:55:27.000000 streamingcli-2.0.2/streamingcli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.846861 streamingcli-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.846861 streamingcli-2.0.2/tests/streamingcli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/tests/streamingcli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.846861 streamingcli-2.0.2/tests/streamingcli/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/tests/streamingcli/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-07-19 12:55:22.000000 streamingcli-2.0.2/tests/streamingcli/jupyter/test_notebook_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.846861 streamingcli-2.0.2/tests/streamingcli/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/tests/streamingcli/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-19 12:55:22.000000 streamingcli-2.0.2/tests/streamingcli/profile/test_profile_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:27.846861 streamingcli-2.0.2/tests/streamingcli/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:22.000000 streamingcli-2.0.2/tests/streamingcli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-19 12:55:22.000000 streamingcli-2.0.2/tests/streamingcli/project/test_yaml_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-19 12:55:22.000000 streamingcli-2.0.2/tests/streamingcli/test_k82_deployment_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-19 12:55:22.000000 streamingcli-2.0.2/tests/streamingcli/test_vvp_deployment_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.996984 streamingcli-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 13:25:29.000000 streamingcli-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 13:25:29.000000 streamingcli-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-25 13:25:35.996984 streamingcli-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-25 13:25:29.000000 streamingcli-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-25 13:25:35.000000 streamingcli-2.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-25 13:25:35.996984 streamingcli-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-25 13:25:29.000000 streamingcli-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.988983 streamingcli-2.0.3/streamingcli/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.992983 streamingcli-2.0.3/streamingcli/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/docker/login_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/docker_response_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.992983 streamingcli-2.0.3/streamingcli/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/jupyter/jar_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/jupyter/notebook_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.992983 streamingcli-2.0.3/streamingcli/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/platform/deployment_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/platform/jinja_prettifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.992983 streamingcli-2.0.3/streamingcli/platform/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/platform/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/platform/k8s/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/platform/k8s/deployment_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.992983 streamingcli-2.0.3/streamingcli/platform/ververica/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/platform/ververica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/platform/ververica/deployment_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/platform/ververica/deployment_target_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.992983 streamingcli-2.0.3/streamingcli/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/profile/profile_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.992983 streamingcli-2.0.3/streamingcli/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/project/build_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/project/deploy_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.992983 streamingcli-2.0.3/streamingcli/project/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/project/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/project/jupyter/jupyter_project_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/project/local_project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/project/project_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/project/publish_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.992983 streamingcli-2.0.3/streamingcli/project/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/project/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/project/python/python_project_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/project/template_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.992983 streamingcli-2.0.3/streamingcli/project/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/project/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/project/templates/flink_app.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-25 13:25:29.000000 streamingcli-2.0.3/streamingcli/project/yaml_merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.988983 streamingcli-2.0.3/streamingcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-25 13:25:35.000000 streamingcli-2.0.3/streamingcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-25 13:25:35.000000 streamingcli-2.0.3/streamingcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:25:35.000000 streamingcli-2.0.3/streamingcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 13:25:35.000000 streamingcli-2.0.3/streamingcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-25 13:25:35.000000 streamingcli-2.0.3/streamingcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-25 13:25:35.000000 streamingcli-2.0.3/streamingcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.992983 streamingcli-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.992983 streamingcli-2.0.3/tests/streamingcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/tests/streamingcli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.996984 streamingcli-2.0.3/tests/streamingcli/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/tests/streamingcli/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-07-25 13:25:29.000000 streamingcli-2.0.3/tests/streamingcli/jupyter/test_notebook_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.996984 streamingcli-2.0.3/tests/streamingcli/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/tests/streamingcli/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-25 13:25:29.000000 streamingcli-2.0.3/tests/streamingcli/profile/test_profile_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:35.996984 streamingcli-2.0.3/tests/streamingcli/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:25:29.000000 streamingcli-2.0.3/tests/streamingcli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-25 13:25:29.000000 streamingcli-2.0.3/tests/streamingcli/project/test_yaml_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-25 13:25:29.000000 streamingcli-2.0.3/tests/streamingcli/test_k82_deployment_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-25 13:25:29.000000 streamingcli-2.0.3/tests/streamingcli/test_vvp_deployment_adapter.py
```

### Comparing `streamingcli-2.0.2/LICENSE` & `streamingcli-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/PKG-INFO` & `streamingcli-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamingcli
-Version: 2.0.2
+Version: 2.0.3
 Summary: Streaming platform CLI
 Home-page: https://github.com/getindata/streaming-cli
 Author: GetInData
 Author-email: office@getindata.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `streamingcli-2.0.2/README.md` & `streamingcli-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/requirements.txt` & `streamingcli-2.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/setup.cfg` & `streamingcli-2.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.0.2
+current_version = 2.0.3
 
 [flake8]
 exclude = .git,__pycache__,build,dist,*.yml
 max-line-length = 120
 extend-ignore = E203
 
 [mypy]
```

### Comparing `streamingcli-2.0.2/setup.py` & `streamingcli-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 from typing import List
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 def get_requirements(filename: str) -> List[str]:
     with open(filename, "r", encoding="utf-8") as fp:
```

### Comparing `streamingcli-2.0.2/streamingcli/config.py` & `streamingcli-2.0.3/streamingcli/config.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/docker/login_command.py` & `streamingcli-2.0.3/streamingcli/docker/login_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/docker_response_reader.py` & `streamingcli-2.0.3/streamingcli/docker_response_reader.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/jupyter/jar_handler.py` & `streamingcli-2.0.3/streamingcli/jupyter/jar_handler.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/jupyter/notebook_converter.py` & `streamingcli-2.0.3/streamingcli/jupyter/notebook_converter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/main.py` & `streamingcli-2.0.3/streamingcli/main.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/platform/deployment_adapter.py` & `streamingcli-2.0.3/streamingcli/platform/deployment_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/platform/k8s/config_loader.py` & `streamingcli-2.0.3/streamingcli/platform/k8s/config_loader.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/platform/k8s/deployment_adapter.py` & `streamingcli-2.0.3/streamingcli/platform/k8s/deployment_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/platform/ververica/deployment_adapter.py` & `streamingcli-2.0.3/streamingcli/platform/ververica/deployment_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/platform/ververica/deployment_target_adapter.py` & `streamingcli-2.0.3/streamingcli/platform/ververica/deployment_target_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/profile/profile_adapter.py` & `streamingcli-2.0.3/streamingcli/profile/profile_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/project/build_command.py` & `streamingcli-2.0.3/streamingcli/project/build_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/project/deploy_command.py` & `streamingcli-2.0.3/streamingcli/project/deploy_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/project/jupyter/jupyter_project_factory.py` & `streamingcli-2.0.3/streamingcli/project/jupyter/jupyter_project_factory.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/project/local_project_config.py` & `streamingcli-2.0.3/streamingcli/project/local_project_config.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/project/publish_command.py` & `streamingcli-2.0.3/streamingcli/project/publish_command.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/project/python/python_project_factory.py` & `streamingcli-2.0.3/streamingcli/project/python/python_project_factory.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/project/template_loader.py` & `streamingcli-2.0.3/streamingcli/project/template_loader.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli/project/templates/flink_app.py.template` & `streamingcli-2.0.3/streamingcli/project/templates/flink_app.py.template`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli.egg-info/PKG-INFO` & `streamingcli-2.0.3/streamingcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamingcli
-Version: 2.0.2
+Version: 2.0.3
 Summary: Streaming platform CLI
 Home-page: https://github.com/getindata/streaming-cli
 Author: GetInData
 Author-email: office@getindata.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `streamingcli-2.0.2/streamingcli.egg-info/SOURCES.txt` & `streamingcli-2.0.3/streamingcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/streamingcli.egg-info/requires.txt` & `streamingcli-2.0.3/streamingcli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/tests/streamingcli/jupyter/test_notebook_converter.py` & `streamingcli-2.0.3/tests/streamingcli/jupyter/test_notebook_converter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/tests/streamingcli/profile/test_profile_adapter.py` & `streamingcli-2.0.3/tests/streamingcli/profile/test_profile_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/tests/streamingcli/test_k82_deployment_adapter.py` & `streamingcli-2.0.3/tests/streamingcli/test_k82_deployment_adapter.py`

 * *Files identical despite different names*

### Comparing `streamingcli-2.0.2/tests/streamingcli/test_vvp_deployment_adapter.py` & `streamingcli-2.0.3/tests/streamingcli/test_vvp_deployment_adapter.py`

 * *Files identical despite different names*

