# Comparing `tmp/taskcluster-taskgraph-5.7.0.tar.gz` & `tmp/taskcluster-taskgraph-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskcluster-taskgraph-5.7.0.tar", last modified: Thu Jul 20 14:25:19 2023, max compression
+gzip compressed data, was "taskcluster-taskgraph-6.0.0.tar", last modified: Tue Jul 25 19:06:11 2023, max compression
```

## Comparing `taskcluster-taskgraph-5.7.0.tar` & `taskcluster-taskgraph-6.0.0.tar`

### file list

```diff
@@ -1,146 +1,148 @@
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.959815 taskcluster-taskgraph-5.7.0/
--rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/LICENSE
--rw-r--r--   0 ahal      (1000) ahal      (1000)      175 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/MANIFEST.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-07-20 14:25:19.959815 taskcluster-taskgraph-5.7.0/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3659 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/README.rst
--rw-r--r--   0 ahal      (1000) ahal      (1000)      602 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.7.0/pyproject.toml
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/requirements/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      179 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/requirements/base.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)    20339 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/requirements/base.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       22 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/requirements/dev.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1281 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.7.0/requirements/dev.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       58 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.7.0/requirements/test.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9241 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/requirements/test.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-07-20 14:25:19.959815 taskcluster-taskgraph-5.7.0/setup.cfg
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1555 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/setup.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/src/
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-07-20 14:25:19.000000 taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3977 2023-07-20 14:25:19.000000 taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-07-20 14:25:19.000000 taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       50 2023-07-20 14:25:19.000000 taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)      203 2023-07-20 14:25:19.000000 taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/requires.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       10 2023-07-20 14:25:19.000000 taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/src/taskgraph/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      729 2023-07-20 14:24:45.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/__init__.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      416 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1836 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/add_new_jobs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1309 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/cancel.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1941 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/cancel_all.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1086 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/rebuild_cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    13122 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/registry.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9387 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/retrigger.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/actions/util.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4822 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/config.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5184 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/create.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12882 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7834 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2793 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/files_changed.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      866 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/filter_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    15667 2023-07-20 14:07:39.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/generator.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4680 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/graph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/src/taskgraph/loader/
--rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/loader/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1185 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/loader/default.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2147 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/loader/transform.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    26201 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/main.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9192 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/morph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/src/taskgraph/optimize/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      123 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/optimize/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    18341 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/optimize/base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2380 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/optimize/strategies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    11918 2023-07-20 14:07:39.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/parameters.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.939818 taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)    29990 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/fetch-content
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)      896 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/hgrc
--rw-r--r--   0 ahal      (1000) ahal      (1000)    30813 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/robustcheckout.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)    45128 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/run-task
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3324 2023-04-03 20:22:29.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/target_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3240 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2434 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/taskgraph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.949816 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      110 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5146 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2607 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      707 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/code_review.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7606 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/docker_image.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10479 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/fetch.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6647 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/from_deps.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.949816 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/
--rw-r--r--   0 ahal      (1000) ahal      (1000)    17324 2023-07-20 14:07:39.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5897 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/common.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1220 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/index_search.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9814 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6015 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/toolchain.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6019 2023-03-09 21:54:49.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/notify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    52254 2023-07-20 14:07:39.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/task.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.949816 taskcluster-taskgraph-5.7.0/src/taskgraph/util/
--rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2855 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/archive.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2964 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/attributes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3406 2023-06-02 18:49:13.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2433 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2592 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/dependencies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    11699 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/hash.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3419 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/keyed_by.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1331 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/memoize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3184 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/parameterization.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4466 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1576 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/python_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      787 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/readonlydict.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     8323 2023-04-18 14:17:54.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/schema.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1317 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/shell.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12445 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/taskcluster.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1969 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/taskgraph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1417 2022-05-30 14:06:28.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/templates.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3390 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/time.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2687 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/treeherder.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    18780 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/vcs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     8947 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/verify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2498 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/workertypes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      990 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/src/taskgraph/util/yaml.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-20 14:25:19.959815 taskcluster-taskgraph-5.7.0/test/
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1584 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.7.0/test/test_actions_rebuild_cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1670 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_actions_registry.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3654 2023-03-09 21:40:30.000000 taskcluster-taskgraph-5.7.0/test/test_create.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7688 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3505 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_files_changed.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     8883 2023-07-20 14:07:39.000000 taskcluster-taskgraph-5.7.0/test/test_generator.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7063 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_graph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7940 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.7.0/test/test_main.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2701 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_morph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    15584 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.7.0/test/test_optimize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1727 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_optimize_strategies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    13921 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_parameters.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2491 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_scripts_fetch_content.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12257 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/test/test_scripts_run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12046 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_target_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3759 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_taskgraph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1812 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_transform_docker_image.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      874 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1527 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_fetch.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6985 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_from_deps.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5181 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_job.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6291 2023-04-19 14:40:27.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_job_run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7131 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_job_toolchain.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6948 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_notify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    25785 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/test/test_transforms_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3596 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_attributes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1120 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/test/test_util_dependencies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10212 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2340 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_memoize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7556 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_util_parameterization.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5906 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1045 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.7.0/test/test_util_python_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1234 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_readonlydict.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6961 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_schema.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10115 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_util_taskcluster.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)     1677 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_templates.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)     2239 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_time.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      913 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_treeherder.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    15598 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/test/test_util_vcs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4981 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.7.0/test/test_util_verify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      942 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.7.0/test/test_util_workertypes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1005 2023-07-19 20:40:46.000000 taskcluster-taskgraph-5.7.0/test/test_util_yaml.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.724823 taskcluster-taskgraph-6.0.0/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    16725 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/LICENSE
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      175 2023-03-14 14:30:55.000000 taskcluster-taskgraph-6.0.0/MANIFEST.in
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      665 2023-07-25 19:06:11.724823 taskcluster-taskgraph-6.0.0/PKG-INFO
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3659 2023-07-24 11:50:22.000000 taskcluster-taskgraph-6.0.0/README.rst
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      602 2023-05-15 20:06:30.000000 taskcluster-taskgraph-6.0.0/pyproject.toml
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.692823 taskcluster-taskgraph-6.0.0/requirements/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      179 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/requirements/base.in
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    20339 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/requirements/base.txt
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       22 2023-02-01 03:17:01.000000 taskcluster-taskgraph-6.0.0/requirements/dev.in
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1281 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.0.0/requirements/dev.txt
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       58 2023-02-01 03:17:01.000000 taskcluster-taskgraph-6.0.0/requirements/test.in
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     9241 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/requirements/test.txt
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       38 2023-07-25 19:06:11.724823 taskcluster-taskgraph-6.0.0/setup.cfg
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1555 2023-05-09 14:44:30.000000 taskcluster-taskgraph-6.0.0/setup.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.688823 taskcluster-taskgraph-6.0.0/src/
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.696823 taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      665 2023-07-25 19:06:11.000000 taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4054 2023-07-25 19:06:11.000000 taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)        1 2023-07-25 19:06:11.000000 taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       50 2023-07-25 19:06:11.000000 taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      203 2023-07-25 19:06:11.000000 taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/requires.txt
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       10 2023-07-25 19:06:11.000000 taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/top_level.txt
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.696823 taskcluster-taskgraph-6.0.0/src/taskgraph/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      729 2023-07-25 19:03:48.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/__init__.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.700823 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      416 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/__init__.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1836 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/add_new_jobs.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1309 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/cancel.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1941 2023-03-27 14:05:26.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/cancel_all.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1086 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/rebuild_cached_tasks.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    13122 2023-07-24 11:50:22.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/registry.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     9387 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/retrigger.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10661 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/util.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4822 2023-07-10 15:52:14.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/config.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5184 2023-03-27 14:05:26.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/create.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12882 2023-03-14 14:30:55.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/decision.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7834 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/docker.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2793 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/files_changed.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      866 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/filter_tasks.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    15667 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/generator.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4680 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/graph.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.700823 taskcluster-taskgraph-6.0.0/src/taskgraph/loader/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)        0 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/loader/__init__.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1185 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/loader/default.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2147 2023-03-28 13:22:32.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/loader/transform.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    26201 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/main.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     9192 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/morph.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.700823 taskcluster-taskgraph-6.0.0/src/taskgraph/optimize/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      123 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/optimize/__init__.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    18341 2023-05-29 20:22:45.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/optimize/base.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2380 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/optimize/strategies.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    11918 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/parameters.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.704823 taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/
+-rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)    29990 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/fetch-content
+-rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)      896 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/hgrc
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    30813 2023-07-07 15:10:12.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/robustcheckout.py
+-rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)    45128 2023-07-12 13:54:36.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/run-task
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3324 2023-02-24 14:13:32.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/target_tasks.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3240 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/task.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2434 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/taskgraph.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.704823 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      110 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/__init__.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5146 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/base.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2607 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/cached_tasks.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      707 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/code_review.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7606 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/docker_image.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10479 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/fetch.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6760 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/from_deps.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.704823 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    17324 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/__init__.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5897 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/common.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1220 2023-05-25 14:12:26.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/index_search.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8385 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/run_task.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6015 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/toolchain.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6019 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/notify.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    52254 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/task.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4272 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/task_context.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.712823 taskcluster-taskgraph-6.0.0/src/taskgraph/util/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)        0 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/__init__.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2855 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/archive.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2964 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/attributes.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3406 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/cached_tasks.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2433 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/decision.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2734 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/dependencies.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    11699 2023-07-24 11:50:22.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/docker.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1661 2023-02-01 03:17:01.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/hash.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3419 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/keyed_by.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1331 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/memoize.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3184 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/parameterization.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4466 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/path.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1576 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/python_path.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      787 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/readonlydict.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8323 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/schema.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1317 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/shell.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12445 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/taskcluster.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1969 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/taskgraph.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2139 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/templates.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3390 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/time.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2687 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/treeherder.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    18780 2023-07-07 15:10:12.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/vcs.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8947 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/verify.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2498 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/workertypes.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      990 2023-07-24 11:50:22.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/yaml.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.724823 taskcluster-taskgraph-6.0.0/test/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1584 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_actions_rebuild_cached_tasks.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1670 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_actions_registry.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3654 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_create.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7688 2023-03-14 14:30:55.000000 taskcluster-taskgraph-6.0.0/test/test_decision.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3505 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_files_changed.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8883 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/test/test_generator.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7063 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.0.0/test/test_graph.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7940 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.0.0/test/test_main.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2701 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_morph.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    15584 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.0.0/test/test_optimize.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1727 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_optimize_strategies.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    13921 2023-03-14 14:30:55.000000 taskcluster-taskgraph-6.0.0/test/test_parameters.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2491 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/test/test_scripts_fetch_content.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12257 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/test/test_scripts_run_task.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12046 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_target_tasks.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3759 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.0.0/test/test_taskgraph.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1812 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/test/test_transform_docker_image.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2716 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/test/test_transform_task_context.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      874 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_base.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1527 2023-05-02 13:16:10.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_fetch.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6985 2023-07-07 15:10:12.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_from_deps.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3798 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_job.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6157 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_job_run_task.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7131 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_job_toolchain.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6948 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_notify.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    25785 2023-07-10 15:52:14.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_task.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3596 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_attributes.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1120 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/test/test_util_dependencies.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10212 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_docker.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2340 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_memoize.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7556 2023-02-01 03:17:01.000000 taskcluster-taskgraph-6.0.0/test/test_util_parameterization.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5906 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_path.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1045 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_python_path.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1234 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_readonlydict.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6961 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_schema.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10115 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.0.0/test/test_util_taskcluster.py
+-rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)     1677 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_templates.py
+-rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)     2239 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_time.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      913 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_treeherder.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    15598 2023-07-07 15:10:12.000000 taskcluster-taskgraph-6.0.0/test/test_util_vcs.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4981 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_verify.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      942 2023-03-03 20:39:07.000000 taskcluster-taskgraph-6.0.0/test/test_util_workertypes.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1005 2023-07-24 11:50:22.000000 taskcluster-taskgraph-6.0.0/test/test_util_yaml.py
```

### Comparing `taskcluster-taskgraph-5.7.0/LICENSE` & `taskcluster-taskgraph-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/PKG-INFO` & `taskcluster-taskgraph-6.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.7.0
+Version: 6.0.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `taskcluster-taskgraph-5.7.0/README.rst` & `taskcluster-taskgraph-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/pyproject.toml` & `taskcluster-taskgraph-6.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/requirements/base.txt` & `taskcluster-taskgraph-6.0.0/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/requirements/dev.txt` & `taskcluster-taskgraph-6.0.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/requirements/test.txt` & `taskcluster-taskgraph-6.0.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/setup.py` & `taskcluster-taskgraph-6.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/PKG-INFO` & `taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.7.0
+Version: 6.0.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `taskcluster-taskgraph-5.7.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt` & `taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 src/taskgraph/transforms/cached_tasks.py
 src/taskgraph/transforms/code_review.py
 src/taskgraph/transforms/docker_image.py
 src/taskgraph/transforms/fetch.py
 src/taskgraph/transforms/from_deps.py
 src/taskgraph/transforms/notify.py
 src/taskgraph/transforms/task.py
+src/taskgraph/transforms/task_context.py
 src/taskgraph/transforms/job/__init__.py
 src/taskgraph/transforms/job/common.py
 src/taskgraph/transforms/job/index_search.py
 src/taskgraph/transforms/job/run_task.py
 src/taskgraph/transforms/job/toolchain.py
 src/taskgraph/util/__init__.py
 src/taskgraph/util/archive.py
@@ -100,14 +101,15 @@
 test/test_optimize_strategies.py
 test/test_parameters.py
 test/test_scripts_fetch_content.py
 test/test_scripts_run_task.py
 test/test_target_tasks.py
 test/test_taskgraph.py
 test/test_transform_docker_image.py
+test/test_transform_task_context.py
 test/test_transforms_base.py
 test/test_transforms_fetch.py
 test/test_transforms_from_deps.py
 test/test_transforms_job.py
 test/test_transforms_job_run_task.py
 test/test_transforms_job_toolchain.py
 test/test_transforms_notify.py
```

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/__init__.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-__version__ = "5.7.0"
+__version__ = "6.0.0"
 
 # Maximum number of dependencies a single task can have
 # https://docs.taskcluster.net/reference/platform/taskcluster-queue/references/api#createTask
 # specifies 100, but we also optionally add the decision task id as a dep in
 # taskgraph.create, so let's set this to 99.
 MAX_DEPENDENCIES = 99
```

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/actions/add_new_jobs.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/actions/add_new_jobs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/actions/cancel.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/actions/cancel.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/actions/cancel_all.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/actions/cancel_all.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/actions/rebuild_cached_tasks.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/actions/rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/actions/registry.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/actions/registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/actions/retrigger.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/actions/retrigger.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/actions/util.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/actions/util.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/config.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/create.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/decision.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/docker.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/files_changed.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/filter_tasks.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/filter_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/generator.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/graph.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/loader/default.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/loader/default.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/loader/transform.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/loader/transform.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/main.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/morph.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/optimize/base.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/optimize/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/optimize/strategies.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/optimize/strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/parameters.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/fetch-content` & `taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/fetch-content`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/hgrc` & `taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/hgrc`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/robustcheckout.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/robustcheckout.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/run-task/run-task` & `taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/run-task`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/target_tasks.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/task.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/taskgraph.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/base.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/cached_tasks.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/code_review.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/code_review.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/docker_image.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/fetch.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/from_deps.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/from_deps.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from textwrap import dedent
 
 from voluptuous import Any, Extra, Optional, Required
 
 from taskgraph.transforms.base import TransformSequence
 from taskgraph.util.attributes import attrmatch
 from taskgraph.util.dependencies import GROUP_BY_MAP
-from taskgraph.util.schema import Schema
+from taskgraph.util.schema import Schema, validate_schema
 
 FROM_DEPS_SCHEMA = Schema(
     {
         Required("from-deps"): {
             Optional(
                 "kinds",
                 description=dedent(
@@ -135,15 +135,17 @@
         groups = set()
 
         if isinstance(group_by, dict):
             assert len(group_by) == 1
             group_by, arg = group_by.popitem()
             func = GROUP_BY_MAP[group_by]
             if func.schema:
-                func.schema(arg)
+                validate_schema(
+                    func.schema, arg, f"Invalid group-by {group_by} argument"
+                )
             groups = func(config, deps, arg)
         else:
             func = GROUP_BY_MAP[group_by]
             groups = func(config, deps)
 
         # Split the task, one per group.
         copy_attributes = from_deps.get("copy-attributes", False)
```

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/__init__.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/common.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/common.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/index_search.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/index_search.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/run_task.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/run_task.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 """
 Support for running jobs that are invoked via the `run-task` script.
 """
 
 import dataclasses
 import os
 
-from voluptuous import Any, Extra, Optional, Required
+from voluptuous import Any, Optional, Required
 
 from taskgraph.transforms.job import run_job_using
 from taskgraph.transforms.job.common import support_vcs_checkout
 from taskgraph.transforms.task import taskref_or_string
 from taskgraph.util import path, taskcluster
 from taskgraph.util.schema import Schema
-from taskgraph.util.yaml import load_yaml
 
 EXEC_COMMANDS = {
     "bash": ["bash", "-cx"],
     "powershell": ["powershell.exe", "-ExecutionPolicy", "Bypass"],
 }
 
 run_task_schema = Schema(
@@ -42,24 +41,14 @@
         # directory where sparse profiles are defined (build/sparse-profiles/).
         Required("sparse-profile"): Any(str, None),
         # The command arguments to pass to the `run-task` script, after the
         # checkout arguments.  If a list, it will be passed directly; otherwise
         # it will be included in a single argument to the command specified by
         # `exec-with`.
         Required("command"): Any([taskref_or_string], taskref_or_string),
-        # Context to substitute into the command using format string
-        # substitution (e.g {value}). This is useful if certain aspects of the
-        # command need to be generated in transforms.
-        Optional("command-context"): {
-            # If present, loads a set of context variables from an unnested yaml
-            # file. If a value is present in both the provided file and directly
-            # in command-context, the latter will take priority.
-            Optional("from-file"): str,
-            Extra: object,
-        },
         # What to execute the command with in the event command is a string.
         Optional("exec-with"): Any(*list(EXEC_COMMANDS)),
         # Command used to invoke the `run-task` script. Can be used if the script
         # or Python installation is in a non-standard location on the workers.
         Optional("run-task-command"): list,
         # Base work directory used to set up the task.
         Required("workdir"): str,
@@ -133,33 +122,14 @@
     # use_proxy = False to avoid having all generic-workers turn on proxy
     # Assumes the cluster allows anonymous downloads of public artifacts
     tc_url = taskcluster.get_root_url(False)
     # TODO: Use util/taskcluster.py:get_artifact_url once hack for Bug 1405889 is removed
     return f"{tc_url}/api/queue/v1/task/{task_id}/artifacts/public/{script}"
 
 
-def substitute_command_context(command_context, command):
-    from_file = command_context.pop("from-file", None)
-    full_context = {}
-    if from_file:
-        full_context = load_yaml(from_file)
-    else:
-        full_context = {}
-
-    full_context.update(command_context)
-
-    if isinstance(command, list):
-        for i in range(len(command)):
-            command[i] = command[i].format(**full_context)
-    else:
-        command = command.format(**full_context)
-
-    return command
-
-
 @run_job_using(
     "docker-worker", "run-task", schema=run_task_schema, defaults=worker_defaults
 )
 def docker_worker_run_task(config, job, taskdesc):
     run = job["run"]
     worker = taskdesc["worker"] = job["worker"]
     command = run.pop("run-task-command", ["/usr/local/bin/run-task"])
@@ -173,21 +143,14 @@
                 "mount-point": "{workdir}/.cache".format(**run),
                 "skip-untrusted": True,
             }
         )
 
     run_command = run["command"]
 
-    if run.get("command-context"):
-        run_command = substitute_command_context(
-            run.get("command-context"), run["command"]
-        )
-    else:
-        run_command = run["command"]
-
     # dict is for the case of `{'task-reference': str}`.
     if isinstance(run_command, str) or isinstance(run_command, dict):
         exec_cmd = EXEC_COMMANDS[run.pop("exec-with", "bash")]
         run_command = exec_cmd + [run_command]
     if run["run-as-root"]:
         command.extend(("--user", "root", "--group", "root"))
     command.append("--")
@@ -246,19 +209,14 @@
 
     if isinstance(run_command, str):
         if is_win:
             run_command = f'"{run_command}"'
         exec_cmd = EXEC_COMMANDS[run.pop("exec-with", "bash")]
         run_command = exec_cmd + [run_command]
 
-    if run.get("command-context"):
-        run_command = substitute_command_context(
-            run.get("command-context"), run_command
-        )
-
     if run["run-as-root"]:
         command.extend(("--user", "root", "--group", "root"))
     command.append("--")
     if is_bitbar:
         # Use the bitbar wrapper script which sets up the device and adb
         # environment variables
         command.append("/builds/taskcluster/script.py")
```

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/job/toolchain.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/notify.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/transforms/task.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/archive.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/attributes.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/cached_tasks.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/decision.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/dependencies.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/dependencies.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 # Define a collection of group_by functions
 GROUP_BY_MAP = {}
 
 
 def group_by(name, schema=None):
     def wrapper(func):
+        assert (
+            name not in GROUP_BY_MAP
+        ), f"duplicate group_by function name {name} ({func} and {GROUP_BY_MAP[name]})"
         GROUP_BY_MAP[name] = func
         func.schema = schema
         return func
 
     return wrapper
```

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/docker.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/hash.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/hash.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/keyed_by.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/keyed_by.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/memoize.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/parameterization.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/path.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/python_path.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/readonlydict.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/schema.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/shell.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/shell.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/taskcluster.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/taskgraph.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/templates.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/templates.py`

 * *Files 24% similar despite different names*

```diff
@@ -44,7 +44,37 @@
     perspective, "parents" should be listed before "children".
 
     Returns the result without modifying any arguments.
     """
     if len(objects) == 1:
         return copy.deepcopy(objects[0])
     return merge_to(objects[-1], merge(*objects[:-1]))
+
+
+def deep_get(dict_, field):
+    container, subfield = dict_, field
+    while "." in subfield:
+        f, subfield = subfield.split(".", 1)
+        if f not in container:
+            return None
+
+        container = container[f]
+
+    return container.get(subfield)
+
+
+def substitute(item, **subs):
+    if isinstance(item, list):
+        for i in range(len(item)):
+            item[i] = substitute(item[i], **subs)
+    elif isinstance(item, dict):
+        new_dict = {}
+        for k, v in item.items():
+            k = k.format(**subs)
+            new_dict[k] = substitute(v, **subs)
+        item = new_dict
+    elif isinstance(item, str):
+        item = item.format(**subs)
+    else:
+        item = item
+
+    return item
```

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/time.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/treeherder.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/vcs.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/verify.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/workertypes.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/src/taskgraph/util/yaml.py` & `taskcluster-taskgraph-6.0.0/src/taskgraph/util/yaml.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_actions_rebuild_cached_tasks.py` & `taskcluster-taskgraph-6.0.0/test/test_actions_rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_actions_registry.py` & `taskcluster-taskgraph-6.0.0/test/test_actions_registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_create.py` & `taskcluster-taskgraph-6.0.0/test/test_create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_decision.py` & `taskcluster-taskgraph-6.0.0/test/test_decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_files_changed.py` & `taskcluster-taskgraph-6.0.0/test/test_files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_generator.py` & `taskcluster-taskgraph-6.0.0/test/test_generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_graph.py` & `taskcluster-taskgraph-6.0.0/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_main.py` & `taskcluster-taskgraph-6.0.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_morph.py` & `taskcluster-taskgraph-6.0.0/test/test_morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_optimize.py` & `taskcluster-taskgraph-6.0.0/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_optimize_strategies.py` & `taskcluster-taskgraph-6.0.0/test/test_optimize_strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_parameters.py` & `taskcluster-taskgraph-6.0.0/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_scripts_fetch_content.py` & `taskcluster-taskgraph-6.0.0/test/test_scripts_fetch_content.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_scripts_run_task.py` & `taskcluster-taskgraph-6.0.0/test/test_scripts_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_target_tasks.py` & `taskcluster-taskgraph-6.0.0/test/test_target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_taskgraph.py` & `taskcluster-taskgraph-6.0.0/test/test_taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_transform_docker_image.py` & `taskcluster-taskgraph-6.0.0/test/test_transform_docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_transforms_base.py` & `taskcluster-taskgraph-6.0.0/test/test_transforms_base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_transforms_fetch.py` & `taskcluster-taskgraph-6.0.0/test/test_transforms_fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_transforms_from_deps.py` & `taskcluster-taskgraph-6.0.0/test/test_transforms_from_deps.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_transforms_job.py` & `taskcluster-taskgraph-6.0.0/test/test_transforms_job.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,23 +10,20 @@
 from copy import deepcopy
 from pprint import pprint
 from unittest.mock import patch
 
 import pytest
 
 # prevent pytest thinking this is a test
-from taskcluster_urls import test_root_url as _test_root_url
-
 from taskgraph.task import Task
 from taskgraph.transforms import job
 from taskgraph.transforms.job import run_task  # noqa: F401
 from taskgraph.transforms.job.common import add_cache
 from taskgraph.transforms.task import payload_builders
 from taskgraph.util.schema import Schema, validate_schema
-from taskgraph.util.taskcluster import get_root_url
 from taskgraph.util.templates import merge
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 TASK_DEFAULTS = {
     "description": "fake description",
@@ -84,58 +81,14 @@
     assert len(taskdesc["worker"][key]) == 2
 
     # Create a new schema object with just the part relevant to caches.
     partial_schema = Schema(payload_builders[impl].schema.schema[key])
     validate_schema(partial_schema, taskdesc["worker"][key], "validation error")
 
 
-@pytest.mark.parametrize(
-    "workerfn", [fn for fn, *_ in job.registry["run-task"].values()]
-)
-@pytest.mark.parametrize(
-    "task",
-    (
-        {
-            "worker-type": "t-linux",
-            "run": {
-                "checkout": True,
-                "comm-checkout": False,
-                "command": "echo '{output}'",
-                "command-context": {"output": "hello", "extra": None},
-                "run-as-root": False,
-                "sparse-profile": False,
-                "tooltool-downloads": False,
-            },
-        },
-    ),
-)
-def test_run_task_command_context(task, transform, workerfn, monkeypatch):
-    if "TASKCLUSTER_ROOT_URL" not in os.environ:
-        monkeypatch.setenv("TASKCLUSTER_ROOT_URL", _test_root_url())
-    # Clear memoized function
-    get_root_url.clear()
-
-    config, job_, taskdesc, _ = transform(task)
-    job_ = deepcopy(job_)
-
-    def assert_cmd(expected):
-        cmd = taskdesc["worker"]["command"]
-        while isinstance(cmd, list):
-            cmd = cmd[-1]
-        assert cmd == expected
-
-    workerfn(config, job_, taskdesc)
-    assert_cmd("echo 'hello'")
-
-    job_copy = job_.copy()
-    del job_copy["run"]["command-context"]
-    workerfn(config, job_copy, taskdesc)
-    assert_cmd("echo '{output}'")
-
-
 def assert_use_fetches_toolchain_env(task):
     assert task["worker"]["env"]["FOO"] == "1"
 
 
 @pytest.mark.parametrize(
     "task,kind_dependencies_tasks",
     (
```

### Comparing `taskcluster-taskgraph-5.7.0/test/test_transforms_job_run_task.py` & `taskcluster-taskgraph-6.0.0/test/test_transforms_job_run_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,15 @@
     "label": "fake-task-label",
     "worker-type": "t-linux",
     "worker": {
         "implementation": "docker-worker",
         "os": "linux",
         "env": {},
     },
-    "run": {
-        "using": "run-task",
-        "command": "echo hello {extra_string}",
-        "command-context": {
-            "from-file": f"{here}/data/command_context.yaml",
-        },
-    },
+    "run": {"using": "run-task", "command": "echo hello world"},
 }
 
 
 @pytest.fixture
 def run_job_using(mocker, run_transform):
     m = mocker.patch("taskgraph.util.hash._get_all_files")
     m.return_value = [
```

### Comparing `taskcluster-taskgraph-5.7.0/test/test_transforms_job_toolchain.py` & `taskcluster-taskgraph-6.0.0/test/test_transforms_job_toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_transforms_notify.py` & `taskcluster-taskgraph-6.0.0/test/test_transforms_notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_transforms_task.py` & `taskcluster-taskgraph-6.0.0/test/test_transforms_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_attributes.py` & `taskcluster-taskgraph-6.0.0/test/test_util_attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_dependencies.py` & `taskcluster-taskgraph-6.0.0/test/test_util_dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_docker.py` & `taskcluster-taskgraph-6.0.0/test/test_util_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_memoize.py` & `taskcluster-taskgraph-6.0.0/test/test_util_memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_parameterization.py` & `taskcluster-taskgraph-6.0.0/test/test_util_parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_path.py` & `taskcluster-taskgraph-6.0.0/test/test_util_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_python_path.py` & `taskcluster-taskgraph-6.0.0/test/test_util_python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_readonlydict.py` & `taskcluster-taskgraph-6.0.0/test/test_util_readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_schema.py` & `taskcluster-taskgraph-6.0.0/test/test_util_schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_taskcluster.py` & `taskcluster-taskgraph-6.0.0/test/test_util_taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_templates.py` & `taskcluster-taskgraph-6.0.0/test/test_util_templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_time.py` & `taskcluster-taskgraph-6.0.0/test/test_util_time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_treeherder.py` & `taskcluster-taskgraph-6.0.0/test/test_util_treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_vcs.py` & `taskcluster-taskgraph-6.0.0/test/test_util_vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_verify.py` & `taskcluster-taskgraph-6.0.0/test/test_util_verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_workertypes.py` & `taskcluster-taskgraph-6.0.0/test/test_util_workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.7.0/test/test_util_yaml.py` & `taskcluster-taskgraph-6.0.0/test/test_util_yaml.py`

 * *Files identical despite different names*

