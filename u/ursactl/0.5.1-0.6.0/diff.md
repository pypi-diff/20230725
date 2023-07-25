# Comparing `tmp/ursactl-0.5.1.tar.gz` & `tmp/ursactl-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jgsmith/Code/ursactl/dist/.tmp-h5e86ofw/ursactl-0.5.1.tar", last modified: Thu Jul 20 19:46:37 2023, max compression
+gzip compressed data, was "/Users/jgsmith/Code/ursactl/dist/.tmp-ievhknl6/ursactl-0.6.0.tar", last modified: Tue Jul 25 12:15:45 2023, max compression
```

## Comparing `ursactl-0.5.1.tar` & `ursactl-0.6.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 19:46:37.000000 ursactl-0.5.1/
--rw-r--r--   0 jgsmith    (501) staff       (20)       67 2023-01-01 19:09:45.000000 ursactl-0.5.1/CHANGELOG.md
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-01-01 19:09:45.000000 ursactl-0.5.1/LICENSE.md
--rw-r--r--   0 jgsmith    (501) staff       (20)      135 2023-01-01 19:09:45.000000 ursactl-0.5.1/MANIFEST.in
--rw-r--r--   0 jgsmith    (501) staff       (20)      994 2023-07-20 19:46:37.000000 ursactl-0.5.1/PKG-INFO
--rw-r--r--   0 jgsmith    (501) staff       (20)     1072 2023-07-20 19:46:18.000000 ursactl-0.5.1/README.md
--rw-r--r--   0 jgsmith    (501) staff       (20)       81 2023-01-01 19:09:45.000000 ursactl-0.5.1/pyproject.toml
--rw-r--r--   0 jgsmith    (501) staff       (20)      144 2023-07-08 17:43:40.000000 ursactl-0.5.1/requirements-dev.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-16 14:14:44.000000 ursactl-0.5.1/requirements.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)     1172 2023-07-20 19:46:37.000000 ursactl-0.5.1/setup.cfg
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 19:46:37.000000 ursactl-0.5.1/tests/
--rw-r--r--   0 jgsmith    (501) staff       (20)      382 2023-01-31 15:40:54.000000 ursactl-0.5.1/tests/test_ursactl.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.5.1/ursactl/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl/airflow_provider/
--rw-r--r--   0 jgsmith    (501) staff       (20)      431 2023-05-04 12:27:25.000000 ursactl-0.5.1/ursactl/airflow_provider/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     3787 2023-05-04 12:27:25.000000 ursactl-0.5.1/ursactl/airflow_provider/hooks.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl/controllers/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.5.1/ursactl/controllers/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1089 2023-01-31 15:40:54.000000 ursactl-0.5.1/ursactl/controllers/base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     7879 2023-07-16 14:14:44.000000 ursactl-0.5.1/ursactl/controllers/create.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     3313 2023-06-04 21:29:27.000000 ursactl-0.5.1/ursactl/controllers/delete.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1150 2023-03-24 15:51:14.000000 ursactl-0.5.1/ursactl/controllers/get.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1224 2023-07-20 19:45:48.000000 ursactl-0.5.1/ursactl/controllers/init.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     7280 2023-07-10 12:55:55.000000 ursactl-0.5.1/ursactl/controllers/list.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      446 2023-02-16 21:42:16.000000 ursactl-0.5.1/ursactl/controllers/refresh.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2293 2023-06-04 21:29:27.000000 ursactl-0.5.1/ursactl/controllers/run.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1944 2023-05-04 12:27:25.000000 ursactl-0.5.1/ursactl/controllers/send.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      762 2023-07-16 14:14:44.000000 ursactl-0.5.1/ursactl/controllers/show.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      764 2023-04-18 14:46:09.000000 ursactl-0.5.1/ursactl/controllers/stop.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     8140 2023-07-20 19:45:48.000000 ursactl-0.5.1/ursactl/controllers/sync.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     6031 2023-07-16 14:14:44.000000 ursactl-0.5.1/ursactl/controllers/update.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl/controllers/utils/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-06-04 21:29:27.000000 ursactl-0.5.1/ursactl/controllers/utils/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     5403 2023-07-16 14:14:44.000000 ursactl-0.5.1/ursactl/controllers/utils/transforms.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl/core/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.5.1/ursactl/core/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      640 2023-07-17 12:46:16.000000 ursactl-0.5.1/ursactl/core/_base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1501 2023-07-17 12:46:16.000000 ursactl-0.5.1/ursactl/core/agent.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2345 2023-07-20 19:45:48.000000 ursactl-0.5.1/ursactl/core/dataset.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      301 2023-04-18 14:46:09.000000 ursactl-0.5.1/ursactl/core/exc.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2023 2023-07-20 15:12:38.000000 ursactl-0.5.1/ursactl/core/pipeline.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1793 2023-07-20 12:42:32.000000 ursactl-0.5.1/ursactl/core/pipeline_run.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1967 2023-07-20 12:42:32.000000 ursactl-0.5.1/ursactl/core/pipeline_sweep.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     3658 2023-07-17 12:46:16.000000 ursactl-0.5.1/ursactl/core/project.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1010 2023-07-20 12:42:32.000000 ursactl-0.5.1/ursactl/core/running_agent.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl/core/services/
--rw-r--r--   0 jgsmith    (501) staff       (20)      871 2023-05-04 12:27:25.000000 ursactl-0.5.1/ursactl/core/services/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1823 2023-07-16 20:42:41.000000 ursactl-0.5.1/ursactl/core/services/_base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)    32670 2023-07-18 20:29:53.000000 ursactl-0.5.1/ursactl/core/services/ape_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     8454 2023-07-17 12:46:16.000000 ursactl-0.5.1/ursactl/core/services/dss_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1892 2023-07-17 12:46:16.000000 ursactl-0.5.1/ursactl/core/services/iam_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)    11923 2023-07-16 14:14:44.000000 ursactl-0.5.1/ursactl/core/services/planning_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2910 2023-05-04 12:27:25.000000 ursactl-0.5.1/ursactl/core/services/project_client.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl/core/utils/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-18 13:39:22.000000 ursactl-0.5.1/ursactl/core/utils/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1470 2023-04-18 14:46:09.000000 ursactl-0.5.1/ursactl/core/utils/magic.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      203 2023-07-20 19:45:48.000000 ursactl-0.5.1/ursactl/core/version.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl/ext/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.5.1/ursactl/ext/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     4269 2023-07-20 19:45:48.000000 ursactl-0.5.1/ursactl/main.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl/plugins/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.5.1/ursactl/plugins/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl/templates/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.5.1/ursactl/templates/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl.egg-info/
--rw-r--r--   0 jgsmith    (501) staff       (20)      994 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl.egg-info/PKG-INFO
--rw-r--r--   0 jgsmith    (501) staff       (20)     1603 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl.egg-info/SOURCES.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl.egg-info/dependency_links.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)       46 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl.egg-info/entry_points.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl.egg-info/requires.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        8 2023-07-20 19:46:37.000000 ursactl-0.5.1/ursactl.egg-info/top_level.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-02-17 20:26:57.000000 ursactl-0.5.1/ursactl.egg-info/zip-safe
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/
+-rw-r--r--   0 jgsmith    (501) staff       (20)       67 2023-01-01 19:09:45.000000 ursactl-0.6.0/CHANGELOG.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-01-01 19:09:45.000000 ursactl-0.6.0/LICENSE.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)      135 2023-01-01 19:09:45.000000 ursactl-0.6.0/MANIFEST.in
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2749 2023-07-25 12:15:45.000000 ursactl-0.6.0/PKG-INFO
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1675 2023-07-25 12:15:23.000000 ursactl-0.6.0/README.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)       81 2023-01-01 19:09:45.000000 ursactl-0.6.0/pyproject.toml
+-rw-r--r--   0 jgsmith    (501) staff       (20)      168 2023-07-25 12:15:23.000000 ursactl-0.6.0/requirements-dev.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-16 14:14:44.000000 ursactl-0.6.0/requirements.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1287 2023-07-25 12:15:45.000000 ursactl-0.6.0/setup.cfg
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/tests/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      382 2023-01-31 15:40:54.000000 ursactl-0.6.0/tests/test_ursactl.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.6.0/ursactl/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/airflow_provider/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      431 2023-05-04 12:27:25.000000 ursactl-0.6.0/ursactl/airflow_provider/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     3787 2023-05-04 12:27:25.000000 ursactl-0.6.0/ursactl/airflow_provider/hooks.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/controllers/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.6.0/ursactl/controllers/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1089 2023-01-31 15:40:54.000000 ursactl-0.6.0/ursactl/controllers/base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     7879 2023-07-16 14:14:44.000000 ursactl-0.6.0/ursactl/controllers/create.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     3313 2023-06-04 21:29:27.000000 ursactl-0.6.0/ursactl/controllers/delete.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1150 2023-03-24 15:51:14.000000 ursactl-0.6.0/ursactl/controllers/get.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1224 2023-07-20 19:45:48.000000 ursactl-0.6.0/ursactl/controllers/init.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     7280 2023-07-10 12:55:55.000000 ursactl-0.6.0/ursactl/controllers/list.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      446 2023-02-16 21:42:16.000000 ursactl-0.6.0/ursactl/controllers/refresh.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2297 2023-07-25 12:15:23.000000 ursactl-0.6.0/ursactl/controllers/run.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1944 2023-05-04 12:27:25.000000 ursactl-0.6.0/ursactl/controllers/send.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      762 2023-07-16 14:14:44.000000 ursactl-0.6.0/ursactl/controllers/show.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      764 2023-04-18 14:46:09.000000 ursactl-0.6.0/ursactl/controllers/stop.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     8140 2023-07-20 19:45:48.000000 ursactl-0.6.0/ursactl/controllers/sync.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     6031 2023-07-16 14:14:44.000000 ursactl-0.6.0/ursactl/controllers/update.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/controllers/utils/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-06-04 21:29:27.000000 ursactl-0.6.0/ursactl/controllers/utils/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     5403 2023-07-16 14:14:44.000000 ursactl-0.6.0/ursactl/controllers/utils/transforms.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/core/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.6.0/ursactl/core/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      640 2023-07-17 12:46:16.000000 ursactl-0.6.0/ursactl/core/_base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1501 2023-07-17 12:46:16.000000 ursactl-0.6.0/ursactl/core/agent.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2345 2023-07-20 19:45:48.000000 ursactl-0.6.0/ursactl/core/dataset.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      301 2023-04-18 14:46:09.000000 ursactl-0.6.0/ursactl/core/exc.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2023 2023-07-20 15:12:38.000000 ursactl-0.6.0/ursactl/core/pipeline.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1793 2023-07-20 12:42:32.000000 ursactl-0.6.0/ursactl/core/pipeline_run.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1967 2023-07-20 12:42:32.000000 ursactl-0.6.0/ursactl/core/pipeline_sweep.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     4578 2023-07-25 12:15:23.000000 ursactl-0.6.0/ursactl/core/project.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1010 2023-07-20 12:42:32.000000 ursactl-0.6.0/ursactl/core/running_agent.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/core/services/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      871 2023-05-04 12:27:25.000000 ursactl-0.6.0/ursactl/core/services/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1823 2023-07-25 12:10:01.000000 ursactl-0.6.0/ursactl/core/services/_base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)    32379 2023-07-25 12:15:23.000000 ursactl-0.6.0/ursactl/core/services/ape_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     8454 2023-07-17 12:46:16.000000 ursactl-0.6.0/ursactl/core/services/dss_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1892 2023-07-17 12:46:16.000000 ursactl-0.6.0/ursactl/core/services/iam_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)    11923 2023-07-16 14:14:44.000000 ursactl-0.6.0/ursactl/core/services/planning_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2910 2023-05-04 12:27:25.000000 ursactl-0.6.0/ursactl/core/services/project_client.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/core/utils/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-18 13:39:22.000000 ursactl-0.6.0/ursactl/core/utils/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1470 2023-04-18 14:46:09.000000 ursactl-0.6.0/ursactl/core/utils/magic.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      203 2023-07-25 12:15:23.000000 ursactl-0.6.0/ursactl/core/version.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/ext/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.6.0/ursactl/ext/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     4269 2023-07-20 19:45:48.000000 ursactl-0.6.0/ursactl/main.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/plugins/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.6.0/ursactl/plugins/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl/templates/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.6.0/ursactl/templates/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl.egg-info/
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2749 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl.egg-info/PKG-INFO
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1603 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl.egg-info/SOURCES.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl.egg-info/dependency_links.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)       46 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl.egg-info/entry_points.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl.egg-info/requires.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        8 2023-07-25 12:15:45.000000 ursactl-0.6.0/ursactl.egg-info/top_level.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-02-17 20:26:57.000000 ursactl-0.6.0/ursactl.egg-info/zip-safe
```

### Comparing `ursactl-0.5.1/ursactl/airflow_provider/hooks.py` & `ursactl-0.6.0/ursactl/airflow_provider/hooks.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/controllers/base.py` & `ursactl-0.6.0/ursactl/controllers/base.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/controllers/create.py` & `ursactl-0.6.0/ursactl/controllers/create.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/controllers/delete.py` & `ursactl-0.6.0/ursactl/controllers/delete.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/controllers/get.py` & `ursactl-0.6.0/ursactl/controllers/get.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/controllers/init.py` & `ursactl-0.6.0/ursactl/controllers/init.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/controllers/list.py` & `ursactl-0.6.0/ursactl/controllers/list.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/controllers/run.py` & `ursactl-0.6.0/ursactl/controllers/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,18 +46,18 @@
         if self.app.pargs.sweep_parameters:
             sweep_parameters = {
                 k: json.loads(v)
                 for k, v in dict(item.split('=') for item in self.app.pargs.sweep_parameters).items()
             }
 
         result = ape_client.run_pipeline(
-            pipeline,
+            pipeline=pipeline,
             parameters=parameters,
             sweep_parameters=sweep_parameters,
-            project_uuid=self._project_scope)
+            project=self._project_scope)
         self._print(result)
 
     def _print(self, data):
         if self.app.pargs.output == 'json':
             print(json.dumps(data))
         else:
             print(yaml.dump(data))
```

### Comparing `ursactl-0.5.1/ursactl/controllers/send.py` & `ursactl-0.6.0/ursactl/controllers/send.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/controllers/show.py` & `ursactl-0.6.0/ursactl/controllers/show.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/controllers/stop.py` & `ursactl-0.6.0/ursactl/controllers/stop.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/controllers/sync.py` & `ursactl-0.6.0/ursactl/controllers/sync.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/controllers/update.py` & `ursactl-0.6.0/ursactl/controllers/update.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/controllers/utils/transforms.py` & `ursactl-0.6.0/ursactl/controllers/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/core/_base.py` & `ursactl-0.6.0/ursactl/core/_base.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/core/agent.py` & `ursactl-0.6.0/ursactl/core/agent.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/core/dataset.py` & `ursactl-0.6.0/ursactl/core/dataset.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/core/pipeline.py` & `ursactl-0.6.0/ursactl/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/core/pipeline_run.py` & `ursactl-0.6.0/ursactl/core/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/core/pipeline_sweep.py` & `ursactl-0.6.0/ursactl/core/pipeline_sweep.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/core/running_agent.py` & `ursactl-0.6.0/ursactl/core/running_agent.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/core/services/__init__.py` & `ursactl-0.6.0/ursactl/core/services/__init__.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/core/services/_base.py` & `ursactl-0.6.0/ursactl/core/services/_base.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/core/services/ape_client.py` & `ursactl-0.6.0/ursactl/core/services/ape_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1072,33 +1072,25 @@
                 return {}
             variables = {'id': pipeline['id']}
 
         result = self.raw_query(query=DELETE_SYNCED_PIPELINE_MUTATION, variables=variables)
 
         return result['data']['deleteSyncedPipeline']
 
-    def run_pipeline(self, id, parameters=None, sweep_parameters=None, project_uuid=None):
+    def run_pipeline(self, pipeline, parameters=None, sweep_parameters=None, project=None):
         """
         Runs the pipeline.
         """
-        if self.is_uuid(id):
-            variables = {
-                'input': {
-                    'pipelineId': id
-                }
-            }
-        else:
-            pipeline = self.get_pipeline(path=id, project_uuid=project_uuid)
-            if pipeline is None:
-                return {}
-            variables = {
-                'input': {
-                    'pipelineId': pipeline['id']
-                }
+
+        variables = {
+            'input': {
+                'pipeline': pipeline,
+                'project': project
             }
+        }
         query = RUN_PIPELINE_MUTATION
         result_key = 'runPipeline'
         if parameters is not None:
             variables['input']['parameters'] = dumps(parameters)
         if sweep_parameters is not None and any(sweep_parameters):
             variables['input']['sweptParameters'] = dumps(sweep_parameters)
             query = SWEEP_PIPELINE_MUTATION
```

### Comparing `ursactl-0.5.1/ursactl/core/services/dss_client.py` & `ursactl-0.6.0/ursactl/core/services/dss_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/core/services/iam_client.py` & `ursactl-0.6.0/ursactl/core/services/iam_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/core/services/planning_client.py` & `ursactl-0.6.0/ursactl/core/services/planning_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/core/services/project_client.py` & `ursactl-0.6.0/ursactl/core/services/project_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/core/utils/magic.py` & `ursactl-0.6.0/ursactl/core/utils/magic.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl/main.py` & `ursactl-0.6.0/ursactl/main.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.5.1/ursactl.egg-info/SOURCES.txt` & `ursactl-0.6.0/ursactl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

