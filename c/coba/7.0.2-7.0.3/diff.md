# Comparing `tmp/coba-7.0.2.tar.gz` & `tmp/coba-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coba-7.0.2.tar", last modified: Thu Jul 20 20:24:30 2023, max compression
+gzip compressed data, was "coba-7.0.3.tar", last modified: Tue Jul 25 03:34:38 2023, max compression
```

## Comparing `coba-7.0.2.tar` & `coba-7.0.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 20:24:30.560417 coba-7.0.2/
--rw-rw-rw-   0        0        0       40 2023-06-12 16:34:36.000000 coba-7.0.2/AUTHORS
--rw-rw-rw-   0        0        0     1593 2023-06-12 16:34:36.000000 coba-7.0.2/LICENSE
--rw-rw-rw-   0        0        0     7942 2023-07-20 20:24:30.560417 coba-7.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     7327 2023-06-16 20:10:41.000000 coba-7.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 20:24:28.418340 coba-7.0.2/coba/
--rw-rw-rw-   0        0        0     1378 2023-07-20 19:07:08.000000 coba-7.0.2/coba/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 20:24:28.598720 coba-7.0.2/coba/backports/
--rw-rw-rw-   0        0        0       50 2023-07-20 03:01:25.000000 coba-7.0.2/coba/backports/__init__.py
--rw-rw-rw-   0        0        0      262 2023-07-20 02:54:01.000000 coba-7.0.2/coba/backports/metadata.py
-drwxrwxrwx   0        0        0        0 2023-07-20 20:24:28.749217 coba-7.0.2/coba/contexts/
--rw-rw-rw-   0        0        0      703 2023-06-22 17:38:27.000000 coba-7.0.2/coba/contexts/__init__.py
--rw-rw-rw-   0        0        0     9727 2023-06-12 16:34:36.000000 coba-7.0.2/coba/contexts/cachers.py
--rw-rw-rw-   0        0        0     9236 2023-07-20 02:56:24.000000 coba-7.0.2/coba/contexts/core.py
--rw-rw-rw-   0        0        0     9726 2023-06-12 16:34:36.000000 coba-7.0.2/coba/contexts/loggers.py
--rw-rw-rw-   0        0        0    15875 2023-07-20 03:19:10.000000 coba-7.0.2/coba/encodings.py
-drwxrwxrwx   0        0        0        0 2023-07-20 20:24:29.524775 coba-7.0.2/coba/environments/
--rw-rw-rw-   0        0        0     1448 2023-07-16 19:49:49.000000 coba-7.0.2/coba/environments/__init__.py
--rw-rw-rw-   0        0        0    22841 2023-07-20 03:16:24.000000 coba-7.0.2/coba/environments/core.py
--rw-rw-rw-   0        0        0    52590 2023-07-20 07:40:57.000000 coba-7.0.2/coba/environments/filters.py
--rw-rw-rw-   0        0        0    14347 2023-07-16 19:49:49.000000 coba-7.0.2/coba/environments/openml.py
--rw-rw-rw-   0        0        0     7646 2023-07-16 19:49:49.000000 coba-7.0.2/coba/environments/primitives.py
--rw-rw-rw-   0        0        0     2966 2023-07-16 19:49:49.000000 coba-7.0.2/coba/environments/serialized.py
--rw-rw-rw-   0        0        0     9524 2023-07-20 02:57:00.000000 coba-7.0.2/coba/environments/supervised.py
--rw-rw-rw-   0        0        0    24174 2023-07-20 02:57:08.000000 coba-7.0.2/coba/environments/synthetics.py
--rw-rw-rw-   0        0        0     6179 2023-06-12 16:34:36.000000 coba-7.0.2/coba/environments/templates.py
-drwxrwxrwx   0        0        0        0 2023-07-20 20:24:29.681247 coba-7.0.2/coba/evaluators/
--rw-rw-rw-   0        0        0      217 2023-06-24 23:45:33.000000 coba-7.0.2/coba/evaluators/__init__.py
--rw-rw-rw-   0        0        0    15064 2023-07-20 07:42:27.000000 coba-7.0.2/coba/evaluators/offline.py
--rw-rw-rw-   0        0        0    22406 2023-07-20 19:01:31.000000 coba-7.0.2/coba/evaluators/online.py
--rw-rw-rw-   0        0        0     2095 2023-07-16 19:49:49.000000 coba-7.0.2/coba/evaluators/primitives.py
--rw-rw-rw-   0        0        0     1126 2023-06-12 16:34:36.000000 coba-7.0.2/coba/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-20 20:24:29.869457 coba-7.0.2/coba/experiments/
--rw-rw-rw-   0        0        0      379 2023-06-22 17:38:27.000000 coba-7.0.2/coba/experiments/__init__.py
--rw-rw-rw-   0        0        0    10512 2023-07-16 19:49:49.000000 coba-7.0.2/coba/experiments/core.py
--rw-rw-rw-   0        0        0     7686 2023-07-16 19:49:49.000000 coba-7.0.2/coba/experiments/process.py
--rw-rw-rw-   0        0        0    65241 2023-07-20 02:57:27.000000 coba-7.0.2/coba/experiments/results.py
-drwxrwxrwx   0        0        0        0 2023-07-20 20:24:30.165037 coba-7.0.2/coba/learners/
--rw-rw-rw-   0        0        0      761 2023-07-16 19:49:49.000000 coba-7.0.2/coba/learners/__init__.py
--rw-rw-rw-   0        0        0     7907 2023-06-24 23:48:29.000000 coba-7.0.2/coba/learners/bandit.py
--rw-rw-rw-   0        0        0     8028 2023-07-20 02:57:43.000000 coba-7.0.2/coba/learners/corral.py
--rw-rw-rw-   0        0        0     4947 2023-06-23 09:01:59.000000 coba-7.0.2/coba/learners/linucb.py
--rw-rw-rw-   0        0        0      958 2023-07-16 19:49:49.000000 coba-7.0.2/coba/learners/misguided.py
--rw-rw-rw-   0        0        0     4376 2023-06-12 16:34:36.000000 coba-7.0.2/coba/learners/primitives.py
--rw-rw-rw-   0        0        0     8887 2023-07-20 08:32:14.000000 coba-7.0.2/coba/learners/safety.py
--rw-rw-rw-   0        0        0    30984 2023-07-20 02:58:04.000000 coba-7.0.2/coba/learners/vowpal.py
--rw-rw-rw-   0        0        0     4139 2023-07-16 19:49:49.000000 coba-7.0.2/coba/multiprocessing.py
-drwxrwxrwx   0        0        0        0 2023-07-20 20:24:30.434702 coba-7.0.2/coba/pipes/
--rw-rw-rw-   0        0        0     1456 2023-07-16 19:49:49.000000 coba-7.0.2/coba/pipes/__init__.py
--rw-rw-rw-   0        0        0     1890 2023-06-12 16:34:36.000000 coba-7.0.2/coba/pipes/core.py
--rw-rw-rw-   0        0        0    16751 2023-07-16 19:49:49.000000 coba-7.0.2/coba/pipes/filters.py
--rw-rw-rw-   0        0        0    16062 2023-07-20 05:27:58.000000 coba-7.0.2/coba/pipes/multiprocessing.py
--rw-rw-rw-   0        0        0     6622 2023-06-12 16:34:36.000000 coba-7.0.2/coba/pipes/primitives.py
--rw-rw-rw-   0        0        0    13003 2023-06-12 16:34:36.000000 coba-7.0.2/coba/pipes/readers.py
--rw-rw-rw-   0        0        0    19458 2023-07-20 02:58:18.000000 coba-7.0.2/coba/pipes/rows.py
--rw-rw-rw-   0        0        0     4474 2023-07-16 19:49:49.000000 coba-7.0.2/coba/pipes/sinks.py
--rw-rw-rw-   0        0        0     6483 2023-07-20 02:58:25.000000 coba-7.0.2/coba/pipes/sources.py
-drwxrwxrwx   0        0        0        0 2023-07-20 20:24:30.560417 coba-7.0.2/coba/primitives/
--rw-rw-rw-   0        0        0      477 2023-06-22 17:38:27.000000 coba-7.0.2/coba/primitives/__init__.py
--rw-rw-rw-   0        0        0      913 2023-06-16 20:10:41.000000 coba-7.0.2/coba/primitives/feedbacks.py
--rw-rw-rw-   0        0        0     4624 2023-07-20 08:45:03.000000 coba-7.0.2/coba/primitives/rewards.py
--rw-rw-rw-   0        0        0     4421 2023-07-16 19:49:49.000000 coba-7.0.2/coba/primitives/rows.py
--rw-rw-rw-   0        0        0      219 2023-07-19 06:20:25.000000 coba-7.0.2/coba/primitives/semantic.py
--rw-rw-rw-   0        0        0      657 2023-06-12 16:34:36.000000 coba-7.0.2/coba/primitives/types.py
--rw-rw-rw-   0        0        0    11151 2023-07-16 18:38:46.000000 coba-7.0.2/coba/random.py
--rw-rw-rw-   0        0        0     1479 2023-07-16 19:49:49.000000 coba-7.0.2/coba/register.py
--rw-rw-rw-   0        0        0    10657 2023-06-12 16:34:36.000000 coba-7.0.2/coba/registry.py
--rw-rw-rw-   0        0        0     9022 2023-07-20 02:56:10.000000 coba-7.0.2/coba/statistics.py
--rw-rw-rw-   0        0        0     5212 2023-06-12 16:34:36.000000 coba-7.0.2/coba/utilities.py
-drwxrwxrwx   0        0        0        0 2023-07-20 20:24:28.557866 coba-7.0.2/coba.egg-info/
--rw-rw-rw-   0        0        0     7942 2023-07-20 20:24:28.000000 coba-7.0.2/coba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1583 2023-07-20 20:24:28.000000 coba-7.0.2/coba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 20:24:28.000000 coba-7.0.2/coba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-20 20:24:28.000000 coba-7.0.2/coba.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2023-07-20 20:24:28.000000 coba-7.0.2/coba.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-20 20:24:28.000000 coba-7.0.2/coba.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1194 2023-07-20 03:21:22.000000 coba-7.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 20:24:30.560417 coba-7.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.556975 coba-7.0.3/
+-rw-rw-rw-   0        0        0       40 2023-06-12 16:34:36.000000 coba-7.0.3/AUTHORS
+-rw-rw-rw-   0        0        0     1593 2023-06-12 16:34:36.000000 coba-7.0.3/LICENSE
+-rw-rw-rw-   0        0        0     7942 2023-07-25 03:34:38.556975 coba-7.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7327 2023-06-16 20:10:41.000000 coba-7.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.006947 coba-7.0.3/coba/
+-rw-rw-rw-   0        0        0     1427 2023-07-25 02:03:33.000000 coba-7.0.3/coba/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.069639 coba-7.0.3/coba/backports/
+-rw-rw-rw-   0        0        0       50 2023-07-20 03:01:25.000000 coba-7.0.3/coba/backports/__init__.py
+-rw-rw-rw-   0        0        0      262 2023-07-20 02:54:01.000000 coba-7.0.3/coba/backports/metadata.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.096052 coba-7.0.3/coba/contexts/
+-rw-rw-rw-   0        0        0      703 2023-06-22 17:38:27.000000 coba-7.0.3/coba/contexts/__init__.py
+-rw-rw-rw-   0        0        0     9727 2023-06-12 16:34:36.000000 coba-7.0.3/coba/contexts/cachers.py
+-rw-rw-rw-   0        0        0     9236 2023-07-20 02:56:24.000000 coba-7.0.3/coba/contexts/core.py
+-rw-rw-rw-   0        0        0     9726 2023-06-12 16:34:36.000000 coba-7.0.3/coba/contexts/loggers.py
+-rw-rw-rw-   0        0        0    15875 2023-07-20 03:19:10.000000 coba-7.0.3/coba/encodings.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.211009 coba-7.0.3/coba/environments/
+-rw-rw-rw-   0        0        0     1448 2023-07-16 19:49:49.000000 coba-7.0.3/coba/environments/__init__.py
+-rw-rw-rw-   0        0        0    22841 2023-07-20 03:16:24.000000 coba-7.0.3/coba/environments/core.py
+-rw-rw-rw-   0        0        0    52650 2023-07-25 01:55:42.000000 coba-7.0.3/coba/environments/filters.py
+-rw-rw-rw-   0        0        0    14347 2023-07-16 19:49:49.000000 coba-7.0.3/coba/environments/openml.py
+-rw-rw-rw-   0        0        0     7646 2023-07-16 19:49:49.000000 coba-7.0.3/coba/environments/primitives.py
+-rw-rw-rw-   0        0        0     2966 2023-07-16 19:49:49.000000 coba-7.0.3/coba/environments/serialized.py
+-rw-rw-rw-   0        0        0     9524 2023-07-20 02:57:00.000000 coba-7.0.3/coba/environments/supervised.py
+-rw-rw-rw-   0        0        0    24174 2023-07-20 02:57:08.000000 coba-7.0.3/coba/environments/synthetics.py
+-rw-rw-rw-   0        0        0     6179 2023-06-12 16:34:36.000000 coba-7.0.3/coba/environments/templates.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.258300 coba-7.0.3/coba/evaluators/
+-rw-rw-rw-   0        0        0      217 2023-06-24 23:45:33.000000 coba-7.0.3/coba/evaluators/__init__.py
+-rw-rw-rw-   0        0        0    15064 2023-07-20 07:42:27.000000 coba-7.0.3/coba/evaluators/offline.py
+-rw-rw-rw-   0        0        0    22406 2023-07-20 19:01:31.000000 coba-7.0.3/coba/evaluators/online.py
+-rw-rw-rw-   0        0        0     2095 2023-07-16 19:49:49.000000 coba-7.0.3/coba/evaluators/primitives.py
+-rw-rw-rw-   0        0        0     1126 2023-06-12 16:34:36.000000 coba-7.0.3/coba/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.289549 coba-7.0.3/coba/experiments/
+-rw-rw-rw-   0        0        0      379 2023-06-22 17:38:27.000000 coba-7.0.3/coba/experiments/__init__.py
+-rw-rw-rw-   0        0        0    10512 2023-07-16 19:49:49.000000 coba-7.0.3/coba/experiments/core.py
+-rw-rw-rw-   0        0        0     7686 2023-07-16 19:49:49.000000 coba-7.0.3/coba/experiments/process.py
+-rw-rw-rw-   0        0        0    65589 2023-07-25 03:02:35.000000 coba-7.0.3/coba/experiments/results.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.383751 coba-7.0.3/coba/learners/
+-rw-rw-rw-   0        0        0      761 2023-07-16 19:49:49.000000 coba-7.0.3/coba/learners/__init__.py
+-rw-rw-rw-   0        0        0     7907 2023-07-23 04:42:34.000000 coba-7.0.3/coba/learners/bandit.py
+-rw-rw-rw-   0        0        0     8028 2023-07-23 04:42:34.000000 coba-7.0.3/coba/learners/corral.py
+-rw-rw-rw-   0        0        0     4947 2023-06-23 09:01:59.000000 coba-7.0.3/coba/learners/linucb.py
+-rw-rw-rw-   0        0        0      958 2023-07-16 19:49:49.000000 coba-7.0.3/coba/learners/misguided.py
+-rw-rw-rw-   0        0        0     4376 2023-06-12 16:34:36.000000 coba-7.0.3/coba/learners/primitives.py
+-rw-rw-rw-   0        0        0     8975 2023-07-21 04:36:06.000000 coba-7.0.3/coba/learners/safety.py
+-rw-rw-rw-   0        0        0    30984 2023-07-23 04:42:34.000000 coba-7.0.3/coba/learners/vowpal.py
+-rw-rw-rw-   0        0        0     4139 2023-07-16 19:49:49.000000 coba-7.0.3/coba/multiprocessing.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.462605 coba-7.0.3/coba/pipes/
+-rw-rw-rw-   0        0        0     1456 2023-07-16 19:49:49.000000 coba-7.0.3/coba/pipes/__init__.py
+-rw-rw-rw-   0        0        0     1890 2023-06-12 16:34:36.000000 coba-7.0.3/coba/pipes/core.py
+-rw-rw-rw-   0        0        0    16751 2023-07-16 19:49:49.000000 coba-7.0.3/coba/pipes/filters.py
+-rw-rw-rw-   0        0        0    16062 2023-07-20 05:27:58.000000 coba-7.0.3/coba/pipes/multiprocessing.py
+-rw-rw-rw-   0        0        0     6622 2023-06-12 16:34:36.000000 coba-7.0.3/coba/pipes/primitives.py
+-rw-rw-rw-   0        0        0    13003 2023-06-12 16:34:36.000000 coba-7.0.3/coba/pipes/readers.py
+-rw-rw-rw-   0        0        0    19458 2023-07-20 02:58:18.000000 coba-7.0.3/coba/pipes/rows.py
+-rw-rw-rw-   0        0        0     4474 2023-07-16 19:49:49.000000 coba-7.0.3/coba/pipes/sinks.py
+-rw-rw-rw-   0        0        0     6483 2023-07-20 02:58:25.000000 coba-7.0.3/coba/pipes/sources.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.556975 coba-7.0.3/coba/primitives/
+-rw-rw-rw-   0        0        0      477 2023-06-22 17:38:27.000000 coba-7.0.3/coba/primitives/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-06-16 20:10:41.000000 coba-7.0.3/coba/primitives/feedbacks.py
+-rw-rw-rw-   0        0        0     4624 2023-07-20 08:45:03.000000 coba-7.0.3/coba/primitives/rewards.py
+-rw-rw-rw-   0        0        0     4421 2023-07-16 19:49:49.000000 coba-7.0.3/coba/primitives/rows.py
+-rw-rw-rw-   0        0        0      219 2023-07-19 06:20:25.000000 coba-7.0.3/coba/primitives/semantic.py
+-rw-rw-rw-   0        0        0      657 2023-06-12 16:34:36.000000 coba-7.0.3/coba/primitives/types.py
+-rw-rw-rw-   0        0        0    11151 2023-07-16 18:38:46.000000 coba-7.0.3/coba/random.py
+-rw-rw-rw-   0        0        0     1479 2023-07-16 19:49:49.000000 coba-7.0.3/coba/register.py
+-rw-rw-rw-   0        0        0    10657 2023-06-12 16:34:36.000000 coba-7.0.3/coba/registry.py
+-rw-rw-rw-   0        0        0     9022 2023-07-20 02:56:10.000000 coba-7.0.3/coba/statistics.py
+-rw-rw-rw-   0        0        0     5212 2023-06-12 16:34:36.000000 coba-7.0.3/coba/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:34:38.054637 coba-7.0.3/coba.egg-info/
+-rw-rw-rw-   0        0        0     7942 2023-07-25 03:34:37.000000 coba-7.0.3/coba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1583 2023-07-25 03:34:37.000000 coba-7.0.3/coba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 03:34:37.000000 coba-7.0.3/coba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-25 03:34:37.000000 coba-7.0.3/coba.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2023-07-25 03:34:37.000000 coba-7.0.3/coba.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-25 03:34:37.000000 coba-7.0.3/coba.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1194 2023-07-20 03:21:22.000000 coba-7.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 03:34:38.556975 coba-7.0.3/setup.cfg
```

### Comparing `coba-7.0.2/LICENSE` & `coba-7.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/PKG-INFO` & `coba-7.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coba
-Version: 7.0.2
+Version: 7.0.3
 Summary: A contextual bandit research package
 Author-email: Mark Rucker <rucker.mark@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/vowpalwabbit/coba
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `coba-7.0.2/README.md` & `coba-7.0.3/README.md`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/__init__.py` & `coba-7.0.3/coba/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,8 +20,10 @@
 from coba.utilities import peek_first
 from coba.exceptions import CobaException
 
 from coba.primitives.semantic import Batch
 from coba.primitives.rewards import L1Reward, HammingReward, BinaryReward, IPSReward
 from coba.primitives.rewards import SequenceReward, MappingReward, MulticlassReward, BatchReward
 
-__version__ = "7.0.2"
+from coba.statistics import BootstrapCI, mean
+
+__version__ = "7.0.3"
```

### Comparing `coba-7.0.2/coba/contexts/__init__.py` & `coba-7.0.3/coba/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/contexts/cachers.py` & `coba-7.0.3/coba/contexts/cachers.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/contexts/core.py` & `coba-7.0.3/coba/contexts/core.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/contexts/loggers.py` & `coba-7.0.3/coba/contexts/loggers.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/encodings.py` & `coba-7.0.3/coba/encodings.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/environments/__init__.py` & `coba-7.0.3/coba/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/environments/core.py` & `coba-7.0.3/coba/environments/core.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/environments/filters.py` & `coba-7.0.3/coba/environments/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1161,15 +1161,16 @@
 
     def __init__(self, learner: Learner, seed: Optional[float] = 1.23) -> None:
         self._learner = learner
         self._seed    = seed
 
     @property
     def params(self) -> Mapping[str, Any]:
-        return {"learner": SafeLearner(self._learner).params, "logged":True, "log_seed":self._seed}
+        learner_params = SafeLearner(self._learner).params
+        return { **learner_params, "learner": learner_params, "logged":True, "log_seed":self._seed}
 
     def filter(self, interactions: Iterable[Interaction]) -> Iterable[Interaction]:
 
         first, interactions = peek_first(interactions)
 
         if not interactions: return []
```

### Comparing `coba-7.0.2/coba/environments/openml.py` & `coba-7.0.3/coba/environments/openml.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/environments/primitives.py` & `coba-7.0.3/coba/environments/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/environments/serialized.py` & `coba-7.0.3/coba/environments/serialized.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/environments/supervised.py` & `coba-7.0.3/coba/environments/supervised.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/environments/synthetics.py` & `coba-7.0.3/coba/environments/synthetics.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/environments/templates.py` & `coba-7.0.3/coba/environments/templates.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/evaluators/offline.py` & `coba-7.0.3/coba/evaluators/offline.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/evaluators/online.py` & `coba-7.0.3/coba/evaluators/online.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/evaluators/primitives.py` & `coba-7.0.3/coba/evaluators/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/exceptions.py` & `coba-7.0.3/coba/exceptions.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/experiments/core.py` & `coba-7.0.3/coba/experiments/core.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/experiments/process.py` & `coba-7.0.3/coba/experiments/process.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/experiments/results.py` & `coba-7.0.3/coba/experiments/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1036,15 +1036,15 @@
         """
         try:
             xlim = xlim or [None,None]
             ylim = ylim or [None,None]
 
             if isinstance(labels,str): labels = [labels]
 
-            plottable = self._plottable(x,y,l,p)
+            plottable = self._plottable(x,y)._finished(x,y,l,p)
             n_interactions = len(next(plottable.interactions.groupby(3))[1])
 
             errevery = errevery or max(int(n_interactions*0.05),1) if x == 'index' else 1
             style    = "-" if x == 'index' else "."
             err      = plottable._confidence(err, errevery)
             x_prep   = str if x != 'index' else (lambda _x: _x)
 
@@ -1135,25 +1135,29 @@
 
         try:
             xlim = xlim or [None,None]
             ylim = ylim or [None,None]
 
             og_l = (l1,l2)
 
-            if not isinstance(l1,(list,tuple)): l1     = [l1]
-            if not isinstance(l2,(list,tuple)): l2     = [l2]
-            if     isinstance(labels,str)     : labels = [labels]
+            list_like=(list,tuple)
+
+            if isinstance(l,list_like) and not isinstance(l1[0],list_like): l1 = [l1]
+            if isinstance(l,list_like) and not isinstance(l2[0],list_like): l2 = [l2]
+            if not isinstance(l,list_like) and not isinstance(l1,list_like): l1 = [l1]
+            if not isinstance(l,list_like) and not isinstance(l2,list_like): l2 = [l2]
+            if isinstance(labels,str): labels = [labels]
 
             if any(_l1 in l2 for _l1 in l1):
                 raise CobaException("A value cannot be in both `l1` and `l2`. Please make a change and run it again.")
 
             contraster = (lambda x,y: y-x) if mode == 'diff' else (lambda x,y: int(y-x>0)) if mode=='prob' else mode
             _boundary  = 0 if mode == 'diff' else .5
 
-            plottable = self._plottable(x,y,l,p)
+            plottable = self._plottable(x,y)
             eid       = 'environment_id'
             lid       = 'learner_id'
 
             n_interactions = len(next(plottable.interactions.groupby(3))[1])
 
             errevery = errevery or max(int(n_interactions*0.05),1) if x == 'index' else 1
             style    = "-" if x == 'index' else "."
@@ -1310,25 +1314,28 @@
 
         #could this be made faster? I could think of special cases but not a general solution to speed it up.
         for e1,l1,x1,y1 in L1:
             for e2,l2,x2,y2 in L2:
                 if env_eq_vals[e1] == env_eq_vals[e2] and lrn_eq_vals[l1] == lrn_eq_vals[l2]:
                     yield ((x1,x2),(y1,y2))
 
-    def _plottable(self, x:Sequence[str], y:str, l: Sequence[str], p: Sequence[str]) -> 'Result':
+    def _plottable(self, x:Sequence[str], y:str) -> 'Result':
 
         if not isinstance(x,str) and 'index' in x and len(x) > 1:
             raise CobaException('The x-axis cannot contain both indexes and parameters.')
 
         if len(self.interactions) == 0:
             raise CobaException("This result does not contain any data to plot.")
 
         if y not in self.interactions.columns:
             raise CobaException(f"This result does not contain column '{y}' in interactions.")
 
+        return self
+
+    def _finished(self,x:Sequence[str], y:str, l: Sequence[str], p: Sequence[str]) -> 'Result':
         only_finished = self._filter_fin('min' if x == 'index' else None, l, p)
 
         if len(only_finished.learners) == 0:
             raise CobaException(f"This result does not contain a {p} that has been finished for every {l}.")
 
         if len(only_finished.environments) != len(self.environments):
             CobaContext.logger.log(f"Every {p} not present for all {l} has been excluded.")
```

### Comparing `coba-7.0.2/coba/learners/__init__.py` & `coba-7.0.3/coba/learners/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/learners/bandit.py` & `coba-7.0.3/coba/learners/bandit.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/learners/corral.py` & `coba-7.0.3/coba/learners/corral.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/learners/linucb.py` & `coba-7.0.3/coba/learners/linucb.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/learners/misguided.py` & `coba-7.0.3/coba/learners/misguided.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/learners/primitives.py` & `coba-7.0.3/coba/learners/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/learners/safety.py` & `coba-7.0.3/coba/learners/safety.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,24 +142,25 @@
         if key in self._method:
             prev_method = self._method[key]
 
             if prev_method==1:
                 return method(*args,**(kwargs or {}))
 
             if prev_method==2:
+                if isinstance(args[0],str): raise Exception() #We don't care which exception we raise.
                 return [ method(*a,**{k:v[i] for k,v in kwargs.items()}) for i,a in enumerate(zip(*args)) ]
 
         try:
             self._method[key] = 1
             return self._safe_call(key, method, args, kwargs)
         except:
             try:
                 self._method[key] = 2
                 return self._safe_call(key, method, args, kwargs)
-            except Exception as ex:
+            except:
                 del self._method[key]
             raise
 
     def request(self, context: Context, actions: Actions, request: Actions) -> Sequence[Prob]:
 
         try:
             return self._safe_call('request', self.learner.request, (context,actions,request))
```

### Comparing `coba-7.0.2/coba/learners/vowpal.py` & `coba-7.0.3/coba/learners/vowpal.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/multiprocessing.py` & `coba-7.0.3/coba/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/pipes/__init__.py` & `coba-7.0.3/coba/pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/pipes/core.py` & `coba-7.0.3/coba/pipes/core.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/pipes/filters.py` & `coba-7.0.3/coba/pipes/filters.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/pipes/multiprocessing.py` & `coba-7.0.3/coba/pipes/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/pipes/primitives.py` & `coba-7.0.3/coba/pipes/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/pipes/readers.py` & `coba-7.0.3/coba/pipes/readers.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/pipes/rows.py` & `coba-7.0.3/coba/pipes/rows.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/pipes/sinks.py` & `coba-7.0.3/coba/pipes/sinks.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/pipes/sources.py` & `coba-7.0.3/coba/pipes/sources.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/primitives/feedbacks.py` & `coba-7.0.3/coba/primitives/feedbacks.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/primitives/rewards.py` & `coba-7.0.3/coba/primitives/rewards.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/primitives/rows.py` & `coba-7.0.3/coba/primitives/rows.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/primitives/types.py` & `coba-7.0.3/coba/primitives/types.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/random.py` & `coba-7.0.3/coba/random.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/register.py` & `coba-7.0.3/coba/register.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/registry.py` & `coba-7.0.3/coba/registry.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/statistics.py` & `coba-7.0.3/coba/statistics.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba/utilities.py` & `coba-7.0.3/coba/utilities.py`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/coba.egg-info/PKG-INFO` & `coba-7.0.3/coba.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coba
-Version: 7.0.2
+Version: 7.0.3
 Summary: A contextual bandit research package
 Author-email: Mark Rucker <rucker.mark@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/vowpalwabbit/coba
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `coba-7.0.2/coba.egg-info/SOURCES.txt` & `coba-7.0.3/coba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coba-7.0.2/pyproject.toml` & `coba-7.0.3/pyproject.toml`

 * *Files identical despite different names*

