# Comparing `tmp/google-cloud-tasks-2.9.0.tar.gz` & `tmp/google-cloud-tasks-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-tasks-2.9.0.tar", last modified: Fri May  6 23:57:28 2022, max compression
+gzip compressed data, was "google-cloud-tasks-2.9.1.tar", last modified: Mon Jun  6 22:05:48 2022, max compression
```

## Comparing `google-cloud-tasks-2.9.0.tar` & `google-cloud-tasks-2.9.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.817560 google-cloud-tasks-2.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     3853 2022-05-06 23:57:28.817560 google-cloud-tasks-2.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2945 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.801552 google-cloud-tasks-2.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.801552 google-cloud-tasks-2.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.805554 google-cloud-tasks-2.9.0/google/cloud/tasks/
--rw-rw-r--   0 root         (0)     1003     2193 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks/__init__.py
--rw-rw-r--   0 root         (0)     1003       79 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.805554 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/
--rw-rw-r--   0 root         (0)     1003     1984 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     4275 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       79 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.805554 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.805554 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/
--rw-rw-r--   0 root         (0)     1003      753 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/__init__.py
--rw-rw-r--   0 root         (0)     1003    87255 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/async_client.py
--rw-rw-r--   0 root         (0)     1003    95681 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/client.py
--rw-rw-r--   0 root         (0)     1003    10428 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.805554 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/transports/
--rw-rw-r--   0 root         (0)     1003     1157 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    15362 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/transports/base.py
--rw-rw-r--   0 root         (0)     1003    33603 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34265 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.809556 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/types/
--rw-rw-r--   0 root         (0)     1003     1832 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    18428 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/types/cloudtasks.py
--rw-rw-r--   0 root         (0)     1003    18175 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/types/queue.py
--rw-rw-r--   0 root         (0)     1003    22798 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/types/target.py
--rw-rw-r--   0 root         (0)     1003    10331 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2/types/task.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.809556 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/
--rw-rw-r--   0 root         (0)     1003     2272 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003     5237 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       79 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.809556 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.809556 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/
--rw-rw-r--   0 root         (0)     1003      753 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/__init__.py
--rw-rw-r--   0 root         (0)     1003   109679 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/async_client.py
--rw-rw-r--   0 root         (0)     1003   118784 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/client.py
--rw-rw-r--   0 root         (0)     1003    10513 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.809556 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/
--rw-rw-r--   0 root         (0)     1003     1157 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    16993 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/base.py
--rw-rw-r--   0 root         (0)     1003    40966 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    41760 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.809556 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/types/
--rw-rw-r--   0 root         (0)     1003     2120 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    30944 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/types/cloudtasks.py
--rw-rw-r--   0 root         (0)     1003    22578 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/types/queue.py
--rw-rw-r--   0 root         (0)     1003    20529 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/types/target.py
--rw-rw-r--   0 root         (0)     1003     9488 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/types/task.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.813558 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/
--rw-rw-r--   0 root         (0)     1003     2125 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003     4285 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       79 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.813558 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.813558 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/
--rw-rw-r--   0 root         (0)     1003      753 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/__init__.py
--rw-rw-r--   0 root         (0)     1003    87879 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/async_client.py
--rw-rw-r--   0 root         (0)     1003    96305 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/client.py
--rw-rw-r--   0 root         (0)     1003    10513 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.813558 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/
--rw-rw-r--   0 root         (0)     1003     1157 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    15387 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/base.py
--rw-rw-r--   0 root         (0)     1003    33811 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34473 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.813558 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/types/
--rw-rw-r--   0 root         (0)     1003     1948 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    19686 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/types/cloudtasks.py
--rw-rw-r--   0 root         (0)     1003    22978 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/types/queue.py
--rw-rw-r--   0 root         (0)     1003    25574 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/types/target.py
--rw-rw-r--   0 root         (0)     1003    11363 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/types/task.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.817560 google-cloud-tasks-2.9.0/google_cloud_tasks.egg-info/
--rw-r--r--   0 root         (0)     1003     3853 2022-05-06 23:57:28.000000 google-cloud-tasks-2.9.0/google_cloud_tasks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3551 2022-05-06 23:57:28.000000 google-cloud-tasks-2.9.0/google_cloud_tasks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-05-06 23:57:28.000000 google-cloud-tasks-2.9.0/google_cloud_tasks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-05-06 23:57:28.000000 google-cloud-tasks-2.9.0/google_cloud_tasks.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-05-06 23:57:28.000000 google-cloud-tasks-2.9.0/google_cloud_tasks.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      128 2022-05-06 23:57:28.000000 google-cloud-tasks-2.9.0/google_cloud_tasks.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-05-06 23:57:28.000000 google-cloud-tasks-2.9.0/google_cloud_tasks.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.817560 google-cloud-tasks-2.9.0/scripts/
--rw-rw-r--   0 root         (0)     1003     6701 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/scripts/fixup_tasks_v2_keywords.py
--rw-rw-r--   0 root         (0)     1003     7036 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/scripts/fixup_tasks_v2beta2_keywords.py
--rw-rw-r--   0 root         (0)     1003     6727 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/scripts/fixup_tasks_v2beta3_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-05-06 23:57:28.817560 google-cloud-tasks-2.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2838 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.817560 google-cloud-tasks-2.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.801552 google-cloud-tasks-2.9.0/tests/system/
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.801552 google-cloud-tasks-2.9.0/tests/system/gapic/
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.817560 google-cloud-tasks-2.9.0/tests/system/gapic/v2/
--rw-rw-r--   0 root         (0)     1003      921 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/tests/system/gapic/v2/test_system_tasks_v2.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.817560 google-cloud-tasks-2.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.817560 google-cloud-tasks-2.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.817560 google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   194286 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2/test_cloud_tasks.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.817560 google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2beta2/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003   228948 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2beta2/test_cloud_tasks.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-06 23:57:28.817560 google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2beta3/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003   196743 2022-05-06 23:54:49.000000 google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2beta3/test_cloud_tasks.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.495355 google-cloud-tasks-2.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     3851 2022-06-06 22:05:48.495355 google-cloud-tasks-2.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2945 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.475345 google-cloud-tasks-2.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.475345 google-cloud-tasks-2.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.479347 google-cloud-tasks-2.9.1/google/cloud/tasks/
+-rw-rw-r--   0 root         (0)     1003     2193 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks/__init__.py
+-rw-rw-r--   0 root         (0)     1003       79 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.479347 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/
+-rw-rw-r--   0 root         (0)     1003     1984 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4275 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       79 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.479347 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.479347 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/
+-rw-rw-r--   0 root         (0)     1003      753 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/__init__.py
+-rw-rw-r--   0 root         (0)     1003    87255 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/async_client.py
+-rw-rw-r--   0 root         (0)     1003    95681 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/client.py
+-rw-rw-r--   0 root         (0)     1003    10428 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.479347 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/transports/
+-rw-rw-r--   0 root         (0)     1003     1157 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15362 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    33603 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34265 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.483349 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/types/
+-rw-rw-r--   0 root         (0)     1003     1832 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18428 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/types/cloudtasks.py
+-rw-rw-r--   0 root         (0)     1003    18175 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/types/queue.py
+-rw-rw-r--   0 root         (0)     1003    22798 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/types/target.py
+-rw-rw-r--   0 root         (0)     1003    10331 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2/types/task.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.483349 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/
+-rw-rw-r--   0 root         (0)     1003     2272 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5237 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       79 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.483349 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.483349 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/
+-rw-rw-r--   0 root         (0)     1003      753 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/__init__.py
+-rw-rw-r--   0 root         (0)     1003   109679 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/async_client.py
+-rw-rw-r--   0 root         (0)     1003   118784 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/client.py
+-rw-rw-r--   0 root         (0)     1003    10513 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.483349 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/
+-rw-rw-r--   0 root         (0)     1003     1157 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16993 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    40966 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    41760 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.487351 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/types/
+-rw-rw-r--   0 root         (0)     1003     2120 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30944 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/types/cloudtasks.py
+-rw-rw-r--   0 root         (0)     1003    22578 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/types/queue.py
+-rw-rw-r--   0 root         (0)     1003    20529 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/types/target.py
+-rw-rw-r--   0 root         (0)     1003     9488 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/types/task.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.487351 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/
+-rw-rw-r--   0 root         (0)     1003     2125 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4285 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       79 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.487351 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.487351 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/
+-rw-rw-r--   0 root         (0)     1003      753 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/__init__.py
+-rw-rw-r--   0 root         (0)     1003    87879 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/async_client.py
+-rw-rw-r--   0 root         (0)     1003    96305 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/client.py
+-rw-rw-r--   0 root         (0)     1003    10513 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.487351 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/
+-rw-rw-r--   0 root         (0)     1003     1157 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15387 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    33811 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34473 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.491353 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/types/
+-rw-rw-r--   0 root         (0)     1003     1948 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19686 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/types/cloudtasks.py
+-rw-rw-r--   0 root         (0)     1003    22978 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/types/queue.py
+-rw-rw-r--   0 root         (0)     1003    25574 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/types/target.py
+-rw-rw-r--   0 root         (0)     1003    11363 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/types/task.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.491353 google-cloud-tasks-2.9.1/google_cloud_tasks.egg-info/
+-rw-r--r--   0 root         (0)     1003     3851 2022-06-06 22:05:47.000000 google-cloud-tasks-2.9.1/google_cloud_tasks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3551 2022-06-06 22:05:48.000000 google-cloud-tasks-2.9.1/google_cloud_tasks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-06-06 22:05:47.000000 google-cloud-tasks-2.9.1/google_cloud_tasks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-06-06 22:05:48.000000 google-cloud-tasks-2.9.1/google_cloud_tasks.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-06-06 22:05:47.000000 google-cloud-tasks-2.9.1/google_cloud_tasks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      165 2022-06-06 22:05:48.000000 google-cloud-tasks-2.9.1/google_cloud_tasks.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-06-06 22:05:48.000000 google-cloud-tasks-2.9.1/google_cloud_tasks.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.491353 google-cloud-tasks-2.9.1/scripts/
+-rw-rw-r--   0 root         (0)     1003     6701 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/scripts/fixup_tasks_v2_keywords.py
+-rw-rw-r--   0 root         (0)     1003     7036 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/scripts/fixup_tasks_v2beta2_keywords.py
+-rw-rw-r--   0 root         (0)     1003     6727 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/scripts/fixup_tasks_v2beta3_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-06-06 22:05:48.495355 google-cloud-tasks-2.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2886 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.491353 google-cloud-tasks-2.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.475345 google-cloud-tasks-2.9.1/tests/system/
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.475345 google-cloud-tasks-2.9.1/tests/system/gapic/
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.491353 google-cloud-tasks-2.9.1/tests/system/gapic/v2/
+-rw-rw-r--   0 root         (0)     1003      921 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/tests/system/gapic/v2/test_system_tasks_v2.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.491353 google-cloud-tasks-2.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.491353 google-cloud-tasks-2.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.491353 google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   194442 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2/test_cloud_tasks.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.491353 google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2beta2/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   229104 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2beta2/test_cloud_tasks.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 22:05:48.491353 google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2beta3/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003   196899 2022-06-06 22:03:09.000000 google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2beta3/test_cloud_tasks.py
```

### Comparing `google-cloud-tasks-2.9.0/LICENSE` & `google-cloud-tasks-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/MANIFEST.in` & `google-cloud-tasks-2.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/PKG-INFO` & `google-cloud-tasks-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-tasks
-Version: 2.9.0
+Version: 2.9.1
 Summary: Cloud Tasks API API client library
 Home-page: https://github.com/googleapis/python-tasks
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -109,9 +109,7 @@
 
 -  Read the `Client Library Documentation`_ for Cloud Tasks API
    to see other available methods on the client.
 -  Read the `Cloud Tasks API Product documentation`_ to learn
    more about the product and see How-to Guides.
 
 .. _Cloud Tasks API Product documentation:  https://cloud.google.com/tasks
-
-
```

### Comparing `google-cloud-tasks-2.9.0/README.rst` & `google-cloud-tasks-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/gapic_metadata.json` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/async_client.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/client.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/pagers.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/transports/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/transports/base.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/transports/grpc.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/services/cloud_tasks/transports/grpc_asyncio.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/services/cloud_tasks/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/types/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/types/cloudtasks.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/types/cloudtasks.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/types/queue.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/types/queue.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/types/target.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/types/target.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2/types/task.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2/types/task.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/gapic_metadata.json` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/async_client.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/client.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/pagers.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/base.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/grpc.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/grpc_asyncio.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/services/cloud_tasks/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/types/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/types/cloudtasks.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/types/cloudtasks.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/types/queue.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/types/queue.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/types/target.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/types/target.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta2/types/task.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta2/types/task.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/gapic_metadata.json` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/async_client.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/client.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/pagers.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/base.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/grpc.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/grpc_asyncio.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/services/cloud_tasks/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/types/__init__.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/types/cloudtasks.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/types/cloudtasks.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/types/queue.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/types/queue.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/types/target.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/types/target.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google/cloud/tasks_v2beta3/types/task.py` & `google-cloud-tasks-2.9.1/google/cloud/tasks_v2beta3/types/task.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/google_cloud_tasks.egg-info/PKG-INFO` & `google-cloud-tasks-2.9.1/google_cloud_tasks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-tasks
-Version: 2.9.0
+Version: 2.9.1
 Summary: Cloud Tasks API API client library
 Home-page: https://github.com/googleapis/python-tasks
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -109,9 +109,7 @@
 
 -  Read the `Client Library Documentation`_ for Cloud Tasks API
    to see other available methods on the client.
 -  Read the `Cloud Tasks API Product documentation`_ to learn
    more about the product and see How-to Guides.
 
 .. _Cloud Tasks API Product documentation:  https://cloud.google.com/tasks
-
-
```

### Comparing `google-cloud-tasks-2.9.0/google_cloud_tasks.egg-info/SOURCES.txt` & `google-cloud-tasks-2.9.1/google_cloud_tasks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/scripts/fixup_tasks_v2_keywords.py` & `google-cloud-tasks-2.9.1/scripts/fixup_tasks_v2_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/scripts/fixup_tasks_v2beta2_keywords.py` & `google-cloud-tasks-2.9.1/scripts/fixup_tasks_v2beta2_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/scripts/fixup_tasks_v2beta3_keywords.py` & `google-cloud-tasks-2.9.1/scripts/fixup_tasks_v2beta3_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/setup.py` & `google-cloud-tasks-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,23 +17,24 @@
 import io
 import os
 
 import setuptools
 
 name = "google-cloud-tasks"
 description = "Cloud Tasks API API client library"
-version = "2.9.0"
+version = "2.9.1"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     # NOTE: Maintainers, please do not require google-api-core>=2.x.x
     # Until this issue is closed
     # https://github.com/googleapis/google-cloud-python/issues/10566
     "google-api-core[grpc] >= 1.31.5, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
-    "proto-plus >= 1.15.0",
+    "proto-plus >= 1.15.0, <2.0.0dev",
+    "protobuf >= 3.19.0, <4.0.0dev",
 ]
 
 extras = {"libcst": "libcst >= 0.2.5"}
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
```

### Comparing `google-cloud-tasks-2.9.0/tests/__init__.py` & `google-cloud-tasks-2.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/tests/system/gapic/v2/test_system_tasks_v2.py` & `google-cloud-tasks-2.9.1/tests/system/gapic/v2/test_system_tasks_v2.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/tests/unit/__init__.py` & `google-cloud-tasks-2.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/tests/unit/gapic/__init__.py` & `google-cloud-tasks-2.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2/__init__.py` & `google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2/test_cloud_tasks.py` & `google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2/test_cloud_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import math
 import os
 
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
+
+import math
+
 from google.api_core import gapic_v1, grpc_helpers, grpc_helpers_async, path_template
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 import google.auth
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
 from google.iam.v1 import iam_policy_pb2  # type: ignore
@@ -30,15 +38,14 @@
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 from google.type import expr_pb2  # type: ignore
 import grpc
 from grpc.experimental import aio
-import mock
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 
 from google.cloud.tasks_v2.services.cloud_tasks import (
     CloudTasksAsyncClient,
     CloudTasksClient,
     pagers,
```

### Comparing `google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2beta2/__init__.py` & `google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2beta2/test_cloud_tasks.py` & `google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2beta2/test_cloud_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import math
 import os
 
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
+
+import math
+
 from google.api_core import gapic_v1, grpc_helpers, grpc_helpers_async, path_template
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 import google.auth
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
 from google.iam.v1 import iam_policy_pb2  # type: ignore
@@ -30,15 +38,14 @@
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 from google.type import expr_pb2  # type: ignore
 import grpc
 from grpc.experimental import aio
-import mock
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 
 from google.cloud.tasks_v2beta2.services.cloud_tasks import (
     CloudTasksAsyncClient,
     CloudTasksClient,
     pagers,
```

### Comparing `google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2beta3/__init__.py` & `google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tasks-2.9.0/tests/unit/gapic/tasks_v2beta3/test_cloud_tasks.py` & `google-cloud-tasks-2.9.1/tests/unit/gapic/tasks_v2beta3/test_cloud_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import math
 import os
 
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
+
+import math
+
 from google.api_core import gapic_v1, grpc_helpers, grpc_helpers_async, path_template
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 import google.auth
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
 from google.iam.v1 import iam_policy_pb2  # type: ignore
@@ -30,15 +38,14 @@
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 from google.type import expr_pb2  # type: ignore
 import grpc
 from grpc.experimental import aio
-import mock
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 
 from google.cloud.tasks_v2beta3.services.cloud_tasks import (
     CloudTasksAsyncClient,
     CloudTasksClient,
     pagers,
```

